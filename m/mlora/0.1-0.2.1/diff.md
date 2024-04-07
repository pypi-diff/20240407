# Comparing `tmp/mlora-0.1.tar.gz` & `tmp/mlora-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlora-0.1.tar", last modified: Thu Dec 14 04:04:39 2023, max compression
+gzip compressed data, was "mlora-0.2.1.tar", last modified: Sun Apr  7 05:43:29 2024, max compression
```

## Comparing `mlora-0.1.tar` & `mlora-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2023-12-14 04:04:39.162299 mlora-0.1/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2023-10-31 06:53:31.000000 mlora-0.1/LICENSE
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10883 2023-12-14 04:04:39.162066 mlora-0.1/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9941 2023-12-11 13:51:27.000000 mlora-0.1/README.md
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2023-12-14 04:04:39.161124 mlora-0.1/mlora/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     3835 2023-12-11 13:32:14.000000 mlora-0.1/mlora/LoraLiner.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)      590 2023-12-11 13:32:17.000000 mlora-0.1/mlora/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     4999 2023-10-31 06:53:31.000000 mlora-0.1/mlora/checkpoint.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    15798 2023-12-11 13:32:18.000000 mlora-0.1/mlora/dispatcher.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1822 2023-10-31 06:53:31.000000 mlora-0.1/mlora/evaluator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     4400 2023-12-11 13:32:19.000000 mlora-0.1/mlora/model.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    13916 2023-12-11 13:32:20.000000 mlora-0.1/mlora/model_chatglm.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    13542 2023-12-11 13:32:21.000000 mlora-0.1/mlora/model_llama.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1074 2023-10-31 06:53:31.000000 mlora-0.1/mlora/modelargs.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1041 2023-10-31 06:53:31.000000 mlora-0.1/mlora/tokenizer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1531 2023-12-11 13:32:23.000000 mlora-0.1/mlora/utils.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2023-12-14 04:04:39.161848 mlora-0.1/mlora.egg-info/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10883 2023-12-14 04:04:39.000000 mlora-0.1/mlora.egg-info/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)      384 2023-12-14 04:04:39.000000 mlora-0.1/mlora.egg-info/SOURCES.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2023-12-14 04:04:39.000000 mlora-0.1/mlora.egg-info/dependency_links.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      189 2023-12-14 04:04:39.000000 mlora-0.1/mlora.egg-info/requires.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2023-12-14 04:04:39.000000 mlora-0.1/mlora.egg-info/top_level.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      956 2023-12-14 04:04:30.000000 mlora-0.1/pyproject.toml
--rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2023-12-14 04:04:39.162342 mlora-0.1/setup.cfg
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 05:43:29.648149 mlora-0.2.1/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.2.1/LICENSE
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10787 2024-04-07 05:43:29.647930 mlora-0.2.1/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10026 2024-04-07 05:32:43.000000 mlora-0.2.1/README.md
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 05:43:29.646726 mlora-0.2.1/mlora/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1292 2024-04-06 03:13:27.000000 mlora-0.2.1/mlora/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    22069 2024-04-06 16:30:59.000000 mlora-0.2.1/mlora/attention.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5068 2024-04-06 16:30:36.000000 mlora-0.2.1/mlora/backends.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     4955 2024-04-05 15:46:05.000000 mlora-0.2.1/mlora/checkpoint.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    13130 2024-04-03 07:55:06.000000 mlora-0.2.1/mlora/dispatcher.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     3865 2024-04-06 16:30:59.000000 mlora-0.2.1/mlora/feed_forward.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-03 07:55:06.000000 mlora-0.2.1/mlora/generate.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    14342 2024-04-06 16:30:59.000000 mlora-0.2.1/mlora/lora_linear.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11045 2024-04-06 08:47:07.000000 mlora-0.2.1/mlora/mix_lora.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1277 2024-04-03 07:55:06.000000 mlora-0.2.1/mlora/model.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    28382 2024-04-06 16:30:59.000000 mlora-0.2.1/mlora/model_llama.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9490 2024-04-03 16:46:28.000000 mlora-0.2.1/mlora/modelargs.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.2.1/mlora/prompter.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1516 2024-04-03 07:55:06.000000 mlora-0.2.1/mlora/tokenizer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7885 2024-04-06 09:10:39.000000 mlora-0.2.1/mlora/train.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1864 2024-04-06 03:11:46.000000 mlora-0.2.1/mlora/utils.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 05:43:29.647733 mlora-0.2.1/mlora.egg-info/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10787 2024-04-07 05:43:29.000000 mlora-0.2.1/mlora.egg-info/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      491 2024-04-07 05:43:29.000000 mlora-0.2.1/mlora.egg-info/SOURCES.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-07 05:43:29.000000 mlora-0.2.1/mlora.egg-info/dependency_links.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-07 05:43:29.000000 mlora-0.2.1/mlora.egg-info/requires.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-07 05:43:29.000000 mlora-0.2.1/mlora.egg-info/top_level.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      816 2024-04-06 16:30:36.000000 mlora-0.2.1/pyproject.toml
+-rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-07 05:43:29.648186 mlora-0.2.1/setup.cfg
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 05:43:29.647469 mlora-0.2.1/tests/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.2.1/tests/test_demo.py
```

### Comparing `mlora-0.1/LICENSE` & `mlora-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlora-0.1/PKG-INFO` & `mlora-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,209 +1,198 @@
-Metadata-Version: 2.1
-Name: mlora
-Version: 0.1
-Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
-Project-URL: Homepage, https://github.com/TUDB-Labs/multi-lora-fine-tune
-Project-URL: Bug Tracker, https://github.com/TUDB-Labs/multi-lora-fine-tune/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch==2.0.1
-Requires-Dist: einops==0.6.1
-Requires-Dist: datasets==2.14.5
-Requires-Dist: accelerate==0.21.0
-Requires-Dist: transformers==4.30.2
-Requires-Dist: bitsandbytes==0.40.0
-Requires-Dist: sentencepiece==0.1.99
-Requires-Dist: scipy==1.10.1
-Requires-Dist: xformers==0.0.20
-Requires-Dist: nltk
-Requires-Dist: jieba
-Requires-Dist: rouge
-Requires-Dist: rouge_chinese
-
 # m-LoRA: Efficient LLM Model Fine-Tune via Multi-LoRA Optimization
-[![](https://github.com/TUDB-Labs/multi-lora-fine-tune/actions/workflows/python-test-main.yml/badge.svg)](https://github.com/TUDB-Labs/multi-lora-fine-tune/actions/workflows/python-test-main.yml)
-[![](https://img.shields.io/github/stars/TUDB-Labs/multi-lora-fine-tune?logo=GitHub)](https://github.com/TUDB-Labs/multi-lora-fine-tune/stargazers)
-[![](https://img.shields.io/github/license/TUDB-Labs/multi-lora-fine-tune)](http://www.apache.org/licenses/LICENSE-2.0)
-[![](https://img.shields.io/github/v/release/TUDB-Labs/multi-lora-fine-tune)](https://github.com/TUDB-Labs/multi-lora-fine-tune/releases/latest)
-[![](https://img.shields.io/github/languages/top/TUDB-Labs/multi-lora-fine-tune)](https://www.python.org/)  
+[![](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/python-test.yml)
+[![](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml/badge.svg)](https://github.com/scukdde-llm/mlora/actions/workflows/mlora-test.yml)
+[![](https://img.shields.io/github/stars/scukdde-llm/mlora?logo=GitHub)](https://github.com/scukdde-llm/mlora/stargazers)
+[![](https://img.shields.io/github/license/scukdde-llm/mlora)](http://www.apache.org/licenses/LICENSE-2.0)
+[![](https://img.shields.io/github/v/release/scukdde-llm/mlora)](https://github.com/scukdde-llm/mlora/releases/latest)
+[![](https://img.shields.io/github/languages/top/scukdde-llm/mlora)](https://www.python.org/)  
 
 m-LoRA (a.k.a Multi-Lora Fine-Tune) is an open-source framework for fine-tuning Large Language Models (LLMs) using the efficient multiple LoRA/QLoRA methods. Key features of m-LoRA include:
 
 - Efficient LoRA/QLoRA: Optimizes the fine-tuning process, significantly reducing GPU memory usage by leveraging a shared frozen-based model.
 
 - Multiple LoRA Adapters: Support for concurrent fine-tuning of multiple LoRA/QLoRA adapters.
 
-## Contents
+- LoRA-based Mix-of-Expert LLM Adapter: [MixLoRA](./docs/MixLoRA.md), which implements a Mix-of-Expert architecture based on multiple LoRA adapters for the frozen FFN layer.
+
+## Note from the maintainer of this repository
+
+This is an actively developing fork of the official m-LoRA repository, focusing on LoRA + MoE and its related improvements, maintained by the authors of m-LoRA.
+
+Please note that the functions, interfaces, and performance of this fork are slightly different from the original m-LoRA. We cannot guarantee compatibility. For production use, please prefer the [original m-LoRA](https://github.com/TUDB-Labs/multi-lora-fine-tune).
 
-- [Updates](#updates)
-- [Supported Models](#Models)
-- [Overview](#overview)
-- [Getting Started](#Quickstart)
-- [Installation](#Installation)
-- [Contributing](#Contributing)
-- [Copyright](#Copyright)
+## Supported Platform
 
-## Updates
-- Support multiple LLaMA2 fine-tuning
-- Support multiple ChatGLM fine-tuning
-- Support multiple LLaMA fine-tuning
-- On the way, Baichuan
+| OS      | Backend | Model Precision        | Quantization  | xFormers | Flash Attention |
+|---------|---------|------------------------|---------------|----------|-----------------|
+| Linux   | CUDA    | FP32, FP16, TF32, BF16 | 8bit and 4bit | &check;  | &check;         |
+| Windows | CUDA    | FP32, FP16, TF32, BF16 | &cross;       | &cross;  | &cross;         |
+| macOS   | MPS     | FP32, FP16             | &cross;       | &cross;  | &cross;         |
 
-## Models
+**Note**: Windows and macOS support are experimental feature.
 
-|                                 | Model                                          | Model size      |
-|---------------------------------|------------------------------------------------|-----------------|
-| <input type="checkbox" checked> | [ChatGLM](https://github.com/THUDM/ChatGLM-6B) | 6B              |
-| <input type="checkbox" checked> | [ChatGLM2](https://github.com/THUDM/ChatGLM2-6B) | 6B/12B          |
-| <input type="checkbox">         | [ChatGLM3](https://github.com/THUDM/ChatGLM3)  | 6B                 |                 |
-| <input type="checkbox" checked> | [LLaMA](https://github.com/facebookresearch/llama) | 7B//13B/33B/65B |
-| <input type="checkbox" checked> | [LLaMA-2](https://huggingface.co/meta-llama)   | 7B/13B/70B      |
-| <input type="checkbox">         | [Baichuan](https://github.com/baichuan-inc/Baichuan-13B) | 7B/13B          |
-| <input type="checkbox">         | [Baichuan2](https://github.com/baichuan-inc/Baichuan2) | 7B/13B                  |
+## Supported Pre-trained Models
 
-> **Example:** Use our system  to improve the LLaMa-2 fine-tuning with less resources
->https://www.kaggle.com/code/rraydata/multi-lora-example/notebook
+|         | Model                                                    | # Parameters    |
+|---------|----------------------------------------------------------|-----------------|
+| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B  |
+| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B      |
+| &check; | [Qwen-2](https://qwenlm.github.io)                       | 4B/7B/14B/72B   |
+| &check; | [Mistral](https://mistral.ai)                            | 7B              |
 
-## Overview
+## Supported LoRA Variants
 
-**m-LoRA** is a high-throughput LLM fine-tuning framework based on LoRA and QLoRA, compatible with HuggingFace-Transformers LLaMA Models and ChatGLM Models.
+|         | LoRA Variants                                            | Arguments*                       |
+|---------|----------------------------------------------------------|----------------------------------|
+| &check; | [QLoRA](https://arxiv.org/abs/2402.12354)                | See *Quantize Methods*           |
+| &check; | [LoRA+](https://arxiv.org/abs/2402.12354)                | `loraplus_lr_ratio: 20.0`        |
+| &check; | [DoRA](https://arxiv.org/abs/2402.09353)                 | `use_dora: true`                 |
+| &check; | [rsLoRA](https://arxiv.org/abs/2312.03732)               | `use_rslora: true`               |
+| &check; | MixLoRA                                                  | See [MixLoRA](./docs/MixLoRA.md) |
 
-This picture shows the basic principle of LoRA and Multi-LoRA.
+*: Arguments of configuration file
 
-<div align="center"><img src="./assets/m-LoRA.png" width=70%"></div>
-The system overview of m-LoRA is as follows.
-<div align="center"><img src="./assets/system_overview.png" width="100%"></div>
+## Supported Attention Methods
 
-m-LoRA requires [PyTorch](https://pytorch.org/) and [NVIDIA CUDA](https://developer.nvidia.com/cuda-toolkit) compatible GPUs.
+|         | Attention Methods                                        | Name           | Arguments*               |
+|---------|----------------------------------------------------------|----------------|--------------------------|
+| &check; | [Scaled Dot Product](https://arxiv.org/abs/1706.03762)   | `"eager"`      | `--attn_impl eager`      |
+| &check; | [xFormers](https://github.com/facebookresearch/xformers) | `"xformers"`   | `--attn_impl xformers`   |
+| &check; | [Flash Attention 2](https://arxiv.org/abs/2307.08691)    | `"flash_attn"` | `--attn_impl flash_attn` |
 
-### Main Contribution
+*: Arguments of `mlora.py`
 
-- Introduces the Multi-LoRA method, capable of enabling the sharing of pre-trained model weights during the fine-tuning process of large language models;
-- Proposes a task scheduling algorithm to enhance the overall throughput of the task training process and reduce total training latency;
-- Builds upon the above by implementing m-LoRA, a high-throughput large language model fine-tuning framework based on LoRA and QLoRA;
-- Evaluates m-LoRA in experiments against existing systems, confirming that m-LoRA effectively utilizes system computing resources, thereby improving training throughput and reducing training latency compared to current systems.
+m-LoRA only supports scaled-dot product attention (eager) by default. Additional requirements are necessary for xFormers and flash attention.
 
-### Experiment Results
+To utilize xFormers attention, you must manually install additional dependencies:
 
-Environment: NVIDIA RTX A6000 with Intel Xeon Silver 4314 on Ubuntu 22.04.3
+```bash
+pip3 install xformers==0.0.23.post1
+```
 
-Baseline: We utilized the widely adopted [Alpaca-LoRA](https://github.com/tloen/alpaca-lora) as a foundation. On a single GPU, we independently ran multiple Alpaca-LoRA processes in parallel (marked as *Baseline@Alpaca-Parallel*) and sequentially (marked as *Baseline@Alpaca-Seq*), forming two baseline methods for the experiments. We test this on A100, and rest of results are based on the same GPU configure.
+For flash attention, manual installation of the following dependencies is required:
+
+```bash
+pip3 install ninja
+pip3 install flash-attn==2.5.6 --no-build-isolation
+```
 
-#### Training Latency and Throughput
+If the attention method is not specified, xFormers is automatically employed during training if available, while scaled-dot product attention is used during inference and evaluation. It's important to note that xFormers attention necessitates aligning the sequence length to a multiple of 8, otherwise, an error will occur.
 
-Method|Latency|Throughput
-:---:|:---:|:---:
-Baseline@Alpaca-Seq|10.51h|608.41 token/s
-Baseline@Alpaca-Parallel|9.85h|649.30 token/s
-m-LoRA|9.46h|674.58 token/s
+## Supported Quantize Methods
 
-We conducted four identical fine-tuning jobs with same dataset and same hyper-parameters, incorporating two baselines and m-LoRA. During the experimental process, we collected the completion times for each task in the baseline methods and calculated the time taken by the slowest task as the *Training Latency*. As shown in Table, m-LoRA exhibits lower *Training Latency* compared to both baseline methods. Specifically, m-LoRA is 9.99% faster than *Baseline@Alpaca-Seq* and 3.92% faster than *Baseline@Alpaca-Parallel*.
-<div align="center"><img src="./assets/throughput_compare.png" width="100%"></div>
+|         | Quantize Methods      | Arguments*    |
+|---------|-----------------------|---------------|
+| &check; | Tensor Float 32       | `--tf32`      |
+| &check; | Half Precision (FP16) | `--fp16`      |
+| &check; | Brain Float 16        | `--bf16`      |
+| &check; | 8bit Quantize         | `--load_8bit` |
+| &check; | 4bit Quantize         | `--load_4bit` |
 
+*: Arguments of `mlora.py`
 
+m-LoRA offers support for various model accuracy and quantization methods. By default, m-LoRA utilizes full precision (Float32), but users can opt for half precision (Float16) using `--fp16` or BrainFloat16 using `--bf16`. Enabling half precision reduces the model size by half, and for further reduction, quantization methods can be employed.
 
-#### Video Memory Usage
-<div align="center"><img src="./assets/GPU_memory_usage.png" width="100%"></div>
+Quantization can be activated using `--load_4bit` for 4-bit quantization or `--load_8bit` for 8-bit quantization. However, when only quantization is enabled, m-LoRA utilizes Float32 for calculations. To achieve memory savings during training, users can combine quantization and half-precision modes.
 
-We conducted several fine-tuning jobs with same dataset and `batch_size = {2,4, 6, 8}`, incorporating  *Baseline@Alpaca-Parallel* and m-LoRA. 
+To enable quantization support, please manually install `bitsandbytes`:
 
-*Baseline@Alpaca-Parallel* triggered OOM error after 3 parallel tasks when batch size = 8, while m-LoRA can handle twice that amount.
+```bash
+pip3 install bitsandbytes==0.41.3
+```
 
-#### Batching Strategies
+It's crucial to note that regardless of the settings, **LoRA weights are always calculated and stored at full precision**. For maintaining calculation accuracy, m-LoRA framework mandates the use of full precision for calculations when accuracy is imperative.
 
-Method|Training Latency|Peak Memory Usage|Average GPU Utilization|Training Throughput
-:---:|:---:|:---:|:---:|:---:
-Baseline@Alpaca-Seq|27.73h|10.68GB|79.39%|653.35 token/s
-m-LoRA@M1|36.82h|23.82GB|96.52%|672.54 token/s
-m-LoRA@M2|39.14h|23.86GB|96.41%|671.28 token/s
-m-LoRA@M3|22.97h|23.85GB|95.22%|674.41 token/s
+For users with NVIDIA Ampere or newer GPU architectures, the `--tf32` option can be utilized to enable full-precision calculation acceleration.
 
-We conducted four fine-tuning jobs with different dataset but same hyper-parameters, incorporating  *Baseline@Alpaca-Seq* and m-LoRA. 
+## Known issues
 
-During the experimental process, we collected following metrics:
- + *Training Latency* = Job completion time
- + *Throughput* = The number of passed tokens in model forward process / training latency
- + *Memory Usage* = Peak video memory usage
- + *GPU Utilization* = Average GPU utilization
+ + DoRA with Quantization on Qwen2
+ + Half Precision with Qwen2
 
-All metrics are computed for each job. `M1, M2, M3` represent three batch strategies of m-LoRA: *Optimal-Fit, Trivial, and Fast-Fit*. `BASELINE` denotes *Baseline@Alpaca-Seq*.
+## Installation
 
-The *Optimal-Fit* strategy performs the best across all four metrics, while the other two strategies also outperform the baseline method other than training latency.
-### Use Cases:
-- Domain-Specific Fine-Tuning: This involves adapting a single model with various parameters particularly for one domain.
-- Cross-Domain Fine-Tuning: This method leverages the base model to fine-tune multiple models, each intended for a different domain.
+Please refer to [Install Guide](./docs/Install.md).
 
 ## Quickstart
 
-Firstly, you should clone this repository and install dependencies:
+You can use m-LoRA via `launch.py` conveniently:
+
 ```bash
-# Clone Repository
-git clone https://github.com/TUDB-Labs/multi-lora-fine-tune
-cd multi-lora-fine-tune
-# Install requirements
-pip install -r requirements.txt
+# Generating configuration
+python launch.py gen --template lora --tasks yahma/alpaca-cleaned
+# Running the training task
+python launch.py run --base_model yahma/llama-7b-hf
 ```
 
+For further detailed usage information, please use the `help` command:
+
+```bash
+python launch.py help
+```
+
+## m-LoRA
+
 The `mlora.py` code is a starting point for finetuning on various datasets.
 Basic command for finetuning a baseline model on the [Alpaca Cleaned](https://github.com/gururise/AlpacaDataCleaned) dataset:
 ```bash
 python mlora.py \
   --base_model yahma/llama-7b-hf \
   --config ./config/alpaca.json \
-  --load_8bit
+  --load_16bit
 ```
 
 You can check the template finetune configuration in [template](./template/) folder.
 
 For further detailed usage information, please use `--help` option:
 ```bash
 python mlora.py --help
 ```
-## Demo on Colab
-You can run finetune on Colab by following this example: [Google Colab Example](https://colab.research.google.com/drive/13ABrrcOv5iG1TCdKGZvxy9QN6YwPpOoI?usp=sharing). Make sure to switch the runtime environment to GPU before running it.
-## Installation
-You can also install m-LoRA into your environment:
-```bash
-# Optional but recommended
-conda create -n mlora_env python=3.8
-conda activate mlora_env
-# Install requirements
-pip install -r requirements.txt
-```
-After installation, you can use m-LoRA directly in your code:
-```python
-import mlora
+
+## Use Docker
+
+Firstly, ensure that you have installed Docker Engine and NVIDIA Container Toolkit correctly.
+
+After that, you can launch the container using the following typical command:
+
 ```
+docker run --gpus all -it --rm mikecovlee/mlora
+```
+
+You can check all available tags from: [mikecovlee/mlora/tags](https://hub.docker.com/r/mikecovlee/mlora/tags)
+
+Please note that this container only provides a proper environment to run m-LoRA. The codes of m-LoRA are not included.
+
 ## Contributing
 We welcome contributions to improve this repository! Please review the contribution guidelines before submitting pull requests or issues.
 
 Fork the repository.
 Create a new branch for your feature or fix.
 Submit a pull request with a detailed explanation of your changes.
 
+You can use the pre-commit to check your code.
+```bash
+ln -s ../../.github/workflows/pre-commit .git/hooks/pre-commit
+```
+
 ## Citation
 Please cite the repo if you use the code in this repo.
 ```bibtex
 @misc{m-LoRA,
   author = {Zhengmao, Ye\textsuperscript{*} and Dengchun, Li\textsuperscript{*} and Jingqi, Tian and Tingfeng, Lan and Yanbo, Liang and Yexi, Jiang and Jie, Zuo and Hui, Lu and Lei, Duan and Mingjie, Tang},
   title = {m-LoRA: Efficient LLM Model Fine-tune and Inference via Multi-Lora Optimization},
   year = {2023},
   publisher = {GitHub},
-  howpublished = {\url{https://github.com/TUDB-Labs/multi-lora-fine-tune}},
+  howpublished = {\url{https://github.com/scukdde-llm/mlora}},
   note={\textsuperscript{*}: these authors contributed equally to this work.}
 }
 ```
 
 ## Copyright
-Copyright © 2023 All Rights Reserved.
+Copyright © 2023-2024 All Rights Reserved.
 
 This project is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
 
 ```
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mlora-0.1/mlora/checkpoint.py` & `mlora-0.2.1/mlora/checkpoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import torch
 from typing import Any, Iterable, List, Tuple
+from mlora.backends import _backend
+
+import torch
 
 
 def detach_variable(inputs: Tuple[Any, ...]) -> Tuple[torch.Tensor, ...]:
     if isinstance(inputs, tuple):
         out = []
         for inp in inputs:
             if not isinstance(inp, torch.Tensor):
@@ -20,29 +22,27 @@
 
 def check_backward_validity(inputs: Iterable[Any]) -> None:
     if not any(inp.requires_grad for inp in inputs if isinstance(inp, torch.Tensor)):
         raise RuntimeError("Input need grad")
 
 
 def get_device_states(*args) -> Tuple[List[int], List[torch.Tensor]]:
-    fwd_gpu_devices = list({arg.get_device() for arg in args
-                            if isinstance(arg, torch.Tensor) and arg.is_cuda})
+    fwd_gpu_devices = list({arg.device.index for arg in args
+                            if isinstance(arg, torch.Tensor) and arg.device.type == _backend.device_name()})
 
     fwd_gpu_states = []
     for device in fwd_gpu_devices:
-        with torch.cuda.device(device):
-            fwd_gpu_states.append(torch.cuda.get_rng_state())
+        fwd_gpu_states.append(_backend.get_rng_state(device))
 
     return fwd_gpu_devices, fwd_gpu_states
 
 
 def set_device_states(devices, states) -> None:
     for device, state in zip(devices, states):
-        with torch.cuda.device(device):
-            torch.cuda.set_rng_state(state)
+        _backend.set_rng_state(device, state)
 
 
 def _get_autocast_kwargs():
     gpu_autocast_kwargs = {"enabled": torch.is_autocast_enabled(),
                            "dtype": torch.get_autocast_gpu_dtype(),
                            "cache_enabled": torch.is_autocast_cache_enabled()}
 
@@ -72,17 +72,17 @@
     @staticmethod
     def forward(ctx, run_function, *args):
         check_backward_validity(args)
         ctx.run_function = run_function
         ctx.gpu_autocast_kwargs, ctx.cpu_autocast_kwargs = _get_autocast_kwargs()
         ctx.fwd_cpu_state = torch.get_rng_state()
 
-        ctx.had_cuda_in_fwd = False
-        if torch.cuda._initialized:
-            ctx.had_cuda_in_fwd = True
+        ctx.had_gpu_in_fwd = False
+        if _backend.is_initialized():
+            ctx.had_gpu_in_fwd = True
             ctx.fwd_gpu_devices, ctx.fwd_gpu_states = get_device_states(
                 *args)
 
         ctx.inputs = []
         ctx.tensor_indices = []
         tensor_inputs = []
         for i, arg in enumerate(args):
@@ -107,36 +107,33 @@
         tensor_indices = ctx.tensor_indices
         tensors = ctx.saved_tensors
 
         for i, idx in enumerate(tensor_indices):
             inputs[idx] = tensors[i]
 
         rng_devices = []
-        if ctx.had_cuda_in_fwd:
+        if ctx.had_gpu_in_fwd:
             rng_devices = ctx.fwd_gpu_devices
-        with torch.random.fork_rng(devices=rng_devices):
+        with _backend.fork_rng(rng_devices):
             torch.set_rng_state(ctx.fwd_cpu_state)
-            if ctx.had_cuda_in_fwd:
+            if ctx.had_gpu_in_fwd:
                 set_device_states(ctx.fwd_gpu_devices, ctx.fwd_gpu_states)
-
             detached_inputs = detach_variable(tuple(inputs))
-            with torch.enable_grad(), \
-                    torch.cuda.amp.autocast(**ctx.gpu_autocast_kwargs), \
+            with torch.enable_grad(), _backend.autocast(**ctx.gpu_autocast_kwargs), \
                     torch.cpu.amp.autocast(**ctx.cpu_autocast_kwargs):
                 outputs = ctx.run_function(*detached_inputs)
-
-        if isinstance(outputs, torch.Tensor):
-            outputs = (outputs,)
+                if isinstance(outputs, torch.Tensor):
+                    outputs = (outputs,)
 
         outputs_with_grad = []
         args_with_grad = []
         for i in range(len(outputs)):
             if torch.is_tensor(outputs[i]) and outputs[i].requires_grad:
                 outputs_with_grad.append(outputs[i])
                 args_with_grad.append(args[i])
         if len(outputs_with_grad) == 0:
-            raise RuntimeError("No output whth grad")
+            raise RuntimeError("No output with grad")
         torch.autograd.backward(outputs_with_grad, args_with_grad)
         grads = tuple(inp.grad if isinstance(inp, torch.Tensor) else None
                       for inp in detached_inputs)
 
-        return (None, None) + grads
+        return (None,) + grads
```

### Comparing `mlora-0.1/pyproject.toml` & `mlora-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlora"
-version = "0.1"
+version = "0.2.1"
 description = "A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "torch==2.0.1",
-    "einops==0.6.1",
-    "datasets==2.14.5",
-    "accelerate==0.21.0",
-    "transformers==4.30.2",
-    "bitsandbytes==0.40.0",
-    "sentencepiece==0.1.99",
-    "scipy==1.10.1",
-    "xformers==0.0.20",
-    "nltk",
-    "jieba",
-    "rouge",
-    "rouge_chinese"
+    "torch>=2.1.2",
+    "datasets",
+    "evaluate",
+    "accelerate",
+    "transformers==4.38.2",
+    "sentencepiece",
+    "huggingface_hub",
+    "scikit-learn",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/TUDB-Labs/multi-lora-fine-tune"
-"Bug Tracker" = "https://github.com/TUDB-Labs/multi-lora-fine-tune/issues"
+"Homepage" = "https://github.com/scukdde-llm/mlora"
+"Bug Tracker" = "https://github.com/scukdde-llm/mlora/issues"
 
 [tool.setuptools.packages.find]
 include = ["mlora"]
```

