# Comparing `tmp/vectara-cli-0.1.5.tar.gz` & `tmp/vectara-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.5.tar", last modified: Sat Apr  6 18:14:29 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.6.tar", last modified: Sat Apr  6 19:32:15 2024, max compression
```

## Comparing `vectara-cli-0.1.5.tar` & `vectara-cli-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.890507 vectara-cli-0.1.5/
--rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/LICENSE.md
--rw-rw-rw-   0        0        0    22346 2024-04-06 18:14:29.888025 vectara-cli-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    21180 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 18:14:29.891015 vectara-cli-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1427 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.834889 vectara-cli-0.1.5/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.5/vectara_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.849896 vectara-cli-0.1.5/vectara_cli/advanced/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.852395 vectara-cli-0.1.5/vectara_cli/advanced/commercial/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/commercial/__init__.py
--rw-rw-rw-   0        0        0     7379 2024-04-06 14:04:07.000000 vectara-cli-0.1.5/vectara_cli/advanced/commercial/enterprise.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.857987 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/__init__.py
--rw-rw-rw-   0        0        0     6061 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/nerdspan.py
--rw-rw-rw-   0        0        0     8476 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/rebel.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.883015 vectara-cli-0.1.5/vectara_cli/commands/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/__init__.py
--rw-rw-rw-   0        0        0      719 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/create_corpus.py
--rw-rw-rw-   0        0        0      752 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/delete_corpus.py
--rw-rw-rw-   0        0        0     1027 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/index_document.py
--rw-rw-rw-   0        0        0     1034 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/nerdspan_upsert_folder.py
--rw-rw-rw-   0        0        0      683 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/query.py
--rw-rw-rw-   0        0        0     1055 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/rebel_upsert_folder.py
--rw-rw-rw-   0        0        0      419 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/set_api_keys.py
--rw-rw-rw-   0        0        0      773 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/span-text.py
--rw-rw-rw-   0        0        0     1119 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/span_enhance_folder.py
--rw-rw-rw-   0        0        0      983 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/upload_document.py
--rw-rw-rw-   0        0        0      932 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/commands/upload_enriched_text.py
--rw-rw-rw-   0        0        0      719 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/config_manager.py
--rw-rw-rw-   0        0        0    17117 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/core.py
--rw-rw-rw-   0        0        0     2933 2024-04-06 18:07:05.000000 vectara-cli-0.1.5/vectara_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:14:29.885505 vectara-cli-0.1.5/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    22346 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1065 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-06 18:14:29.000000 vectara-cli-0.1.5/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.696351 vectara-cli-0.1.6/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0    22346 2024-04-06 19:32:15.692781 vectara-cli-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    21180 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:32:15.697354 vectara-cli-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.535153 vectara-cli-0.1.6/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.6/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.577930 vectara-cli-0.1.6/vectara_cli/advanced/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/advanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.588693 vectara-cli-0.1.6/vectara_cli/advanced/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/advanced/commercial/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.607301 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     9784 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.681456 vectara-cli-0.1.6/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0      906 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      750 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0     1081 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0     1115 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      689 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1391 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/set_api_keys.py
+-rw-rw-rw-   0        0        0      773 2024-04-06 18:07:05.000000 vectara-cli-0.1.6/vectara_cli/commands/span-text.py
+-rw-rw-rw-   0        0        0     1173 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0      806 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/span_text.py
+-rw-rw-rw-   0        0        0     1005 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      962 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0      753 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/config_manager.py
+-rw-rw-rw-   0        0        0    18174 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     3072 2024-04-06 19:29:01.000000 vectara-cli-0.1.6/vectara_cli/main.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:32:15.686720 vectara-cli-0.1.6/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    22346 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1099 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-06 19:32:15.000000 vectara-cli-0.1.6/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.5/LICENSE.md` & `vectara-cli-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.5/PKG-INFO` & `vectara-cli-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vectara-cli-0.1.5/README.md` & `vectara-cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.5/setup.py` & `vectara-cli-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
- # ./setup.py
+# ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.5",
+    version="0.1.6",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
-    long_description=open('README.md').read(),
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     extras_require={
@@ -21,23 +21,23 @@
             "torch>=1.8.0",
             "transformers>=4.5.0",
             "span_marker",
             "spacy",
         ],
     },
     entry_points={
-        'console_scripts': [
-            'vectara=vectara_cli.main:main',
+        "console_scripts": [
+            "vectara=vectara_cli.main:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
-    python_requires='>=3.9',
+    python_requires=">=3.9",
     license="MIT",
     keywords="vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing",
-)
+)
```

### Comparing `vectara-cli-0.1.5/vectara_cli/advanced/commercial/enterprise.py` & `vectara-cli-0.1.6/vectara_cli/advanced/commercial/enterprise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # ./advanced/commercial/enterpise.py
 
 import logging
 from typing import List, Any, Dict
-from core import VectaraClient
-import span_marker from span_marker import SpanMarkerModel
+from vectara_cli.core import VectaraClient
+import span_marker
+from span_marker import SpanMarkerModel
 import random
 import string
 
+
 class EnterpriseSpan:
     """
     EnterpriseSpan class for handling advanced text processing and analysis in enterprise applications.
     This class wraps around the SpanMarkerModel for keyphrase extraction and adds enterprise-level features
     such as detailed logging, error handling, and customization options, including an easy way to specify models.
     """
+
     MODEL_MAP = {
         "keyphrase": "tomaarsen/span-marker-bert-base-uncased-keyphrase-inspec",
         "science": "tomaarsen/span-marker-bert-base-ncbi-disease",
     }
 
     def __init__(self, model_name: str):
         """
@@ -37,15 +40,17 @@
 
         Returns:
             str: The model identifier.
         """
         if self.model_name in self.MODEL_MAP:
             return self.MODEL_MAP[self.model_name]
         else:
-            self.logger.warning(f"Model name {self.model_name} not recognized. Attempting to use it as a direct path or identifier.")
+            self.logger.warning(
+                f"Model name {self.model_name} not recognized. Attempting to use it as a direct path or identifier."
+            )
             return self.model_name
 
     def _load_model(self) -> SpanMarkerModel:
         """
         Loads the SpanMarkerModel from the specified path.
 
         Returns:
@@ -55,15 +60,14 @@
             model = SpanMarkerModel.from_pretrained(self.model_path)
             self.logger.info(f"Model loaded successfully from {self.model_path}")
             return model
         except Exception as e:
             self.logger.error(f"Failed to load model from {self.model_path}: {e}")
             raise
 
-
     def predict(self, text: str) -> List[Dict[str, Any]]:
         """
         Runs inference on the given text and returns the extracted entities.
 
         Parameters:
             text (str): The input text for which to predict entities.
 
@@ -71,65 +75,73 @@
             List[Dict[str, Any]]: A list of entities with their respective information.
         """
         try:
             entities = self.model.predict(text)
             self.logger.info(f"Prediction successful for input text: {text[:30]}...")
             return entities
         except Exception as e:
-            self.logger.error(f"Prediction failed for input text: {text[:30]}... Error: {e}")
+            self.logger.error(
+                f"Prediction failed for input text: {text[:30]}... Error: {e}"
+            )
             raise
 
     def format_predictions(self, predictions: List[Dict[str, Any]]) -> str:
         """
         Formats the predictions into a structured string that can be easily read and used.
 
         Parameters:
             predictions (List[Dict[str, Any]]): The list of entities predicted by the model.
 
         Returns:
             str: A formatted string of predictions.
         """
         formatted = ""
         for pred in predictions:
-            formatted += f"{pred['entity_group']}: {pred['word']} (Score: {pred['score']:.2f})\n"
+            formatted += (
+                f"{pred['entity_group']}: {pred['word']} (Score: {pred['score']:.2f})\n"
+            )
         return formatted.strip()
 
     def format_predictions(self, predictions: List[Dict[str, Any]]) -> str:
         formatted = ""
         for pred in predictions:
-            formatted += f"{pred['entity_group']}: {pred['word']} (Score: {pred['score']:.2f})\n"
+            formatted += (
+                f"{pred['entity_group']}: {pred['word']} (Score: {pred['score']:.2f})\n"
+            )
         return formatted.strip()
 
     def generate_metadata(self, predictions: List[Dict[str, Any]]) -> Dict[str, Any]:
         metadata = {}
         for pred in predictions:
-            key = pred['entity_group']
+            key = pred["entity_group"]
             if key not in metadata:
                 metadata[key] = []
-            metadata[key].append(pred['word'])
+            metadata[key].append(pred["word"])
         return metadata
 
     def text_chunk(self, text, chunk_size=512):
         """
         Breaks down text into smaller chunks of a specified size.
 
         Parameters:
             text (str): The text to be chunked.
             chunk_size (int): The maximum size of each text chunk.
 
         Returns:
             List[str]: A list of text chunks.
         """
-        return [text[i:i+chunk_size] for i in range(0, len(text), chunk_size)]
+        return [text[i : i + chunk_size] for i in range(0, len(text), chunk_size)]
 
     def upload_enriched_text(self, corpus_id, document_id, text, predictions):
         metadata = self.generate_metadata(predictions)
         enriched_text = self.format_predictions(predictions) + "\n\n" + text
         try:
-            response, success = self.vectara_client.index_document(corpus_id, document_id, "Enriched Text", metadata, enriched_text)
+            response, success = self.vectara_client.index_document(
+                corpus_id, document_id, "Enriched Text", metadata, enriched_text
+            )
             if success:
                 self.logger.info("Enriched document uploaded successfully.")
             else:
                 self.logger.error("Failed to upload enriched document.")
         except Exception as e:
             self.logger.error(f"An error occurred while uploading the document: {e}")
 
@@ -139,30 +151,40 @@
 
         Args:
             corpus_id_1 (int): ID for the first corpus (plain text).
             corpus_id_2 (int): ID for the second corpus (enhanced text).
             folder_path (str): Path to the folder containing documents.
         """
         # Create two new corpora
-        corpus_id_1 = ''.join(random.choices(string.ascii_letters + string.digits, k=7))
-        corpus_id_2 = ''.join(random.choices(string.ascii_letters + string.digits, k=7))
-        self.vectara_client.create_corpus(corpus_id=corpus_id_1, name=f"{corpus_id_1}_Plain", description="Plain Document Index")
-        self.vectara_client.create_corpus(corpus_id=corpus_id_2, name=f"{corpus_id_2}_Enhanced", description="Enhanced Document Index")
-
-        results = self.vectara_client.index_documents_from_folder(corpus_id_1, folder_path, return_extracted_document=True)
+        corpus_id_1 = "".join(random.choices(string.ascii_letters + string.digits, k=7))
+        corpus_id_2 = "".join(random.choices(string.ascii_letters + string.digits, k=7))
+        self.vectara_client.create_corpus(
+            corpus_id=corpus_id_1,
+            name=f"{corpus_id_1}_Plain",
+            description="Plain Document Index",
+        )
+        self.vectara_client.create_corpus(
+            corpus_id=corpus_id_2,
+            name=f"{corpus_id_2}_Enhanced",
+            description="Enhanced Document Index",
+        )
+
+        results = self.vectara_client.index_documents_from_folder(
+            corpus_id_1, folder_path, return_extracted_document=True
+        )
 
         for document_id, success, extracted_text in results:
             if not success or not extracted_text:
                 continue
             text_chunks = self.text_chunk(extracted_text)
 
             for chunk in text_chunks:
                 predictions = self.predict(chunk)
                 self.upload_enriched_text(corpus_id_2, document_id, chunk, predictions)
-                
+
 
 # # Example usage
 # if __name__ == "__main__":
 #     logging.basicConfig(level=logging.INFO)
 #     enterprise_model = EnterpriseSpan("keyphrase")
 #     text = "Example text for processing."
 #     try:
```

### Comparing `vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/nerdspan.py` & `vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/nerdspan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # ./vectara-cli/advanced/nerdspan.py
 
 import spacy
 import span_marker
 from span_marker import SpanMarkerModel
 from vectara_cli.core import VectaraClient
 
+
 class Span:
     def __init__(self, text, customer_id, api_key):
         super().__init__(text)
         self.vectara_client = VectaraClient(customer_id, api_key)
         self.model_mapping = {
             "fewnerdsuperfine": "tomaarsen/span-marker-bert-base-fewnerd-fine-super",
             "multinerd": "tomaarsen/span-marker-mbert-base-multinerd",
-            "largeontonote": "tomaarsen/span-marker-roberta-large-ontonotes5"
+            "largeontonote": "tomaarsen/span-marker-roberta-large-ontonotes5",
         }
 
     def load_model(self, model_name, model_type):
         """
         Load a model given its name and type.
         """
         # Resolve the model name to its full identifier
@@ -34,15 +35,15 @@
 
     def run_inference(self, model_name):
         """
         Run inference using a specified model.
         """
         if model_name not in self.models:
             raise ValueError("Model not loaded")
-        
+
         model = self.models[model_name]
         if isinstance(model, SpanMarkerModel):
             return model.predict(self.text)
         elif isinstance(model, spacy.language.Language):
             doc = model(self.text)
             return [(entity.text, entity.label_) for entity in doc.ents]
         else:
@@ -57,15 +58,17 @@
         for entity in entities:
             if isinstance(entity, tuple):
                 # spaCy output
                 output_str += f"{entity[0]}: {entity[1]}\n"
                 key_value_pairs.append({"span": entity[0], "label": entity[1]})
             else:
                 # SpanMarkerModel output
-                output_str += f"{entity['span']}: {entity['label']}, Score: {entity['score']}\n"
+                output_str += (
+                    f"{entity['span']}: {entity['label']}, Score: {entity['score']}\n"
+                )
                 key_value_pairs.append(entity)
         return output_str, key_value_pairs
 
     def analyze_text(self, model_name):
         """
         Analyze the text with a given model and return formatted outputs.
         """
@@ -83,60 +86,68 @@
             swapQenc=False,
             swapIenc=False,
             textless=False,
             encrypted=False,
             encoderId="default",
             metadataMaxBytes=10000,
             customDimensions=[],
-            filterAttributes=[]
+            filterAttributes=[],
         )
         print(f"Corpus creation response: {response}")
         return corpus_id
 
     def text_chunker(self, text, chunk_size=512):
-        return [text[i:i+chunk_size] for i in range(0, len(text), chunk_size)]
+        return [text[i : i + chunk_size] for i in range(0, len(text), chunk_size)]
 
     def process_and_upload(self, folder_path, model_name, model_type):
         # Create two corpora
         corpus_id_1 = self.create_corpus("Corpus 1", "First corpus for raw uploads")
-        corpus_id_2 = self.create_corpus("Corpus 2", "Second corpus for processed uploads")
+        corpus_id_2 = self.create_corpus(
+            "Corpus 2", "Second corpus for processed uploads"
+        )
 
         # Upload documents from folder to the first corpus
-        upload_results = self.vectara_client.index_documents_from_folder(corpus_id_1, folder_path, return_extracted_document=True)
+        upload_results = self.vectara_client.index_documents_from_folder(
+            corpus_id_1, folder_path, return_extracted_document=True
+        )
 
         for document_id, success, extracted_text in upload_results:
             if not success or extracted_text is None:
-                print(f"Skipping document {document_id}, upload failed or no text extracted.")
+                print(
+                    f"Skipping document {document_id}, upload failed or no text extracted."
+                )
                 continue
 
             # Chunk the text
             chunks = self.text_chunker(extracted_text)
 
             # Process each chunk and re-upload to the second corpus
             self.load_model(model_name, model_type)
             for chunk in chunks:
                 self.text = chunk  # Update the Span text to the current chunk
                 _, key_value_pairs = self.analyze_text(model_name)
                 # Convert key-value pairs to a metadata JSON string
                 metadata_json = json.dumps({"entities": key_value_pairs})
                 # Index processed chunk into the second corpus
-                self.vectara_client.index_text(corpus_id_2, document_id, chunk, metadata_json=metadata_json)
+                self.vectara_client.index_text(
+                    corpus_id_2, document_id, chunk, metadata_json=metadata_json
+                )
 
         return corpus_id_1, corpus_id_2
 
 
 # # Example usage
 # if __name__ == "__main__":
 #     text = "Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris."
 #     span = Span(text)
-    
+
 #     # Load and run SpanMarkerModel
 #     span.load_model("tomaarsen/span-marker-mbert-base-multinerd", "span_marker")
 #     output_str, key_value_pairs = span.analyze_text("tomaarsen/span-marker-mbert-base-multinerd")
 #     print(output_str)
 #     print(key_value_pairs)
-    
+
 #     # Load and run spaCy model with span_marker pipeline
 #     span.load_model("tomaarsen/span-marker-roberta-large-ontonotes5", "spacy")
 #     output_str, key_value_pairs = span.analyze_text("tomaarsen/span-marker-roberta-large-ontonotes5")
 #     print(output_str)
 #     print(key_value_pairs)
```

### Comparing `vectara-cli-0.1.5/vectara_cli/advanced/noncommercial/rebel.py` & `vectara-cli-0.1.6/vectara_cli/advanced/noncommercial/rebel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,71 @@
 # vectara-cli\advanced\non-commercial\rebel.py
 
 import torch
 from torch.nn import CrossEntropyLoss, BCEWithLogitsLoss
 from transformers import DebertaV2Config, DebertaV2PreTrainedModel, DebertaV2Model
-from transformers.models.deberta_v2.modeling_deberta_v2 import ContextPooler, StableDropout
+from transformers.models.deberta_v2.modeling_deberta_v2 import (
+    ContextPooler,
+    StableDropout,
+)
 from transformers.file_utils import ModelOutput
 from transformers import pipeline
 from dataclasses import dataclass
 from typing import Optional, Tuple
 from vectara_cli.core import VectaraClient
 
+
 @dataclass
 class TXNLIClassifierOutput(ModelOutput):
     loss: Optional[torch.FloatTensor] = None
     logits: torch.FloatTensor = None
     logits_xnli: torch.FloatTensor = None
     hidden_states: Optional[Tuple[torch.FloatTensor]] = None
     attentions: Optional[Tuple[torch.FloatTensor]] = None
 
+
 class DebertaV2ForTripletClassification(DebertaV2PreTrainedModel):
     def __init__(self, config):
         super().__init__(config)
         self.num_labels = getattr(config, "num_labels", 2)
         self.deberta = DebertaV2Model(config)
         self.pooler = ContextPooler(config)
         self.classifier = nn.Linear(self.pooler.output_dim, self.num_labels)
         drop_out = getattr(config, "cls_dropout", None)
-        self.dropout = StableDropout(drop_out if drop_out is not None else config.hidden_dropout_prob)
+        self.dropout = StableDropout(
+            drop_out if drop_out is not None else config.hidden_dropout_prob
+        )
         self.classifier_xnli = nn.Linear(self.pooler.output_dim, 3)
         self.post_init()
 
-    def forward(self, input_ids=None, attention_mask=None, token_type_ids=None, position_ids=None, inputs_embeds=None, labels=None, output_attentions=None, output_hidden_states=None, return_dict=None):
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-        outputs = self.deberta(input_ids, token_type_ids=token_type_ids, attention_mask=attention_mask, position_ids=position_ids, inputs_embeds=inputs_embeds, output_attentions=output_attentions, output_hidden_states=output_hidden_states, return_dict=return_dict)
+    def forward(
+        self,
+        input_ids=None,
+        attention_mask=None,
+        token_type_ids=None,
+        position_ids=None,
+        inputs_embeds=None,
+        labels=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+    ):
+        return_dict = (
+            return_dict if return_dict is not None else self.config.use_return_dict
+        )
+        outputs = self.deberta(
+            input_ids,
+            token_type_ids=token_type_ids,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
         encoder_layer = outputs[0]
         pooled_output = self.pooler(encoder_layer)
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
         logits_xnli = self.classifier_xnli(pooled_output)
         loss = None
         if labels is not None:
@@ -45,55 +74,94 @@
                 loss = loss_fct(logits.view(-1, self.num_labels), labels.view(-1))
             else:
                 loss_fct = BCEWithLogitsLoss()
                 loss = loss_fct(logits_xnli.view(-1, 3), labels.view(-1).long())
         if not return_dict:
             output = (logits,) + outputs[2:]
             return ((loss,) + output) if loss is not None else output
-        return TXNLIClassifierOutput(loss=loss, logits=logits, logits_xnli=logits_xnli, hidden_states=outputs.hidden_states, attentions=outputs.attentions)
+        return TXNLIClassifierOutput(
+            loss=loss,
+            logits=logits,
+            logits_xnli=logits_xnli,
+            hidden_states=outputs.hidden_states,
+            attentions=outputs.attentions,
+        )
+
 
 class Rebel:
-    def __init__(self, model_path='microsoft/deberta-v2-xlarge'):
+    def __init__(self, model_path="microsoft/deberta-v2-xlarge"):
         self.config = DebertaV2Config.from_pretrained(model_path)
         self.model = DebertaV2ForTripletClassification(self.config)
-        self.triplet_extractor = pipeline('text2text-generation', model='Babelscape/rebel-large', tokenizer='Babelscape/rebel-large')
+        self.triplet_extractor = pipeline(
+            "text2text-generation",
+            model="Babelscape/rebel-large",
+            tokenizer="Babelscape/rebel-large",
+        )
 
     def extract_triplets(self, text):
         triplets = []
-        relation, subject, relation, object_ = '', '', '', ''
+        relation, subject, relation, object_ = "", "", "", ""
         text = text.strip()
-        current = 'x'
-        for token in text.replace("<s>", "").replace("<pad>", "").replace("</s>", "").split():
+        current = "x"
+        for token in (
+            text.replace("<s>", "").replace("<pad>", "").replace("</s>", "").split()
+        ):
             if token == "<triplet>":
-                current = 't'
-                if relation != '':
-                    triplets.append({'head': subject.strip(), 'type': relation.strip(),'tail': object_.strip()})
-                    relation = ''
-                subject = ''
+                current = "t"
+                if relation != "":
+                    triplets.append(
+                        {
+                            "head": subject.strip(),
+                            "type": relation.strip(),
+                            "tail": object_.strip(),
+                        }
+                    )
+                    relation = ""
+                subject = ""
             elif token == "<subj>":
-                current = 's'
-                if relation != '':
-                    triplets.append({'head': subject.strip(), 'type': relation.strip(),'tail': object_.strip()})
-                object_ = ''
+                current = "s"
+                if relation != "":
+                    triplets.append(
+                        {
+                            "head": subject.strip(),
+                            "type": relation.strip(),
+                            "tail": object_.strip(),
+                        }
+                    )
+                object_ = ""
             elif token == "<obj>":
-                current = 'o'
-                relation = ''
+                current = "o"
+                relation = ""
             else:
-                if current == 't':
-                    subject += ' ' + token
-                elif current == 's':
-                    object_ += ' ' + token
-                elif current == 'o':
-                    relation += ' ' + token
-        if subject != '' and relation != '' and object_ != '':
-            triplets.append({'head': subject.strip(), 'type': relation.strip(),'tail': object_.strip()})
+                if current == "t":
+                    subject += " " + token
+                elif current == "s":
+                    object_ += " " + token
+                elif current == "o":
+                    relation += " " + token
+        if subject != "" and relation != "" and object_ != "":
+            triplets.append(
+                {
+                    "head": subject.strip(),
+                    "type": relation.strip(),
+                    "tail": object_.strip(),
+                }
+            )
         return triplets
-      
+
     def extract_text(self, text):
-        extracted_text = self.triplet_extractor.tokenizer.batch_decode([self.triplet_extractor(text, return_tensors=True, return_text=True)[0]["generated_token_ids"]])[0] # return text true so the text chunk is directly useable.
+        extracted_text = self.triplet_extractor.tokenizer.batch_decode(
+            [
+                self.triplet_extractor(text, return_tensors=True, return_text=True)[0][
+                    "generated_token_ids"
+                ]
+            ]
+        )[
+            0
+        ]  # return text true so the text chunk is directly useable.
         return extracted_text
 
     def forward_pass(self, **kwargs):
         # Perform forward pass with the model
         return self.model(**kwargs)
 
     def chunk_text(self, text, chunk_size=512):
@@ -103,15 +171,15 @@
         Args:
             text (str): The text to be chunked.
             chunk_size (int): The desired size of each text chunk.
 
         Returns:
             list: A list of text chunks.
         """
-        return [text[i:i+chunk_size] for i in range(0, len(text), chunk_size)]
+        return [text[i : i + chunk_size] for i in range(0, len(text), chunk_size)]
 
     def extract_keywords(self, model_output):
         """
         Extracts keywords or metadata from the model's output. Placeholder implementation.
 
         Args:
             model_output: The output from the model's forward pass.
@@ -120,49 +188,70 @@
             dict: A dictionary representing the extracted metadata.
         """
         keywords = []
         for triplet in self.extract_triplets(model_output):
             keywords.append(f"{triplet['head']}:{triplet['type']}:{triplet['tail']}")
         return {"keywords": keywords}
 
-    def advanced_upsert_folder(self, vectara_client: VectaraClient, corpus_id_1, corpus_id_2, folder_path):
+    def advanced_upsert_folder(
+        self, vectara_client: VectaraClient, corpus_id_1, corpus_id_2, folder_path
+    ):
         """
         Handles the creation of two corpora, indexing documents, and uploading text chunks with metadata.
 
         Args:
             vectara_client (VectaraClient): An instance of the VectaraClient to interact with the Vectara API.
             corpus_id_1 (int): The ID of the first corpus.
             corpus_id_2 (int): The ID of the second corpus.
             folder_path (str): The path to the folder containing documents to be indexed.
         """
         # Step 1: Create two corpora
-        corpus_id_1 = ''.join(random.choices(string.ascii_letters + string.digits, k=7))
-        corpus_id_2 = ''.join(random.choices(string.ascii_letters + string.digits, k=7))
-        vectara_client.create_corpus(corpus_id=corpus_id_1, name="{corpus_id_1}_Plain", description="Plain Document Index for ")
-        vectara_client.create_corpus(corpus_id=corpus_id_2, name="{corpus_id_2}_Advanced", description="Second corpus")
+        corpus_id_1 = "".join(random.choices(string.ascii_letters + string.digits, k=7))
+        corpus_id_2 = "".join(random.choices(string.ascii_letters + string.digits, k=7))
+        vectara_client.create_corpus(
+            corpus_id=corpus_id_1,
+            name="{corpus_id_1}_Plain",
+            description="Plain Document Index for ",
+        )
+        vectara_client.create_corpus(
+            corpus_id=corpus_id_2,
+            name="{corpus_id_2}_Advanced",
+            description="Second corpus",
+        )
 
         # Step 2: Index documents from folder into the first corpus and get plain text
-        results = vectara_client.index_documents_from_folder(corpus_id_1, folder_path, return_extracted_document=True)
+        results = vectara_client.index_documents_from_folder(
+            corpus_id_1, folder_path, return_extracted_document=True
+        )
 
         for document_id, success, extracted_text in results:
             if not success or not extracted_text:
-                print(f"Skipping document {document_id} due to failure in extraction or indexing.")
+                print(
+                    f"Skipping document {document_id} due to failure in extraction or indexing."
+                )
                 continue
 
             # Step 3: Chunk plain text into sized text chunks (assuming a function to do this)
             text_chunks = self.chunk_text(extracted_text)
 
             for chunk in text_chunks:
                 output = self.forward_pass(text=chunk)
                 metadata = self.extract_keywords(output)
 
-                vectara_client.index_document(corpus_id_2, document_id, title="Chunk Title", metadata=metadata, section_text=chunk)
+                vectara_client.index_document(
+                    corpus_id_2,
+                    document_id,
+                    title="Chunk Title",
+                    metadata=metadata,
+                    section_text=chunk,
+                )
 
         return corpus_id_1, corpus_id_2
-    
+
+
 # # Example usage
 # advanced = Advanced()
 # # For triplet extraction
 # triplets = advanced.extract_triplets("Punta Cana is a resort town in the municipality of Higuey, in La Altagracia Province, the eastern most province of the Dominican Republic")
 # print(triplets)
 # # For classification/forward pass (fill in the actual arguments)
 # # output = advanced.forward_pass(input_ids=input_ids, attention_mask=attention_mask, labels=labels)
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/create_corpus.py` & `vectara-cli-0.1.6/vectara_cli/commands/create_corpus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 # create_corpus.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 3:
         print("Usage: vectara-cli create-corpus corpus_id name")
         return
     corpus_id = args[1]
     name = args[2]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
-        response = vectara_client.create_corpus(corpus_id, name, "Description", 1234567890, True, False, False, False, False, "default", 10000, [], [])
+        response = vectara_client.create_corpus(
+            corpus_id,
+            name,
+            "Description",
+            1234567890,
+            True,
+            False,
+            False,
+            False,
+            False,
+            "default",
+            10000,
+            [],
+            [],
+        )
         print(response)
     except ValueError as e:
         print(e)
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/delete_corpus.py` & `vectara-cli-0.1.6/vectara_cli/commands/delete_corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # ./commands/delete_corpus.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 2:
         print("Usage: vectara-cli delete-corpus corpus_id")
         return
 
     corpus_id = args[1]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
         response, success = vectara_client.delete_corpus(corpus_id)
-        
+
         if success:
             print("Corpus deleted successfully.")
         else:
             print("Failed to delete corpus:", response)
     except ValueError as e:
         print(e)
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/index_document.py` & `vectara-cli-0.1.6/vectara_cli/commands/index_document.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # index_document.py
 
 import json
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 6:
-        print("Usage: vectara-cli index-document corpus_id document_id title metadata_json section_text")
+        print(
+            "Usage: vectara-cli index-document corpus_id document_id title metadata_json section_text"
+        )
         return
     corpus_id = args[1]
     document_id = args[2]
     title = args[3]
     metadata = json.loads(args[4])
     section_text = args[5]
 
     # Assuming ConfigManager and VectaraClient are set up to handle API keys
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
-        response, success = vectara_client.index_document(corpus_id, document_id, title, metadata, section_text)
+        response, success = vectara_client.index_document(
+            corpus_id, document_id, title, metadata, section_text
+        )
         if success:
             print("Document indexed successfully.")
         else:
             print("Document indexing failed.", response)
     except ValueError as e:
         print(e)
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/nerdspan_upsert_folder.py` & `vectara-cli-0.1.6/vectara_cli/commands/nerdspan_upsert_folder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # ./commands/nerdspan_upsert_folder.py
 
 import os
-from vectara_cli.core import Span
+from vectara_cli.advanced.noncommercial.nerdspan import Span
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 5:
         print("Usage: vectara-cli process-and-upload folder_path model_name model_type")
         return
 
     folder_path = args[1]
     model_name = args[2]
@@ -16,15 +17,21 @@
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         if not os.path.isdir(folder_path):
             print(f"The specified folder path does not exist: {folder_path}")
             return
 
         span = Span("", customer_id, api_key)
-        corpus_id_1, corpus_id_2 = span.process_and_upload(folder_path, model_name, model_type)
-        print(f"Documents processed and uploaded. Raw uploads in Corpus ID: {corpus_id_1}, Processed uploads in Corpus ID: {corpus_id_2}")
+        corpus_id_1, corpus_id_2 = span.process_and_upload(
+            folder_path, model_name, model_type
+        )
+        print(
+            f"Documents processed and uploaded. Raw uploads in Corpus ID: {corpus_id_1}, Processed uploads in Corpus ID: {corpus_id_2}"
+        )
     except Exception as e:
         print("An error occurred during processing:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/query.py` & `vectara-cli-0.1.6/vectara_cli/commands/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # query.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 4:
         print("Usage: vectara-cli query query_text num_results corpus_id")
         return
     query_text = args[1]
     num_results = int(args[2])
     corpus_id = args[3]
@@ -15,10 +16,12 @@
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
         response = vectara_client.query(query_text, num_results, corpus_id)
         print(response)
     except ValueError as e:
         print(e)
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/rebel_upsert_folder.py` & `vectara-cli-0.1.6/vectara_cli/commands/rebel_upsert_folder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 # ./commands/rebel_upsert_folder.py
 
 import os
-from vectara_cli.core import Rebel, VectaraClient
+from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
+from vectara_cli.advanced.noncommercial.rebel import Rebel
+
 
 def main(args):
     if len(args) < 4:
-        print("Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2")
+        print(
+            "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
+        )
+        print(
+            "Usage: vectara-cli advanced-upsert-folder folder_path corpus_id_1 corpus_id_2"
+        )
         return
 
     folder_path = args[1]
     corpus_id_1 = args[2]
     corpus_id_2 = args[3]
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
-        
+
         if not os.path.isdir(folder_path):
             print(f"The specified folder path does not exist: {folder_path}")
             return
 
         rebel = Rebel()
-        rebel.advanced_upsert_folder(vectara_client, corpus_id_1, corpus_id_2, folder_path)
+        rebel.advanced_upsert_folder(
+            vectara_client, corpus_id_1, corpus_id_2, folder_path
+        )
+        rebel.advanced_upsert_folder(
+            vectara_client, corpus_id_1, corpus_id_2, folder_path
+        )
         print(f"Advanced processing and upsert completed for folder: {folder_path}")
     except Exception as e:
         print("An error occurred during the upsert process:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/span-text.py` & `vectara-cli-0.1.6/vectara_cli/commands/span-text.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/span_enhance_folder.py` & `vectara-cli-0.1.6/vectara_cli/commands/span_enhance_folder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # ./commands/span_enhance_folder.py
 
 import os
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
 
+
 def main(args):
     if len(args) < 5:
-        print("Usage: vectara-cli span-enhance-folder corpus_id_1 corpus_id_2 model_name folder_path")
+        print(
+            "Usage: vectara-cli span-enhance-folder corpus_id_1 corpus_id_2 model_name folder_path"
+        )
         return
 
     corpus_id_1 = args[1]
     corpus_id_2 = args[2]
     model_name = args[3]
     folder_path = args[4]
 
@@ -18,14 +21,18 @@
         customer_id, api_key = ConfigManager.get_api_keys()
         if not os.path.isdir(folder_path):
             print(f"The specified folder path does not exist: {folder_path}")
             return
 
         enterprise_span = EnterpriseSpan(model_name, customer_id, api_key)
         enterprise_span.span_enhance(corpus_id_1, corpus_id_2, folder_path)
-        print(f"Documents in {folder_path} enhanced and uploaded to corpora: {corpus_id_1} (plain), {corpus_id_2} (enhanced)")
+        print(
+            f"Documents in {folder_path} enhanced and uploaded to corpora: {corpus_id_1} (plain), {corpus_id_2} (enhanced)"
+        )
     except Exception as e:
         print("An error occurred during the enhancement process:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/upload_document.py` & `vectara-cli-0.1.6/vectara_cli/commands/upload_document.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # ./commands/upload_document.py
 
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
+
 def main(args):
     if len(args) < 4:
         print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
         return
 
     corpus_id = args[1]
     file_path = args[2]
     document_id = args[3] if len(args) > 3 else None
     metadata = {}  # Extend this to accept metadata as an argument if needed
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         vectara_client = VectaraClient(customer_id, api_key)
-        response, status = vectara_client.upload_document(corpus_id, file_path, document_id, metadata)
-        
+        response, status = vectara_client.upload_document(
+            corpus_id, file_path, document_id, metadata
+        )
+
         if status:
             print("Upload successful:", response)
         else:
             print("Upload failed:", response)
     except Exception as e:
         print("Upload failed:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/commands/upload_enriched_text.py` & `vectara-cli-0.1.6/vectara_cli/commands/upload_enriched_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # ./commands/upload_enriched_text.py
 
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.advanced.commercial.enterprise import EnterpriseSpan
 
+
 def main(args):
     if len(args) < 6:
-        print("Usage: vectara-cli upload-enriched-text corpus_id document_id model_name text")
+        print(
+            "Usage: vectara-cli upload-enriched-text corpus_id document_id model_name text"
+        )
         return
 
     corpus_id = args[1]
     document_id = args[2]
     model_name = args[3]
     text = " ".join(args[4:])
 
@@ -18,10 +21,12 @@
         enterprise_span = EnterpriseSpan(model_name, customer_id, api_key)
         predictions = enterprise_span.predict(text)
         enterprise_span.upload_enriched_text(corpus_id, document_id, text, predictions)
         print("Enriched text uploaded successfully.")
     except Exception as e:
         print("Failed to upload enriched text:", str(e))
 
+
 if __name__ == "__main__":
     import sys
+
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.5/vectara_cli/config_manager.py` & `vectara-cli-0.1.6/vectara_cli/config_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # config_manager.py
 
 import os
 
+
 class ConfigManager:
     @staticmethod
     def set_api_keys(customer_id, api_key):
         """Sets the customer ID and API key as environment variables."""
-        os.environ['VECTARA_CUSTOMER_ID'] = customer_id
-        os.environ['VECTARA_API_KEY'] = api_key
+        os.environ["VECTARA_CUSTOMER_ID"] = customer_id
+        os.environ["VECTARA_API_KEY"] = api_key
 
     @staticmethod
     def get_api_keys():
         """Retrieves the customer ID and API key from environment variables."""
-        customer_id = os.getenv('VECTARA_CUSTOMER_ID')
-        api_key = os.getenv('VECTARA_API_KEY')
+        customer_id = os.getenv("VECTARA_CUSTOMER_ID")
+        api_key = os.getenv("VECTARA_API_KEY")
         if not customer_id or not api_key:
-            raise ValueError("API keys are not set. Please set them using the 'set-api-keys' command.")
+            raise ValueError(
+                "API keys are not set. Please set them using the 'set-api-keys' command."
+            )
         return customer_id, api_key
```

### Comparing `vectara-cli-0.1.5/vectara_cli/core.py` & `vectara-cli-0.1.6/vectara_cli/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 # ./vectara-cli/core.py
 
 import requests
 import json
 import os
 import logging
 
+
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
             "customer-id": customer_id,
-            "x-api-key": api_key
+            "x-api-key": api_key,
         }
 
-    def index_text(self, corpus_id, document_id, text, context="", metadata_json="", custom_dims=None):
+    def index_text(
+        self,
+        corpus_id,
+        document_id,
+        text,
+        context="",
+        metadata_json="",
+        custom_dims=None,
+    ):
         if custom_dims is None:
             custom_dims = []
 
         url = f"{self.base_url}/v1/core/index"
         payload = {
             "customerId": self.headers["customer-id"],
             "corpusId": corpus_id,
@@ -27,53 +36,57 @@
                 "documentId": document_id,
                 "metadataJson": metadata_json,
                 "parts": [
                     {
                         "text": text,
                         "context": context,
                         "metadataJson": metadata_json,
-                        "customDims": custom_dims
+                        "customDims": custom_dims,
                     }
                 ],
                 "defaultPartContext": context,
-                "customDims": custom_dims
-            }
+                "customDims": custom_dims,
+            },
         }
 
         response = requests.post(url, headers=self.headers, data=json.dumps(payload))
 
         if response.status_code == 200:
             response_data = response.json()
-            if 'status' in response_data and response_data['status']['code'] == "OK":
+            if "status" in response_data and response_data["status"]["code"] == "OK":
                 print("Indexing successful.")
                 return response_data
             else:
-                print("Indexing completed with status:", response_data['status']['code'])
+                print(
+                    "Indexing completed with status:", response_data["status"]["code"]
+                )
                 return response_data
         else:
             try:
                 error_response = response.json()
-                print(f"Error indexing text: {error_response.get('message', 'Unknown error')}")
+                print(
+                    f"Error indexing text: {error_response.get('message', 'Unknown error')}"
+                )
             except json.JSONDecodeError:
                 print(f"Non-JSON error response from server: {response.text}")
             return None
 
     def query(self, query_text, num_results=10, corpus_id=None):
         url = f"{self.base_url}/v1/query"
         data_dict = {
             "query": [
                 {
                     "query": query_text,
                     "num_results": num_results,
                     "corpus_key": [
                         {
                             "customer_id": self.headers["customer-id"],
-                            "corpus_id": corpus_id
+                            "corpus_id": corpus_id,
                         }
-                    ]
+                    ],
                 }
             ]
         }
 
         response = requests.post(url, headers=self.headers, data=json.dumps(data_dict))
         if response.status_code != 200:
             print(f"Query failed with status code: {response.status_code}")
@@ -89,30 +102,34 @@
 
     def _parse_query_response(self, response_data):
         if "responseSet" in response_data:
             for response_set in response_data["responseSet"]:
                 if "response" in response_set:
                     # Extracting and returning the first response for simplicity. Adjust as needed.
                     responses = response_set["response"]
-                    return [self._extract_response_info(response) for response in responses]
+                    return [
+                        self._extract_response_info(response) for response in responses
+                    ]
         else:
             print("No response set found in the data")
         return []
 
     @staticmethod
     def _extract_response_info(response):
         return {
             "text": response.get("text", ""),
             "score": response.get("score", 0),
             "metadata": response.get("metadata", []),
             "documentIndex": response.get("documentIndex"),
             "corpusKey": response.get("corpusKey", {}),
         }
-    
-    def _get_index_request_json(self, corpus_id, document_id, title, metadata, section_text):
+
+    def _get_index_request_json(
+        self, corpus_id, document_id, title, metadata, section_text
+    ):
         """Constructs the JSON payload for a document to be indexed."""
         document = {
             "document_id": document_id,
             "title": title,
             "metadata_json": json.dumps(metadata),
             "section": [
                 {"text": section_text},
@@ -123,15 +140,30 @@
             "customer_id": self.customer_id,
             "corpus_id": corpus_id,
             "document": document,
         }
 
         return json.dumps(request)
 
-    def create_corpus(self, corpus_id, name, description, dtProvision, enabled, swapQenc, swapIenc, textless, encrypted, encoderId, metadataMaxBytes, customDimensions, filterAttributes):
+    def create_corpus(
+        self,
+        corpus_id,
+        name,
+        description,
+        dtProvision,
+        enabled,
+        swapQenc,
+        swapIenc,
+        textless,
+        encrypted,
+        encoderId,
+        metadataMaxBytes,
+        customDimensions,
+        filterAttributes,
+    ):
         url = f"{self.base_url}/v1/create-corpus"
         payload = {
             "corpus": {
                 "id": corpus_id,
                 "name": name,
                 "description": description,
                 "dtProvision": dtProvision,
@@ -139,50 +171,57 @@
                 "swapQenc": swapQenc,
                 "swapIenc": swapIenc,
                 "textless": textless,
                 "encrypted": encrypted,
                 "encoderId": encoderId,
                 "metadataMaxBytes": metadataMaxBytes,
                 "customDimensions": customDimensions,
-                "filterAttributes": filterAttributes
+                "filterAttributes": filterAttributes,
             }
         }
 
         response = requests.post(url, headers=self.headers, data=json.dumps(payload))
-        
+
         if response.status_code == 200:
             # Assuming a successful response will have a JSON body
             try:
                 response_data = response.json()
                 # Check if the response contains the expected 'status' field with 'OK'
-                if response_data.get('status', {}).get('code') == "OK":
+                if response_data.get("status", {}).get("code") == "OK":
                     return {"success": True, "data": response_data}
                 else:
-                    return {"success": False, "error": response_data.get('status', {})}
+                    return {"success": False, "error": response_data.get("status", {})}
             except ValueError:
                 # In case the response body does not contain valid JSON
                 return {"success": False, "error": "Invalid JSON in response"}
         else:
             # Handle HTTP errors
             try:
                 error_data = response.json()
                 return {"success": False, "error": error_data}
             except ValueError:
-                return {"success": False, "error": f"HTTP Error {response.status_code}: {response.text}"}
+                return {
+                    "success": False,
+                    "error": f"HTTP Error {response.status_code}: {response.text}",
+                }
 
-    def _get_index_request_json(self, corpus_id, document_id, title, metadata, section_text):
+    def _get_index_request_json(
+        self, corpus_id, document_id, title, metadata, section_text
+    ):
         # Assuming this method correctly formats the request payload for indexing a document.
         # This is a placeholder implementation.
-        return json.dumps({
-            "corpusId": corpus_id,
-            "documentId": document_id,
-            "title": title,
-            "metadata": metadata,
-            "sectionText": section_text
-        })
+        return json.dumps(
+            {
+                "corpusId": corpus_id,
+                "documentId": document_id,
+                "title": title,
+                "metadata": metadata,
+                "sectionText": section_text,
+            }
+        )
 
     def index_document(self, corpus_id, document_id, title, metadata, section_text):
         """Indexes a document to the specified corpus using the Vectara platform.
 
         Args:
             corpus_id: ID of the corpus to which data needs to be indexed.
             document_id: Unique identifier for the document.
@@ -190,37 +229,49 @@
             metadata: A dictionary containing metadata about the document.
             section_text: The main content/text of the document.
 
         Returns:
             A tuple containing the response and a boolean indicating success or failure.
         """
         idx_address = f"{self.base_url}/v1/index"
-        payload = self._get_index_request_json(corpus_id, document_id, title, metadata, section_text)
+        payload = self._get_index_request_json(
+            corpus_id, document_id, title, metadata, section_text
+        )
         try:
             response = requests.post(idx_address, data=payload, headers=self.headers)
             response.raise_for_status()  # Raises HTTPError for bad responses
 
             message = response.json()
-            if "status" in message and message["status"]["code"] in ("OK", "ALREADY_EXISTS"):
+            if "status" in message and message["status"]["code"] in (
+                "OK",
+                "ALREADY_EXISTS",
+            ):
                 logging.info("Document indexed successfully or already exists.")
                 return message, True
             else:
-                logging.error("Indexing failed with status: %s", message.get("status", {}))
+                logging.error(
+                    "Indexing failed with status: %s", message.get("status", {})
+                )
                 return message.get("status", {}), False
         except requests.exceptions.HTTPError as e:
             logging.error("HTTP error occurred: %s", e)
             return {"code": "HTTP_ERROR", "message": str(e)}, False
         except requests.exceptions.RequestException as e:
             logging.error("Error during requests to Vectara API: %s", e)
             return {"code": "REQUEST_EXCEPTION", "message": str(e)}, False
         except ValueError as e:
             logging.error("Invalid response received from Vectara API: %s", e)
-            return {"code": "INVALID_RESPONSE", "message": "The response from Vectara API could not be decoded."}, False
-
-    def index_documents_from_folder(self, corpus_id, folder_path, return_extracted_document=False):
+            return {
+                "code": "INVALID_RESPONSE",
+                "message": "The response from Vectara API could not be decoded.",
+            }, False
+
+    def index_documents_from_folder(
+        self, corpus_id, folder_path, return_extracted_document=False
+    ):
         """Indexes all documents in a specified folder.
 
         Args:
             corpus_id: The ID of the corpus to which the documents will be indexed.
             folder_path: The path to the folder containing the documents.
 
         Returns:
@@ -228,63 +279,80 @@
         """
         results = []
         for file_name in os.listdir(folder_path):
             file_path = os.path.join(folder_path, file_name)
             document_id = os.path.splitext(file_name)[0]
 
             try:
-                response, status = self.upload_document(corpus_id, file_path, document_id=document_id, return_extracted_document=return_extracted_document)
-                extracted_text = response.get('extractedText', '') if return_extracted_document else None
+                response, status = self.upload_document(
+                    corpus_id,
+                    file_path,
+                    document_id=document_id,
+                    return_extracted_document=return_extracted_document,
+                )
+                extracted_text = (
+                    response.get("extractedText", "")
+                    if return_extracted_document
+                    else None
+                )
                 results.append((document_id, status == "Success", extracted_text))
                 if status != "Success":
                     logging.error(f"Failed to index document {document_id}: {response}")
                 else:
                     logging.info(f"Successfully indexed document {document_id}")
             except Exception as e:
                 logging.error(f"Error uploading or indexing file {file_name}: {e}")
                 results.append((document_id, False, None))
 
         return results
- 
+
     def delete_corpus(self, corpus_id):
         """Deletes a specified corpus.
 
         Args:
             corpus_id: The ID of the corpus to be deleted.
 
         Returns:
             A tuple containing the response JSON and a boolean indicating success or failure.
         """
         url = f"{self.base_url}/v1/delete-corpus"
-        payload = json.dumps({
-            "corpusId": corpus_id
-        })
+        payload = json.dumps({"corpusId": corpus_id})
 
         try:
             response = requests.post(url, headers=self.headers, data=payload)
             response_json = response.json()
 
             # Check if the response has a 'status' field and handle accordingly
-            if 'status' in response_json:
-                vectara_status_code = response_json['status'].get('code', 'UNKNOWN')
-                if vectara_status_code == 'OK':
+            if "status" in response_json:
+                vectara_status_code = response_json["status"].get("code", "UNKNOWN")
+                if vectara_status_code == "OK":
                     logging.info("Corpus deleted successfully.")
                     return response_json, True
                 else:
-                    logging.error("Failed to delete corpus with Vectara status code %s, detail: %s",
-                                  vectara_status_code, response_json['status'].get('statusDetail', 'No detail'))
+                    logging.error(
+                        "Failed to delete corpus with Vectara status code %s, detail: %s",
+                        vectara_status_code,
+                        response_json["status"].get("statusDetail", "No detail"),
+                    )
                     return response_json, False
             else:
                 logging.error("Unexpected response format: %s", response.text)
                 return response_json, False
         except requests.exceptions.RequestException as e:
             logging.error("Request failed: %s", e)
             return {"error": str(e)}, False
 
-    def upload_document(self, corpus_id, file_path, document_id=None, metadata=None, return_extracted_document=False):
+    def upload_document(
+        self,
+        corpus_id,
+        file_path,
+        document_id=None,
+        metadata=None,
+        return_extracted_document=False,
+    ):
         """
         Uploads and indexes a document into a corpus.
 
         Args:
             corpus_id: The ID of the corpus into which the document should be indexed.
             file_path: The path to the file to be uploaded.
             document_id: Optional. The Document ID to assign to the file.
@@ -294,31 +362,39 @@
         Returns:
             A tuple containing the server's response as a JSON object and a status message.
         """
         url = f"{self.base_url}/v1/upload?c={self.customer_id}&o={corpus_id}"
         if return_extracted_document:
             url += "&d=true"
 
-
-        files = {'file': open(file_path, 'rb')}
+        files = {"file": open(file_path, "rb")}
         if metadata is not None:
-            files['doc_metadata'] = (None, json.dumps(metadata), 'application/json')
+            files["doc_metadata"] = (None, json.dumps(metadata), "application/json")
 
-        response = requests.post(url, headers={key: val for key, val in self.headers.items() if key != 'Content-Type'}, files=files)
+        response = requests.post(
+            url,
+            headers={
+                key: val for key, val in self.headers.items() if key != "Content-Type"
+            },
+            files=files,
+        )
 
         if response.status_code == 200:
             return response.json(), "Success"
         else:
             try:
                 error_response = response.json()
-                error_message = error_response.get('message', 'Unknown error')
+                error_message = error_response.get("message", "Unknown error")
             except json.JSONDecodeError:
                 error_message = "Failed to parse error response."
 
-            raise Exception(f"Failed to upload document: HTTP {response.status_code} - {error_message}")
+            raise Exception(
+                f"Failed to upload document: HTTP {response.status_code} - {error_message}"
+            )
+
 
 # # Example usage
 # CUSTOMER_ID = "your_customer_id"
 # API_KEY = "your_api_key"
 # CORPUS_ID = "your_corpus_id"
 # FILE_PATH = "/path/to/your/document.pdf"
 # DOCUMENT_ID = "unique_document_id"  # Optional
```

### Comparing `vectara-cli-0.1.5/vectara_cli/main.py` & `vectara-cli-0.1.6/vectara_cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 # vectara_cli/main.py
 
 import sys
-from vectara_cli.commands import set_api_keys, index_document, query, create_corpus, delete_corpus
+from vectara_cli.commands import (
+    nerdspan_upsert_folder,
+    set_api_keys,
+    index_document,
+    query,
+    create_corpus,
+    delete_corpus,
+    span_enhance_folder,
+    upload_document,
+    upload_enriched_text,
+    span_text,
+    rebel_upsert_folder,
+)
+
 from vectara_cli.config_manager import ConfigManager
 from vectara_cli.core import VectaraClient
 
+
 def get_vectara_client():
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
         return VectaraClient(customer_id, api_key)
     except ValueError as e:
         print(e)
         sys.exit(1)
 
+
 def print_help():
     help_text = """
     Usage: vectara-cli <command> [arguments]
 
     Commands:
     set-api-keys <customer_id> <api_key> - Set the API keys for Vectara client.
     index-document <args> - Index a document in the Vectara platform.
@@ -30,47 +45,47 @@
     nerdspan-upsert-folder <args> - Process and upload documents in a folder using the nerdspan model.
     rebel-upsert-folder <args> - Perform advanced upsert for a folder using the rebel model.
 
     Use 'vectara-cli help' to display this help message.
     """
     print(help_text)
 
+
 def main():
     args = sys.argv[1:]
-    if not args or args[0] in ('help', '--help', '-h'):
+    if not args or args[0] in ("help", "--help", "-h"):
         print_help()
         return
 
     command = args[0]
 
-    '''TODO create help function for all commands and what they do'''
-
     if command == "set-api-keys":
         set_api_keys.main(args)
     else:
         vectara_client = get_vectara_client()
 
         if command == "index-document":
             index_document.main(args, vectara_client)
         elif command == "query":
             query.main(args, vectara_client)
         elif command == "create-corpus":
             create_corpus.main(args, vectara_client)
         elif command == "delete-corpus":
             delete_corpus.main(args, vectara_client)
         elif command == "span-text":
-            delete_corpus.main(args, vectara_client)
-        elif command == "span-enchance-folder":
-            delete_corpus.main(args, vectara_client)
+            span_text.main(args, vectara_client)
+        elif command == "span-enhance-folder":
+            span_enhance_folder.main(args, vectara_client)
         elif command == "upload-document":
-            delete_corpus.main(args, vectara_client)
+            upload_document.main(args, vectara_client)
         elif command == "upload-enriched-text":
-            delete_corpus.main(args, vectara_client)
+            upload_enriched_text.main(args, vectara_client)
         elif command == "nerdspan-upsert-folder":
-            delete_corpus.main(args, vectara_client)
+            nerdspan_upsert_folder.main(args, vectara_client)
         elif command == "rebel-upsert-folder":
-            delete_corpus.main(args, vectara_client)
+            rebel_upsert_folder.main(args, vectara_client)
         else:
             print(f"Unknown command: {command}")
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `vectara-cli-0.1.5/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.6/vectara_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vectara-cli-0.1.5/vectara_cli.egg-info/SOURCES.txt` & `vectara-cli-0.1.6/vectara_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 vectara_cli/commands/index_document.py
 vectara_cli/commands/nerdspan_upsert_folder.py
 vectara_cli/commands/query.py
 vectara_cli/commands/rebel_upsert_folder.py
 vectara_cli/commands/set_api_keys.py
 vectara_cli/commands/span-text.py
 vectara_cli/commands/span_enhance_folder.py
+vectara_cli/commands/span_text.py
 vectara_cli/commands/upload_document.py
 vectara_cli/commands/upload_enriched_text.py
```

