# Comparing `tmp/vectara-cli-0.1.7.tar.gz` & `tmp/vectara-cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.7.tar", last modified: Sun Apr  7 07:32:49 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.8.tar", last modified: Sun Apr  7 10:21:46 2024, max compression
```

## Comparing `vectara-cli-0.1.7.tar` & `vectara-cli-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.167303 vectara-cli-0.1.7/
--rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/LICENSE.md
--rw-rw-rw-   0        0        0    22560 2024-04-07 07:32:49.165298 vectara-cli-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    21394 2024-04-06 21:55:14.000000 vectara-cli-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 07:32:49.167303 vectara-cli-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1428 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.128798 vectara-cli-0.1.7/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.7/vectara_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.137299 vectara-cli-0.1.7/vectara_cli/advanced/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/advanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.138799 vectara-cli-0.1.7/vectara_cli/advanced/commercial/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/advanced/commercial/__init__.py
--rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.7/vectara_cli/advanced/commercial/enterprise.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.143300 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/nerdspan.py
--rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/rebel.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.161298 vectara-cli-0.1.7/vectara_cli/commands/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.7/vectara_cli/commands/__init__.py
--rw-rw-rw-   0        0        0      860 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/create_corpus.py
--rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/delete_corpus.py
--rw-rw-rw-   0        0        0      957 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/index_document.py
--rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/nerdspan_upsert_folder.py
--rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/query.py
--rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/rebel_upsert_folder.py
--rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/commands/set_api_keys.py
--rw-rw-rw-   0        0        0      789 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span-text.py
--rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span_enhance_folder.py
--rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/span_text.py
--rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/upload_document.py
--rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/commands/upload_enriched_text.py
--rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/config_manager.py
--rw-rw-rw-   0        0        0    18548 2024-04-06 21:50:16.000000 vectara-cli-0.1.7/vectara_cli/core.py
--rw-rw-rw-   0        0        0     3072 2024-04-06 19:29:01.000000 vectara-cli-0.1.7/vectara_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 07:32:49.162798 vectara-cli-0.1.7/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    22560 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1099 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 07:32:49.000000 vectara-cli-0.1.7/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.853767 vectara-cli-0.1.8/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/LICENSE.md
+-rw-rw-rw-   0        0        0    22546 2024-04-07 10:21:46.852767 vectara-cli-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    21380 2024-04-07 08:11:24.000000 vectara-cli-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 10:21:46.854266 vectara-cli-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2024-04-07 10:21:35.000000 vectara-cli-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.815769 vectara-cli-0.1.8/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.8/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.822768 vectara-cli-0.1.8/vectara_cli/advanced/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/advanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.825268 vectara-cli-0.1.8/vectara_cli/advanced/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/advanced/commercial/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.8/vectara_cli/advanced/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.829266 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.848767 vectara-cli-0.1.8/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-07 10:07:18.000000 vectara-cli-0.1.8/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0      957 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.8/vectara_cli/commands/set_api_keys.py
+-rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/span_text.py
+-rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/config_manager.py
+-rw-rw-rw-   0        0        0    17356 2024-04-07 09:45:39.000000 vectara-cli-0.1.8/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     1550 2024-04-07 09:49:58.000000 vectara-cli-0.1.8/vectara_cli/corpus_data.py
+-rw-rw-rw-   0        0        0      500 2024-04-07 09:11:10.000000 vectara-cli-0.1.8/vectara_cli/custom_dimension.py
+-rw-rw-rw-   0        0        0      937 2024-04-07 09:41:11.000000 vectara-cli-0.1.8/vectara_cli/defaults.py
+-rw-rw-rw-   0        0        0      479 2024-04-07 09:10:54.000000 vectara-cli-0.1.8/vectara_cli/filter_attribute.py
+-rw-rw-rw-   0        0        0     3138 2024-04-07 10:18:19.000000 vectara-cli-0.1.8/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.850436 vectara-cli-0.1.8/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    22546 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.7/LICENSE.md` & `vectara-cli-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/PKG-INFO` & `vectara-cli-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -456,16 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,15 +517,16 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.7/README.md` & `vectara-cli-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -430,16 +430,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -491,15 +491,16 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.7/setup.py` & `vectara-cli-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.7",
+    version="0.1.8",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
```

### Comparing `vectara-cli-0.1.7/vectara_cli/advanced/commercial/enterprise.py` & `vectara-cli-0.1.8/vectara_cli/advanced/commercial/enterprise.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/nerdspan.py` & `vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/nerdspan.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/advanced/noncommercial/rebel.py` & `vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/rebel.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/create_corpus.py` & `vectara-cli-0.1.8/vectara_cli/commands/upload_document.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-# create_corpus.py
+# ./commands/upload_document.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
 def main(args, vectara_client):
-    if len(args) < 3:
-        print("Usage: vectara-cli create-corpus corpus_id name")
+    if len(args) < 4:
+        print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
         return
+
     corpus_id = args[1]
-    name = args[2]
+    file_path = args[2]
+    document_id = args[3] if len(args) > 3 else None
+    metadata = {}
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        response = vectara_client.create_corpus(
-            corpus_id,
-            name,
-            "Description",
-            1234567890,
-            True,
-            False,
-            False,
-            False,
-            False,
-            "default",
-            10000,
-            [],
-            [],
+        response, status = vectara_client.upload_document(
+            corpus_id, file_path, document_id, metadata
         )
-        print(response)
-    except ValueError as e:
-        print(e)
+
+        if status:
+            print("Upload successful:", response)
+        else:
+            print("Upload failed:", response)
+    except Exception as e:
+        print("Upload failed:", str(e))
 
 
 if __name__ == "__main__":
     import sys
 
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/delete_corpus.py` & `vectara-cli-0.1.8/vectara_cli/commands/delete_corpus.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/index_document.py` & `vectara-cli-0.1.8/vectara_cli/commands/index_document.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/nerdspan_upsert_folder.py` & `vectara-cli-0.1.8/vectara_cli/commands/nerdspan_upsert_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/query.py` & `vectara-cli-0.1.8/vectara_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/rebel_upsert_folder.py` & `vectara-cli-0.1.8/vectara_cli/commands/rebel_upsert_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/span-text.py` & `vectara-cli-0.1.8/vectara_cli/commands/span_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ./commands/span_text.py
 
-from vectara_cli.core import Span
+from vectara_cli.advanced.noncommercial.nerdspan import Span
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args, vectara_client):
     if len(args) < 5:
         print("Usage: vectara-cli process-text text model_name model_type")
         return
 
     text = args[1]
     model_name = args[2]
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

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/span_enhance_folder.py` & `vectara-cli-0.1.8/vectara_cli/commands/span_enhance_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/commands/upload_document.py` & `vectara-cli-0.1.8/vectara_cli/commands/upload_enriched_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-# ./commands/upload_document.py
+# ./commands/upload_enriched_text.py
 
-from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
+from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
 
 
 def main(args, vectara_client):
-    if len(args) < 4:
-        print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
+    if len(args) < 6:
+        print(
+            "Usage: vectara-cli upload-enriched-text corpus_id document_id model_name text"
+        )
         return
 
     corpus_id = args[1]
-    file_path = args[2]
-    document_id = args[3] if len(args) > 3 else None
-    metadata = {}
+    document_id = args[2]
+    model_name = args[3]
+    text = " ".join(args[4:])
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        response, status = vectara_client.upload_document(
-            corpus_id, file_path, document_id, metadata
-        )
-
-        if status:
-            print("Upload successful:", response)
-        else:
-            print("Upload failed:", response)
+        enterprise_span = EnterpriseSpan(model_name, customer_id, api_key)
+        predictions = enterprise_span.predict(text)
+        enterprise_span.upload_enriched_text(corpus_id, document_id, text, predictions)
+        print("Enriched text uploaded successfully.")
     except Exception as e:
-        print("Upload failed:", str(e))
+        print("Failed to upload enriched text:", str(e))
 
 
 if __name__ == "__main__":
     import sys
 
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.7/vectara_cli/config_manager.py` & `vectara-cli-0.1.8/vectara_cli/config_manager.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.7/vectara_cli/core.py` & `vectara-cli-0.1.8/vectara_cli/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ./vectara-cli/core.py
 
 import requests
 import json
 import os
 import logging
-
+from .corpus_data import CorpusData
+from .defaults import CorpusDefaults
 
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
         self.customer_id = customer_id
         self.api_key = api_key
         self.headers = {
@@ -142,73 +143,34 @@
             "customer_id": self.customer_id,
             "corpus_id": corpus_id,
             "document": document,
         }
 
         return json.dumps(request)
 
-    def create_corpus(
-        self,
-        corpus_id,
-        name,
-        description,
-        dtProvision,
-        enabled,
-        swapQenc,
-        swapIenc,
-        textless,
-        encrypted,
-        encoderId,
-        metadataMaxBytes,
-        customDimensions,
-        filterAttributes,
-    ):
+    def create_corpus(self, corpus_data: CorpusData):
         url = f"{self.base_url}/v1/create-corpus"
-        payload = {
-            "corpus": {
-                "id": corpus_id,
-                "name": name,
-                "description": description,
-                "dtProvision": dtProvision,
-                "enabled": enabled,
-                "swapQenc": swapQenc,
-                "swapIenc": swapIenc,
-                "textless": textless,
-                "encrypted": encrypted,
-                "encoderId": encoderId,
-                "metadataMaxBytes": metadataMaxBytes,
-                "customDimensions": customDimensions,
-                "filterAttributes": filterAttributes,
-            }
-        }
+        payload = {"corpus": {corpus_data.to_dict()}}
 
         response = requests.post(url, headers=self.headers, data=json.dumps(payload))
+        return self._parse_response(response)
 
+    def _parse_response(self, response):
         if response.status_code == 200:
-            # Assuming a successful response will have a JSON body
             try:
                 response_data = response.json()
-                # Check if the response contains the expected 'status' field with 'OK'
-                if response_data.get("status", {}).get("code") == "OK":
-                    return {"success": True, "data": response_data}
-                else:
-                    return {"success": False, "error": response_data.get("status", {})}
+                return {"success": True, "data": response_data}
             except ValueError:
-                # In case the response body does not contain valid JSON
                 return {"success": False, "error": "Invalid JSON in response"}
         else:
-            # Handle HTTP errors
             try:
                 error_data = response.json()
                 return {"success": False, "error": error_data}
             except ValueError:
-                return {
-                    "success": False,
-                    "error": f"HTTP Error {response.status_code}: {response.text}",
-                }
+                return {"success": False, "error": f"HTTP Error {response.status_code}: {response.text}"}
 
     def _get_index_request_json(
         self, corpus_id, document_id, title, metadata, section_text
     ):
         # Construct the document payload
         document = {
             "document_id": document_id,
```

### Comparing `vectara-cli-0.1.7/vectara_cli/main.py` & `vectara-cli-0.1.8/vectara_cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # vectara_cli/main.py
+from .defaults import CorpusDefaults
 
 import sys
 from vectara_cli.commands import (
     nerdspan_upsert_folder,
     set_api_keys,
     index_document,
     query,
@@ -47,20 +48,21 @@
 
     Use 'vectara-cli help' to display this help message.
     """
     print(help_text)
 
 
 def main():
-    args = sys.argv[1:]
-    if not args or args[0] in ("help", "--help", "-h"):
+    
+    if len(sys.argv) < 2 or sys.argv[1] in ("help", "--help", "-h"):
         print_help()
         return
-
-    command = args[0]
+    
+    command = sys.argv[1]
+    args = sys.argv[2:] 
 
     if command == "set-api-keys":
         set_api_keys.main(args)
     else:
         vectara_client = get_vectara_client()
 
         if command == "index-document":
```

### Comparing `vectara-cli-0.1.7/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.8/vectara_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
@@ -456,16 +456,16 @@
 
 This example showcases how to enrich text with additional metadata using the `EnterpriseSpan` class and upload it to a specified corpus in Vectara. By leveraging advanced models for text processing, users can significantly enhance the quality and relevance of their search and retrieval operations on the Vectara platform.
 
 ### Non-Commercial Advanced Usage
 
 The advanced features allow you to enrich your indexes with additional information automatically. This should produce better results for retrieval.
 
-![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
-![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
+
+![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/res/images/image.png?ref_type=heads)
 
 ### Non-Commercial Advanced Usage Using Span Models
 
 The `vectara-cli` package extends its functionality through the advanced usage of Span Models, enabling users to perform sophisticated text analysis and entity recognition tasks. This feature is particularly beneficial for non-commercial applications that require deep understanding and processing of textual data.
 
 The `Span` class supports processing and indexing documents from a folder, enabling batch operations for efficiency. This feature allows for the automatic extraction of entities from multiple documents, which are then indexed into specified corpora with enriched metadata.
 
@@ -517,15 +517,16 @@
     vectara_client.index_text(corpus_id, document_id, text, metadata_json=metadata_json)
     ```
 
 **Reference:** Aarsen, T. (2023). SpanMarker for Named Entity Recognition. Radboud University. Supervised by Prof. Dr. Fermin Moscoso del Prado Martin (fermin.moscoso-del-prado@ru.nl) and Dr. Daniel Vila Suero (daniel@argilla.io). Second assessor: Dr. Harrie Oosterhuis (harrie.oosterhuis@ru.nl).
 
 #### Non-Commercial Advanced Rag Using Rebel
 
-![The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/image.png?ref_type=heads)
+![mRebel](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112158.png?ref_type=heads)
+![Span Models for Named Entity Recognition](https://git.tonic-ai.com/releases/vectara-cli/-/raw/devbranch/res/images/Screenshot_2024-04-05_112142.png?ref_type=heads)
 
 The mRebel pre-trained model is able to extract triplets for up to 400 relation types from Wikidata.
 
 
 Use the use the `Rebel Class` for advanced indexing. This will automatically extract `named entities`, `key phrases`, and other relevant information from your documents :
```

### Comparing `vectara-cli-0.1.7/vectara_cli.egg-info/SOURCES.txt` & `vectara-cli-0.1.8/vectara_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 LICENSE.md
 README.md
 setup.py
 vectara_cli/__init__.py
 vectara_cli/config_manager.py
 vectara_cli/core.py
+vectara_cli/corpus_data.py
+vectara_cli/custom_dimension.py
+vectara_cli/defaults.py
+vectara_cli/filter_attribute.py
 vectara_cli/main.py
 vectara_cli.egg-info/PKG-INFO
 vectara_cli.egg-info/SOURCES.txt
 vectara_cli.egg-info/dependency_links.txt
 vectara_cli.egg-info/entry_points.txt
 vectara_cli.egg-info/requires.txt
 vectara_cli.egg-info/top_level.txt
@@ -21,12 +25,11 @@
 vectara_cli/commands/create_corpus.py
 vectara_cli/commands/delete_corpus.py
 vectara_cli/commands/index_document.py
 vectara_cli/commands/nerdspan_upsert_folder.py
 vectara_cli/commands/query.py
 vectara_cli/commands/rebel_upsert_folder.py
 vectara_cli/commands/set_api_keys.py
-vectara_cli/commands/span-text.py
 vectara_cli/commands/span_enhance_folder.py
 vectara_cli/commands/span_text.py
 vectara_cli/commands/upload_document.py
 vectara_cli/commands/upload_enriched_text.py
```

