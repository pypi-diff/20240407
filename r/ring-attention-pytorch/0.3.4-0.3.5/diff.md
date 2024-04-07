# Comparing `tmp/ring-attention-pytorch-0.3.4.tar.gz` & `tmp/ring-attention-pytorch-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.4.tar", last modified: Sat Apr  6 16:19:32 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.5.tar", last modified: Sun Apr  7 18:00:06 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.4.tar` & `ring-attention-pytorch-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:19:32.384626 ring-attention-pytorch-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 16:19:32.384626 ring-attention-pytorch-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:19:32.384626 ring-attention-pytorch-0.3.4/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25501 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:19:32.384626 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 16:19:32.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 16:19:32.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:19:32.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-06 16:19:32.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 16:19:32.000000 ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:19:32.384626 ring-attention-pytorch-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-06 16:19:23.000000 ring-attention-pytorch-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.622834 ring-attention-pytorch-0.3.5/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/setup.py
```

### Comparing `ring-attention-pytorch-0.3.4/LICENSE` & `ring-attention-pytorch-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.4/PKG-INFO` & `ring-attention-pytorch-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.4
+Version: 0.3.5
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.4/README.md` & `ring-attention-pytorch-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="./ring.png" width="450px"></img>
 
 ## Ring Attention - Pytorch
 
-Explorations into <a href="https://arxiv.org/abs/2310.01889">Ring Attention</a>, from <a href="https://www.haoliu.site/">Liu</a> et al. at Berkeley AI.
+Implementation of <a href="https://arxiv.org/abs/2310.01889">Ring Attention</a>, from <a href="https://www.haoliu.site/">Liu</a> et al. at Berkeley AI, in Pytorch.
 
 It basically splits the data across the sequence dimension (instead of batch) and applies ring reduce to the processing of the tiles of the attention matrix, flash attention style.
 
 I believe this is being used for the 1-10 million tokens for the latest Gemini. At least some form of it; the other possibility would be unpublished improvements on top of <a href="https://github.com/lucidrains/recurrent-memory-transformer-pytorch">RMT</a>.
 
 In addition, the repository also contains the logic for <a href="https://arxiv.org/abs/2311.09431">Striped Attention</a>, a follow up paper that permutes the sequence for better workload balancing for autoregressive transformers.
 
@@ -89,19 +89,18 @@
     - [x] dk, dv needs to be float32, while kv needs to be float16. see if both can be cast to int before stacked and ring passed all in one go, then reinterpret back to float32 and float16
     - [x] prevent an unnecessary `tl.load` on the first ring pass
     - [x] cuda backwards pass must have same dq, dk, dv as naive
 - [x] fix naive flash attention backwards
 - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise flash attention is ineffective
 - [x] for cuda striped attention, for backwards hack, pad the extra token once and index out when passing into Tri's cuda kernel
+- [x] find a machine with 8 GPUs and test with a quarter million tokens first
 
-- [ ] find a machine with 8 GPUs and test with a quarter million tokens first
 - [ ] think about how to craft a special `Dataset` that shards across sequence length (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some cuda ring reduce impl
-- [ ] `batch_isend_irecv` in the presence of key padding mask needing ring exchange, but not a big priority
 - [ ] figure out how to pytest distributed pytorch
 - [ ] use sdp context manager to validate when it is possible to use `ring_flash_attn_cuda`, otherwise assert out
 
 ## Citations
 
 ```bibtex
 @article{Liu2023RingAW,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-[./ring.png]## Ring Attention - Pytorch Explorations into _R_i_n_g_ _A_t_t_e_n_t_i_o_n, from
-_L_i_u et al. at Berkeley AI. It basically splits the data across the sequence
-dimension (instead of batch) and applies ring reduce to the processing of the
-tiles of the attention matrix, flash attention style. I believe this is being
-used for the 1-10 million tokens for the latest Gemini. At least some form of
-it; the other possibility would be unpublished improvements on top of _R_M_T. In
-addition, the repository also contains the logic for _S_t_r_i_p_e_d_ _A_t_t_e_n_t_i_o_n, a
-follow up paper that permutes the sequence for better workload balancing for
+[./ring.png]## Ring Attention - Pytorch Implementation of _R_i_n_g_ _A_t_t_e_n_t_i_o_n, from
+_L_i_u et al. at Berkeley AI, in Pytorch. It basically splits the data across the
+sequence dimension (instead of batch) and applies ring reduce to the processing
+of the tiles of the attention matrix, flash attention style. I believe this is
+being used for the 1-10 million tokens for the latest Gemini. At least some
+form of it; the other possibility would be unpublished improvements on top of
+_R_M_T. In addition, the repository also contains the logic for _S_t_r_i_p_e_d_ _A_t_t_e_n_t_i_o_n,
+a follow up paper that permutes the sequence for better workload balancing for
 autoregressive transformers. ## Appreciation - _A_1_6_Z_ _O_p_e_n_ _S_o_u_r_c_e_ _A_I_ _G_r_a_n_t
 _P_r_o_g_r_a_m for the generous sponsorship, as well as my other sponsors, for
 affording me the independence to open source current artificial intelligence
 research ## Install ```bash $ pip install ring-attention-pytorch ``` ## Usage
 ```python import torch from ring_attention_pytorch import RingAttention attn =
 RingAttention( dim = 512, dim_head = 64, heads = 8, causal = True,
 auto_shard_seq = True, ring_attn = True, ring_seq_size = 512 ) tokens =
@@ -49,35 +49,34 @@
 stacked and ring passed all in one go, then reinterpret back to float32 and
 float16 - [x] prevent an unnecessary `tl.load` on the first ring pass - [x]
 cuda backwards pass must have same dq, dk, dv as naive - [x] fix naive flash
 attention backwards - [x] validate cuda causal and striped ring attention works
 - [x] make sure cuda striped attention works for multiple buckets, otherwise
 flash attention is ineffective - [x] for cuda striped attention, for backwards
 hack, pad the extra token once and index out when passing into Tri's cuda
-kernel - [ ] find a machine with 8 GPUs and test with a quarter million tokens
+kernel - [x] find a machine with 8 GPUs and test with a quarter million tokens
 first - [ ] think about how to craft a special `Dataset` that shards across
 sequence length (take into account labels for cross entropy loss) for ring
 transformer training - [ ] add ring attention to Tri's flash attention
-implementation. find some cuda ring reduce impl - [ ] `batch_isend_irecv` in
-the presence of key padding mask needing ring exchange, but not a big priority
-- [ ] figure out how to pytest distributed pytorch - [ ] use sdp context
-manager to validate when it is possible to use `ring_flash_attn_cuda`,
-otherwise assert out ## Citations ```bibtex @article{Liu2023RingAW, title =
-{Ring Attention with Blockwise Transformers for Near-Infinite Context}, author
-= {Hao Liu and Matei Zaharia and Pieter Abbeel}, journal = {ArXiv}, year =
-{2023}, volume = {abs/2310.01889}, url = {https://api.semanticscholar.org/
-CorpusID:263608461} } ``` ```bibtex @article{Brandon2023StripedAF, title =
-{Striped Attention: Faster Ring Attention for Causal Transformers}, author =
-{William Brandon and Aniruddha Nrusimha and Kevin Qian and Zachary Ankner and
-Tian Jin and Zhiye Song and Jonathan Ragan-Kelley}, journal = {ArXiv}, year =
-{2023}, volume = {abs/2311.09431}, url = {https://api.semanticscholar.org/
-CorpusID:265220849} } ``` ```bibtex @article{Dao2022FlashAttentionFA, title =
-{FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness},
-author = {Tri Dao and Daniel Y. Fu and Stefano Ermon and Atri Rudra and
-Christopher R'e}, journal = {ArXiv}, year = {2022}, volume = {abs/2205.14135} }
-``` ```bibtex @article{dao2023flashattention2, title = {Flash{A}ttention-2:
-Faster Attention with Better Parallelism and Work Partitioning, author = {Dao,
-Tri}, year = {2023} } ``` ```bibtex @article{Tillet2019TritonAI, title =
-{Triton: an intermediate language and compiler for tiled neural network
-computations}, author = {Philippe Tillet and H. Kung and D. Cox}, journal =
-{Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning
-and Programming Languages}, year = {2019} } ```
+implementation. find some cuda ring reduce impl - [ ] figure out how to pytest
+distributed pytorch - [ ] use sdp context manager to validate when it is
+possible to use `ring_flash_attn_cuda`, otherwise assert out ## Citations
+```bibtex @article{Liu2023RingAW, title = {Ring Attention with Blockwise
+Transformers for Near-Infinite Context}, author = {Hao Liu and Matei Zaharia
+and Pieter Abbeel}, journal = {ArXiv}, year = {2023}, volume = {abs/
+2310.01889}, url = {https://api.semanticscholar.org/CorpusID:263608461} } ```
+```bibtex @article{Brandon2023StripedAF, title = {Striped Attention: Faster
+Ring Attention for Causal Transformers}, author = {William Brandon and
+Aniruddha Nrusimha and Kevin Qian and Zachary Ankner and Tian Jin and Zhiye
+Song and Jonathan Ragan-Kelley}, journal = {ArXiv}, year = {2023}, volume =
+{abs/2311.09431}, url = {https://api.semanticscholar.org/CorpusID:265220849} }
+``` ```bibtex @article{Dao2022FlashAttentionFA, title = {FlashAttention: Fast
+and Memory-Efficient Exact Attention with IO-Awareness}, author = {Tri Dao and
+Daniel Y. Fu and Stefano Ermon and Atri Rudra and Christopher R'e}, journal =
+{ArXiv}, year = {2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
+{dao2023flashattention2, title = {Flash{A}ttention-2: Faster Attention with
+Better Parallelism and Work Partitioning, author = {Dao, Tri}, year = {2023} }
+``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
+language and compiler for tiled neural network computations}, author =
+{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
+SIGPLAN International Workshop on Machine Learning and Programming Languages},
+year = {2019} } ```
```

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,15 @@
         self.use_cuda_kernel = use_cuda_kernel
 
         self.eps = eps
         self.heads = heads
         self.scale = dim_head ** -0.5
         self.causal = causal
 
-        assert divisible_by(ring_seq_size, bucket_size)
+        assert (not ring_attn) or divisible_by(ring_seq_size, bucket_size), f'ring seq size {ring_seq_size} is not divisible by bucket size {bucket_size}'
 
         self.ring_attn = ring_attn
         self.max_lookback_seq_len = max_lookback_seq_len
         self.striped_ring_attn = striped_ring_attn
 
         self.using_striped_ring_cuda = striped_ring_attn and use_cuda_kernel
 
@@ -464,15 +464,16 @@
         self.ring_attn = ring_attn
         self.striped_ring_attn = striped_ring_attn
 
         self.using_striped_ring_cuda = use_cuda_kernel and striped_ring_attn
 
         self.ring_seq_size = ring_seq_size
         self.bucket_size = bucket_size
-        assert divisible_by(ring_seq_size, bucket_size)
+
+        assert (not ring_attn) or divisible_by(ring_seq_size, bucket_size), f'ring seq size {ring_seq_size} is not divisible by bucket size {bucket_size}'
 
         self.auto_shard_seq = default(auto_shard_seq, ring_attn) # if ring attention is turned on, auto-shard across sequence dimension. this can also be turned off and done manually elsewhere in the data loading
 
         assert not (not self.ring_attn and self.auto_shard_seq)
         assert not (not self.ring_attn and self.striped_ring_attn)
         assert not (self.striped_ring_attn and not causal), 'striped ring attention only applies to autoregressive models'
```

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 from einops import rearrange, repeat
 
 # helpers
 
 def exists(v):
     return v is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
+def divisible_by(num, den):
+    return (num % den) == 0
+
 def first(seq):
     return seq[0]
 
 def pad_at_dim(t, pad: Tuple[int, int], *, dim = -1, value = 0.):
     dims_from_right = (- dim - 1) if dim < 0 else (t.ndim - dim - 1)
     zeros = ((0, 0) * dims_from_right)
     return F.pad(t, (*zeros, *pad), value = value)
@@ -457,25 +463,14 @@
         BLOCK_N = BLOCK,
         num_warps = num_warps,
         num_stages = 1,
     )
 
     return o, m, lse
 
-# helper functions
-
-def exists(val):
-    return val is not None
-
-def default(val, d):
-    return val if exists(val) else d
-
-def divisible_by(num, den):
-    return (num % den) == 0
-
 # ring + (flash) attention forwards and backwards
 
 # flash attention v1 - https://arxiv.org/abs/2205.14135
 # flash attention v2 - https://tridao.me/publications/flash2/flash2.pdf
 # ring attention - https://arxiv.org/abs/2310.01889
 
 class RingFlashAttentionCUDAFunction(Function):
```

### Comparing `ring-attention-pytorch-0.3.4/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.4
+Version: 0.3.5
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.4/setup.py` & `ring-attention-pytorch-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.4',
+  version = '0.3.5',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

