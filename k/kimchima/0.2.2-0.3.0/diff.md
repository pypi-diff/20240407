# Comparing `tmp/kimchima-0.2.2.tar.gz` & `tmp/kimchima-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.2.2.tar", max compression
+gzip compressed data, was "kimchima-0.3.0.tar", max compression
```

## Comparing `kimchima-0.2.2.tar` & `kimchima-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
--rw-r--r--   0        0        0    11343 2024-04-02 12:46:40.224640 kimchima-0.2.2/LICENSE
--rw-r--r--   0        0        0      647 2024-04-02 12:46:40.228640 kimchima-0.2.2/README.md
--rw-r--r--   0        0        0      620 2024-04-02 12:46:40.228640 kimchima-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      688 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1577 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1334 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0       95 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     3298 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/auto.py
--rw-r--r--   0        0        0     1469 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0        0 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/test_auto.py
--rw-r--r--   0        0        0     1766 2024-04-02 12:46:40.228640 kimchima-0.2.2/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 kimchima-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-07 12:39:37.614397 kimchima-0.3.0/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-07 12:39:37.614397 kimchima-0.3.0/README.md
+-rw-r--r--   0        0        0     2530 2024-04-07 12:39:37.614397 kimchima-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      991 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1558 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0      674 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1014 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3222 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4727 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1659 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3475 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1818 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     2032 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     1992 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kimchima-0.3.0/PKG-INFO
```

### Comparing `kimchima-0.2.2/LICENSE` & `kimchima-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.2.2/src/kimchima/cmds/auto_cli.py` & `kimchima-0.3.0/src/kimchima/cmds/auto_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from kimchima.pkg import Auto
+from kimchima.pkg import ModelFactory
 
 
-class CommandAuto:
+class CommandAutoModel:
     """
-    A class for auto command.
+    A class for loading models.
     """
 
     @staticmethod
     def auto(args):
         """
         Get embeddings of text.
 
         Args:
             args (argparse.Namespace): The arguments.
 
         Returns:
             torch.tensor: The embeddings of text.
         """
-        model = Auto(model_name_or_path=args.model_name_or_path)
-        embeddings = model.get_embeddings(text=args.text)
-        print(embeddings)
+        model = ModelFactory.auto_model(pretrained_model_name_or_path=args.model_name)
+        print(model.config)
```

### Comparing `kimchima-0.2.2/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.3.0/src/kimchima/cmds/kimchima_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 
-from kimchima.cmds.auto_cli import CommandAuto
+from kimchima.cmds.auto_cli import CommandAutoModel
 
 
 def main():
     """
     Main function for kimchima.
     """
     parser = argparse.ArgumentParser(
@@ -27,15 +27,15 @@
     )
     subparsers = parser.add_subparsers(help="sub-command help")
 
 
     parser_auto=subparsers.add_parser("auto", help="auto help")
     parser_auto.add_argument("model_name_or_path", default="sentence-transformers/all-MiniLM-L6-v2", help="model name or path")
     parser_auto.add_argument("text", help="text str or list of text str")
-    parser_auto.set_defaults(func=CommandAuto.auto)
+    parser_auto.set_defaults(func=CommandAutoModel.auto)
 
     args = parser.parse_args()
     args.func(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `kimchima-0.2.2/src/kimchima/pkg/auto.py` & `kimchima-0.3.0/src/kimchima/pkg/embedding_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 # coding=utf-8
-# Copyright [2024] [Aisuko]
+# Copyright [2024] [SkywardAI]
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #        http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 import torch
 import torch.nn.functional as F
-from transformers import AutoTokenizer, AutoModel
+from kimchima.pkg import logging
 
 
-class Auto:
-    """
-    A class for load model and it's tokenizer by using model name or path of model.
+logger = logging.get_logger(__name__)
+
+
+class EmbeddingsFactory:
+    r"""
+
+    Embeddings class to get embeddings from the specified model and tokenizer.
+    The embeddings mean pooling is used to get the embeddings from the model,
+    and the embeddings are normalized using L2 normalization.
+
+    Args:
+        pretrained_model_name_or_path: pretrained model name or path
+
+    Returns:
+        sentence_embeddings: sentence embeddings type torch.Tensor
+
     """
-    def __init__(self, *args, **kwargs):
-        """
-        Initialize the class with model name or path of model.
-        
+
+    def __init__(self):
+        raise EnvironmentError(
+            "Embeddings is designed to be instantiated "
+            "using the `Embeddings.from_pretrained(pretrained_model_name_or_path)` method."
+        )
+
+
+    @classmethod
+    def get_text_embeddings(cls, *args, **kwargs)-> torch.Tensor:
+        r"""
+        Get embeddings from the model.
+
         Args:
-            model_name_or_path (str): The model name or path of model.
-        
-        Returns:
-            None
+            prompt: prompt text
+            device: device to run the model
+            max_length: maximum length of the input text
         """
-        model_name_or_path = kwargs.pop('model_name_or_path', None)
-        if model_name_or_path is None:
-            return None
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
-        # https://github.com/huggingface/transformers/blob/v4.39.2/src/transformers/models/auto/auto_factory.py#L444
-        # TODO @aisuko: add more parameters
-        self.model = AutoModel.from_pretrained(model_name_or_path)
+        model=kwargs.pop('model', None)
+        tokenizer=kwargs.pop('tokenizer', None)
+        prompt = kwargs.pop('prompt', None)
+        device = kwargs.pop('device', 'cpu')
+        max_length = kwargs.pop('max_length', 512)
 
-    def get_embeddings(self, *args, **kwargs):
-        """
-        Get embeddings of text.
 
-        Args:
-            text (str): The text to get embeddings.
-            device (str): The device to use. Default is 'cpu'.
-            max_length (int): The maximum length of text. Default is 512.
+        inputs_ids = tokenizer(prompt, return_tensors='pt',max_length=max_length, padding=True, truncation=True).to(device)
 
-        Returns:
-            torch.tensor: The embeddings of text.
-        """
-        try:
-            text = kwargs.pop('text', None)
-            device = kwargs.pop('device', 'cpu')
-            max_length = kwargs.pop('max_length', 512)
-
-            inputs_ids = self.tokenizer(text, return_tensors='pt',max_length=max_length, padding=True, truncation=True).to(device)
-
-            with torch.no_grad():
-                output = self.model(**inputs_ids)
-            
-            embeddings=Auto.mean_pooling(output, inputs_ids['attention_mask'])
+        model=model.to(device)
+        with torch.no_grad():
+            output = model(**inputs_ids)
+
+        embeddings=cls.mean_pooling(model_output=output, attention_mask=inputs_ids['attention_mask'])
+        logger.debug(f"Embedding mean pooling: {embeddings.shape}")
 
-            # Normalize embeddings
-            sentence_embeddings = F.normalize(embeddings, p=2, dim=1)
+        # Normalize embeddings
+        sentence_embeddings = F.normalize(embeddings, p=2, dim=1)
 
-        except Exception as e:
-            sentence_embeddings=None
         return sentence_embeddings
 
-    @staticmethod
+
+    @classmethod
     #Mean Pooling - Take attention mask into account for correct averaging
-    def mean_pooling(model_output, attention_mask):
-        """
-        Mean pooling of model output.
+    def mean_pooling(cls, **kwargs) -> torch.Tensor:
+        r"""
+        Mean Pooling - Take attention mask into account for correct averaging.
 
         Args:
-            model_output (torch.tensor): The model output.
-            attention_mask (torch.tensor): The attention mask.
-
-        Returns:
-            torch.tensor: The mean pooling of model output.
+            model_output: model output
+            attention_mask: attention mask
         """
+        model_output = kwargs.get('model_output')
+        attention_mask = kwargs.get('attention_mask')
         token_embeddings = model_output[0] #First element of model_output contains all token embeddings
         input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
-        return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
+        return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
```

### Comparing `kimchima-0.2.2/src/kimchima/pkg/devices.py` & `kimchima-0.3.0/src/kimchima/pkg/devices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright [2024] [Aisuko]
+# Copyright [2024] [SkywardAI]
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #        http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
@@ -24,30 +24,31 @@
 class Devices(Enum):
     Silicon = 'mps'
     CPU = 'cpu'
     # only Nvidia GPU is supported currently
     GPU = 'cuda'
 
 
-def get_device()-> Devices:
-    """
-    Only support Single GPU for now
-    """
-    if platform.system() == 'Darwin':
-        return Devices.Silicon
-    elif torch.cuda.is_available():
-        return Devices.GPU
-    return Devices.CPU
-
-
-def get_capability()-> Tuple[int, int]:
-    """
-    Get the capability of the device(GPU) for current env, this is used for support latest quantization techniques like: Marlin
-    
-    Returns:
-        tuple: The capability of the device(GPU) for current env.
-
-    For not GPU env, return (0, 0)
-    """
-    if get_device() == Devices.GPU:
-        return torch.cuda.get_device_capability()
-    return (0, 0)
+    @classmethod
+    def get_device(cls)-> Devices:
+        """
+        Only support Single GPU for now
+        """
+        if platform.system() == 'Darwin':
+            return Devices.Silicon
+        elif torch.cuda.is_available():
+            return Devices.GPU
+        return Devices.CPU
+
+    @classmethod
+    def get_capability(cls)-> Tuple[int, int]:
+        """
+        Get the capability of the device(GPU) for current env, this is used for support latest quantization techniques like: Marlin
+        
+        Returns:
+            tuple: The capability of the device(GPU) for current env.
+
+        For not GPU env, return (0, 0)
+        """
+        if cls.get_device() == Devices.GPU:
+            return torch.cuda.get_device_capability()
+        return (0, 0)
```

### Comparing `kimchima-0.2.2/src/kimchima/tests/test_auto.py` & `kimchima-0.3.0/src/kimchima/tests/test_embedding_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,74 @@
 # coding=utf-8
-# Copyright [2024] [Aisuko]
+# Copyright [2024] [SkywardAI]
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #        http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from kimchima.pkg import Auto
+from kimchima.pkg import (
+    ModelFactory,
+    TokenizerFactory,
+    EmbeddingsFactory
+)
 
 
-class TestAuto(unittest.TestCase):
+class TestAutoFactory(unittest.TestCase):
 
     model_name = 'sentence-transformers/all-MiniLM-L6-v2'
+    model=None
+    tokenizer=None
+
+    @classmethod
+    def setUpClass(cls):
+        cls.model = ModelFactory.auto_model(pretrained_model_name_or_path=cls.model_name)
+        cls.tokenizer = TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=cls.model_name)
+
+
+    @classmethod
+    def tearDownClass(cls):
+        pass
+
 
     def test_get_embeddings(self):
         """
         Test get_embeddings method
         """
-        model = Auto(model_name_or_path=self.model_name)
-        embeddings = model.get_embeddings(text='Melbourne')
+
+        self.assertIsNotNone(self.model)
+
+        embeddings = EmbeddingsFactory.get_text_embeddings(
+            model=self.model,
+            tokenizer=self.tokenizer, 
+            prompt='Melbourne',
+            device='cpu'
+            )
+
         self.assertIsNotNone(embeddings)
         self.assertEqual(embeddings.shape, (1, 384))
 
 
     def test_get_embeddings_with_list(self):
         """
-        Test get_embeddings method with list of text
+        Test get_embeddings method with list
         """
-        model = Auto(model_name_or_path=self.model_name)
-        embeddings = model.get_embeddings(text=['Melbourne', 'Sydney'])
+
+        self.assertIsNotNone(self.model)
+
+        embeddings = EmbeddingsFactory.get_text_embeddings(
+            model=self.model,
+            tokenizer=self.tokenizer, 
+            prompt=['Melbourne', 'Sydney'],
+            device='cpu'
+            )
+
         self.assertIsNotNone(embeddings)
         self.assertEqual(embeddings.shape, (2, 384))
-
```

### Comparing `kimchima-0.2.2/PKG-INFO` & `kimchima-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.2.2
+Version: 0.3.0
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
-Keywords: ai,llm
+Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: accelerate (==0.28.0)
+Requires-Dist: bitsandbytes (==0.43.0)
 Requires-Dist: sentencepiece (==0.2.0)
 Requires-Dist: torch (==2.2.2)
 Requires-Dist: transformers (==4.39.2)
 Project-URL: Repository, https://github.com/Aisuko/kimchi
 Description-Content-Type: text/markdown
 
 # kimchima
 
 [![Backend CI/CD 🚀](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml)
 [![Release Drafter 🚀](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 The collections of tools for ML model development.
 
 
 # Usage
 
 See examples in the [examples](./examples) directory.
 
+
+# Development
+
+Please kindly check the .devcontainer directory for the development environment setup.
+
 # Acknowledgement
 
 - [Llama2-burn Project](https://github.com/Gadersd/llama2-burn/tree/main)
 
 
 # License
```

