# Comparing `tmp/vectara-cli-0.1.6.tar.gz` & `tmp/vectara-cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.6.tar", last modified: Sat Apr  6 19:32:15 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.7.tar", last modified: Sun Apr  7 07:32:49 2024, max compression
```

## Comparing `vectara-cli-0.1.6.tar` & `vectara-cli-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.696351 vectara-cli-0.1.6/
--rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/LICENSE.md
--rw-rw-rw-   0        0        0    22346 2024-04-06 19:32:15.692781 vectara-cli-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    21180 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 19:32:15.697354 vectara-cli-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1428 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.535153 vectara-cli-0.1.6/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.6/vectara_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.577930 vectara-cli-0.1.6/vectara_cli/advanced/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/advanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.588693 vectara-cli-0.1.6/vectara_cli/advanced/commercial/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/advanced/commercial/__init__.py
--rw-rw-rw-   0        0        0     7672 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/commercial/enterprise.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.607301 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/nerdspan.py
--rw-rw-rw-   0        0        0     9784 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/rebel.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.681456 vectara-cli-0.1.6/vectara_cli/commands/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/commands/__init__.py
--rw-rw-rw-   0        0        0      906 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/create_corpus.py
--rw-rw-rw-   0        0        0      750 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/delete_corpus.py
--rw-rw-rw-   0        0        0     1081 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/index_document.py
--rw-rw-rw-   0        0        0     1115 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/nerdspan_upsert_folder.py
--rw-rw-rw-   0        0        0      689 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/query.py
--rw-rw-rw-   0        0        0     1391 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/rebel_upsert_folder.py
--rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/set_api_keys.py
--rw-rw-rw-   0        0        0      773 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/commands/span-text.py
--rw-rw-rw-   0        0        0     1173 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/span_enhance_folder.py
--rw-rw-rw-   0        0        0      806 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/span_text.py
--rw-rw-rw-   0        0        0     1005 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/upload_document.py
--rw-rw-rw-   0        0        0      962 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/upload_enriched_text.py
--rw-rw-rw-   0        0        0      753 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/config_manager.py
--rw-rw-rw-   0        0        0    18174 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/core.py
--rw-rw-rw-   0        0        0     3072 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.686720 vectara-cli-0.1.6/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    22346 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1099 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.167303 vectara-cli-0.1.7/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/LICENSE.md
+-rw-rw-rw-   0        0        0    22560 2024-04-07 07:32:49.165298 vectara-cli-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    21394 2024-04-06 21:55:14.000000 vectara-cli-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 07:32:49.167303 vectara-cli-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.128798 vectara-cli-0.1.7/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.7/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.137299 vectara-cli-0.1.7/vectara_cli/advanced/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/advanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.138799 vectara-cli-0.1.7/vectara_cli/advanced/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/advanced/commercial/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.7/vectara_cli/advanced/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.143300 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.161298 vectara-cli-0.1.7/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0      860 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0      957 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/commands/set_api_keys.py
+-rw-rw-rw-   0        0        0      789 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span-text.py
+-rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span_text.py
+-rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/config_manager.py
+-rw-rw-rw-   0        0        0    18548 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     3072 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.162798 vectara-cli-0.1.7/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    22560 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1099 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.6/LICENSE.md` & `vectara-cli-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.6/PKG-INFO` & `vectara-cli-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -344,15 +344,15 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
-### Advanced Useage
+### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
@@ -456,16 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
-![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,15 +517,15 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](<Screenshot 2024-04-05 112142.png>)
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.6/README.md` & `vectara-cli-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
-### Advanced Useage
+### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
@@ -430,16 +430,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
-![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -491,15 +491,15 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](<Screenshot 2024-04-05 112142.png>)
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.6/setup.py` & `vectara-cli-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.6",
+    version="0.1.7",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
```

### Comparing `vectara-cli-0.1.6/vectara_cli/advanced/commercial/enterprise.py` & `vectara-cli-0.1.7/vectara_cli/advanced/commercial/enterprise.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/nerdspan.py` & `vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/nerdspan.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/rebel.py` & `vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/rebel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # vectara-cli\advanced\non-commercial\rebel.py
 
 import torch
+import torch.nn as nn 
 from torch.nn import CrossEntropyLoss, BCEWithLogitsLoss
 from transformers import DebertaV2Config, DebertaV2PreTrainedModel, DebertaV2Model
 from transformers.models.deberta_v2.modeling_deberta_v2 import (
     ContextPooler,
     StableDropout,
 )
 from transformers.file_utils import ModelOutput
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/create_corpus.py` & `vectara-cli-0.1.7/vectara_cli/commands/create_corpus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # create_corpus.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 3:
         print("Usage: vectara-cli create-corpus corpus_id name")
         return
     corpus_id = args[1]
     name = args[2]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        vectara_client = VectaraClient(customer_id, api_key)
         response = vectara_client.create_corpus(
             corpus_id,
             name,
             "Description",
             1234567890,
             True,
             False,
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/delete_corpus.py` & `vectara-cli-0.1.7/vectara_cli/commands/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# ./commands/delete_corpus.py
+# query.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
-def main(args):
-    if len(args) < 2:
-        print("Usage: vectara-cli delete-corpus corpus_id")
+def main(args, vectara_client):
+    if len(args) < 4:
+        print("Usage: vectara-cli query query_text num_results corpus_id")
         return
-
-    corpus_id = args[1]
+    query_text = args[1]
+    num_results = int(args[2])
+    corpus_id = args[3]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        vectara_client = VectaraClient(customer_id, api_key)
-        response, success = vectara_client.delete_corpus(corpus_id)
-
-        if success:
-            print("Corpus deleted successfully.")
-        else:
-            print("Failed to delete corpus:", response)
+        response = vectara_client.query(query_text, num_results, corpus_id)
+        print(response)
     except ValueError as e:
         print(e)
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/index_document.py` & `vectara-cli-0.1.7/vectara_cli/commands/index_document.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # index_document.py
 
 import json
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 6:
         print(
             "Usage: vectara-cli index-document corpus_id document_id title metadata_json section_text"
         )
         return
     corpus_id = args[1]
     document_id = args[2]
     title = args[3]
     metadata = json.loads(args[4])
     section_text = args[5]
 
-    # Assuming ConfigManager and VectaraClient are set up to handle API keys
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        vectara_client = VectaraClient(customer_id, api_key)
         response, success = vectara_client.index_document(
             corpus_id, document_id, title, metadata, section_text
         )
         if success:
             print("Document indexed successfully.")
         else:
             print("Document indexing failed.", response)
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/nerdspan_upsert_folder.py` & `vectara-cli-0.1.7/vectara_cli/commands/nerdspan_upsert_folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ./commands/nerdspan_upsert_folder.py
 
 import os
 from vectara_cli.advanced.noncommercial.nerdspan import Span
 from vectara_cli.config_manager import ConfigManager
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 5:
         print("Usage: vectara-cli process-and-upload folder_path model_name model_type")
         return
 
     folder_path = args[1]
     model_name = args[2]
     model_type = args[3]
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/query.py` & `vectara-cli-0.1.7/vectara_cli/commands/span-text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# query.py
+# ./commands/span_text.py
 
-from vectara_cli.core import VectaraClient
+from vectara_cli.core import Span
 from vectara_cli.config_manager import ConfigManager
 
-
-def main(args):
-    if len(args) < 4:
-        print("Usage: vectara-cli query query_text num_results corpus_id")
+def main(args, vectara_client):
+    if len(args) < 5:
+        print("Usage: vectara-cli process-text text model_name model_type")
         return
-    query_text = args[1]
-    num_results = int(args[2])
-    corpus_id = args[3]
+
+    text = args[1]
+    model_name = args[2]
+    model_type = args[3]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        vectara_client = VectaraClient(customer_id, api_key)
-        response = vectara_client.query(query_text, num_results, corpus_id)
-        print(response)
-    except ValueError as e:
-        print(e)
-
+        span = Span(text, customer_id, api_key)
+        span.load_model(model_name, model_type)
+        output_str, key_value_pairs = span.analyze_text(model_name)
+        print(output_str)
+        print(key_value_pairs)
+    except Exception as e:
+        print("Error processing text:", str(e))
 
 if __name__ == "__main__":
     import sys
-
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/rebel_upsert_folder.py` & `vectara-cli-0.1.7/vectara_cli/commands/rebel_upsert_folder.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.advanced.noncommercial.rebel import Rebel
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 4:
         print(
             "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
         )
         print(
             "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
         )
@@ -18,15 +18,14 @@
 
     folder_path = args[1]
     corpus_id_1 = args[2]
     corpus_id_2 = args[3]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        vectara_client = VectaraClient(customer_id, api_key)
 
         if not os.path.isdir(folder_path):
             print(f"The specified folder path does not exist: {folder_path}")
             return
 
         rebel = Rebel()
         rebel.advanced_upsert_folder(
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/span-text.py` & `vectara-cli-0.1.7/vectara_cli/commands/span_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ./commands/span_text.py
 
-from vectara_cli.core import Span
+from vectara_cli.advanced.noncommercial.nerdspan import Span
 from vectara_cli.config_manager import ConfigManager
 
-def main(args):
+
+def main(args, vectara_client):
     if len(args) < 5:
         print("Usage: vectara-cli process-text text model_name model_type")
         return
 
     text = args[1]
     model_name = args[2]
     model_type = args[3]
@@ -18,10 +19,12 @@
         span.load_model(model_name, model_type)
         output_str, key_value_pairs = span.analyze_text(model_name)
         print(output_str)
         print(key_value_pairs)
     except Exception as e:
         print("Error processing text:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/span_enhance_folder.py` & `vectara-cli-0.1.7/vectara_cli/commands/span_enhance_folder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ./commands/span_enhance_folder.py
 
 import os
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 5:
         print(
             "Usage: vectara-cli span-enhance-folder corpus_id_1 corpus_id_2 model_name folder_path"
         )
         return
 
     corpus_id_1 = args[1]
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/span_text.py` & `vectara-cli-0.1.7/vectara_cli/commands/upload_document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-# ./commands/span_text.py
+# ./commands/upload_document.py
 
-from vectara_cli.advanced.noncommercial.nerdspan import Span
+from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
-def main(args):
-    if len(args) < 5:
-        print("Usage: vectara-cli process-text text model_name model_type")
+def main(args, vectara_client):
+    if len(args) < 4:
+        print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
         return
 
-    text = args[1]
-    model_name = args[2]
-    model_type = args[3]
+    corpus_id = args[1]
+    file_path = args[2]
+    document_id = args[3] if len(args) > 3 else None
+    metadata = {}
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        span = Span(text, customer_id, api_key)
-        span.load_model(model_name, model_type)
-        output_str, key_value_pairs = span.analyze_text(model_name)
-        print(output_str)
-        print(key_value_pairs)
+        response, status = vectara_client.upload_document(
+            corpus_id, file_path, document_id, metadata
+        )
+
+        if status:
+            print("Upload successful:", response)
+        else:
+            print("Upload failed:", response)
     except Exception as e:
-        print("Error processing text:", str(e))
+        print("Upload failed:", str(e))
 
 
 if __name__ == "__main__":
     import sys
 
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.6/vectara_cli/commands/upload_enriched_text.py` & `vectara-cli-0.1.7/vectara_cli/commands/upload_enriched_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ./commands/upload_enriched_text.py
 
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
 
 
-def main(args):
+def main(args, vectara_client):
     if len(args) < 6:
         print(
             "Usage: vectara-cli upload-enriched-text corpus_id document_id model_name text"
         )
         return
 
     corpus_id = args[1]
```

### Comparing `vectara-cli-0.1.6/vectara_cli/core.py` & `vectara-cli-0.1.7/vectara_cli/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import os
 import logging
 
 
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
+        self.customer_id = customer_id
+        self.api_key = api_key
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "customer-id": customer_id,
             "x-api-key": api_key,
         }
 
@@ -203,25 +205,37 @@
                     "success": False,
                     "error": f"HTTP Error {response.status_code}: {response.text}",
                 }
 
     def _get_index_request_json(
         self, corpus_id, document_id, title, metadata, section_text
     ):
-        # Assuming this method correctly formats the request payload for indexing a document.
-        # This is a placeholder implementation.
-        return json.dumps(
-            {
-                "corpusId": corpus_id,
-                "documentId": document_id,
-                "title": title,
-                "metadata": metadata,
-                "sectionText": section_text,
-            }
-        )
+        # Construct the document payload
+        document = {
+            "document_id": document_id,
+            "title": title,
+            "metadata_json": metadata,  # Pass the dictionary directly if the API expects an object
+            "section": [
+                {"text": section_text},
+            ],
+        }
+
+        # Construct the full request payload
+        request = {
+            "customer_id": self.customer_id,
+            "corpus_id": corpus_id,
+            "document": document,
+        }
+
+        # Convert the request payload to JSON and log it
+        json_payload = json.dumps(request)
+        print("Constructed JSON payload:", json_payload)  # Log the payload for debugging
+
+        return json_payload
+
 
     def index_document(self, corpus_id, document_id, title, metadata, section_text):
         """Indexes a document to the specified corpus using the Vectara platform.
 
         Args:
             corpus_id: ID of the corpus to which data needs to be indexed.
             document_id: Unique identifier for the document.
@@ -234,15 +248,15 @@
         """
         idx_address = f"{self.base_url}/v1/index"
         payload = self._get_index_request_json(
             corpus_id, document_id, title, metadata, section_text
         )
         try:
             response = requests.post(idx_address, data=payload, headers=self.headers)
-            response.raise_for_status()  # Raises HTTPError for bad responses
+            response.raise_for_status()
 
             message = response.json()
             if "status" in message and message["status"]["code"] in (
                 "OK",
                 "ALREADY_EXISTS",
             ):
                 logging.info("Document indexed successfully or already exists.")
```

### Comparing `vectara-cli-0.1.6/vectara_cli/main.py` & `vectara-cli-0.1.7/vectara_cli/main.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.6/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.7/vectara_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -344,15 +344,15 @@
 try:
     response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
     print("Upload successful:", response)
 except Exception as e:
     print("Upload failed:", str(e))
 ```
 
-### Advanced Useage
+### Advanced Usage
 
 
 To leverage the advanced text processing capabilities, ensure you have completed the advanced installation of `vectara-cli`. This includes the necessary dependencies for text analysis:
 
 ```bash
 pip install vectara-cli[advanced]
 ```
@@ -456,16 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](/res/images/Screenshot_2024-04-05_112158.png)
-![Span Models for Named Entity Recognition](/res/images/Screenshot_2024-04-05_112142.png)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,15 +517,15 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](<Screenshot 2024-04-05 112142.png>)
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.6/vectara_cli.egg-info/SOURCES.txt` & `vectara-cli-0.1.7/vectara_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

