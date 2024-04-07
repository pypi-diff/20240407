# Comparing `tmp/exl2conv-0.0.17.tar.gz` & `tmp/exl2conv-0.0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exl2conv-0.0.17.tar", last modified: Mon Apr  1 05:03:50 2024, max compression
+gzip compressed data, was "exl2conv-0.0.17.1.tar", last modified: Sun Apr  7 08:03:46 2024, max compression
```

## Comparing `exl2conv-0.0.17.tar` & `exl2conv-0.0.17.1.tar`

### file list

```diff
@@ -1,162 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 05:03:23.000000 exl2conv-0.0.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 05:03:23.000000 exl2conv-0.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 05:03:50.942948 exl2conv-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-01 05:03:23.000000 exl2conv-0.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.930948 exl2conv-0.0.17/exl2conv/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.934948 exl2conv-0.0.17/exl2conv/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    19087 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/adaptivegptq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    23645 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/qparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    18190 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/quantize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.934948 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/
--rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/c4.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/code.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/multilingual.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/technical.utf8
--rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/tiny.utf8
--rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/wiki.utf8
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/conversion/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.938948 exl2conv-0.0.17/exl2conv/exl2conv_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.938948 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)    24023 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/quantize_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/util.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.938948 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/cache.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/cache.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.938948 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/compat.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_add.cu
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_add.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/layer_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/lora.cu
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/lora.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_attn.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_attn.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_matrix.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quantize.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quantize.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rms_norm.cu
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rope.cu
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rope.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/util.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/util.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_cache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_gemm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_gemm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_norm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_norm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qattn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qattn.h
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmlp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_quant.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_quant.h
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_rope.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_rope.h
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_safetensors.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_safetensors.h
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_sampling.h
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/fasttensors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/exl2conv/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/exl2conv/generator/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/filters/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/filters/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/ngram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    33049 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/generator/streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    28061 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/model_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/moe_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/parallel_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/exl2conv/server/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/server/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/server/websocket_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.942948 exl2conv-0.0.17/exl2conv/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer/spm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 05:03:23.000000 exl2conv-0.0.17/exl2conv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:03:50.930948 exl2conv-0.0.17/exl2conv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 05:03:50.000000 exl2conv-0.0.17/exl2conv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-01 05:03:50.000000 exl2conv-0.0.17/exl2conv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 05:03:50.000000 exl2conv-0.0.17/exl2conv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 05:03:50.000000 exl2conv-0.0.17/exl2conv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 05:03:50.000000 exl2conv-0.0.17/exl2conv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 05:03:50.942948 exl2conv-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-01 05:03:23.000000 exl2conv-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.704609 exl2conv-0.0.17.1/exl2conv/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32609 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.704609 exl2conv-0.0.17.1/exl2conv/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/adaptivegptq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/qparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/quantize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.704609 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   332173 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/c4.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   248834 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/code.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   222555 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/multilingual.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   196701 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/technical.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)   261693 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/tiny.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)  2093275 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/wiki.utf8
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/conversion/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.708609 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.708609 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/avx2_target.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24414 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/profiling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/profiling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/quantize_func.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/quantize_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling_avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/cache.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/cache.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/compat.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_add.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_add.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/head_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/head_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/layer_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/layer_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/lora.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/lora.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/matrix_view.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/pack_tensor.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_attn.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_attn.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    21831 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_matrix.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_matrix.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quantize.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quantize.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rms_norm.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rms_norm.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rope.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rope.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/util.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_norm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qattn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qattn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmlp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_quant.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_quant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_rope.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_rope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_safetensors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_safetensors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/fasttensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/generator/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/filters/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/filters/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/ngram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33049 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/generator/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/headnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10977 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/model_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/moe_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/parallel_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/server/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/server/websocket_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/exl2conv/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer/spm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22386 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/exl2conv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:03:46.704609 exl2conv-0.0.17.1/exl2conv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 08:03:46.000000 exl2conv-0.0.17.1/exl2conv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-07 08:03:46.000000 exl2conv-0.0.17.1/exl2conv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:03:46.000000 exl2conv-0.0.17.1/exl2conv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 08:03:46.000000 exl2conv-0.0.17.1/exl2conv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 08:03:46.000000 exl2conv-0.0.17.1/exl2conv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:03:46.712609 exl2conv-0.0.17.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-07 08:03:13.000000 exl2conv-0.0.17.1/setup.py
```

### Comparing `exl2conv-0.0.17/LICENSE` & `exl2conv-0.0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/README.md` & `exl2conv-0.0.17.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
 This will install the "JIT version" of the package, i.e. it will install the Python components without building the
 C++ extension in the process. Instead, the extension will be built the first time the library is used, then cached in 
 `~/.cache/torch_extensions` for subsequent use.
 
 ### Method 2: Install from PyPI
 
-A PyPI package is NOT YET available as well. It can NOT be installed with:
+A PyPI package is available as well. It can be installed with:
 
 ```
-DON'T pip install exl2conv
+pip install exl2conv
 ```
 
 The version available through PyPI is the JIT version (see above). Still working on a solution for distributing
 prebuilt wheels via PyPI.
 
 
 ## EXL2 quantization
```

### Comparing `exl2conv-0.0.17/exl2conv/architecture.py` & `exl2conv-0.0.17.1/exl2conv/architecture.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/attn.py` & `exl2conv-0.0.17.1/exl2conv/attn.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/cache.py` & `exl2conv-0.0.17.1/exl2conv/cache.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/compat.py` & `exl2conv-0.0.17.1/exl2conv/compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-
+from __future__ import annotations
 import torch
 
 # On some setups Torch will attempt to use GPU peer-to-peer copies even when they are not supported. This is either
 # a driver issue, a bug in Torch, or both. Either way, the result is that .to() will create an empty tensor on the
 # target device and silently fail to copy any data into it. This is a workaround.
 
 tested_peer_copy = None
 
-def test_gpu_peer_copy(device_a, device_b):
+def test_gpu_peer_copy(device_a: torch.Device,
+                       device_b: torch.Device):
     global tested_peer_copy
 
     if tested_peer_copy is None:
         num_dev = torch.cuda.device_count()
         tested_peer_copy = [[0 for _ in range(num_dev)] for _ in range(num_dev)]
 
     idx_a = device_a.index
@@ -31,15 +32,16 @@
         tested_peer_copy[idx_a][idx_b] = 1
         return True
     else:
         tested_peer_copy[idx_a][idx_b] = -1
         return False
 
 
-def safe_move_tensor(tensor, device):
+def safe_move_tensor(tensor: torch.Tensor | tuple[torch.Tensor],
+                     device: torch.Device | str):
 
     # Accept tensor or tuple of tensors
 
     if isinstance(tensor, tuple):
         return tuple(safe_move_tensor(x, device) for x in tensor)
 
     # Accept torch.device or string
```

### Comparing `exl2conv-0.0.17/exl2conv/config.py` & `exl2conv-0.0.17.1/exl2conv/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     scale_pos_emb: float                        # Factor by which to scale positional embeddings, e.g. for 4096-token sequence use a scaling factor of 2.0, requires finetuned model or LoRA
     scale_alpha_value: float                    # Alpha value for NTK RoPE scaling. Similar to compress_pos_emb but works without finetuned model
 
     no_flash_attn: bool                         # Implementation will automatically use flash-attn-2 when available
     fasttensors: bool                           # Experimental, Linux only
     load_in_q4: bool                            # Load float linear layers in Q4 format (for test/dev purposes, not performant)
 
+    max_dq_size: int                            # Max number of elements to dequantize at once
+
     # Loaded/set by .prepare():
 
     architecture: str
     arch: ExLlamaV2ArchParams
 
     model_config: str
     tensor_file_map: dict
@@ -83,14 +85,15 @@
     norm_eps: float | None
     vocab_size: int
     rotary_embedding_base: float
     head_dim: int
     num_experts: int | None
     num_experts_per_token: int | None
     logit_scale: float
+    use_qk_norm: bool
 
     checkpoint_fused_mlp: bool
 
 
     def __init__(self,
                  model_dir: str | None = None):
         """
@@ -111,14 +114,15 @@
 
         if model_dir is not None:
             self.model_dir = model_dir
             self.prepare()
         else:
             self.model_dir = None
 
+        self.max_dq_size = 512*(1024**2)
 
     # Set low-mem options
 
     def set_low_mem(self):
 
         self.max_input_len = 1024
         self.max_attention_size = 1024 ** 2
@@ -172,15 +176,15 @@
         # Attn params
 
         self.num_attention_heads = read(read_config, int, ["num_attention_heads", "n_heads"])
         self.head_dim = read(read_config, int, "head_dim", self.hidden_size // self.num_attention_heads)
 
         self.num_key_value_heads = read(read_config, int, ["num_key_value_heads", "attn_config->kv_n_heads"], self.num_attention_heads)
         self.num_key_value_groups = self.num_attention_heads // self.num_key_value_heads
-
+        self.use_qk_norm = read(read_config, bool, ["use_qk_norm"], False)
 
         # MLP params
 
         self.intermediate_size = read(read_config, int, ["intermediate_size", "ffn_config->ffn_hidden_size"])
         self.num_experts = read(read_config, int, ["num_local_experts", "ffn_config->moe_num_experts"], None)
         self.num_experts_per_token = read(read_config, int,["num_experts_per_tok", "ffn_config->moe_top_k"], None)
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/adaptivegptq.py` & `exl2conv-0.0.17.1/exl2conv/conversion/adaptivegptq.py`

 * *Files 16% similar despite different names*

```diff
@@ -102,14 +102,17 @@
     quant: torch.Tensor | None
     weights: torch.Tensor | None
     hessian: torch.Tensor | None
     hessian_inv: torch.Tensor | None
     num_samples: int = 0
     num_batches: int = 0
 
+    quant_device: int = 0
+    hessian_device: int = 0
+
 
     def __init__(self,
                  layer: nn.Linear):
 
         self.layer = layer
         self.device = layer.weight.device
 
@@ -128,14 +131,17 @@
 
         self.scale = None
         self.qscale = None
         self.qscale_max = None
         self.qweight = None
         self.qgroups = None
 
+        self.quant_device = 0
+        self.hessian_device = 0
+
 
     def drop_buffers(self):
 
         self.perm = None
         self.perm_cpu = None
         self.invperm = None
         # self.g_idx = None
@@ -204,37 +210,37 @@
         with torch.inference_mode():
 
             self.hessian /= self.num_batches
             diagonal = torch.diag(self.hessian)
 
             # Prepare weights
 
-            self.weights = self.layer.weight.data.T.clone().float().contiguous().cpu()
+            self.weights = self.layer.weight.data.cpu().T.clone().float().contiguous()
 
             # Zero weights that have no impact. Disabling this since it feels a little drastic based on just the calibration
             # data. It likely never triggers, anyway.
 
             # dead = diagonal == 0.0
             # self.hessian[dead, dead] = 1
             # self.weights[dead, :] = 0
 
             # Activation order
 
             self.perm = torch.argsort(diagonal, descending = True)
             self.perm_cpu = self.perm.cpu()
-
-            # if self.weights.numel() > 1e9:
-            #     self.weights = self.weights.to("cpu")
-            #     self.weights = self.weights[self.perm_cpu, :]
-            #     self.weights = self.weights.to("cuda:0")
-            # else:
             self.weights = self.weights[self.perm_cpu, :]
 
-            hessian = self.hessian[self.perm][:, self.perm]
-            self.hessian = None
+            if self.hessian.numel() > 6e8:
+                hessian_cpu = self.hessian.cpu()
+                self.hessian = None
+                hessian = hessian_cpu[self.perm_cpu][:, self.perm_cpu]
+                hessian = hessian.to("cuda:0")
+            else:
+                hessian = self.hessian[self.perm][:, self.perm]
+                self.hessian = None
 
             # In case numerical errors have caused some asymmetry in H, assume it's close to symmetrical and force it.
             # (Doesn't seem to be needed)
 
             # torch.cuda.empty_cache()
             # hessian = (hessian + hessian.T) * 0.5
             # torch.cuda.empty_cache()
@@ -250,47 +256,48 @@
             while not no_h_inv:
 
                 try:
 
                     d = torch.arange(self.rows, device = self.device)
                     hessian[d, d] += damp
 
-                    # Dump condition number and smallest eigenvalue (should be positive)
+                    current_device = self.hessian_device
+                    max_devices = torch.cuda.device_count()
 
-                    # fro_norm_hessian = torch.norm(hessian, p = 'fro')
-                    # fro_norm_inv = torch.norm(torch.linalg.inv(hessian), p = 'fro')
-                    # cond_number = fro_norm_hessian * fro_norm_inv
-                    # print(cond_number)
+                    done = False
+                    fail_device = False
+                    while not done:
+                        try:
+                            hessian = hessian.to(torch.device(current_device))
 
-                    # eigenvalues = torch.linalg.eigvalsh(hessian)
-                    # is_pd = torch.all(eigenvalues > 0)
-                    # print(is_pd)
-                    # print(torch.min(eigenvalues))
+                            hessian_inv = torch.linalg.cholesky(hessian)
+                            hessian_inv = torch.cholesky_inverse(hessian_inv)
 
-                    hessian_inv = torch.linalg.cholesky(hessian)
-                    hessian_inv = torch.cholesky_inverse(hessian_inv)
+                            # The Cholesky inverse will sometimes fail to compute due to accumulated rounding errors when H
+                            # is very large (e.g. 70B MLP down proj) and a lot of calibration data is used (e.g. 100 rows of
+                            # 4096 tokens). This won't always throw an exception and sometimes just results in a NaN tensor.
 
-                    # The Cholesky inverse will sometimes fail to compute due to accumulated rounding errors when H
-                    # is very large (e.g. 70B MLP down proj) and a lot of calibration data is used (e.g. 100 rows of
-                    # 4096 tokens). This won't always throw an exception and sometimes just results in a NaN tensor.
+                            if torch.any(torch.isnan(hessian_inv)): raise RuntimeError
 
-                    if torch.any(torch.isnan(hessian_inv)): raise RuntimeError
+                            # Test inversion
 
-                    # Test inversion
+                            hessian_inv = torch.linalg.cholesky(hessian_inv, upper = True)
+                            hessian_inv = hessian_inv.contiguous()
 
-                    # test = hessian_inv @ hessian
-                    # test.sub_(torch.eye(test.size(0), device = test.device, dtype = test.dtype))
-                    # test **= 2
-                    # test = test.mean()
-                    # print(test)
+                            done = True
+                            break
 
-                    hessian_inv = torch.linalg.cholesky(hessian_inv, upper = True)
-                    hessian_inv = hessian_inv.contiguous()
+                        except torch.cuda.OutOfMemoryError as e:
+                            current_device += 1
+                            print(f" !! Out of memory (H), moving to device {current_device}")
+                            if current_device == max_devices:
+                                raise e
+                            self.hessian_device = current_device
 
-                    break
+                    if done: break
 
                 except RuntimeError as runtime_error:
 
                     if "out of memory" in str(runtime_error):
                         raise runtime_error
 
                     # If inverting failed, assume there were non-positive eigenvalues, so apply more damping to shift
@@ -310,182 +317,222 @@
 
     def reuse_h(self, other):
 
         with torch.inference_mode():
 
             # Prepare weights
 
-            self.weights = self.layer.weight.data.T.clone().float().contiguous().cpu()
+            self.weights = self.layer.weight.data.cpu().T.clone().float().contiguous()
 
             self.hessian_inv = other.hessian_inv
             self.hessian = None
             self.perm = other.perm
             self.perm_cpu = other.perm_cpu
             self.weights = self.weights[self.perm_cpu, :]
 
 
     def quantize_rtn_inplace(self, keep_qweight = False, apply = False):
         assert apply and keep_qweight
 
         with torch.inference_mode():
 
-            weights = self.weights.to("cuda:0")
-            self.qweight = torch.zeros_like(self.weights, dtype = torch.short, device = "cuda:0")
+            current_device = self.quant_device
+            max_devices = torch.cuda.device_count()
 
-            num_groups = 0
-            for bits_idx in range(len(self.bits)):
-                num_groups += self.bits_groups[bits_idx]
-
-            scale = []
-            qscale = []
-            qscale_max = torch.empty((num_groups,), dtype = torch.float, device = "cuda:0")
-            qgroups = []
-
-            group_idx = 0
-            group_idx_list = []
-
-            b = 0
-            for bits_idx, bits in enumerate(self.bits):
-                quantizer = AdaptiveQuantizer(bits = bits, scale_bits = self.scale_bits)
-
-                for group in range(self.bits_groups[bits_idx]):
-                    a = b
-                    b = min(a + self.group_size[bits], self.rows)
-
-                    qgroups.append(bits)
-                    qgroups.append(0)
-
-                    quantizer.find_params(self.weights[a : b, :])
-                    scale.append(quantizer.scale)
-                    qscale.append(quantizer.qscale)
-                    qscale_max[group_idx] = quantizer.qscale_max
+            weights_cpu = self.weights.cpu().contiguous()
 
-                    ext_c.quantize_range_inplace(self.weights,
-                                                 quantizer.scale,
-                                                 self.qweight,
-                                                 quantizer.qzero,
-                                                 quantizer.maxq,
-                                                 a,
-                                                 b)
+            done = False
+            while not done:
 
-                    group_idx_list += [group_idx] * (b - a)
-                    group_idx += 1
+                try:
+
+                    weights = weights_cpu.to(torch.device(current_device))
+                    self.qweight = torch.zeros_like(weights, dtype = torch.short, device = torch.device(current_device))
+
+                    num_groups = 0
+                    for bits_idx in range(len(self.bits)):
+                        num_groups += self.bits_groups[bits_idx]
+
+                    scale = []
+                    qscale = []
+                    qscale_max = torch.empty((num_groups,), dtype = torch.float, device = torch.device(current_device))
+                    qgroups = []
+
+                    group_idx = 0
+                    group_idx_list = []
+
+                    b = 0
+                    for bits_idx, bits in enumerate(self.bits):
+                        quantizer = AdaptiveQuantizer(bits = bits, scale_bits = self.scale_bits)
+
+                        for group in range(self.bits_groups[bits_idx]):
+                            a = b
+                            b = min(a + self.group_size[bits], self.rows)
+
+                            qgroups.append(bits)
+                            qgroups.append(0)
+
+                            quantizer.find_params(weights[a : b, :])
+                            scale.append(quantizer.scale)
+                            qscale.append(quantizer.qscale)
+                            qscale_max[group_idx] = quantizer.qscale_max
+
+                            ext_c.quantize_range_inplace(weights,
+                                                         quantizer.scale,
+                                                         self.qweight,
+                                                         quantizer.qzero,
+                                                         quantizer.maxq,
+                                                         a,
+                                                         b)
+
+                            group_idx_list += [group_idx] * (b - a)
+                            group_idx += 1
+
+                    done = True
+
+                except torch.cuda.OutOfMemoryError as e:
+                    current_device += 1
+                    print(f" !! Out of memory (Q), moving to device {current_device}")
+                    if current_device == max_devices:
+                        raise e
+                    self.quant_device = current_device
 
             # Create g_idx to store inverse activation order
 
-            self.invperm = torch.argsort(self.perm)
+            self.invperm = torch.argsort(self.perm).to("cuda:0")
 
             # Store scales
 
-            self.scale = torch.stack(scale, dim = 0)
-            self.qscale = torch.stack(qscale, dim = 0)
-            self.qscale_max = qscale_max.to(torch.float16)
-            self.qgroups = torch.tensor(qgroups, dtype = torch.short)
+            self.scale = torch.stack(scale, dim = 0).to("cuda:0")
+            self.qscale = torch.stack(qscale, dim = 0).to("cuda:0")
+            self.qscale_max = qscale_max.to(torch.float16).to("cuda:0")
+            self.qgroups = torch.tensor(qgroups, dtype = torch.short).to("cuda:0")
 
             # I love Python
 
             scale = None
             qscale = None
             qscale_max = None
             qgroups = None
             group_idx_list = None
 
             qc = weights.cpu()
             qc = qc.to(torch.half)
             invperm = self.invperm.cpu()
             q = qc[invperm, :].T
-            q = q.reshape(self.weights.T.shape)
+            q = q.reshape(weights.T.shape)
 
             dev = weights.device
-            self.weights = None
+            weights = None
+            torch.cuda.synchronize()
             gc.collect()
             torch.cuda.empty_cache()
 
             q = q.to(dev)
             self.layer.weight.data = q
             self.weights = q.T
 
 
     def quantize(self, keep_qweight = False, apply = False):
 
         with torch.inference_mode():
 
-            hessian_inv_cuda = self.hessian_inv.to("cuda:0")
+            current_device = self.quant_device
+            max_devices = torch.cuda.device_count()
+
+            weights_cpu = self.weights.cpu()
+
+            done = False
+            while not done:
+
+                try:
+
+                    hessian_inv_cuda = self.hessian_inv.to(torch.device(current_device))
+
+                    # if apply:
+                    #     weights = self.weights
+                    #     self.layer.weight.data = torch.zeros((1, 1), dtype = torch.float32, device = weights.device)
+                    # else:
+                    #     weights = self.weights.clone()
+                    weights = weights_cpu.to(torch.device(current_device))
+
+                    self.quant = torch.zeros_like(weights_cpu, device = torch.device(current_device))
+
+                    if keep_qweight:
+                        self.qweight = torch.zeros_like(weights, dtype = torch.short)
+
+                    # Quantize groups
+
+                    num_groups = 0
+                    for bits_idx in range(len(self.bits)):
+                        num_groups += self.bits_groups[bits_idx]
+
+                    scale = []
+                    qscale = []
+                    qscale_max = torch.empty((num_groups,), dtype = torch.float, device = torch.device(current_device))
+                    qgroups = []
+
+                    error = weights.clone()
+                    group_idx = 0
+                    group_idx_list = []
+
+                    b = 0
+                    for bits_idx, bits in enumerate(self.bits):
+                        quantizer = AdaptiveQuantizer(bits = bits, scale_bits = self.scale_bits)
+
+                        for group in range(self.bits_groups[bits_idx]):
+                            a = b
+                            b = min(a + self.group_size[bits], self.rows)
+
+                            qgroups.append(bits)
+                            qgroups.append(0)
+
+                            quantizer.find_params(weights[a : b, :])
+                            scale.append(quantizer.scale)
+                            qscale.append(quantizer.qscale)
+                            qscale_max[group_idx] = quantizer.qscale_max
+
+                            ext_c.quantize_range(self.quant,
+                                                 quantizer.scale,
+                                                 self.qweight if keep_qweight else none_tensor,
+                                                 quantizer.qzero,
+                                                 quantizer.maxq,
+                                                 hessian_inv_cuda,
+                                                 weights,
+                                                 error,
+                                                 a,
+                                                 b)
+
+                            group_idx_list += [group_idx] * (b - a)
+                            group_idx += 1
 
-            # if apply:
-            #     weights = self.weights
-            #     self.layer.weight.data = torch.zeros((1, 1), dtype = torch.float32, device = weights.device)
-            # else:
-            #     weights = self.weights.clone()
-            weights = self.weights.to("cuda:0")
-
-            self.quant = torch.zeros_like(self.weights, device = "cuda:0")
-
-            if keep_qweight:
-                self.qweight = torch.zeros_like(weights, dtype = torch.short)
-
-            # Quantize groups
-
-            num_groups = 0
-            for bits_idx in range(len(self.bits)):
-                num_groups += self.bits_groups[bits_idx]
-
-            scale = []
-            qscale = []
-            qscale_max = torch.empty((num_groups,), dtype = torch.float, device = "cuda:0")
-            qgroups = []
-
-            error = weights.clone()
-            group_idx = 0
-            group_idx_list = []
-
-            b = 0
-            for bits_idx, bits in enumerate(self.bits):
-                quantizer = AdaptiveQuantizer(bits = bits, scale_bits = self.scale_bits)
-
-                for group in range(self.bits_groups[bits_idx]):
-                    a = b
-                    b = min(a + self.group_size[bits], self.rows)
-
-                    qgroups.append(bits)
-                    qgroups.append(0)
-
-                    quantizer.find_params(weights[a : b, :])
-                    scale.append(quantizer.scale)
-                    qscale.append(quantizer.qscale)
-                    qscale_max[group_idx] = quantizer.qscale_max
-
-                    ext_c.quantize_range(self.quant,
-                                         quantizer.scale,
-                                         self.qweight if keep_qweight else none_tensor,
-                                         quantizer.qzero,
-                                         quantizer.maxq,
-                                         hessian_inv_cuda,
-                                         weights,
-                                         error,
-                                         a,
-                                         b)
+                    done = True
 
-                    group_idx_list += [group_idx] * (b - a)
-                    group_idx += 1
+                except torch.cuda.OutOfMemoryError as e:
+                    current_device += 1
+                    print(f" !! Out of memory (Q), moving to device {current_device}")
+                    if current_device == max_devices:
+                        raise e
+                    self.quant_device = current_device
 
             # Create g_idx to store inverse activation order
 
             # self.g_idx = torch.tensor(group_idx_list, dtype = torch.int32, device = self.device)
             # self.g_idx = torch.tensor(group_idx_list, dtype = torch.int32)
 
-            self.invperm = torch.argsort(self.perm)
+            self.quant = self.quant.to("cuda:0")
+            self.invperm = torch.argsort(self.perm).to("cuda:0")
             # self.g_idx = self.g_idx[self.invperm]
 
             # Store scales
 
-            self.scale = torch.stack(scale, dim = 0)
-            self.qscale = torch.stack(qscale, dim = 0)
-            self.qscale_max = qscale_max.to(torch.float16)
-            self.qgroups = torch.tensor(qgroups, dtype = torch.short)
+            self.scale = torch.stack(scale, dim = 0).to("cuda:0")
+            self.qscale = torch.stack(qscale, dim = 0).to("cuda:0")
+            self.qscale_max = qscale_max.to(torch.float16).to("cuda:0")
+            self.qgroups = torch.tensor(qgroups, dtype = torch.short).to("cuda:0")
 
             # I love Python
 
             weights = None
             error = None
             scale = None
             qscale = None
@@ -519,15 +566,15 @@
         invperm = self.invperm.cpu()
         q = qc[invperm, :].T
         q = q.reshape(self.quant.T.shape)
 
         gc.collect()
         torch.cuda.empty_cache()
 
-        q = q.to(self.quant.device)
+        q = q.to(torch.device(self.quant_device))
         self.layer.weight.data = q
 
 
     def apply_temp(self):
 
         q = self.quant[self.invperm, :].T
         temp_layer = nn.Linear(self.layer.in_features, self.layer.out_features, False, device = "meta", dtype = torch.float16)
@@ -581,15 +628,15 @@
             rows = min(self.group_size[bits], rem_rows)
             wpqr = 32 / bits
             qrows = rows / wpqr
             assert i == self.qgroups.shape[-1] or qrows == int(qrows)
             qrows = math.ceil(qrows)
 
             g_qwt = qwt[row:row+rows, :].contiguous()
-            g_qwt_packed = torch.zeros((qrows, columns + padding), dtype = torch.int32, device = self.device)
+            g_qwt_packed = torch.zeros((qrows, columns + padding), dtype = torch.int32, device = g_qwt.device)
 
             if padding > 0: g_qwt[:, -padding:] = 2 ** (bits - 1)
 
             ext_c.pack_columns(g_qwt, g_qwt_packed, bits)
             qwt_packed.append(g_qwt_packed)
 
             # print(row, rows, bits)
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/compile.py` & `exl2conv-0.0.17.1/exl2conv/conversion/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,20 +93,25 @@
                 d = get_q_module(job, module.w1[i]); out_dict.update(d); current_size += _dsize(d)
                 d = get_q_module(job, module.w3[i]); out_dict.update(d); current_size += _dsize(d)
                 d = get_q_module(job, module.w2[i]); out_dict.update(d); current_size += _dsize(d)
 
         if isinstance(module, ExLlamaV2ParallelDecoder):
 
             has_gate = model.config.arch.mlp_gate
+            has_qk_norm = model.config.use_qk_norm
             d = get_f_module(job, module.input_layernorm); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.attn.q_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.attn.k_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.attn.v_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.attn.o_proj); out_dict.update(d); current_size += _dsize(d)
-            if has_gate: d = get_q_module(job, module.mlp.gate_proj); out_dict.update(d); current_size += _dsize(d)
+            if has_qk_norm:
+                d = get_f_module(job, module.attn.q_norm); out_dict.update(d); current_size += _dsize(d)
+                d = get_f_module(job, module.attn.k_norm); out_dict.update(d); current_size += _dsize(d)
+            if has_gate:
+                d = get_q_module(job, module.mlp.gate_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.mlp.up_proj); out_dict.update(d); current_size += _dsize(d)
             d = get_q_module(job, module.mlp.down_proj); out_dict.update(d); current_size += _dsize(d)
 
         if isinstance(module, ExLlamaV2RMSNorm) or isinstance(module, ExLlamaV2LayerNorm):
 
             d = get_f_module(job, module); out_dict.update(d); current_size += _dsize(d)
 
@@ -202,31 +207,33 @@
             print(f" --   {f}")
             source_file_path = os.path.join(input_dir, f)
             target_file_path = os.path.join(out_dir, f)
             shutil.copy(source_file_path, target_file_path)
 
     # Add signature to config.json
 
-    ds = job["cal_dataset"]
-    if ds is not None: qcfg_ds = os.path.split(ds)[1]
-    else: qcfg_ds = "(default)"
-
-    qcfg = {
-        "quant_method": "exl2",
-        "version": __version__,
-        "bits": job["bits"],
-        "head_bits": job["head_bits"],
-        "calibration": {
-            "rows": job["dataset_rows"],
-            "length": job["length"],
-            "dataset": qcfg_ds
-        },
-    }
-
-    config_json = os.path.join(out_dir, "config.json")
-    with open(config_json, "r") as f:
-        config_dict = json.load(f)
+    if job["compile_full"] is not None:
+
+        ds = job["cal_dataset"]
+        if ds is not None: qcfg_ds = os.path.split(ds)[1]
+        else: qcfg_ds = "(default)"
+
+        qcfg = {
+            "quant_method": "exl2",
+            "version": __version__,
+            "bits": job["bits"],
+            "head_bits": job["head_bits"],
+            "calibration": {
+                "rows": job["dataset_rows"],
+                "length": job["length"],
+                "dataset": qcfg_ds
+            },
+        }
+
+        config_json = os.path.join(out_dir, "config.json")
+        with open(config_json, "r") as f:
+            config_dict = json.load(f)
 
-    config_dict["quantization_config"] = qcfg
+        config_dict["quantization_config"] = qcfg
 
-    with open(config_json, "w") as f:
-        f.write(json.dumps(config_dict, indent = 4))
+        with open(config_json, "w") as f:
+            f.write(json.dumps(config_dict, indent = 4))
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/convert.py` & `exl2conv-0.0.17.1/exl2conv/conversion/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,25 +179,36 @@
             print(f" -- Token embeddings (measurement)...")
             embeddings(job, save_job, model)
             job["progress"] = "measure_quant"
             save_job()
 
         if progress == "measure_quant":
             print(f" -- Measuring quantization impact...")
+
+            model.unload()
+            config.max_output_len = 16
+            model = ExLlamaV2(config)
+            model.load(lazy = True)
+
             status = measure_quant(job, save_job, model)  # capturing the graceful exits
             if status == "interrupted":
                 print("Process interrupted. Exiting gracefully.")
                 save_job()
                 sys.exit(1)
             if job["output_measurement"] is None:
                 job["progress"] = "optimize"
             else:
                 job["progress"] = "finished"
             save_job()
 
+            model.unload()
+            config.max_output_len = None
+            model = ExLlamaV2(config)
+            model.load(lazy = True)
+
         if progress == "optimize":
 
             print(f" -- Optimizing...")
             optimize(job, save_job, model)
             job["progress"] = "tokens_cal"
             save_job()
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/measure.py` & `exl2conv-0.0.17.1/exl2conv/conversion/measure.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         xref = xref[0].float()
         rfn_sum += (torch.linalg.norm(xtest - xref, 'fro') / torch.linalg.norm(xref, 'fro')).item()
         rfn_count += 1
 
     return max(1e-6, 1 - (rfn_sum / rfn_count))
 
 
-def measure_attn(module, hidden_states, target_states, quantizers, cache, attn_params):
+def measure_attn(module, hidden_states, target_states, quantizers, cache, attn_params, keep_q = False):
 
     qjobs, qmaps = get_qparams_reduced(qparams_attn)
     results = []
 
     quantizers["q_proj"].prepare()
     quantizers["k_proj"].reuse_h(quantizers["q_proj"])
     quantizers["v_proj"].reuse_h(quantizers["q_proj"])
@@ -177,14 +177,18 @@
               "total_bits": total_bits,
               "q_proj": qjobs[0][q].get_dict(),
               "k_proj": qjobs[1][k].get_dict(),
               "v_proj": qjobs[2][v].get_dict(),
               "o_proj": qjobs[3][o].get_dict() }
         results.append(r)
 
+    for x in ["k_proj", "v_proj", "o_proj"] + (["q_proj"] if not keep_q else []):
+        if x in quantizers:
+            del quantizers[x]
+
     return results
 
 
 def measure_mlp(module, hidden_states, target_states, quantizers, cache, attn_params, reuse_h_up_proj = None):
 
     has_gate = module.model.config.arch.mlp_gate
 
@@ -253,14 +257,17 @@
 
             r = { "accuracy": accuracy,
                   "total_bits": total_bits,
                   "up_proj": qjobs[1][u].get_dict(),
                   "down_proj": qjobs[2][d].get_dict() }
             results.append(r)
 
+    for x in ["up_proj", "down_proj", "gate_proj"]:
+        if x in quantizers:
+            del quantizers[x]
 
     return results
 
 
 def measure_moe_mlp(module, hidden_states, target_states, quantizers, cache, attn_mask):
 
     qjobs, qmaps = get_qparams_reduced(qparams_mlp)
@@ -325,18 +332,30 @@
         results.append(r)
 
     return results
 
 
 def measure_parallel_decoder(module, hidden_states, target_states_attn, target_states_mlp, quantizers, cache, attn_params):
 
+    for i in range(len(hidden_states)):
+        hidden_states[i] = hidden_states[i].cpu()
+
     print(f" -- Sublayer: {module.key}.self_attn")
-    results_attn = measure_attn(module.attn, hidden_states, target_states_attn, quantizers, cache, attn_params)
+    results_attn = measure_attn(module.attn, hidden_states, target_states_attn, quantizers, cache, attn_params, keep_q = True)
+
+    module.attn.unload()
+    gc.collect()
+    torch.cuda.empty_cache()
+
     print(f" -- Sublayer: {module.key}.mlp")
     results_mlp = measure_mlp(module.mlp, hidden_states, target_states_mlp, quantizers, cache, attn_params, "q_proj")
+
+    for i in range(len(hidden_states)):
+        hidden_states[i] = hidden_states[i].to("cuda:0")
+
     r = { "attn": results_attn,
           "mlp": results_mlp }
     return r
 
 
 # helpful status box for insights around conversions
 def get_remaining_time_str(estimated_time_remaining):
@@ -363,15 +382,17 @@
     time_spent_list = []  
     rolling_window_size = 10 # (increase to average over larger window)
     completed_steps = 0  
     accuracy_sum = 0  
     accuracy_count = 0  
     overall_rolling_accuracy = 0  
 
-    snapshot_interval = 10
+    last_snapshot_time = time.time()
+    snapshot_interval_s = 90
+
     temp_filename = os.path.join(job["out_dir"], "hidden_states_temp.safetensors")
     states_filename = os.path.join(job["out_dir"], "hidden_states.safetensors")
     measurement = job.get("measurement", {})
 
     # Quantize
 
     last_ckpt_layer_name = "None"
@@ -598,15 +619,18 @@
         # if accuracy_count > 0:
         #     content_lines.append(overall_accuracy_str)
 
         print_status_box(*content_lines)
 
         # Checkpoint
 
-        if index % snapshot_interval == 0 or index == len(model.modules) - 1:
+        time_since_snapshot = time.time() - last_snapshot_time
+        if time_since_snapshot > snapshot_interval_s or index == len(model.modules) - 1:
+
+            print(" -- Saving checkpoint...")
 
             save_dict = {f"row.{idx:05}": h for idx, h in enumerate(hidden_states)}
             save_file(save_dict, temp_filename)
             save_dict = None
 
             job["invalid"] = True
             save_fn()
@@ -617,14 +641,16 @@
             job["last_module_idx"] = index
 
             last_ckpt_layer_name = f"{module.key} ({module.name})"
 
             del job["invalid"]
             save_fn()
 
+            last_snapshot_time = time.time()
+
     # Export measurement
 
     exp_measurement = { "measurement": job["measurement"],
                         "last_module_idx": job["last_module_idx"] }
 
     measurement_files = [os.path.join(job["out_dir"], "measurement.json")]
     if job["output_measurement"] is not None:
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/optimize.py` & `exl2conv-0.0.17.1/exl2conv/conversion/optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     has_gate = model.config.arch.mlp_gate
     if has_gate: mlp_key_gate = model.config.arch.mlp_key_gate
     mlp_key_up = model.config.arch.mlp_key_up
     mlp_key_down = model.config.arch.mlp_key_down
 
     error_norm = 2.4
     max_step_size = 2
+    first_layer_bias = 10
+    bias_layers = 2
+    bias_iter = 10
 
     key = "model.layers.0"
     key_q = key + ".self_attn.q_proj"
     key_k = key + ".self_attn.k_proj"
     key_v = key + ".self_attn.v_proj"
     key_o = key + ".self_attn.o_proj"
 
@@ -56,29 +59,32 @@
     target_bpw = job["bits"]
     weight_budget = numel * target_bpw
 
     # Compile options
 
     measurement = job["measurement"]
 
-    def fn(x):
-        return 1 - ((1 - x) ** error_norm)
+    def fn(x, idx):
+        if idx < bias_layers:
+            return 1 - ((1 - x) ** error_norm) * first_layer_bias
+        else:
+            return 1 - ((1 - x) ** error_norm)
 
     weights = []
     values = []
     params = []
     for i in range(num_layers):
         if model.config.arch.parallel_decoder_blocks:
             m1 = measurement["model.layers." + str(i) + ".parallel_decoder"]["attn"]
             m2 = measurement["model.layers." + str(i) + ".parallel_decoder"]["mlp"]
         else:
             m1 = measurement["model.layers." + str(i) + ".self_attn"]
             m2 = measurement["model.layers." + str(i) + "." + mlp_mode]
         for m in [m1, m2]:
-            v = [fn(e["accuracy"]) for e in m]
+            v = [fn(e["accuracy"], i) for e in m]
             w = [e["total_bits"] for e in m]
             weights.append(w)
             values.append(v)
             params.append(m)
 
     print(" -- Pruning...")
 
@@ -107,18 +113,21 @@
     print(" -- Solving...")
 
     f_solution = [0] * num_layers * 2
     weight = sum(weights[i][0] for i in range(num_layers * 2))
     value = 1
     for i in range(num_layers * 2): value *= values[i][0]
 
+    iteration = 0
+
     while True:
         min_idx = -1
         min_value = float("inf")
-        for i in range(num_layers * 2):
+        iteration += 1
+        for i in range(bias_layers if iteration < bias_iter else num_layers * 2):
             s = f_solution[i]
             if values[i][s] < min_value:
                 if s < len(weights[i]) - 1:
                     added_w = weights[i][s + 1] - weights[i][s]
                     if added_w + weight <= weight_budget:
                         min_idx = i
                         min_value = values[i][s]
@@ -207,22 +216,26 @@
         print(f" -- Score: {best_value:.8f}  bpw: {bpw:.4f}")
         prev_best_value = best_value
 
     # Save strategy
 
     print(" -- Quantization strategy:")
 
+    errp = 1
     job["strategy"] = {}
     for layer_ in range(num_layers):
 
         k1 = "model.layers." + str(layer_) + ".self_attn"
         k2 = "model.layers." + str(layer_) + "." + mlp_mode
         p1 = params[layer_ * 2][f_solution[layer_ * 2]]
         p2 = params[layer_ * 2 + 1][f_solution[layer_ * 2 + 1]]
 
         for (k, p, n) in zip((k1, k2), (p1, p2), (numel_attn, numel_mlp)):
             job["strategy"][k] = p
             bpw = p["total_bits"] / n
             err = 1 - p["accuracy"]
             print(f" --   {k:50} {bpw:1.4f} bpw - exp. error: {err:1.8f}")
+            errp *= (1 - err)
+
+    print(f" -- Total exp. error: {1 - errp:1.12f}")
 
     xx = 0
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/qparams.py` & `exl2conv-0.0.17.1/exl2conv/conversion/qparams.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/quantize.py` & `exl2conv-0.0.17.1/exl2conv/conversion/quantize.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,32 +79,38 @@
     # Reconstruct from packed layer
 
     recons_linear = ExLlamaV2Linear(source.model, source.key, source.in_features, source.out_features, source.has_bias)
     recons_linear.device_idx = source.device_idx
     recons_dict = {}
     recons_keys = ["q_weight", "q_invperm", "q_scale", "q_scale_max", "q_groups"]
     if source.has_bias: recons_keys += ["bias"]
+    r_device = packed_dict[source.key + ".q_weight"].device
+    recons_linear.set_device_idx(r_device.index)
     for k in recons_keys:
-        recons_dict[k] = packed_dict[source.key + "." + k]
+        recons_dict[k] = packed_dict[source.key + "." + k].to(r_device)
     recons_dict["q_perm"] = torch.argsort(recons_dict["q_invperm"]).to(torch.int)
-    recons_linear.load(recons_dict)
+    recons_linear.load(recons_dict, device_tensors = False)
 
     # Sanity test to ensure reconstructed matrix matches unpacked matrix
 
     quant_w = source.linear.weight.T
     recons_w = recons_linear.get_weight_tensor_dq()
 
-    if quant_w.numel() <= 1e9:
-        ident = torch.eye(recons_linear.in_features, dtype = torch.half).cuda()
-        recons_w2 = recons_linear.forward(ident, force_cuda = True)
-        recons_w2.sub_(quant_w)
-        if recons_linear.has_bias: recons_w2.sub_(recons_dict["bias"])
-        recons_w2.abs_()
-        diff2 = torch.max(recons_w2)
-    else:
+    try:
+        if quant_w.numel() <= 1e9:
+            ident = torch.eye(recons_linear.in_features, dtype = torch.half, device = r_device)
+            recons_w2 = recons_linear.forward(ident, force_cuda = True)
+            recons_w2.sub_(quant_w)
+            if recons_linear.has_bias: recons_w2.sub_(recons_dict["bias"])
+            recons_w2.abs_()
+            diff2 = torch.max(recons_w2)
+        else:
+            diff2 = 0
+    except torch.cuda.OutOfMemoryError as e:
+        print(f" !! Warning, not enough VRAM for second sanity check of {source.key}")
         diff2 = 0
 
     quant_w.sub_(recons_w)
     quant_w.abs_()
     diff1 = torch.max(quant_w)
     quant_w = None
 
@@ -116,15 +122,15 @@
 
     # Free reconstructed linear layer
 
     recons_linear.unload()
 
     # Apply reconstructed matrix to source layer
 
-    source.linear.weight.data = recons_w.T
+    source.linear.weight.data = recons_w.T.to("cuda:0")
 
 
 def quant_attn(job, module, hidden_states, target_states, quantizers, attn_params, strat):
 
     quantizers["q_proj"].prepare()
     quantizers["k_proj"].reuse_h(quantizers["q_proj"])
     quantizers["v_proj"].reuse_h(quantizers["q_proj"])
@@ -242,15 +248,17 @@
 #
 #     xx = 0
 
 
 @torch.inference_mode()
 def quant(job, save_fn, model):
 
-    snapshot_interval = 10
+    last_snapshot_time = time.time()
+    snapshot_interval_s = 90
+
     temp_filename = os.path.join(job["out_dir"], "hidden_states_temp.safetensors")
     states_filename = os.path.join(job["out_dir"], "hidden_states.safetensors")
     strategy = job["strategy"]
 
     # Quantize
 
     if not "q_last_module_idx" in job:
@@ -408,23 +416,25 @@
             quant_lm_head(job, module, hidden_states, quantizers, attn_params, rtn)
 
         if mode == "parallel_decoder":
             strat_attn = strategy[module.key + ".self_attn"]
             strat_mlp = strategy[module.key + ".mlp"]
             quant_parallel_decoder(job, module, hidden_states, target_states, quantizers, attn_params, strat_attn, strat_mlp)
 
+        torch.cuda.synchronize()
         quantizers.clear()
         gc.collect()
         torch.cuda.empty_cache()
 
         # Post-quantization forward pass
 
         if mode == "linear":
             with safe_open(job["cal_filename"], framework = "pt", device = "cpu") as f:
                 cal_ids = f.get_tensor("input_ids")
+            module.linear.weight.data = module.linear.weight.data.to("cuda:0")
 
         rfn_sum = 0
         rfn_count = 0
         logprob_sum = 0.0
         logprob_count = 0
 
         q_states = []
@@ -490,15 +500,18 @@
             # hidden_states = target_states
             # hidden_states = [(x + y) / 2 for x, y in zip(target_states, q_states)]
             hidden_states = q_states
             q_states = None
 
         # Checkpoint
 
-        if index % snapshot_interval == 0 or index == len(model.modules) - 1:
+        time_since_snapshot = time.time() - last_snapshot_time
+        if time_since_snapshot > snapshot_interval_s or index == len(model.modules) - 1:
+
+            print(" -- Saving checkpoint...")
 
             if mode != "linear":
                 save_dict = {f"row.{idx:05}": h for idx, h in enumerate(hidden_states)}
                 # save_dict.update( {f"i_row.{idx:05}": h for idx, h in enumerate(hidden_i_states)} )
                 save_file(save_dict, temp_filename)
                 save_dict = None
 
@@ -508,7 +521,9 @@
             if mode != "linear":
                 os.replace(temp_filename, states_filename)
 
             job["q_last_module_idx"] = index
 
             del job["invalid"]
             save_fn()
+
+            time_since_snapshot = time.time()
```

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/c4.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/c4.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/code.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/code.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/multilingual.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/multilingual.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/technical.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/technical.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/tiny.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/tiny.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/standard_cal_data/wiki.utf8` & `exl2conv-0.0.17.1/exl2conv/conversion/standard_cal_data/wiki.utf8`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/conversion/tokenize.py` & `exl2conv-0.0.17.1/exl2conv/conversion/tokenize.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/embedding.py` & `exl2conv-0.0.17.1/exl2conv/embedding.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/avx_mathfun.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/avx_mathfun.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,16 @@
 #ifndef _avx_mathfun_h
 #define _avx_mathfun_h
 
 #ifndef __linux__
 #include <intrin.h>
 #endif
+#include <immintrin.h>
 
-bool avx2_check = false;
-bool avx2_supported = false;
-
-bool is_avx2_supported()
-{
-    if (avx2_check)
-        return avx2_supported;
-#ifdef __linux__
-    avx2_supported = __builtin_cpu_supports("avx2");
-#else
-    int cpuInfo[4];
-    __cpuidex(cpuInfo, 7, 0);
-    avx2_supported = (cpuInfo[1] & (1 << 5)) != 0;
-#endif
-    avx2_check = true;
-//    if (avx2_supported) printf("AVX2 supported\n");
-//    else printf("AVX2 not supported\n");
-    return avx2_supported;
-}
+#include "avx2_target.h"
 
 /*
    AVX implementation of sin, cos, sincos, exp and log
 
    Based on "sse_mathfun.h", by Julien Pommier
    http://gruntthepeon.free.fr/ssemath/
 
@@ -119,33 +102,58 @@
 _PS256_CONST(cephes_log_p7, - 2.4999993993E-1);
 _PS256_CONST(cephes_log_p8, + 3.3333331174E-1);
 _PS256_CONST(cephes_log_q1, -2.12194440e-4);
 _PS256_CONST(cephes_log_q2, 0.693359375);
 
 #ifndef __AVX2__
 
-typedef union imm_xmm_union {
-  v8si imm;
-  v4si xmm[2];
-} imm_xmm_union;
-
-#define COPY_IMM_TO_XMM(imm_, xmm0_, xmm1_) {    \
-    imm_xmm_union u __attribute__((aligned(32)));  \
-    u.imm = imm_;				   \
-    xmm0_ = u.xmm[0];                            \
-    xmm1_ = u.xmm[1];                            \
-}
+#ifdef __linux__
+
+    typedef union imm_xmm_union {
+      v8si imm;
+      v4si xmm[2];
+    } imm_xmm_union;
+
+    #define COPY_IMM_TO_XMM(imm_, xmm0_, xmm1_) {    \
+        imm_xmm_union u __attribute__((aligned(32)));  \
+        u.imm = imm_;				   \
+        xmm0_ = u.xmm[0];                            \
+        xmm1_ = u.xmm[1];                            \
+    }
+
+    #define COPY_XMM_TO_IMM(xmm0_, xmm1_, imm_) {                       \
+        imm_xmm_union u __attribute__((aligned(32))); \
+        u.xmm[0]=xmm0_; u.xmm[1]=xmm1_; imm_ = u.imm; \
+    }
 
-#define COPY_XMM_TO_IMM(xmm0_, xmm1_, imm_) {                       \
-    imm_xmm_union u __attribute__((aligned(32))); \
-    u.xmm[0]=xmm0_; u.xmm[1]=xmm1_; imm_ = u.imm; \
-  }
+#else
+
+    typedef union imm_xmm_union {
+        __m256i imm;
+        __m128i xmm[2];
+    } imm_xmm_union;
+
+    #define COPY_IMM_TO_XMM(imm_, xmm0_, xmm1_) { \
+        imm_xmm_union u;                          \
+        u.imm = imm_;                             \
+        xmm0_ = u.xmm[0];                         \
+        xmm1_ = u.xmm[1];                         \
+    }
+
+    #define COPY_XMM_TO_IMM(xmm0_, xmm1_, imm_) { \
+        imm_xmm_union u;                          \
+        u.xmm[0] = xmm0_;                         \
+        u.xmm[1] = xmm1_;                         \
+        imm_ = u.imm;                             \
+    }
 
+#endif
 
 #define AVX2_BITOP_USING_SSE2(fn) \
+AVX2_TARGET \
 static inline v8si avx2_mm256_##fn(v8si x, int a) \
 { \
   /* use SSE2 instruction to perform the bitop AVX2 */ \
   v4si x1, x2; \
   v8si ret; \
   COPY_IMM_TO_XMM(x, x1, x2); \
   x1 = _mm_##fn(x1,a); \
@@ -155,14 +163,15 @@
 }
 
 //#warning "Using SSE2 to perform AVX2 bitshift ops"
 AVX2_BITOP_USING_SSE2(slli_epi32)
 AVX2_BITOP_USING_SSE2(srli_epi32)
 
 #define AVX2_INTOP_USING_SSE2(fn) \
+AVX2_TARGET \
 static inline v8si avx2_mm256_##fn(v8si x, v8si y) \
 { \
   /* use SSE2 instructions to perform the AVX2 integer operation */ \
   v4si x1, x2; \
   v4si y1, y2; \
   v8si ret; \
   COPY_IMM_TO_XMM(x, x1, x2); \
@@ -191,14 +200,15 @@
 #define avx2_mm256_add_epi32 _mm256_add_epi32
 #endif /* __AVX2__ */
 
 
 /* natural logarithm computed for 8 simultaneous float 
    return NaN for x <= 0
 */
+AVX2_TARGET
 v8sf log256_ps(v8sf x) {
   v8si imm0;
   v8sf one = *(v8sf*)_ps256_1;
 
   //v8sf invalid_mask = _mm256_cmple_ps(x, _mm256_setzero_ps());
   v8sf invalid_mask = _mm256_cmp_ps(x, _mm256_setzero_ps(), _CMP_LE_OS);
 
@@ -277,14 +287,15 @@
 _PS256_CONST(cephes_exp_p0, 1.9875691500E-4);
 _PS256_CONST(cephes_exp_p1, 1.3981999507E-3);
 _PS256_CONST(cephes_exp_p2, 8.3334519073E-3);
 _PS256_CONST(cephes_exp_p3, 4.1665795894E-2);
 _PS256_CONST(cephes_exp_p4, 1.6666665459E-1);
 _PS256_CONST(cephes_exp_p5, 5.0000001201E-1);
 
+AVX2_TARGET
 v8sf exp256_ps(v8sf x) {
   v8sf tmp = _mm256_setzero_ps(), fx;
   v8si imm0;
   v8sf one = *(v8sf*)_ps256_1;
 
   x = _mm256_min_ps(x, *(v8sf*)_ps256_exp_hi);
   x = _mm256_max_ps(x, *(v8sf*)_ps256_exp_lo);
@@ -357,14 +368,15 @@
    -- it does not return garbage for arguments over 8192, though, but
    the extra precision is missing).
 
    Note that it is such that sinf((float)M_PI) = 8.74e-8, which is the
    surprising but correct result.
 
 */
+AVX2_TARGET
 v8sf sin256_ps(v8sf x) { // any x
   v8sf xmm1, xmm2 = _mm256_setzero_ps(), xmm3, sign_bit, y;
   v8si imm0, imm2;
 
 #ifndef __AVX2__
   v4si imm0_1, imm0_2;
   v4si imm2_1, imm2_2;
@@ -484,14 +496,15 @@
   /* update the sign */
   y = _mm256_xor_ps(y, sign_bit);
 
   return y;
 }
 
 /* almost the same as sin_ps */
+AVX2_TARGET
 v8sf cos256_ps(v8sf x) { // any x
   v8sf xmm1, xmm2 = _mm256_setzero_ps(), xmm3, y;
   v8si imm0, imm2;
 
 #ifndef __AVX2__
   v4si imm0_1, imm0_2;
   v4si imm2_1, imm2_2;
@@ -601,14 +614,15 @@
   y = _mm256_xor_ps(y, sign_bit);
 
   return y;
 }
 
 /* since sin256_ps and cos256_ps are almost identical, sincos256_ps could replace both of them..
    it is almost as fast, and gives you a free cosine with your sine */
+AVX2_TARGET
 void sincos256_ps(v8sf x, v8sf *s, v8sf *c) {
 
   v8sf xmm1, xmm2, xmm3 = _mm256_setzero_ps(), sign_bit_sin, y;
   v8si imm0, imm2, imm4;
 
 #ifndef __AVX2__
   v4si imm0_1, imm0_2;
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/quantize_func.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/quantize_func.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include "quantize_func.h"
 #include "../cuda/quantize.cuh"
+#include <c10/cuda/CUDAGuard.h>
 
 void quantize_range
 (
     torch::Tensor quant,
     torch::Tensor scale,
     torch::Tensor out_q,
     float qzero,
@@ -15,14 +16,16 @@
     int b
 )
 {
     int columns = weights.size(1);
     int hcolumns = hessian_inv.size(1);
     TORCH_CHECK(hcolumns == weights.size(0), "H shape mismatch")
 
+    const at::cuda::OptionalCUDAGuard device_guard(device_of(weights));
+
     for (int c = a; c < b; c++)
     {
         fused_quantize_adjust_cuda
         (
             (const float*) weights.data_ptr(),
             (float*) quant.data_ptr(),
             (const float*) scale.data_ptr(),
@@ -61,14 +64,16 @@
     int a,
     int b
 )
 {
     int columns = weights.size(1);
     int rows = weights.size(0);
 
+    const at::cuda::OptionalCUDAGuard device_guard(device_of(weights));
+
     for (int c = a; c < b; c++)
     {
         quantize_rtn_cuda
         (
             (float*) weights.data_ptr(),
             (const float*) scale.data_ptr(),
             out_q.device().is_meta() ? NULL : (uint16_t*) out_q.data_ptr(),
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/quantize_func.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/quantize_func.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/safetensors.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/safetensors.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/safetensors.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/safetensors.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/sampling.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,26 @@
 #include "sampling.h"
 #include "util.h"
 #include "algorithm"
 #include <math.h>
 #include <vector>
 #include <queue>
 #include <utility>
-#include <chrono>
-#include <map>
-#include <string>
-
-#define USE_AVX2
-//#define PROFILING
-
-#ifdef USE_AVX2
-#include "avx_mathfun.h"
-#endif
-
-struct ProfileItem
-{
-    uint64_t min;
-    uint64_t max;
-    uint64_t total;
-    uint64_t count;
-};
-
-std::map<std::string, ProfileItem> all_stages = {};
-std::string current_stage = "";
-std::chrono::time_point<std::chrono::high_resolution_clock> stage_start;
-
-inline void profile_start(std::string stage)
-{
-#ifdef PROFILING
-    current_stage = stage;
-    stage_start = std::chrono::high_resolution_clock::now();
-#endif
-}
-
-inline void profile_stop()
-{
-#ifdef PROFILING
-    auto stage_stop = std::chrono::high_resolution_clock::now();
-    uint64_t duration = std::chrono::duration_cast<std::chrono::microseconds>(stage_stop - stage_start).count();
-    auto r = all_stages.find(current_stage);
-    if (r == all_stages.end())
-    {
-        ProfileItem item;
-        item.min = duration;
-        item.max = duration;
-        item.total = duration;
-        item.count = 1;
-        all_stages[current_stage] = item;
-    }
-    else
-    {
-        ProfileItem* item = &(r->second);
-        item->total += duration;
-        item->min = std::min(item->min, duration);
-        item->max = std::max(item->max, duration);
-        item->count++;
-    }
-#endif
-}
-
-void profile_results()
-{
-#ifdef PROFILING
-    printf("stage                               total             min             max            mean\n");
-    printf("-----------------------------------------------------------------------------------------\n");
-    for (const auto& entry : all_stages)
-    {
-        printf("%26s %11llu us  %11llu us  %11llu us  %11llu us\n", entry.first.c_str(), entry.second.total, entry.second.min, entry.second.max, entry.second.total / entry.second.count);
-    }
-#endif
-}
+#include "avx2_target.h"
+#include "sampling_avx2.h"
+#include "profiling.h"
 
 const int top_k_heap_threshold = 500;
 
 bool* g_rep_mask = NULL;
 int g_vocab_size = 0;
 
+// Repetition penalty
+
+AVX2_TARGET_OPTIONAL
 void apply_rep_penalty_cpu
 (
     const int vocab_size,
     const uint64_t* sequence,
     const float penalty_max,
     const int sustain,
     const int decay,
@@ -163,128 +101,15 @@
             pres_p += d_pres_p;
         }
     }
 
     profile_stop();
 }
 
-void softmax_cpu_avx2
-(
-    const int vocab_size,
-    const float temperature,
-    const float* logits,
-    const bool* logits_filter,
-    const float exponent,
-    float* output
-)
-{
-    profile_start("softmax_cpu (AVX2)");
-
-    int vocab_size_aligned = ((vocab_size + 31) / 32) * 32;
-    float esum = 0.0f;
-    float itemp = 1.0f / temperature;
-    const float minf = -1e38;
-    float maxl = minf;
-
-    // Apply logit filter and find max logit
-
-    int i = 0;
-    for (; i < vocab_size; ++i)
-    {
-        float l = logits[i];
-        bool f = logits_filter[i];
-        l = f ? l : minf;
-        maxl = fmaxf(l, maxl);
-        output[i] = l;
-    }
-    for (; i < vocab_size_aligned; i++)
-        output[i] = minf;
-
-    // SIMD values
-
-    __m256 maxl8  = _mm256_set1_ps(maxl);
-    __m256 itemp8 = _mm256_set1_ps(itemp);
-    __m256 esum8  = _mm256_set1_ps(esum);
-
-    // Apply temperature, exponentiate and compute exponential sum
-
-    if (exponent == 2.0f)
-    {
-        __m256 sign_mask = _mm256_set1_ps(-0.0f);
-        i = 0;
-        for (; i < vocab_size_aligned; i += 8)
-        {
-            __m256 x = _mm256_load_ps(&output[i]);
-            x = _mm256_sub_ps(x, maxl8);
-            x = _mm256_mul_ps(x, x);
-            x = _mm256_xor_ps(x, sign_mask);
-            x = _mm256_mul_ps(x, itemp8);
-            x = exp256_ps(x);
-            _mm256_store_ps(&output[i], x);
-            esum8 = _mm256_add_ps(esum8, x);
-        }
-    }
-    else if (exponent != 1.0f)
-    {
-        // TODO: SIMD version of this
-        for (int i = 0; i < vocab_size_aligned; i++)
-        {
-            float l = output[i] - maxl;
-            l = -powf(fabs(l), exponent);
-            float e = expf(l * itemp);
-            output[i] = e;
-            esum += e;
-        }
-    }
-    else
-    {
-        i = 0;
-        for (; i < vocab_size_aligned; i += 8)
-        {
-            __m256 x = _mm256_load_ps(&output[i]);
-            x = _mm256_sub_ps(x, maxl8);
-            x = _mm256_mul_ps(x, itemp8);
-            x = exp256_ps(x);
-            _mm256_store_ps(&output[i], x);
-            esum8 = _mm256_add_ps(esum8, x);
-        }
-    }
-
-    // Normalize
-
-    float xv[8];
-    _mm256_store_ps(xv, esum8);
-    for (int k = 0; k < 8; ++k) esum += xv[k];
-    float isum = 1.0f / esum;
-    __m256 isum8  = _mm256_set1_ps(isum);
-
-    i = 0;
-    for (; i < vocab_size_aligned; i += 8)
-    {
-        __m256 x = _mm256_load_ps(&output[i]);
-        x = _mm256_mul_ps(x, isum8);
-        _mm256_store_ps(&output[i], x);
-    }
-
-    profile_stop();
-
-//    printf("Softmax:");
-//    float summ = 0.0f;
-//    for (int i = 0; i < vocab_size; i++)
-//    {
-//        if (logits_filter[i])
-//        {
-//            summ += output[i];
-//            if (output[i] < 1e-5) continue;
-//            printf("%d, %f\n", i, output[i]);
-//        }
-//    }
-//    printf("sum: %f\n\n", summ);
-}
-
+AVX2_TARGET_OPTIONAL
 void softmax_cpu_nonavx2
 (
     const int vocab_size,
     const float temperature,
     const float* logits,
     const bool* logits_filter,
     const float exponent,
@@ -346,22 +171,21 @@
     const float temperature,
     const float* logits,
     const bool* logits_filter,
     const float exponent,
     float* output
 )
 {
-#ifdef USE_AVX2
     if (is_avx2_supported())
         return softmax_cpu_avx2(vocab_size, temperature, logits, logits_filter, exponent, output);
-#endif
-
-    return softmax_cpu_nonavx2(vocab_size, temperature, logits, logits_filter, exponent, output);
+    else
+        return softmax_cpu_nonavx2(vocab_size, temperature, logits, logits_filter, exponent, output);
 }
 
+AVX2_TARGET_OPTIONAL
 int post_softmax_temperature
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float temperature,
     float min_temp = 0,
@@ -423,14 +247,15 @@
 //        DBGIF(i, temp_probs[i]);
 //    printf("\n");
 
     profile_stop();
     return num_candidates;
 }
 
+AVX2_TARGET_OPTIONAL
 void normalize_cpu
 (
     const int num_candidates,
     float* probs
 )
 {
     profile_start("normalize_cpu");
@@ -460,14 +285,15 @@
 
 inline bool cmp_desc(const float& a, const float& b)
 {
     return a < b;
 }
 
 template <bool (*cmp_func)(const float&, const float&)>
+AVX2_TARGET_OPTIONAL
 void quicksort_with_idx
 (
     float* arr,
     int* idx,
     int low,
     int high,
     int max_index
@@ -555,14 +381,15 @@
         quicksort_with_idx<cmp_func>(arr, idx, low, pos - 1, max_index);
     if (max_index == 0 || pos <= max_index)
         quicksort_with_idx<cmp_func>(arr, idx, pos + 1, high, max_index);
 }
 
 // Discard tiny probabilities, improves performance when temperature is very low
 
+AVX2_TARGET_OPTIONAL
 int pre_sort_descending
 (
     const int num_candidates,
     float* arr,
     int* idx
 )
 {
@@ -579,14 +406,15 @@
         i++;
         j--;
     }
 
     return i;
 }
 
+AVX2_TARGET_OPTIONAL
 int sort_descending
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     int max_index
 )
@@ -597,14 +425,15 @@
 //    int m = (max_index == 0 ? num_candidates : max_index);
 //    for (int i = 0; i < m; i++) printf("%i - %f \n", temp_indices[i], temp_probs[i] * 10000.0);
 //    for (int i = 0; i < m - 1; i++) if (temp_probs[i] < temp_probs[i + 1] - 2e-8) DBGI(i);
 
     return pre;
 }
 
+AVX2_TARGET_OPTIONAL
 int top_k_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     int top_k
 )
@@ -665,14 +494,15 @@
         sort_descending(num_candidates, temp_probs, temp_indices, top_k);
     }
 
     profile_stop();
     return top_k;
 }
 
+AVX2_TARGET_OPTIONAL
 int top_p_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float top_p
 )
@@ -709,14 +539,15 @@
         min_heap.pop();
     }
 
     profile_stop();
     return k;
 }
 
+AVX2_TARGET_OPTIONAL
 int keep_threshold
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float threshold
 )
@@ -759,14 +590,15 @@
     // Use the keep_threshold function to keep only probabilities above the threshold
     int n = keep_threshold(num_candidates, temp_probs, temp_indices, threshold);
 
     profile_stop();
     return n;
 }
 
+AVX2_TARGET_OPTIONAL
 int min_p_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float min_p
 )
@@ -780,14 +612,15 @@
     float threshold = top_prob * min_p;
     int n = keep_threshold(num_candidates, temp_probs, temp_indices, threshold);
 
     profile_stop();
     return n;
 }
 
+AVX2_TARGET_OPTIONAL
 int tfs_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float tfs
 )
@@ -828,14 +661,15 @@
     //TIME_STOP;
 
     free(derivative);
     profile_stop();
     return k;
 }
 
+AVX2_TARGET_OPTIONAL
 int mirostat_pre_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float mirostat_mu,
     float mirostat_tau,
@@ -884,14 +718,15 @@
     float observed_surprise = -log2(temp_probs[0]);
     mu += mirostat_eta * (mirostat_tau - observed_surprise);
 
     profile_stop();
     return mu;
 }
 
+AVX2_TARGET_OPTIONAL
 int typical_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float typical
 )
@@ -948,14 +783,15 @@
 
     if (num == 0) num = 1;
 
     profile_stop();
     return num;
 }
 
+AVX2_TARGET_OPTIONAL
 int multinomial_cpu
 (
     const int num_candidates,
     float* temp_probs,
     int* temp_indices,
     float random
 )
@@ -984,10 +820,8 @@
     }
 
     swap<float>(temp_probs[0], temp_probs[idx]);
     swap<int>(temp_indices[0], temp_indices[idx]);
 
     profile_stop();
     return 1;
-}
-
-
+}
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/sampling.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/sampling.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #ifndef _sampling_h
 #define _sampling_h
 
 #include <cstdlib>
 #include <cstring>
 #include <cstdint>
 #include <cstdio>
+#include <string>
 
 void profile_results();
+void profile_start(std::string stage);
+void profile_stop();
 
 void apply_rep_penalty_cpu
 (
     const int vocab_size,
     const uint64_t* sequence,
     const float penalty_max,
     const int sustain,
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cpp/util.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cpp/util.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/cache.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/cache.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/cache.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/cache.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/compat.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/compat.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_add.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_add.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_gemm.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_gemm.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/h_gemm.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/h_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/layer_norm.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/layer_norm.cu`

 * *Files 14% similar despite different names*

```diff
@@ -141,24 +141,35 @@
         half2 nh = __halves2half2(__float2half_rn(n0), __float2half_rn(n1));
         if (b) nh = __hadd2(nh, b2[column]);  // Optional bias
 
         y_row[column] = nh;
     }
 }
 
+#define kernel_instance(bpw) \
+    if (blocks_per_warp == bpw) return layer_norm_kernel<bpw>
+
 fp_layer_norm_kernel pick_layer_norm_kernel(const int blocks_per_warp)
 {
-    if (blocks_per_warp == 1) return layer_norm_kernel<1>;
-    if (blocks_per_warp == 2) return layer_norm_kernel<2>;
-    if (blocks_per_warp == 3) return layer_norm_kernel<3>;
-    if (blocks_per_warp == 4) return layer_norm_kernel<4>;
-    if (blocks_per_warp == 5) return layer_norm_kernel<5>;
-    if (blocks_per_warp == 6) return layer_norm_kernel<6>;
-    if (blocks_per_warp == 7) return layer_norm_kernel<7>;
-    if (blocks_per_warp == 8) return layer_norm_kernel<8>;
+    kernel_instance(1);
+    kernel_instance(2);
+    kernel_instance(3);
+    kernel_instance(4);
+    kernel_instance(5);
+    kernel_instance(6);
+    kernel_instance(7);
+    kernel_instance(8);
+    kernel_instance(9);
+    kernel_instance(10);
+    kernel_instance(11);
+    kernel_instance(12);
+    kernel_instance(13);
+    kernel_instance(14);
+    kernel_instance(15);
+    kernel_instance(16);
 	return NULL;
 }
 
 void layer_norm_cuda
 (
     const half* x,
     const half* w,
@@ -173,11 +184,11 @@
     blockDim.x = NUM_THREADS;
     blockDim.y = 1;
     gridDim.x = rows;
     gridDim.y = 1;
 
     float r_dim = 1.0f / (float) dim;
 
-    int blocks_per_warp = DIVIDE(dim, NUM_THREADS);
+    int blocks_per_warp = DIVIDE(dim, NUM_THREADS * 2);
     fp_layer_norm_kernel kernel = pick_layer_norm_kernel(blocks_per_warp);
     kernel<<<gridDim, blockDim>>>(x, w, b, y, epsilon, r_dim, rows, dim);
 }
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/lora.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/lora.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/matrix_view.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/matrix_view.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/pack_tensor.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/pack_tensor.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/pack_tensor.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_attn.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_attn.cu`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "q_attn.cuh"
 #include "q_gemm.cuh"
 #include "rms_norm.cuh"
 #include "layer_norm.cuh"
+#include "head_norm.cuh"
 #include "rope.cuh"
 #include "util.cuh"
 #include "lora.cuh"
 
 const int THREADS_X = 32;
 const int THREADS_Y = 1;
 const int THREADS_Z = 4;
@@ -86,15 +87,17 @@
     int _max_rows,
     int _hidden_size,
     int _num_heads,
     int _num_kv_heads,
     int _head_dim,
     int _max_seq_len,
     bool _has_residual,
-    bool _neox_style
+    bool _neox_style,
+    half* _q_norm,
+    half* _k_norm
 ):
     layernorm(_layernorm),
     layernorm_bias(_layernorm_bias),
     layernorm_is_rms(_layernorm_is_rms),
     norm_epsilon(_norm_epsilon),
     q_proj(_q_proj),
     k_proj(_k_proj),
@@ -108,15 +111,17 @@
     max_rows(_max_rows),
     hidden_size(_hidden_size),
     num_heads(_num_heads),
     num_kv_heads(_num_kv_heads),
     head_dim(_head_dim),
     max_seq_len(_max_seq_len),
     has_residual(_has_residual),
-    neox_style(_neox_style)
+    neox_style(_neox_style),
+    q_norm(_q_norm),
+    k_norm(_k_norm)
 {
 }
 
 QAttn::~QAttn()
 {
 }
 
@@ -148,14 +153,20 @@
         norm_state = temp_state;
     }
 
     gemm_half_q_half_cuda(cublas_handle, norm_state, q_proj, temp_q, q_len * batch_size, q_proj->width, hidden_size, true, temp_dq);
     gemm_half_q_half_cuda(cublas_handle, norm_state, k_proj, temp_k, q_len * batch_size, k_proj->width, hidden_size, true, temp_dq);
     gemm_half_q_half_cuda(cublas_handle, norm_state, v_proj, temp_v, q_len * batch_size, v_proj->width, hidden_size, true, temp_dq);
 
+    if (q_norm)
+        head_norm_cuda(temp_q, q_norm, NULL, temp_q, norm_epsilon, q_len * batch_size, num_heads, head_dim);
+
+    if (k_norm)
+        head_norm_cuda(temp_k, k_norm, NULL, temp_k, norm_epsilon, q_len * batch_size, num_kv_heads, head_dim);
+
     apply_loras_cuda(cublas_handle, q_proj_lora, loras, q_proj, norm_state, temp_q, lora_temp, q_len * batch_size);
     apply_loras_cuda(cublas_handle, k_proj_lora, loras, k_proj, norm_state, temp_k, lora_temp, q_len * batch_size);
     apply_loras_cuda(cublas_handle, v_proj_lora, loras, v_proj, norm_state, temp_v, lora_temp, q_len * batch_size);
 
 //    rope_cuda(temp_q, sin, cos, batch_size, q_len * num_heads,    head_dim, num_heads,    past_len, past_lens);
 //    rope_cuda(temp_k, sin, cos, batch_size, q_len * num_kv_heads, head_dim, num_kv_heads, past_len, past_lens);
     rope_cuda_qk
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_attn.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_attn.cuh`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 public:
 
     half* layernorm;
     half* layernorm_bias;
     bool layernorm_is_rms;
     float norm_epsilon;
 
+    half* q_norm;
+    half* k_norm;
+
     QMatrix* q_proj;
     QMatrix* k_proj;
     QMatrix* v_proj;
     QMatrix* o_proj;
 
     half* temp_state;
 //     half* temp_q;
@@ -63,15 +66,17 @@
         int _max_rows,
         int _hidden_size,
         int _num_heads,
         int _num_kv_heads,
         int _head_dim,
         int _max_seq_len,
         bool _has_residual,
-        bool _neox_style
+        bool _neox_style,
+        half* _q_norm,
+        half* _k_norm
     );
 
     ~QAttn();
 
     void forward_cuda_1
     (
         cublasHandle_t cublas_handle,
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm.cu`

 * *Files 2% similar despite different names*

```diff
@@ -199,32 +199,57 @@
     half* temp_dq,
     bool force_cuda,
     const half* r_weights,
     const int r_weights_stride,
     bool mul_r_weights
 )
 {
-    if (size_m > MAX_Q_GEMM_ROWS && !force_cuda)
+    // Here we force CUDA matmul for matrices that are too big to dequantize. This is necessary for the
+    // extremely large output layers of some models. Splitting along K and dequantizing/multiplying in
+    // chunks would work also except the remapping of EXL2 matrices complicates it.
+    //
+    // TODO: Finish the chunking stuff
+
+    int row_step = (b->max_dq_rows / 128) * 128;
+
+    if (size_m > MAX_Q_GEMM_ROWS && !force_cuda && size_k <= row_step)
     {
-        // Reconstruct FP16 matrix, then cuBLAS
+        int row_b = 0;
+        if (row_step == 0) row_step = size_k;
+
+        while (row_b < size_k)
+        {
+            int row_a = row_b;
+            row_b += row_step;
+            row_b = min(row_b, size_k);
+            int chunk_k = row_b - row_a;
+
+            // Reconstruct FP16 matrix, then cuBLAS
 
-        if (!temp_dq) temp_dq = b->temp_dq;
-        b->reconstruct(temp_dq);
+            if (!temp_dq) temp_dq = b->temp_dq;
+            b->reconstruct(temp_dq, row_a, row_b);
 
-        //cublasSetMathMode(cublas_handle, CUBLAS_TENSOR_OP_MATH);
+            const half alpha = __float2half(1.0f);
+            const half beta = (clear && row_a == 0) ? __float2half(0.0f) : __float2half(1.0f);
+            cublasHgemm(cublas_handle,
+                        CUBLAS_OP_N,
+                        CUBLAS_OP_N,
+                        size_n, size_m, chunk_k,
+                        &alpha, temp_dq,   size_n,
+                                a + row_a, size_k,
+                        &beta,  c,         size_n);
 
-        const half alpha = __float2half(1.0f);
-        const half beta = clear ? __float2half(0.0f) : __float2half(1.0f);
-        cublasHgemm(cublas_handle,
-                    CUBLAS_OP_N,
-                    CUBLAS_OP_N,
-                    size_n, size_m, size_k,
-                    &alpha, temp_dq, size_n,
-                            a,       size_k,
-                    &beta,  c,       size_n);
+//            cublasHgemm(cublas_handle,
+//                        CUBLAS_OP_N,
+//                        CUBLAS_OP_N,
+//                        size_n, size_m, size_k,
+//                        &alpha, temp_dq, size_n,
+//                                a,       size_k,
+//                        &beta,  c,       size_n);
+        }
 
         //const float alpha = 1.0f;
         //const float beta = clear ? 0.0f : 1.0f;
         //cublasSgemmEx(cublas_handle,
         //             CUBLAS_OP_N,
         //             CUBLAS_OP_N,
         //             size_n, size_m, size_k,
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_autotune.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_kernel.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_gemm_kernel_gptq.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_matrix.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_matrix.cu`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,23 @@
 
     uint32_t* _gptq_qzeros,
     half* _gptq_scales,
     uint32_t* _gptq_g_idx,
 
     half* _bias,
 
-    half* _temp_dq
+    half* _temp_dq,
+    const int _max_dq_rows
 ) :
     device(_device),
     height(_height),
     width(_width),
     groups(_groups),
-    temp_dq(_temp_dq)
+    temp_dq(_temp_dq),
+    max_dq_rows(_max_dq_rows)
 {
     cudaSetDevice(device);
 
     failed = false;
 
     cuda_q_weight = _q_weight;
     cuda_q_perm = _q_perm;
@@ -193,15 +195,17 @@
     const half* __restrict__ b_gptq_scales,
     //const uint16_t* __restrict__ b_q_groups,
     const int size_k,
     const int size_n,
     const int groupsize,
     const int groups,
     half* __restrict__ b,
-    const int rows_4
+    const int rows_4,
+    const int row_a,
+    const int row_b
 )
 {
     MatrixView_half_rw b_(b, size_k, size_n);
     MatrixView_q4_row b_gptq_qzeros_(b_gptq_qzeros, groups, size_n);
     MatrixView_half b_gptq_scales_(b_gptq_scales, groups, size_n);
 
     int offset_k = BLOCK_KN_SIZE * blockIdx.y;
@@ -245,16 +249,14 @@
     b_gptq_qzeros_.item4(zeros, group, n);
     b_gptq_scales_.item4_h2(scales, group, n);
     dequant_4bit_8_prep_zero(zeros[0] + 1, z1z16[0], y1y16[0]);
     dequant_4bit_8_prep_zero(zeros[1] + 1, z1z16[1], y1y16[1]);
     dequant_4bit_8_prep_zero(zeros[2] + 1, z1z16[2], y1y16[2]);
     dequant_4bit_8_prep_zero(zeros[3] + 1, z1z16[3], y1y16[3]);
 
-    __syncthreads();
-
     int k = offset_k;
     int lk = 0;
 
     while (k < end_k)
     {
         if (k == nextgroup)
         {
@@ -320,15 +322,17 @@
     const int groups,
     half* __restrict__ b,
     const int rows_8,
     const int rows_6,
     const int rows_5,
     const int rows_4,
     const int rows_3,
-    const int rows_2
+    const int rows_2,
+    const int row_a,
+    const int row_b
 )
 {
     MatrixView_half_rw b_(b, size_k, size_n);
     MatrixView_q4_row b_q_scale_(b_q_scale, groups, size_n);
 
     int offset_k = BLOCK_KN_SIZE * blockIdx.y;
     int offset_n = BLOCK_KN_SIZE * blockIdx.x;
@@ -472,20 +476,22 @@
             half* dqh = (half*) dq;
             for (int j = 0; j < 16; j++) b_.set(perm[lk++], n, dqh[j]);
         }
         k += 16;
     }
 }
 
-void QMatrix::reconstruct(half* out)
+void QMatrix::reconstruct(half* out, int row_a, int row_b)
 {
     dim3 blockDim, gridDim;
     blockDim.x = BLOCK_KN_SIZE;
     blockDim.y = 1;
-    gridDim.y = DIVIDE(height, BLOCK_KN_SIZE);
+    if (row_a == 0 && row_b == 0) row_b = height;
+
+    gridDim.y = DIVIDE(row_b - row_a, BLOCK_KN_SIZE);
 
     if (!is_gptq)
     {
         gridDim.x = DIVIDE(width, BLOCK_KN_SIZE);
         reconstruct_kernel<<<gridDim, blockDim>>>
         (
             cuda_q_weight,
@@ -499,15 +505,17 @@
             groups,
             out,
             rows_8,
             rows_6,
             rows_5,
             rows_4,
             rows_3,
-            rows_2
+            rows_2,
+            row_a,
+            row_b
         );
     }
     else
     {
         gridDim.x = DIVIDE(width, BLOCK_KN_SIZE * 4);
         reconstruct_gptq_kernel<<<gridDim, blockDim>>>
         (
@@ -517,15 +525,17 @@
             cuda_gptq_scales,
             //const uint16_t* __restrict__ b_q_groups,
             height,
             width,
             gptq_groupsize,
             groups,
             out,
-            rows_4
+            rows_4,
+            row_a,
+            row_b
         );
     }
 }
 
 __global__ void make_sequential_kernel
 (
     const uint32_t* __restrict__ w,
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_matrix.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_matrix.cuh`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     uint16_t* cuda_q_groups = NULL;
     uint16_t* cuda_q_group_map = NULL;
     uint32_t* cuda_gptq_qzeros = NULL;
     half* cuda_gptq_scales = NULL;
     half* cuda_bias = NULL;
 
     half* temp_dq;
+    int max_dq_rows;
 
     bool failed;
 
     QMatrix
     (
         const int _device,
         const int _height,
@@ -60,20 +61,21 @@
 
         uint32_t* _gptq_qzeros,
         half* _gptq_scales,
         uint32_t* _gptq_g_idx,
 
         half* bias,
 
-        half* _temp_dq
+        half* _temp_dq,
+        const int _max_dq_rows
     );
 
     ~QMatrix();
 
-    void reconstruct(half* out);
+    void reconstruct(half* out, int row_a = 0, int row_b = 0);
     bool make_sequential(const uint32_t* cpu_g_idx);
 
 private:
 
 };
 
 void matrix_q4_to_fp16_cuda
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp_activation.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/q_mlp_softmax.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_2.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_3.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_4.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_5.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_6.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_8.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quant/qdq_util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quantize.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quantize.cu`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     float qzero,                                // 2^(bits - 1)
     float maxq                                  // (2^bits) - 1
 )
 {
     int column = blockIdx.x * blockDim.x + threadIdx.x;
     if (column >= columns) return;
 
-    int idx = row * columns + column;
+    uint64_t idx = (uint64_t)row * (uint64_t)columns + (uint64_t)column;
 
     // Quantize
 
     float x = weights[idx];
     float s = scale[column];
     x /= s;
     x = rintf(x);
@@ -93,15 +93,15 @@
     float qzero,                                // 2^(bits - 1)
     float maxq                                  // (2^bits) - 1
 )
 {
     int column = blockIdx.x * blockDim.x + threadIdx.x;
     if (column >= columns) return;
 
-    int idx = row * columns + column;
+    uint64_t idx = (uint64_t)row * (uint64_t)columns + (uint64_t)column;
 
     // Quantize
 
     float x = weights[idx];
     float s = scale[column];
     x /= s;
     x = rintf(x);
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/quantize.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/quantize.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rms_norm.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rms_norm.cu`

 * *Files 16% similar despite different names*

```diff
@@ -99,24 +99,35 @@
         float w_itemf1 = __half2float(__high2half(w2_));
         float n0 = x_itemf0 * w_itemf0 * rmf;
         float n1 = x_itemf1 * w_itemf1 * rmf;
         y_row[column] = __halves2half2(__float2half_rn(n0), __float2half_rn(n1));
     }
 }
 
+#define kernel_instance(bpw) \
+    if (blocks_per_warp == bpw) return rms_norm_kernel<bpw>
+
 fp_rms_norm_kernel pick_rms_norm_kernel(const int blocks_per_warp)
 {
-    if (blocks_per_warp == 1) return rms_norm_kernel<1>;
-    if (blocks_per_warp == 2) return rms_norm_kernel<2>;
-    if (blocks_per_warp == 3) return rms_norm_kernel<3>;
-    if (blocks_per_warp == 4) return rms_norm_kernel<4>;
-    if (blocks_per_warp == 5) return rms_norm_kernel<5>;
-    if (blocks_per_warp == 6) return rms_norm_kernel<6>;
-    if (blocks_per_warp == 7) return rms_norm_kernel<7>;
-    if (blocks_per_warp == 8) return rms_norm_kernel<8>;
+    kernel_instance(1);
+    kernel_instance(2);
+    kernel_instance(3);
+    kernel_instance(4);
+    kernel_instance(5);
+    kernel_instance(6);
+    kernel_instance(7);
+    kernel_instance(8);
+    kernel_instance(9);
+    kernel_instance(10);
+    kernel_instance(11);
+    kernel_instance(12);
+    kernel_instance(13);
+    kernel_instance(14);
+    kernel_instance(15);
+    kernel_instance(16);
 	return NULL;
 }
 
 void rms_norm_cuda
 (
     const half* x,
     const half* w,
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rope.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rope.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/rope.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/rope.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/util.cu` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/util.cu`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/cuda/util.cuh` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/cuda/util.cuh`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_bindings.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_bindings.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -91,12 +91,14 @@
 
     // norm
 
     m.def("rms_norm", &rms_norm, "rms_norm");
     m.def("rms_norm_", &rms_norm_, "rms_norm_");
     m.def("layer_norm", &layer_norm, "layer_norm");
     m.def("layer_norm_", &layer_norm_, "layer_norm_");
+    m.def("head_norm", &head_norm, "head_norm");
+    m.def("head_norm_", &head_norm_, "head_norm_");
 
     // rope
 
     m.def("rope_", &rope_, "rope_");
 }
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_cache.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_cache.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_cache.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_cache.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_gemm.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_gemm.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_norm.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_norm.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #include <pybind11/stl.h>
 
 #include "config.h"
 #include "ext_norm.h"
 
 #include "cuda/rms_norm.cuh"
 #include "cuda/layer_norm.cuh"
+#include "cuda/head_norm.cuh"
 
 #include "cpp/util.h"
 
 
 // RMS layernorm
 
 void rms_norm
@@ -27,15 +28,14 @@
     float epsilon
 )
 {
     TORCH_CHECK_DTYPE(x, kHalf);
     TORCH_CHECK_DTYPE(w, kHalf);
     TORCH_CHECK_DTYPE(y, kHalf);
     TORCH_CHECK_SHAPES(x, 1, w, 0, 1);
-    TORCH_CHECK_SHAPES(x, 1, w, 0, 1);
     TORCH_CHECK_SHAPES(x, 0, y, 0, 1);
     TORCH_CHECK_SHAPES(x, 1, y, 1, 1);
 
     int rows = x.size(0);
     int dim = x.size(1);
 
     const at::cuda::OptionalCUDAGuard device_guard(device_of(x));
@@ -74,15 +74,14 @@
 )
 {
     TORCH_CHECK_DTYPE(x, kHalf);
     TORCH_CHECK_DTYPE(w, kHalf);
     TORCH_CHECK_DTYPE_OPT(b, kHalf);
     TORCH_CHECK_DTYPE(y, kHalf);
     TORCH_CHECK_SHAPES(x, 1, w, 0, 1);
-    TORCH_CHECK_SHAPES(x, 1, w, 0, 1);
     TORCH_CHECK_SHAPES(x, 0, y, 0, 1);
     TORCH_CHECK_SHAPES(x, 1, y, 1, 1);
     TORCH_CHECK_SHAPES_OPT(b, 0, w, 0, 1);
 
     int rows = x.size(0);
     int dim = x.size(1);
 
@@ -106,7 +105,60 @@
     torch::Tensor w,
     torch::Tensor b,
     float epsilon
 )
 {
     layer_norm(x, w, b, x, epsilon);
 }
+
+
+// Head norm
+
+void head_norm
+(
+    torch::Tensor x,
+    torch::Tensor w,
+    torch::Tensor b,
+    torch::Tensor y,
+    float epsilon
+)
+{
+    TORCH_CHECK_DTYPE(x, kHalf);
+    TORCH_CHECK_DTYPE(w, kHalf);
+    TORCH_CHECK_DTYPE_OPT(b, kHalf);
+    TORCH_CHECK_DTYPE(y, kHalf);
+    TORCH_CHECK_SHAPES(x, -1, w, -1, 1);
+    TORCH_CHECK_SHAPES(x, -2, w, -2, 1);
+    TORCH_CHECK_SHAPES(x, 0, y, 0, 1);
+    TORCH_CHECK_SHAPES(x, 1, y, 1, 1);
+    TORCH_CHECK_SHAPES_OPT(b, 0, w, 0, 1);
+    TORCH_CHECK_SHAPES_OPT(b, 1, w, 1, 1);
+
+    int head_dim = x.size(-1);
+    int num_heads = x.size(-2);
+    int rows = x.numel() / head_dim / num_heads;
+
+    const at::cuda::OptionalCUDAGuard device_guard(device_of(x));
+
+    head_norm_cuda
+    (
+        (half*) x.data_ptr(),
+        (half*) w.data_ptr(),
+        b.device().is_meta() ? NULL : (half*) b.data_ptr(),
+        (half*) y.data_ptr(),
+        epsilon,
+        rows,
+        num_heads,
+        head_dim
+    );
+}
+
+void head_norm_
+(
+    torch::Tensor x,
+    torch::Tensor w,
+    torch::Tensor b,
+    float epsilon
+)
+{
+    head_norm(x, w, b, x, epsilon);
+}
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qattn.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qattn.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     int max_rows,
     int hidden_size,
     int num_heads,
     int num_kv_heads,
     int head_dim,
     int max_seq_len,
     bool has_residual,
-    bool neox_style
+    bool neox_style,
+    torch::Tensor q_norm,
+    torch::Tensor k_norm
 )
 {
     QMatrix* qm_q_proj = reinterpret_cast<QMatrix*> (q_q_proj);
     QMatrix* qm_k_proj = reinterpret_cast<QMatrix*> (q_k_proj);
     QMatrix* qm_v_proj = reinterpret_cast<QMatrix*> (q_v_proj);
     QMatrix* qm_o_proj = reinterpret_cast<QMatrix*> (q_o_proj);
 
@@ -70,15 +72,17 @@
         max_rows,
         hidden_size,
         num_heads,
         num_kv_heads,
         head_dim,
         max_seq_len,
         has_residual,
-        neox_style
+        neox_style,
+        (half*) q_norm.is_meta() ? NULL : (half*) q_norm.data_ptr(),
+        (half*) k_norm.is_meta() ? NULL : (half*) k_norm.data_ptr()
     );
 
     return reinterpret_cast<uintptr_t> (attn);
 }
 
 void free_q_attn
 (
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qattn.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qattn.h`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     int max_rows,
     int hidden_size,
     int num_heads,
     int num_kv_heads,
     int head_dim,
     int max_seq_len,
     bool has_residual,
-    bool neox_style
+    bool neox_style,
+    torch::Tensor q_norm,
+    torch::Tensor k_norm
 );
 
 void free_q_attn
 (
     uintptr_t handle
 );
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmatrix.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmatrix.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     torch::Tensor q_scale_max,
     torch::Tensor q_groups,
     torch::Tensor q_group_map,
     torch::Tensor gptq_qzeros,
     torch::Tensor gptq_scales,
     torch::Tensor gptq_g_idx,
     torch::Tensor bias,
-    torch::Tensor temp_dq
+    torch::Tensor temp_dq,
+    int max_dq_rows
 )
 {
     TORCH_CHECK_DTYPE(q_weight, kInt);
     TORCH_CHECK_DTYPE_OPT(q_perm, kShort);
     TORCH_CHECK_DTYPE_OPT(q_invperm, kShort);
     TORCH_CHECK_DTYPE_OPT(q_scale, kInt);
     TORCH_CHECK_DTYPE_OPT(q_scale_max, kHalf);
@@ -68,15 +69,16 @@
     }
 
     if (!bias.device().is_meta())
     {
         TORCH_CHECK_SHAPES(q_weight, 1, bias, 0, 1);
     }
 
-    TORCH_CHECK(temp_dq.size(0) >= width * height, "Insufficient size of temp_dq buffer")
+    if (!temp_dq.device().is_meta())
+        TORCH_CHECK(temp_dq.size(0) >= width * height, "Insufficient size of temp_dq buffer")
 
     QMatrix* m = new QMatrix
     (
         device,
         height,
         width,
         groups,
@@ -87,15 +89,16 @@
         q_scale_max.device().is_meta() ? NULL : (half*) q_scale_max.data_ptr(),
         q_groups.device().is_meta() ? NULL : (uint16_t*) q_groups.data_ptr(),
         q_group_map.device().is_meta() ? NULL : (uint16_t*) q_group_map.data_ptr(),
         gptq_qzeros.device().is_meta() ? NULL : (uint32_t*) gptq_qzeros.data_ptr(),
         gptq_scales.device().is_meta() ? NULL : (half*) gptq_scales.data_ptr(),
         gptq_g_idx.device().is_meta() ? NULL : (uint32_t*) gptq_g_idx.data_ptr(),
         bias.device().is_meta() ? NULL : (half*) bias.data_ptr(),
-        (half*) temp_dq.data_ptr()
+        (half*) temp_dq.data_ptr(),
+        max_dq_rows
     );
 
     if (m->failed) throw std::runtime_error("CUDA out of memory");
 
     return reinterpret_cast<uintptr_t> (m);
 }
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmatrix.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmatrix.h`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     torch::Tensor q_scale_max,
     torch::Tensor q_groups,
     torch::Tensor q_group_map,
     torch::Tensor gptq_qzeros,
     torch::Tensor gptq_scales,
     torch::Tensor gptq_g_idx,
     torch::Tensor bias,
-    torch::Tensor temp_dq
+    torch::Tensor temp_dq,
+    int max_dq_rows
 );
 
 void free_q_matrix
 (
     uintptr_t handle
 );
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmlp.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmlp.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_qmlp.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_qmlp.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_quant.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_quant.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     TORCH_CHECK_DTYPE(input, kFloat);
     TORCH_CHECK_DTYPE(output, kFloat);
     // TORCH_CHECK_SHAPES(input, 0, output, 0, 1);
     // TORCH_CHECK_SHAPES(input, 1, output, 1, 1);
     TORCH_CHECK_SHAPES(input, 1, scale, 0, 1);
     TORCH_CHECK(output.size(0) == p_grid + 1, "Output vector shape doesn't match grid")
 
+    const at::cuda::OptionalCUDAGuard device_guard(device_of(input));
+
     int rows = input.size(0);
     int columns = input.size(1);
 
     quantize_err_cuda
     (
         (float*) input.data_ptr(),
         (float*) output.data_ptr(),
```

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_quant.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_quant.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_rope.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_rope.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_sampling.cpp` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_sampling.cpp`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/exl2conv_ext/ext_sampling.h` & `exl2conv-0.0.17.1/exl2conv/exl2conv_ext/ext_sampling.h`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/ext.py` & `exl2conv-0.0.17.1/exl2conv/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,23 +75,22 @@
                     print(" -- Injected compiler path:", cl_path)
                 os.environ["path"] += ";" + cl_path
             else:
                 print(" !! Unable to find cl.exe; compilation will probably fail", file = sys.stderr)
 
     # gcc / cl.exe flags
 
-    extra_cflags = ["/Ox", "/arch:AVX2"] if windows else ["-O3", "-mavx2"]
+    extra_cflags = ["/Ox"] if windows else ["-O3"]
 
     if ext_debug:
         extra_cflags += ["-ftime-report", "-DTORCH_USE_CUDA_DSA"]
 
     # nvcc flags
 
     extra_cuda_cflags = ["-lineinfo", "-O3"]
-    # extra_cuda_cflags += ["-maxrregcount=128"]
 
     if torch.version.hip:
         extra_cuda_cflags += ["-DHIPBLAS_USE_HIP_HALF"]
 
     # linker flags
 
     extra_ldflags = []
@@ -125,14 +124,15 @@
         "cuda/pack_tensor.cu",
         "cuda/quantize.cu",
         "cuda/q_matrix.cu",
         "cuda/q_attn.cu",
         "cuda/q_mlp.cu",
         "cuda/q_gemm.cu",
         "cuda/rms_norm.cu",
+        "cuda/head_norm.cu",
         "cuda/layer_norm.cu",
         "cuda/rope.cu",
         "cuda/cache.cu",
         "cuda/util.cu",
         "cuda/comp_units/kernel_select.cu",
         "cuda/comp_units/unit_gptq_1.cu",
         "cuda/comp_units/unit_gptq_2.cu",
@@ -140,15 +140,17 @@
         "cuda/comp_units/unit_exl2_1a.cu",
         "cuda/comp_units/unit_exl2_1b.cu",
         "cuda/comp_units/unit_exl2_2a.cu",
         "cuda/comp_units/unit_exl2_2b.cu",
         "cuda/comp_units/unit_exl2_3a.cu",
         "cuda/comp_units/unit_exl2_3b.cu",
         "cpp/quantize_func.cpp",
+        "cpp/profiling.cpp",
         "cpp/sampling.cpp",
+        "cpp/sampling_avx2.cpp",
         "cpp/safetensors.cpp"
     ]
 
     sources = [os.path.join(sources_dir, s) for s in sources_]
 
     # Load extension
 
@@ -195,16 +197,17 @@
 
 
 # Create Q matrix
 
 def make_q_matrix(w: dict,
                   temp_dq: torch.Tensor,
                   key: str = None,
-                  prescale: float = 1):
-                  
+                  prescale: float = 1,
+                  max_dq_rows = 0):
+
     # EXL2
 
     if "q_weight" in w:
 
         w["q_scale_max"] *= prescale / 256
         w["q_perm"] = w["q_perm"].short()
         w["q_invperm"] = w["q_invperm"].short()
@@ -219,15 +222,16 @@
                                    w["q_scale_max"],
                                    w["q_groups"],
                                    w["q_group_map"],
                                    none_tensor,
                                    none_tensor,
                                    none_tensor,
                                    w.get("bias", none_tensor),
-                                   temp_dq)
+                                   temp_dq,
+                                   max_dq_rows)
 
     # GPTQ
 
     elif "qweight" in w:
 
         if prescale != 1: w["scales"] *= prescale
         if w["scales"].dtype == torch.float: w["scales"] = w["scales"].half()
@@ -246,15 +250,16 @@
                                        none_tensor,
                                        none_tensor,
                                        none_tensor,
                                        w["qzeros"],
                                        w["scales"],
                                        w["g_idx"].cpu(),
                                        w.get("bias", none_tensor),
-                                       temp_dq)
+                                       temp_dq,
+                                       max_dq_rows)
 
         # GPTQ without g_idx
 
         else:
 
             return ext_c.make_q_matrix(w["qweight"],
                                        none_tensor,
@@ -263,10 +268,11 @@
                                        none_tensor,
                                        none_tensor,
                                        none_tensor,
                                        w["qzeros"],
                                        w["scales"],
                                        none_tensor,
                                        w.get("bias", none_tensor),
-                                       temp_dq)
+                                       temp_dq,
+                                       max_dq_rows)
```

### Comparing `exl2conv-0.0.17/exl2conv/fasttensors.py` & `exl2conv-0.0.17.1/exl2conv/fasttensors.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/filters/base.py` & `exl2conv-0.0.17.1/exl2conv/generator/filters/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/filters/prefix.py` & `exl2conv-0.0.17.1/exl2conv/generator/filters/prefix.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/filters/select.py` & `exl2conv-0.0.17.1/exl2conv/generator/filters/select.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/ngram.py` & `exl2conv-0.0.17.1/exl2conv/generator/ngram.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/sampler.py` & `exl2conv-0.0.17.1/exl2conv/generator/sampler.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/generator/streaming.py` & `exl2conv-0.0.17.1/exl2conv/generator/streaming.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/layernorm.py` & `exl2conv-0.0.17.1/exl2conv/layernorm.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,20 @@
         if bias is not None:
             self.layernorm.bias = bias
             self.bias = bias
 
         self.variance_epsilon = self.model.config.norm_eps
 
 
+    def numel(self):
+
+        return 0
+        # return self.layernorm.weight.data.numel()
+
+
     def unload(self):
 
         self.layernorm = None
         self.weight = None
         self.bias = None
 
 
@@ -88,15 +94,16 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache = None,
                 attn_params = None,
                 past_len = None,
                 intermediates: bool = False,
-                loras = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         output_shape = hidden_states.shape
         hidden_states = hidden_states.view(-1, hidden_states.shape[-1])
         norm = torch.empty_like(hidden_states)
         ext_c.layer_norm(hidden_states,
                          self.weight.data,
                          self.bias.data if self.bias is not None else none_tensor,
@@ -113,15 +120,16 @@
 
     def forward_torch(self,
                       hidden_states: torch.Tensor,
                       cache = None,
                       attn_params = None,
                       past_len = None,
                       intermediates: bool = False,
-                      loras = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                      loras = None,
+                      **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         hidden_states = self.layernorm(hidden_states)
 
         if intermediates:
             return {"hidden_states": hidden_states}
         else:
             return hidden_states
```

### Comparing `exl2conv-0.0.17/exl2conv/linear.py` & `exl2conv-0.0.17.1/exl2conv/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 import torch
 import torch.nn.functional as F
-from exl2conv.module import ExLlamaV2Module
 from torch import nn
 from exl2conv import ext
 from exl2conv.ext import exl2conv_ext as ext_c, none_tensor
+from exl2conv.module import ExLlamaV2Module
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from exl2conv.lora import ExLlamaV2Lora
     from exl2conv.model import ExLlamaV2
 
+
 class ExLlamaV2Linear(ExLlamaV2Module):
 
     name: str = "Linear"
 
     in_features: int
     out_features: int
     has_bias: bool
@@ -80,32 +81,39 @@
         self.f_beg = f_beg
         self.f_end = f_end
 
         self.assumed_footprint = in_features * (out_features + self.padding) * 2 + 128
 
 
     def load(self,
-             w: dict | nn.Parameter | tuple | None = None):
+             w: dict | nn.Parameter | tuple | None = None,
+             device_tensors: bool = True):
 
         if self.f_key: w = self.load_weight_fused(self.f_key, self.f_beg, self.f_end, self.in_features, self.out_features)
         if w is None: w = self.load_weight()
 
         # Load quantized linear layer from dictionary
 
         if isinstance(w, dict):
             assert not self.model.config.load_in_q4, "Can't load quantized layer in Q4 mode"
             if self.has_bias:
                 assert "bias" in w, self.key + " has no bias but bias expected"
             else:
                 assert "bias" not in w, self.key + " has bias but bias is not expected"
-            device_tensors = self.model.get_device_tensors(self.device_idx)
-            device_tensors.begin_scratch_alloc()
-            self.temp_dq = device_tensors.get_scratch_slice(self.temp_dq_size())
+            if device_tensors:
+                device_tensors = self.model.get_device_tensors(self.device_idx)
+                device_tensors.begin_scratch_alloc()
+                self.temp_dq = device_tensors.get_scratch_slice(self.temp_dq_size())
+            else:
+                self.temp_dq = none_tensor
             self.q_tensors = w
-            self.q_handle = ext.make_q_matrix(w, self.temp_dq, prescale = self.prescale)
+            self.q_handle = ext.make_q_matrix(w,
+                                              self.temp_dq,
+                                              prescale = self.prescale,
+                                              max_dq_rows = self.model.config.max_dq_size // self.out_features)
             self.prev_prescale = self.prescale
             self.prescale = 1
 
         # Load FP16 linear layer without bias, optionally quantize to Q4
 
         elif isinstance(w, nn.Parameter):
             assert not self.has_bias, self.key + " has no bias tensor but bias is expected"
@@ -195,15 +203,18 @@
 
         return self.temp_dq_size() + \
                self.temp_fwd_size()
 
 
     def temp_dq_size(self) -> int:
 
-        return self.in_features * self.out_features * 2 + 128
+        dq = self.in_features * self.out_features
+        dq = min(dq, self.model.config.max_dq_size)
+        dq = dq * 2 + 128
+        return dq
 
 
     def temp_fwd_size(self) -> int:
 
         max_len = self.model.config.max_input_len if self.max_out_len is None else \
             min(self.max_out_len, self.model.config.max_input_len)
         return self.out_features * max_len * self.model.config.max_batch_size * 4 + 128
@@ -213,15 +224,16 @@
                 hidden_states: torch.Tensor,
                 cache = None,
                 attn_params = None,
                 past_len = None,
                 intermediates: bool = False,
                 loras: list[ExLlamaV2Lora] | None = None,
                 force_recons: bool = False,
-                force_cuda: bool = False) -> torch.Tensor | dict[str: torch.Tensor]:
+                force_cuda: bool = False,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         # Linear forward
 
         if self.q_handle is not None and not force_recons:
 
             output_shape = hidden_states.shape[:-1] + (self.out_features,)
             hidden_states = hidden_states.view(-1, hidden_states.shape[-1])
```

### Comparing `exl2conv-0.0.17/exl2conv/lora.py` & `exl2conv-0.0.17.1/exl2conv/lora.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import torch
 from exl2conv.compat import safe_move_tensor
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from exl2conv.model import ExLlamaV2
 
-
 class ExLlamaV2Lora:
 
     model: ExLlamaV2
 
     lora_config_path: str
     lora_path: str
```

### Comparing `exl2conv-0.0.17/exl2conv/mlp.py` & `exl2conv-0.0.17.1/exl2conv/mlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,21 +71,24 @@
             self.submodules += [self.gate_proj]
         else:
             self.gate_proj = None
 
 
     def numel(self) -> int:
 
+        numel = self.up_proj.numel() + \
+                self.down_proj.numel()
+
         if self.model.config.arch.mlp_gate:
-            return self.gate_proj.numel() + \
-                   self.up_proj.numel() + \
-                   self.down_proj.numel()
-        else:
-            return self.up_proj.numel() + \
-                   self.down_proj.numel()
+            numel += self.gate_proj.numel()
+
+        if self.post_attention_layernorm is not None:
+            numel += self.post_attention_layernorm.numel()
+
+        return numel
 
 
     def load(self):
 
         if self.post_attention_layernorm is not None:
             self.post_attention_layernorm.load()
 
@@ -214,18 +217,19 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache = None,
                 attn_params = None,
                 past_len = None,
                 intermediates: bool = False,
-                loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras: list[ExLlamaV2Lora] | None = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         if self.q_handle is None or intermediates:
-            return self.forward_torch(hidden_states, cache, attn_params, past_len, intermediates, loras = loras)
+            return self.forward_torch(hidden_states, cache, attn_params, past_len, intermediates, loras = loras, **kwargs)
 
         if loras is None or self.temp_lora_size == 0:
             pass_loras = []
             pass_lora_temp = none_tensor
         else:
             pass_loras = [id(x) for x in loras]
             pass_lora_temp = torch.empty((self.temp_lora_size,), dtype = torch.half, device = hidden_states.device)
@@ -240,15 +244,16 @@
 
     def forward_torch(self,
                       hidden_states: torch.Tensor,
                       cache = None,
                       attn_params = None,
                       past_len = None,
                       intermediates: bool = False,
-                      loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                      loras: list[ExLlamaV2Lora] | None = None,
+                      **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         residual = hidden_states
         post_norm = self.post_attention_layernorm.forward(hidden_states) \
             if self.has_norm else hidden_states
 
         if self.gate_proj is not None:
             gate = self.gate_proj.forward(post_norm, loras = loras)
```

### Comparing `exl2conv-0.0.17/exl2conv/model.py` & `exl2conv-0.0.17.1/exl2conv/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,15 +572,16 @@
                 cache: ExLlamaV2CacheBase | list[ExLlamaV2CacheBase] | None = None,
                 input_mask: torch.Tensor | None = None,
                 preprocess_only: bool = False,
                 last_id_only: bool = False,
                 loras: list[ExLlamaV2Lora] | None = None,
                 return_last_state: bool = False,
                 position_offsets: torch.Tensor | None = None,
-                abort_event: threading.Event | None = None) \
+                abort_event: threading.Event | None = None,
+                **kwargs) \
         -> torch.Tensor | tuple[torch.Tensor, torch.Tensor] | None:
         """
         Runs a forward pass through the model. If a cache is used, also appends keys/values to the cache
         and advances it.
 
         :param input_ids:
             LongTensor of input token IDs, shape (batch_size, q_len)
@@ -611,14 +612,18 @@
 
         :param abort_event:
             Optional event that, if set, will abort the forward pass. Function will return None if aborted.
 
         :return:
             FP16 logits tensor, shape (batch_size, q_len, vocab_size)
             (optional) state tensor, shape (batch_size, q_len, hidden_size)
+
+        :indexed_embeddings:
+            Tensor of embeddings, shape (batch_size, q_len, hidden_size), indexed by input token IDs >=
+            ExLlamaV2.EMBEDDING_INDEX
         """
 
         bsz, q_len = input_ids.shape
         remaining_q_len = q_len
 
         # Attn and MLP layers have preallocated buffers for temp states, sized by the model config. Effective max input
         # length depends on the current batch size
@@ -636,15 +641,16 @@
                                                cache = cache,
                                                input_mask = input_mask,
                                                preprocess_only = preprocess_only,
                                                last_id_only = last_id_only,
                                                loras = loras,
                                                return_last_state = return_last_state,
                                                position_offsets = position_offsets,
-                                               abort_event = abort_event)
+                                               abort_event = abort_event,
+                                               **kwargs)
 
             if abort_event and abort_event.is_set(): return
 
             if last_state is None:
                 return result
             else:
                 return result, last_state
@@ -688,15 +694,16 @@
                                   cache = cache,
                                   input_mask = input_mask,
                                   preprocess_only = _preprocess_only,
                                   last_id_only = _last_id_only,
                                   loras = loras,
                                   return_last_state = return_last_state and remaining_q_len <= chunk_size,
                                   position_offsets = position_offsets,
-                                  abort_event = abort_event)
+                                  abort_event = abort_event,
+                                  **kwargs)
 
             if abort_event and abort_event.is_set(): return
 
             if not _preprocess_only:
                 result = r if result is None else torch.cat((result, r), dim = 1)
                 r = None
 
@@ -716,15 +723,16 @@
                  cache: ExLlamaV2CacheBase | list[ExLlamaV2CacheBase] | None = None,
                  input_mask: torch.Tensor | None = None,
                  preprocess_only: bool = False,
                  last_id_only: bool = False,
                  loras: list[ExLlamaV2Lora] | None = None,
                  return_last_state: bool = False,
                  position_offsets: torch.Tensor | None = None,
-                 abort_event: threading.Event | None = None) \
+                 abort_event: threading.Event | None = None,
+                 **kwargs) \
         -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
 
         batch_size, seq_len = input_ids.shape
         past_len = 0
         if cache is not None:
             if isinstance(cache, ExLlamaV2CacheBase):
                 past_len = cache.current_seq_len
@@ -738,14 +746,15 @@
             "seq_len exceeds max_output_len"
 
         # assert cache is None or isinstance(cache, list) or batch_size <= cache.batch_size
 
         x = input_ids
         attn_params = ExLlamaV2Attention.Params(batch_size, seq_len, past_len, input_mask, position_offsets)
         last_state = None
+        last_module = None
 
         for idx, module in enumerate(self.modules):
 
             # Respect abort signal
 
             if abort_event and abort_event.is_set(): return None, None
 
@@ -759,15 +768,15 @@
                     last_state = x
                 elif last_id_only:
                     x = x.narrow(-2, -1, 1)
                 elif return_last_state:
                     last_state = x.narrow(-2, -1, 1)
 
             x = safe_move_tensor(x, device)
-            x = module.forward(x, cache = cache, attn_params = attn_params, past_len = past_len, loras = loras)
+            x = module.forward(x, cache = cache, attn_params = attn_params, past_len = past_len, loras = loras, **kwargs)
 
             if preprocess_only and idx == self.last_kv_layer_idx:
                 x = None
                 break
 
         # Advance cache
```

### Comparing `exl2conv-0.0.17/exl2conv/model_init.py` & `exl2conv-0.0.17.1/exl2conv/model_init.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/module.py` & `exl2conv-0.0.17.1/exl2conv/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch.nn as nn
 from exl2conv.config import ExLlamaV2Config
 from exl2conv.fasttensors import STFile
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from exl2conv.model import ExLlamaV2
-
+    from exl2conv.lora import ExLlamaV2Lora
 
 def _torch_device(idx: int) -> str:
     if idx == -1: return "cpu"
     return f"cuda:{idx}"
 
 
 class ExLlamaV2Module:
```

### Comparing `exl2conv-0.0.17/exl2conv/moe_mlp.py` & `exl2conv-0.0.17.1/exl2conv/moe_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,23 +213,24 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache = None,
                 attn_params = None,
                 past_len = None,
                 intermediates: bool = False,
-                loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras: list[ExLlamaV2Lora] | None = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         batch_size, sequence_length, hidden_dim = hidden_states.shape
 
         # TODO: LoRA currently uses the Torch codepath. Needs conditional (early-exit) kernels with output scaling
         # for the LoRA matmuls in order to work with the C++ path
 
         if self.q_handle is None or intermediates or batch_size * sequence_length > 4 or self.num_experts not in [4, 8, 16] or (loras is not None and len(loras) > 0):
-            return self.forward_torch(hidden_states, cache, attn_params, past_len, intermediates, loras = loras)
+            return self.forward_torch(hidden_states, cache, attn_params, past_len, intermediates, loras = loras, **kwargs)
 
         # if loras is None or self.temp_lora_size == 0:
         #     pass_loras = []
         #     pass_lora_temp = none_tensor
         # else:
         #     pass_loras = [id(x) for x in loras]
         #     pass_lora_temp = torch.empty((self.temp_lora_size,), dtype = torch.half, device = hidden_states.device)
@@ -243,15 +244,16 @@
 
     def forward_torch(self,
                       hidden_states: torch.Tensor,
                       cache = None,
                       attn_params = None,
                       past_len = None,
                       intermediates = False,
-                      loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                      loras: list[ExLlamaV2Lora] | None = None,
+                      **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         residual = hidden_states
 
         batch_size, sequence_length, hidden_dim = hidden_states.shape
         hidden_states = hidden_states.view(-1, hidden_dim)
 
         # Layernorm
```

### Comparing `exl2conv-0.0.17/exl2conv/parallel_decoder.py` & `exl2conv-0.0.17.1/exl2conv/parallel_decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
         self.submodules = self.attn.submodules + self.mlp.submodules
 
 
     def numel(self) -> int:
 
         return self.attn.numel() + \
-               self.mlp.numel()
+               self.mlp.numel() + \
+               self.input_layernorm.numel()
 
 
     def load(self):
 
         self.input_layernorm.load()
         self.attn.load()
         self.mlp.load()
@@ -91,41 +92,49 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache: ExLlamaV2CacheBase | None = None,
                 attn_params: ExLlamaV2Attention.Params | None = None,
                 past_len: int | None = None,
                 intermediates: bool = False,
-                loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras: list[ExLlamaV2Lora] | None = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         if intermediates:
-            return self.forward_interm(hidden_states, cache, attn_params, past_len, intermediates, loras)
+            return self.forward_interm(hidden_states,
+                                       cache,
+                                       attn_params,
+                                       past_len,
+                                       intermediates,
+                                       loras,
+                                       **kwargs)
 
         a = self.input_layernorm.forward(hidden_states)
         b = a.clone()
-        a = self.attn.forward(a, cache, attn_params, past_len, intermediates, loras)
-        b = self.mlp.forward(b, cache, attn_params, past_len, intermediates, loras)
+        a = self.attn.forward(a, cache, attn_params, past_len, intermediates, loras, **kwargs)
+        b = self.mlp.forward(b, cache, attn_params, past_len, intermediates, loras, **kwargs)
         hidden_states += a
         hidden_states += b
         return hidden_states
 
 
     def forward_interm(self,
                        hidden_states: torch.Tensor,
                        cache: ExLlamaV2CacheBase | None = None,
                        attn_params: ExLlamaV2Attention.Params | None = None,
                        past_len: int | None = None,
                        intermediates: bool = False,
-                       loras: list[ExLlamaV2Lora] | None = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                       loras: list[ExLlamaV2Lora] | None = None,
+                       **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         a = self.input_layernorm.forward(hidden_states)
         b = a.clone()
         post_norm = a.clone()
-        res_a = self.attn.forward(a, cache, attn_params, past_len, True, loras)
-        res_b = self.mlp.forward(b, cache, attn_params, past_len, True, loras)
+        res_a = self.attn.forward(a, cache, attn_params, past_len, True, loras, **kwargs)
+        res_b = self.mlp.forward(b, cache, attn_params, past_len, True, loras, **kwargs)
         hidden_states += res_a["hidden_states"]
         hidden_states += res_b["hidden_states"]
 
         if intermediates:
             return {"post_norm": post_norm,
                     "attn_output": res_a["attn_output"],
                     "pre_down": res_b["pre_down"],
```

### Comparing `exl2conv-0.0.17/exl2conv/rmsnorm.py` & `exl2conv-0.0.17.1/exl2conv/rmsnorm.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,20 @@
             self.weight = None
 
         if self.bias is not None:
             del self.bias
             self.bias = None
 
 
+    def numel(self):
+
+        return 0
+        # return self.weight.numel()
+
+
     def get_weight(self) -> torch.Tensor:
 
         # Make sure to return the original weight tensor for Gemma
         if self.model.config.arch.norm_constant_bias != 0:
             return self.weight.data - self.model.config.arch.norm_constant_bias
 
         return self.weight.data
@@ -86,15 +92,16 @@
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 cache = None,
                 attn_params = None,
                 past_len = None,
                 intermediates: bool = False,
-                loras = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                loras = None,
+                **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         output_shape = hidden_states.shape
         hidden_states = hidden_states.view(-1, hidden_states.shape[-1])
         norm = torch.empty_like(hidden_states)
         ext_c.rms_norm(hidden_states, self.weight, norm, self.variance_epsilon)
         hidden_states = norm.view(output_shape)
 
@@ -106,15 +113,16 @@
 
     def forward_torch(self,
                       hidden_states: torch.Tensor,
                       cache = None,
                       attn_params = None,
                       past_len = None,
                       intermediates: bool = False,
-                      loras = None) -> torch.Tensor | dict[str: torch.Tensor]:
+                      loras = None,
+                      **kwargs) -> torch.Tensor | dict[str: torch.Tensor]:
 
         hidden_states[hidden_states == -float('inf')] = -65504.0
         hidden_states[hidden_states == float('inf')] = 65504.0
 
         variance = hidden_states.to(torch.float32).pow(2).mean(-1, keepdim = True)
         hidden_states = hidden_states * torch.rsqrt(variance + self.variance_epsilon)
         hidden_states = hidden_states.to(self.weight.dtype)
```

### Comparing `exl2conv-0.0.17/exl2conv/server/websocket.py` & `exl2conv-0.0.17.1/exl2conv/server/websocket.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/server/websocket_actions.py` & `exl2conv-0.0.17.1/exl2conv/server/websocket_actions.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/tokenizer/base.py` & `exl2conv-0.0.17.1/exl2conv/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/tokenizer/hf.py` & `exl2conv-0.0.17.1/exl2conv/tokenizer/hf.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/tokenizer/spm.py` & `exl2conv-0.0.17.1/exl2conv/tokenizer/spm.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/tokenizer/tokenizer.py` & `exl2conv-0.0.17.1/exl2conv/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/tokenizer.py` & `exl2conv-0.0.17.1/exl2conv/tokenizer.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv/util.py` & `exl2conv-0.0.17.1/exl2conv/util.py`

 * *Files identical despite different names*

### Comparing `exl2conv-0.0.17/exl2conv.egg-info/SOURCES.txt` & `exl2conv-0.0.17.1/exl2conv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 exl2conv/attn.py
 exl2conv/cache.py
 exl2conv/compat.py
 exl2conv/config.py
 exl2conv/embedding.py
 exl2conv/ext.py
 exl2conv/fasttensors.py
+exl2conv/headnorm.py
 exl2conv/layernorm.py
 exl2conv/linear.py
 exl2conv/lora.py
 exl2conv/mlp.py
 exl2conv/model.py
 exl2conv/model_init.py
 exl2conv/module.py
@@ -61,29 +62,36 @@
 exl2conv/exl2conv_ext/ext_quant.h
 exl2conv/exl2conv_ext/ext_rope.cpp
 exl2conv/exl2conv_ext/ext_rope.h
 exl2conv/exl2conv_ext/ext_safetensors.cpp
 exl2conv/exl2conv_ext/ext_safetensors.h
 exl2conv/exl2conv_ext/ext_sampling.cpp
 exl2conv/exl2conv_ext/ext_sampling.h
+exl2conv/exl2conv_ext/cpp/avx2_target.h
 exl2conv/exl2conv_ext/cpp/avx_mathfun.h
+exl2conv/exl2conv_ext/cpp/profiling.cpp
+exl2conv/exl2conv_ext/cpp/profiling.h
 exl2conv/exl2conv_ext/cpp/quantize_func.cpp
 exl2conv/exl2conv_ext/cpp/quantize_func.h
 exl2conv/exl2conv_ext/cpp/safetensors.cpp
 exl2conv/exl2conv_ext/cpp/safetensors.h
 exl2conv/exl2conv_ext/cpp/sampling.cpp
 exl2conv/exl2conv_ext/cpp/sampling.h
+exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp
+exl2conv/exl2conv_ext/cpp/sampling_avx2.h
 exl2conv/exl2conv_ext/cpp/util.h
 exl2conv/exl2conv_ext/cuda/cache.cu
 exl2conv/exl2conv_ext/cuda/cache.cuh
 exl2conv/exl2conv_ext/cuda/compat.cuh
 exl2conv/exl2conv_ext/cuda/h_add.cu
 exl2conv/exl2conv_ext/cuda/h_add.cuh
 exl2conv/exl2conv_ext/cuda/h_gemm.cu
 exl2conv/exl2conv_ext/cuda/h_gemm.cuh
+exl2conv/exl2conv_ext/cuda/head_norm.cu
+exl2conv/exl2conv_ext/cuda/head_norm.cuh
 exl2conv/exl2conv_ext/cuda/layer_norm.cu
 exl2conv/exl2conv_ext/cuda/layer_norm.cuh
 exl2conv/exl2conv_ext/cuda/lora.cu
 exl2conv/exl2conv_ext/cuda/lora.cuh
 exl2conv/exl2conv_ext/cuda/matrix_view.cuh
 exl2conv/exl2conv_ext/cuda/pack_tensor.cu
 exl2conv/exl2conv_ext/cuda/pack_tensor.cuh
```

### Comparing `exl2conv-0.0.17/setup.py` & `exl2conv-0.0.17.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,29 +49,32 @@
                 "exl2conv/exl2conv_ext/cuda/quantize.cu",
                 "exl2conv/exl2conv_ext/cuda/q_matrix.cu",
                 "exl2conv/exl2conv_ext/cuda/q_attn.cu",
                 "exl2conv/exl2conv_ext/cuda/q_mlp.cu",
                 "exl2conv/exl2conv_ext/cuda/q_gemm.cu",
                 "exl2conv/exl2conv_ext/cuda/rms_norm.cu",
                 "exl2conv/exl2conv_ext/cuda/layer_norm.cu",
+                "exl2conv/exl2conv_ext/cuda/head_norm.cu",
                 "exl2conv/exl2conv_ext/cuda/rope.cu",
                 "exl2conv/exl2conv_ext/cuda/cache.cu",
                 "exl2conv/exl2conv_ext/cuda/util.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/kernel_select.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_1.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_2.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_gptq_3.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1a.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_1b.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2a.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_2b.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3a.cu",
                 "exl2conv/exl2conv_ext/cuda/comp_units/unit_exl2_3b.cu",
                 "exl2conv/exl2conv_ext/cpp/quantize_func.cpp",
+                "exl2conv/exl2conv_ext/cpp/profiling.cpp",
                 "exl2conv/exl2conv_ext/cpp/sampling.cpp",
+                "exl2conv/exl2conv_ext/cpp/sampling_avx2.cpp",
                 "exl2conv/exl2conv_ext/cpp/safetensors.cpp"
             ],
             extra_compile_args=extra_compile_args,
             libraries=["cublas"] if windows else [],
         )],
     "cmdclass": {"build_ext": cpp_extension.BuildExtension}
 } if precompile else {}
```

