# Comparing `tmp/billm-0.1.1.tar.gz` & `tmp/billm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billm-0.1.1.tar", last modified: Tue Mar 19 04:23:13 2024, max compression
+gzip compressed data, was "billm-0.1.2.tar", last modified: Sun Apr  7 02:07:53 2024, max compression
```

## Comparing `billm-0.1.1.tar` & `billm-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1060 2024-03-14 10:50:27.655921 billm-0.1.1/LICENSE
--rw-r--r--   0        0        0     3934 2024-03-19 04:22:01.106485 billm-0.1.1/README.md
--rw-r--r--   0        0        0      486 2024-03-19 04:23:13.476404 billm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      127 2024-03-19 04:22:19.359678 billm-0.1.1/src/billm/__init__.py
--rw-r--r--   0        0        0      267 2024-03-17 05:50:48.094383 billm-0.1.1/src/billm/config.py
--rw-r--r--   0        0        0    13485 2024-03-19 04:22:01.108432 billm-0.1.1/src/billm/modeling_llama.py
--rw-r--r--   0        0        0    11543 2024-03-19 04:22:01.109209 billm-0.1.1/src/billm/modeling_mistral.py
--rw-r--r--   0        0        0        0 2024-03-17 05:50:48.095776 billm-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      458 2024-03-17 05:50:48.096777 billm-0.1.1/tests/test_modeling_llama.py
--rw-r--r--   0        0        0      483 2024-03-17 05:50:48.097312 billm-0.1.1/tests/test_modeling_mistral.py
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 billm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-14 10:50:27.655921 billm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3934 2024-03-19 04:22:01.106485 billm-0.1.2/README.md
+-rw-r--r--   0        0        0      486 2024-04-07 02:07:53.413924 billm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-04-07 02:06:41.946201 billm-0.1.2/src/billm/__init__.py
+-rw-r--r--   0        0        0      267 2024-03-17 05:50:48.094383 billm-0.1.2/src/billm/config.py
+-rw-r--r--   0        0        0    13843 2024-04-07 02:06:29.685294 billm-0.1.2/src/billm/modeling_llama.py
+-rw-r--r--   0        0        0    11901 2024-04-07 02:06:29.688044 billm-0.1.2/src/billm/modeling_mistral.py
+-rw-r--r--   0        0        0        0 2024-03-17 05:50:48.095776 billm-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      458 2024-03-17 05:50:48.096777 billm-0.1.2/tests/test_modeling_llama.py
+-rw-r--r--   0        0        0      483 2024-03-17 05:50:48.097312 billm-0.1.2/tests/test_modeling_mistral.py
+-rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 billm-0.1.2/PKG-INFO
```

### Comparing `billm-0.1.1/LICENSE` & `billm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `billm-0.1.1/README.md` & `billm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `billm-0.1.1/src/billm/modeling_llama.py` & `billm-0.1.2/src/billm/modeling_llama.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,15 +228,21 @@
     LLAMA_START_DOCSTRING,
 )
 class LlamaForTokenClassification(LlamaPreTrainedModel):
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = config.num_labels
         self.model = LlamaModel(config)
-        self.dropout = nn.Dropout(0.1)
+        if hasattr(config, "classifier_dropout") and config.classifier_dropout is not None:
+            classifier_dropout = config.classifier_dropout
+        elif hasattr(config, "hidden_dropout") and config.hidden_dropout is not None:
+            classifier_dropout = config.hidden_dropout
+        else:
+            classifier_dropout = 0.1
+        self.dropout = nn.Dropout(classifier_dropout)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
         return self.model.embed_tokens
```

### Comparing `billm-0.1.1/src/billm/modeling_mistral.py` & `billm-0.1.2/src/billm/modeling_mistral.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,15 +202,21 @@
     MISTRAL_START_DOCSTRING,
 )
 class MistralForTokenClassification(MistralPreTrainedModel):
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = config.num_labels
         self.model = MistralModel(config)
-        self.dropout = nn.Dropout(0.1)
+        if hasattr(config, "classifier_dropout") and config.classifier_dropout is not None:
+            classifier_dropout = config.classifier_dropout
+        elif hasattr(config, "hidden_dropout") and config.hidden_dropout is not None:
+            classifier_dropout = config.hidden_dropout
+        else:
+            classifier_dropout = 0.1
+        self.dropout = nn.Dropout(classifier_dropout)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
 
         # Initialize weights and apply final processing
         self.post_init()
 
     def get_input_embeddings(self):
         return self.model.embed_tokens
```

### Comparing `billm-0.1.1/PKG-INFO` & `billm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BiLLM
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tool for converting LLMs from uni-directional to bi-directional for tasks like classification and sentence embeddings.
 Author-Email: Sean Lee <xmlee97@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: transformers>=4.38.2
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BiLLM Version: 0.1.1 Summary: Tool for converting
+Metadata-Version: 2.1 Name: BiLLM Version: 0.1.2 Summary: Tool for converting
 LLMs from uni-directional to bi-directional for tasks like classification and
 sentence embeddings. Author-Email: Sean Lee
 gmail.com> License: MIT Requires-Python: >=3.8 Requires-Dist:
 transformers>=4.38.2 Description-Content-Type: text/markdown # BiLLM Tool for
 converting LLMs from uni-directional to bi-directional for tasks like
 classification and sentence embeddings. Compatible with ð¤ transformers.
 _[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_0_._0_1_2_0_8_]_[_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_1_1_._0_5_2_9_6_]_[_P_y_P_I
```

