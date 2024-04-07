# Comparing `tmp/torchao-nightly-2024.4.5.tar.gz` & `tmp/torchao-nightly-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-nightly-2024.4.5.tar", last modified: Fri Apr  5 00:19:11 2024, max compression
+gzip compressed data, was "torchao-nightly-2024.4.6.tar", last modified: Sat Apr  6 00:18:22 2024, max compression
```

## Comparing `torchao-nightly-2024.4.5.tar` & `torchao-nightly-2024.4.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/nf4tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/dtypes/uint4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.347684 torchao-nightly-2024.4.5/torchao/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/autotuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/intmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/kernel/intmm_triton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)    52411 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/GPTQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/dynamic_quant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/quant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/quant_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/smoothquant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/unified.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/quantization/weight_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao/sparsity/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-05 00:19:03.000000 torchao-nightly-2024.4.5/torchao/sparsity/wanda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 00:19:11.351683 torchao-nightly-2024.4.5/torchao_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 00:19:11.000000 torchao-nightly-2024.4.5/torchao_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.336605 torchao-nightly-2024.4.6/torchao/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.336605 torchao-nightly-2024.4.6/torchao/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/dtypes/nf4tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/dtypes/uint4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.336605 torchao-nightly-2024.4.6/torchao/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/kernel/autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/kernel/intmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/kernel/intmm_triton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/torchao/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)    52411 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/GPTQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/autoquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/dynamic_quant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/quant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/quant_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/smoothquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/unified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/quantization/weight_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/torchao/sparsity/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/sparsity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/sparsity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-06 00:18:09.000000 torchao-nightly-2024.4.6/torchao/sparsity/wanda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:18:22.340605 torchao-nightly-2024.4.6/torchao_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-06 00:18:22.000000 torchao-nightly-2024.4.6/torchao_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-06 00:18:22.000000 torchao-nightly-2024.4.6/torchao_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:18:22.000000 torchao-nightly-2024.4.6/torchao_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 00:18:22.000000 torchao-nightly-2024.4.6/torchao_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 00:18:22.000000 torchao-nightly-2024.4.6/torchao_nightly.egg-info/top_level.txt
```

### Comparing `torchao-nightly-2024.4.5/LICENSE` & `torchao-nightly-2024.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/PKG-INFO` & `torchao-nightly-2024.4.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-Metadata-Version: 2.1
-Name: torchao-nightly
-Version: 2024.4.5
-Summary: Package for applying ao techniques to GPU models
-Home-page: https://github.com/pytorch-labs/ao
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: numpy
-Requires-Dist: sentencepiece
-Requires-Dist: packaging
-
-# torchao: PyTorch Architecture Optimization 
+# torchao: PyTorch Architecture Optimization
 
 **Note: This repository is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open an github issue**
 
-The `torchao` package allows you to quantize and prune your models using native PyTorch. 
+The `torchao` package allows you to quantize and prune your models using native PyTorch.
 
 The repo hosts both
 1. lower precision [dtypes](./torchao/dtypes) such as nf4, uint4
 2. Quantization [algorithms](./torchao/quantization) such as dynamic quant, smoothquant
 3. Sparsity [algorithms](./torchao/sparsity) such as Wanda
 
 ## Success stories
@@ -46,47 +34,64 @@
 pip install -e .
 ```
 
 ## Examples
 
 Typically quantization algorithms will have different schemes for how the activation and weights are quantized so A16W8 for instance means the activations are quantized to 16 bits wheras the weights are quantized to 8 bits. Trying out different quantization schemes in `torchao` is generally a 1 line change.
 
-### A8W8 Dynamic Quantization
+### Autoquantization
+
+The `autoquant` api can be used to quickly and accurately quantize your model. When used as in the example below, the api first identifies the shapes
+of the activations that the different linear layers see, it then benchmarks these shapes across different types of quantized and non-quantized layers in order to pick the fastest one, attempting to take into account fusions where possible. Finally once the best class is found for each layer, it swaps the linear. Currently this api chooses between no quantization, int8 dynamic quantization and int8 weight only quantization for each layer.
 
-```Python
+```python
 import torch
-from torchao.quantization import quant_api
+import torchao
 
-# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+# inductor settings which improve torch.compile performance for quantized modules
 torch._inductor.config.force_fuse_int_mm_with_mul = True
+torch._inductor.config.use_mixed_mm = True
 
 # Plug in your model and example input
 model = torch.nn.Sequential(torch.nn.Linear(32, 64)).cuda().to(torch.bfloat16)
 input = torch.randn(32,32, dtype=torch.bfloat16, device='cuda')
 
-# convert linear modules to quantized linear modules
-quant_api.change_linear_weights_to_int8_dqtensors(model)
+# perform autoquantization
+torchao.autoquant(model, (input))
 
 # compile the model to improve performance
 model = torch.compile(model, mode='max-autotune')
 model(input)
 ```
 
+
+### A8W8 Dynamic Quantization
+
+```python
+# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+torch._inductor.config.force_fuse_int_mm_with_mul = True
+from torchao.quantization import quant_api
+# convert linear modules to quantized tensor subclasses
+quant_api.change_linear_weights_to_int8_dqtensors(model)
+```
+
 ### A16W8 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int8_woqtensors(model)
 ```
 
 This technique works best when the torch._inductor.config.use_mixed_mm option is enabled. This avoids dequantizing the weight tensor before the matmul, instead fusing the dequantization into the matmul, thereby avoiding materialization of a large floating point weight tensor.
 
 
 ### A16W4 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int4_woqtensors(model)
 ```
 
 Note: The quantization error incurred by applying int4 quantization to your model can be fairly significant, so using external techniques like GPTQ may be necessary to obtain a usable model.
 
 
 ### A8W8 Dynamic Quantization with Smoothquant
```

### Comparing `torchao-nightly-2024.4.5/README.md` & `torchao-nightly-2024.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,24 @@
-# torchao: PyTorch Architecture Optimization 
+Metadata-Version: 2.1
+Name: torchao-nightly
+Version: 2024.4.6
+Summary: Package for applying ao techniques to GPU models
+Home-page: https://github.com/pytorch-labs/ao
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+Requires-Dist: numpy
+Requires-Dist: sentencepiece
+Requires-Dist: packaging
+
+# torchao: PyTorch Architecture Optimization
 
 **Note: This repository is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open an github issue**
 
-The `torchao` package allows you to quantize and prune your models using native PyTorch. 
+The `torchao` package allows you to quantize and prune your models using native PyTorch.
 
 The repo hosts both
 1. lower precision [dtypes](./torchao/dtypes) such as nf4, uint4
 2. Quantization [algorithms](./torchao/quantization) such as dynamic quant, smoothquant
 3. Sparsity [algorithms](./torchao/sparsity) such as Wanda
 
 ## Success stories
@@ -34,47 +46,64 @@
 pip install -e .
 ```
 
 ## Examples
 
 Typically quantization algorithms will have different schemes for how the activation and weights are quantized so A16W8 for instance means the activations are quantized to 16 bits wheras the weights are quantized to 8 bits. Trying out different quantization schemes in `torchao` is generally a 1 line change.
 
-### A8W8 Dynamic Quantization
+### Autoquantization
+
+The `autoquant` api can be used to quickly and accurately quantize your model. When used as in the example below, the api first identifies the shapes
+of the activations that the different linear layers see, it then benchmarks these shapes across different types of quantized and non-quantized layers in order to pick the fastest one, attempting to take into account fusions where possible. Finally once the best class is found for each layer, it swaps the linear. Currently this api chooses between no quantization, int8 dynamic quantization and int8 weight only quantization for each layer.
 
-```Python
+```python
 import torch
-from torchao.quantization import quant_api
+import torchao
 
-# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+# inductor settings which improve torch.compile performance for quantized modules
 torch._inductor.config.force_fuse_int_mm_with_mul = True
+torch._inductor.config.use_mixed_mm = True
 
 # Plug in your model and example input
 model = torch.nn.Sequential(torch.nn.Linear(32, 64)).cuda().to(torch.bfloat16)
 input = torch.randn(32,32, dtype=torch.bfloat16, device='cuda')
 
-# convert linear modules to quantized linear modules
-quant_api.change_linear_weights_to_int8_dqtensors(model)
+# perform autoquantization
+torchao.autoquant(model, (input))
 
 # compile the model to improve performance
 model = torch.compile(model, mode='max-autotune')
 model(input)
 ```
 
+
+### A8W8 Dynamic Quantization
+
+```python
+# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+torch._inductor.config.force_fuse_int_mm_with_mul = True
+from torchao.quantization import quant_api
+# convert linear modules to quantized tensor subclasses
+quant_api.change_linear_weights_to_int8_dqtensors(model)
+```
+
 ### A16W8 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int8_woqtensors(model)
 ```
 
 This technique works best when the torch._inductor.config.use_mixed_mm option is enabled. This avoids dequantizing the weight tensor before the matmul, instead fusing the dequantization into the matmul, thereby avoiding materialization of a large floating point weight tensor.
 
 
 ### A16W4 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int4_woqtensors(model)
 ```
 
 Note: The quantization error incurred by applying int4 quantization to your model can be fairly significant, so using external techniques like GPTQ may be necessary to obtain a usable model.
 
 
 ### A8W8 Dynamic Quantization with Smoothquant
```

### Comparing `torchao-nightly-2024.4.5/setup.py` & `torchao-nightly-2024.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/dtypes/nf4tensor.py` & `torchao-nightly-2024.4.6/torchao/dtypes/nf4tensor.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/dtypes/uint4.py` & `torchao-nightly-2024.4.6/torchao/dtypes/uint4.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/kernel/autotuner.py` & `torchao-nightly-2024.4.6/torchao/kernel/autotuner.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/kernel/intmm.py` & `torchao-nightly-2024.4.6/torchao/kernel/intmm.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/kernel/intmm_triton.py` & `torchao-nightly-2024.4.6/torchao/kernel/intmm_triton.py`

 * *Files 2% similar despite different names*

```diff
@@ -352,7 +352,13 @@
     K, N = b.shape
     c = torch.empty((M, N), device=a.device, dtype=scales1.dtype)
     # 1D launch kernel where each block gets its own program.
     best_config = get_best_config_fn(
         int_scaled_matmul_kernel, [a, b, scales1, c], int8_mm_kernel_configs
     )
     return int_scaled_matmul_kernel(a, b, scales1, c, best_config)
+
+
+@torch.library.impl(lib, "int_scaled_matmul", "CPU")
+def int_scaled_matmul_cpu(a, b, scales1):
+    c = torch._int_mm(a, b)
+    return c.to(scales1.dtype) * scales1
```

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/GPTQ.py` & `torchao-nightly-2024.4.6/torchao/quantization/GPTQ.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/__init__.py` & `torchao-nightly-2024.4.6/torchao/quantization/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .smoothquant import *  # noqa: F403
 from .quant_api import *  # noqa: F403
 from .subclass import *  # noqa: F403
 from .quant_primitives import *  # noqa: F403
 from .utils import *  # noqa: F403
 from .weight_only import *  # noqa: F403
 from .unified import *
+from .autoquant import *
 
 __all__ = [
     "DynamicallyPerAxisQuantizedLinear",
     "apply_weight_only_int8_quant",
     "apply_dynamic_quant",
     "change_linear_weights_to_int8_dqtensors",
     "change_linear_weights_to_int8_woqtensors",
@@ -22,14 +23,17 @@
     "swap_conv2d_1x1_to_linear"
     "safe_int_mm",
     "dynamically_quantize_per_tensor",
     "quantize_activation_per_token_absmax",
     "dynamically_quantize_per_channel",
     "dequantize_per_tensor",
     "dequantize_per_channel",
+    "autoquant",
+    "change_linears_to_autoquantizable",
+    "change_autoquantizable_to_quantized",
     "quant_int8_dynamic_linear",
     "quant_int8_matmul",
     "quant_int8_dynamic_per_token_linear",
     "quant_int8_per_token_matmul",
     "get_scale",
     "SmoothFakeDynQuantMixin",
     "SmoothFakeDynamicallyQuantizedLinear",
```

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/dynamic_quant.py` & `torchao-nightly-2024.4.6/torchao/quantization/dynamic_quant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/quant_api.py` & `torchao-nightly-2024.4.6/torchao/quantization/quant_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         Int8DynActInt4WeightQuantizer,
         Int8DynActInt4WeightGPTQQuantizer,
 
     )
     __all__ += [
         "Int8DynActInt4WeightQuantizer",
         "Int8DynActInt4WeightGPTQQuantizer",
-
     ]
 
 
 def _replace_with_custom_fn_if_matches_filter(
     model,
     replacement_fn,
     filter_fn,
@@ -115,18 +114,19 @@
     quantization to all linear layers by converting all linear weight
     tensors to the `Int8DynamicallyQuantizedLinearWeight` Tensor subclass.
     """
     change_linear_weights_to_int8_dqtensors(model, filter_fn)
 
 
 def _get_subclass_inserter(cls, **kwargs):
-
+    method = kwargs.pop("method", "from_float")
     def insert_subclass(lin):
         lin.weight = torch.nn.Parameter(
-            cls.from_float(lin.weight, **kwargs), requires_grad=False
+            # cls.from_float(...)
+            getattr(cls, method)(lin.weight, **kwargs), requires_grad=False
         )
         return lin
 
     return insert_subclass
 
 
 def change_linear_weights_to_int8_dqtensors(model, filter_fn=None):
@@ -170,15 +170,14 @@
 
     _replace_with_custom_fn_if_matches_filter(
         model,
         _get_subclass_inserter(Int4WeightOnlyQuantizedLinearWeight, **kwargs),
         filter_fn,
     )
 
-
 def swap_conv2d_1x1_to_linear(model, filter_fn=None):
     """
     Changes all conv2d 1x1 modules to equivalent linear modules so that they can then be quantized.
     """
 
     class PermuteSandwich(torch.nn.Module):
         def __init__(self, mod):
```

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/quant_primitives.py` & `torchao-nightly-2024.4.6/torchao/quantization/quant_primitives.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/smoothquant.py` & `torchao-nightly-2024.4.6/torchao/quantization/smoothquant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/subclass.py` & `torchao-nightly-2024.4.6/torchao/quantization/subclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         )
         # the desired representation shape for fast quantized matmul is
         # transposed compared to how it's stored as a linear weight,
         # i.e. we want in_channels as dim=0 and out_channels (and quantized axis) as dim=1
         # however the external representation of our tensor will maintain the correct
         # shape attribute which needs to be tracked directly.
         int_data = w_int_repr.contiguous().t()
-        if cls is not Int8DynamicallyQuantizedLinearWeight:
+        if not issubclass(cls, Int8DynamicallyQuantizedLinearWeight):
             int_data = int_data.contiguous()
         return cls(
             int_data, w_scales, False, input_float.shape, dtype=input_float.dtype
         )
 
 
 class Int8WeightOnlyQuantizedLinearWeight(Int8DynamicallyQuantizedLinearWeight):
```

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/unified.py` & `torchao-nightly-2024.4.6/torchao/quantization/unified.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/utils.py` & `torchao-nightly-2024.4.6/torchao/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/quantization/weight_only.py` & `torchao-nightly-2024.4.6/torchao/quantization/weight_only.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/sparsity/utils.py` & `torchao-nightly-2024.4.6/torchao/sparsity/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao/sparsity/wanda.py` & `torchao-nightly-2024.4.6/torchao/sparsity/wanda.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.5/torchao_nightly.egg-info/PKG-INFO` & `torchao-nightly-2024.4.6/torchao_nightly.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
 Requires-Dist: packaging
 
-# torchao: PyTorch Architecture Optimization 
+# torchao: PyTorch Architecture Optimization
 
 **Note: This repository is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open an github issue**
 
-The `torchao` package allows you to quantize and prune your models using native PyTorch. 
+The `torchao` package allows you to quantize and prune your models using native PyTorch.
 
 The repo hosts both
 1. lower precision [dtypes](./torchao/dtypes) such as nf4, uint4
 2. Quantization [algorithms](./torchao/quantization) such as dynamic quant, smoothquant
 3. Sparsity [algorithms](./torchao/sparsity) such as Wanda
 
 ## Success stories
@@ -46,47 +46,64 @@
 pip install -e .
 ```
 
 ## Examples
 
 Typically quantization algorithms will have different schemes for how the activation and weights are quantized so A16W8 for instance means the activations are quantized to 16 bits wheras the weights are quantized to 8 bits. Trying out different quantization schemes in `torchao` is generally a 1 line change.
 
-### A8W8 Dynamic Quantization
+### Autoquantization
+
+The `autoquant` api can be used to quickly and accurately quantize your model. When used as in the example below, the api first identifies the shapes
+of the activations that the different linear layers see, it then benchmarks these shapes across different types of quantized and non-quantized layers in order to pick the fastest one, attempting to take into account fusions where possible. Finally once the best class is found for each layer, it swaps the linear. Currently this api chooses between no quantization, int8 dynamic quantization and int8 weight only quantization for each layer.
 
-```Python
+```python
 import torch
-from torchao.quantization import quant_api
+import torchao
 
-# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+# inductor settings which improve torch.compile performance for quantized modules
 torch._inductor.config.force_fuse_int_mm_with_mul = True
+torch._inductor.config.use_mixed_mm = True
 
 # Plug in your model and example input
 model = torch.nn.Sequential(torch.nn.Linear(32, 64)).cuda().to(torch.bfloat16)
 input = torch.randn(32,32, dtype=torch.bfloat16, device='cuda')
 
-# convert linear modules to quantized linear modules
-quant_api.change_linear_weights_to_int8_dqtensors(model)
+# perform autoquantization
+torchao.autoquant(model, (input))
 
 # compile the model to improve performance
 model = torch.compile(model, mode='max-autotune')
 model(input)
 ```
 
+
+### A8W8 Dynamic Quantization
+
+```python
+# Fuse the int8*int8 -> int32 matmul and subsequent mul op avoiding materialization of the int32 intermediary tensor
+torch._inductor.config.force_fuse_int_mm_with_mul = True
+from torchao.quantization import quant_api
+# convert linear modules to quantized tensor subclasses
+quant_api.change_linear_weights_to_int8_dqtensors(model)
+```
+
 ### A16W8 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int8_woqtensors(model)
 ```
 
 This technique works best when the torch._inductor.config.use_mixed_mm option is enabled. This avoids dequantizing the weight tensor before the matmul, instead fusing the dequantization into the matmul, thereby avoiding materialization of a large floating point weight tensor.
 
 
 ### A16W4 WeightOnly Quantization
 
 ```python
+from torchao.quantization import quant_api
 quant_api.change_linear_weights_to_int4_woqtensors(model)
 ```
 
 Note: The quantization error incurred by applying int4 quantization to your model can be fairly significant, so using external techniques like GPTQ may be necessary to obtain a usable model.
 
 
 ### A8W8 Dynamic Quantization with Smoothquant
```

### Comparing `torchao-nightly-2024.4.5/torchao_nightly.egg-info/SOURCES.txt` & `torchao-nightly-2024.4.6/torchao_nightly.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 torchao/dtypes/uint4.py
 torchao/kernel/__init__.py
 torchao/kernel/autotuner.py
 torchao/kernel/intmm.py
 torchao/kernel/intmm_triton.py
 torchao/quantization/GPTQ.py
 torchao/quantization/__init__.py
+torchao/quantization/autoquant.py
 torchao/quantization/dynamic_quant.py
 torchao/quantization/quant_api.py
 torchao/quantization/quant_primitives.py
 torchao/quantization/smoothquant.py
 torchao/quantization/subclass.py
 torchao/quantization/unified.py
 torchao/quantization/utils.py
```

