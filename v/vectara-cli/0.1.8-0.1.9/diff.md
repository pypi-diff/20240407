# Comparing `tmp/vectara-cli-0.1.8.tar.gz` & `tmp/vectara-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-cli-0.1.8.tar", last modified: Sun Apr  7 10:21:46 2024, max compression
+gzip compressed data, was "vectara-cli-0.1.9.tar", last modified: Sun Apr  7 15:46:34 2024, max compression
```

## Comparing `vectara-cli-0.1.8.tar` & `vectara-cli-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.853767 vectara-cli-0.1.8/
--rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/LICENSE.md
--rw-rw-rw-   0        0        0    22546 2024-04-07 10:21:46.852767 vectara-cli-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    21380 2024-04-07 08:11:24.000000 vectara-cli-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 10:21:46.854266 vectara-cli-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1428 2024-04-07 10:21:35.000000 vectara-cli-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.815769 vectara-cli-0.1.8/vectara_cli/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.8/vectara_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.822768 vectara-cli-0.1.8/vectara_cli/advanced/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/advanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.825268 vectara-cli-0.1.8/vectara_cli/advanced/commercial/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/advanced/commercial/__init__.py
--rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.8/vectara_cli/advanced/commercial/enterprise.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.829266 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/__init__.py
--rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/nerdspan.py
--rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/rebel.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.848767 vectara-cli-0.1.8/vectara_cli/commands/
--rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.8/vectara_cli/commands/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-07 10:07:18.000000 vectara-cli-0.1.8/vectara_cli/commands/create_corpus.py
--rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/delete_corpus.py
--rw-rw-rw-   0        0        0      957 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/index_document.py
--rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/nerdspan_upsert_folder.py
--rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/query.py
--rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/rebel_upsert_folder.py
--rw-rw-rw-   0        0        0      425 2024-04-06 19:29:01.000000 vectara-cli-0.1.8/vectara_cli/commands/set_api_keys.py
--rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/span_enhance_folder.py
--rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/span_text.py
--rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/upload_document.py
--rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/commands/upload_enriched_text.py
--rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.8/vectara_cli/config_manager.py
--rw-rw-rw-   0        0        0    17356 2024-04-07 09:45:39.000000 vectara-cli-0.1.8/vectara_cli/core.py
--rw-rw-rw-   0        0        0     1550 2024-04-07 09:49:58.000000 vectara-cli-0.1.8/vectara_cli/corpus_data.py
--rw-rw-rw-   0        0        0      500 2024-04-07 09:11:10.000000 vectara-cli-0.1.8/vectara_cli/custom_dimension.py
--rw-rw-rw-   0        0        0      937 2024-04-07 09:41:11.000000 vectara-cli-0.1.8/vectara_cli/defaults.py
--rw-rw-rw-   0        0        0      479 2024-04-07 09:10:54.000000 vectara-cli-0.1.8/vectara_cli/filter_attribute.py
--rw-rw-rw-   0        0        0     3138 2024-04-07 10:18:19.000000 vectara-cli-0.1.8/vectara_cli/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:21:46.850436 vectara-cli-0.1.8/vectara_cli.egg-info/
--rw-rw-rw-   0        0        0    22546 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1180 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       83 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 10:21:46.000000 vectara-cli-0.1.8/vectara_cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.808295 vectara-cli-0.1.9/
+-rw-rw-rw-   0        0        0    33954 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/LICENSE.md
+-rw-rw-rw-   0        0        0    22546 2024-04-07 15:46:34.806212 vectara-cli-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    21380 2024-04-07 08:11:24.000000 vectara-cli-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 15:46:34.808792 vectara-cli-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2024-04-07 15:46:32.000000 vectara-cli-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.770661 vectara-cli-0.1.9/vectara_cli/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.9/vectara_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.780173 vectara-cli-0.1.9/vectara_cli/advanced/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/advanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.781673 vectara-cli-0.1.9/vectara_cli/advanced/commercial/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/advanced/commercial/__init__.py
+-rw-rw-rw-   0        0        0     7672 2024-04-06 19:42:54.000000 vectara-cli-0.1.9/vectara_cli/advanced/commercial/enterprise.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.785188 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:13:47.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/__init__.py
+-rw-rw-rw-   0        0        0     6223 2024-04-06 19:29:01.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/nerdspan.py
+-rw-rw-rw-   0        0        0     9808 2024-04-06 21:57:37.000000 vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/rebel.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.801780 vectara-cli-0.1.9/vectara_cli/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-06 18:07:05.000000 vectara-cli-0.1.9/vectara_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     4109 2024-04-07 15:24:00.000000 vectara-cli-0.1.9/vectara_cli/commands/create_corpus.py
+-rw-rw-rw-   0        0        0      704 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/delete_corpus.py
+-rw-rw-rw-   0        0        0     1575 2024-04-07 14:14:09.000000 vectara-cli-0.1.9/vectara_cli/commands/index_document.py
+-rw-rw-rw-   0        0        0      944 2024-04-07 12:31:13.000000 vectara-cli-0.1.9/vectara_cli/commands/index_text.py
+-rw-rw-rw-   0        0        0     1131 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/nerdspan_upsert_folder.py
+-rw-rw-rw-   0        0        0      643 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/query.py
+-rw-rw-rw-   0        0        0     1345 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/rebel_upsert_folder.py
+-rw-rw-rw-   0        0        0     1189 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/span_enhance_folder.py
+-rw-rw-rw-   0        0        0      822 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/span_text.py
+-rw-rw-rw-   0        0        0      900 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/upload_document.py
+-rw-rw-rw-   0        0        0      978 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/commands/upload_enriched_text.py
+-rw-rw-rw-   0        0        0      893 2024-04-06 21:50:16.000000 vectara-cli-0.1.9/vectara_cli/config_manager.py
+-rw-rw-rw-   0        0        0    17818 2024-04-07 14:24:08.000000 vectara-cli-0.1.9/vectara_cli/core.py
+-rw-rw-rw-   0        0        0     1675 2024-04-07 14:22:48.000000 vectara-cli-0.1.9/vectara_cli/corpus_data.py
+-rw-rw-rw-   0        0        0      528 2024-04-07 11:57:54.000000 vectara-cli-0.1.9/vectara_cli/custom_dimension.py
+-rw-rw-rw-   0        0        0      937 2024-04-07 09:41:11.000000 vectara-cli-0.1.9/vectara_cli/defaults.py
+-rw-rw-rw-   0        0        0      506 2024-04-07 11:49:57.000000 vectara-cli-0.1.9/vectara_cli/filter_attribute.py
+-rw-rw-rw-   0        0        0     2885 2024-04-07 15:00:09.000000 vectara-cli-0.1.9/vectara_cli/main.py
+-rw-rw-rw-   0        0        0      405 2024-04-07 14:58:40.000000 vectara-cli-0.1.9/vectara_cli/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:46:34.803715 vectara-cli-0.1.9/vectara_cli.egg-info/
+-rw-rw-rw-   0        0        0    22546 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       83 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 15:46:34.000000 vectara-cli-0.1.9/vectara_cli.egg-info/top_level.txt
```

### Comparing `vectara-cli-0.1.8/LICENSE.md` & `vectara-cli-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/PKG-INFO` & `vectara-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vectara-cli-0.1.8/README.md` & `vectara-cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/setup.py` & `vectara-cli-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ./setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="vectara-cli",
-    version="0.1.8",
+    version="0.1.9",
     author="Tonic-AI",
     author_email="team@tonic-ai.com",
     description="A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://git.tonic-ai.com/releases/vectara-cli",
     packages=find_packages(),
```

### Comparing `vectara-cli-0.1.8/vectara_cli/advanced/commercial/enterprise.py` & `vectara-cli-0.1.9/vectara_cli/advanced/commercial/enterprise.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/nerdspan.py` & `vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/nerdspan.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/advanced/noncommercial/rebel.py` & `vectara-cli-0.1.9/vectara_cli/advanced/noncommercial/rebel.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/delete_corpus.py` & `vectara-cli-0.1.9/vectara_cli/commands/delete_corpus.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/index_document.py` & `vectara-cli-0.1.9/vectara_cli/commands/upload_document.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-# index_document.py
+# ./commands/upload_document.py
 
-import json
 from vectara_cli.core import VectaraClient
 from vectara_cli.config_manager import ConfigManager
 
 
 def main(args, vectara_client):
-    if len(args) < 6:
-        print(
-            "Usage: vectara-cli index-document corpus_id document_id title metadata_json section_text"
-        )
+    if len(args) < 4:
+        print("Usage: vectara-cli upload-document corpus_id file_path [document_id]")
         return
+
     corpus_id = args[1]
-    document_id = args[2]
-    title = args[3]
-    metadata = json.loads(args[4])
-    section_text = args[5]
+    file_path = args[2]
+    document_id = args[3] if len(args) > 3 else None
+    metadata = {}
 
     try:
         customer_id, api_key = ConfigManager.get_api_keys()
-        response, success = vectara_client.index_document(
-            corpus_id, document_id, title, metadata, section_text
+        response, status = vectara_client.upload_document(
+            corpus_id, file_path, document_id, metadata
         )
-        if success:
-            print("Document indexed successfully.")
+
+        if status:
+            print("Upload successful:", response)
         else:
-            print("Document indexing failed.", response)
-    except ValueError as e:
-        print(e)
+            print("Upload failed:", response)
+    except Exception as e:
+        print("Upload failed:", str(e))
 
 
 if __name__ == "__main__":
     import sys
 
     main(sys.argv[1:])
```

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/nerdspan_upsert_folder.py` & `vectara-cli-0.1.9/vectara_cli/commands/nerdspan_upsert_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/query.py` & `vectara-cli-0.1.9/vectara_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/rebel_upsert_folder.py` & `vectara-cli-0.1.9/vectara_cli/commands/rebel_upsert_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/span_enhance_folder.py` & `vectara-cli-0.1.9/vectara_cli/commands/span_enhance_folder.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/span_text.py` & `vectara-cli-0.1.9/vectara_cli/commands/span_text.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/commands/upload_document.py` & `vectara-cli-0.1.9/vectara_cli/commands/upload_enriched_text.py`

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

### Comparing `vectara-cli-0.1.8/vectara_cli/config_manager.py` & `vectara-cli-0.1.9/vectara_cli/config_manager.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/core.py` & `vectara-cli-0.1.9/vectara_cli/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,46 +6,49 @@
 import logging
 from .corpus_data import CorpusData
 from .defaults import CorpusDefaults
 
 class VectaraClient:
     def __init__(self, customer_id, api_key):
         self.base_url = "https://api.vectara.io"
-        self.customer_id = customer_id
+        self.customer_id = str(customer_id)
         self.api_key = api_key
         self.headers = {
             "Content-Type": "application/json",
             "Accept": "application/json",
-            "customer-id": customer_id,
+            "customer-id": str(customer_id),
             "x-api-key": api_key,
         }
 
     def index_text(
         self,
         corpus_id,
         document_id,
         text,
         context="",
         metadata_json="",
         custom_dims=None,
     ):
         if custom_dims is None:
             custom_dims = []
-
+        if not isinstance(metadata_json, str):
+            metadata_json = json.dumps(metadata_json)
+        corpus_id = str(corpus_id)
         url = f"{self.base_url}/v1/core/index"
         payload = {
-            "customerId": self.headers["customer-id"],
-            "corpusId": corpus_id,
+            "customerId": int(self.customer_id),
+            "corpusId": int(corpus_id), 
             "document": {
                 "documentId": document_id,
-                "metadataJson": metadata_json,
+                "metadataJson": metadata_json.replace('"', '\\"'),
                 "parts": [
                     {
                         "text": text,
                         "context": context,
+#                       "metadataJson": json.dumps(metadata_json),
                         "metadataJson": metadata_json,
                         "customDims": custom_dims,
                     }
                 ],
                 "defaultPartContext": context,
                 "customDims": custom_dims,
             },
@@ -145,15 +148,15 @@
             "document": document,
         }
 
         return json.dumps(request)
 
     def create_corpus(self, corpus_data: CorpusData):
         url = f"{self.base_url}/v1/create-corpus"
-        payload = {"corpus": {corpus_data.to_dict()}}
+        payload = corpus_data.to_dict()
 
         response = requests.post(url, headers=self.headers, data=json.dumps(payload))
         return self._parse_response(response)
 
     def _parse_response(self, response):
         if response.status_code == 200:
             try:
@@ -192,58 +195,64 @@
         json_payload = json.dumps(request)
         print("Constructed JSON payload:", json_payload)  # Log the payload for debugging
 
         return json_payload
 
 
     def index_document(self, corpus_id, document_id, title, metadata, section_text):
-        """Indexes a document to the specified corpus using the Vectara platform.
+        """
+        Indexes a document to the specified corpus using the Vectara platform.
 
         Args:
-            corpus_id: ID of the corpus to which data needs to be indexed.
-            document_id: Unique identifier for the document.
-            title: Title of the document.
-            metadata: A dictionary containing metadata about the document.
-            section_text: The main content/text of the document.
+            corpus_id (int): ID of the corpus to which data needs to be indexed.
+            document_id (str): Unique identifier for the document.
+            title (str): Title of the document.
+            metadata (dict): A dictionary containing metadata about the document.
+            section_text (str): The main content/text of the document.
 
         Returns:
             A tuple containing the response and a boolean indicating success or failure.
         """
         idx_address = f"{self.base_url}/v1/index"
-        payload = self._get_index_request_json(
-            corpus_id, document_id, title, metadata, section_text
-        )
+        metadata_json = json.dumps(metadata)  # Convert metadata to a JSON string
+
+        payload = {
+            "customerId": self.customer_id,
+            "corpusId": corpus_id,
+            "document": {
+                "documentId": document_id,
+                "title": title,
+                "metadataJson": metadata_json, 
+                "sections": [{
+                    "text": section_text
+                }]
+            }
+        }
+
         try:
-            response = requests.post(idx_address, data=payload, headers=self.headers)
-            response.raise_for_status()
+            response = requests.post(idx_address, headers=self.headers, json=payload) 
+            response.raise_for_status()  
 
             message = response.json()
-            if "status" in message and message["status"]["code"] in (
-                "OK",
-                "ALREADY_EXISTS",
-            ):
+            if "status" in message and message["status"]["code"] in ("OK", "ALREADY_EXISTS"):
                 logging.info("Document indexed successfully or already exists.")
                 return message, True
             else:
-                logging.error(
-                    "Indexing failed with status: %s", message.get("status", {})
-                )
+                logging.error("Indexing failed with status: %s", message.get("status", {}))
                 return message.get("status", {}), False
         except requests.exceptions.HTTPError as e:
             logging.error("HTTP error occurred: %s", e)
             return {"code": "HTTP_ERROR", "message": str(e)}, False
         except requests.exceptions.RequestException as e:
             logging.error("Error during requests to Vectara API: %s", e)
             return {"code": "REQUEST_EXCEPTION", "message": str(e)}, False
         except ValueError as e:
             logging.error("Invalid response received from Vectara API: %s", e)
-            return {
-                "code": "INVALID_RESPONSE",
-                "message": "The response from Vectara API could not be decoded.",
-            }, False
+            return {"code": "INVALID_RESPONSE", "message": "The response from Vectara API could not be decoded."}, False
+
 
     def index_documents_from_folder(
         self, corpus_id, folder_path, return_extracted_document=False
     ):
         """Indexes all documents in a specified folder.
 
         Args:
```

### Comparing `vectara-cli-0.1.8/vectara_cli/corpus_data.py` & `vectara-cli-0.1.9/vectara_cli/corpus_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+# ./corpus_data.py
+
 from .filter_attribute import FilterAttribute
 from .custom_dimension import CustomDimension
 
 class CorpusData:
     def __init__(self, corpus_id, name, description, dtProvision, enabled, swapQenc, swapIenc, textless, encrypted, encoderId, metadataMaxBytes, customDimensions, filterAttributes):
         self.corpus_id = corpus_id
         self.name = name
         self.description = description
-        self.dtProvision = dtProvision
+        self.dtProvision = int(dtProvision) if encoderId.isdigit() else None
         self.enabled = enabled
         self.swapQenc = swapQenc
         self.swapIenc = swapIenc
         self.textless = textless
         self.encrypted = encrypted
-        self.encoderId = encoderId
+        self.encoderId = int(encoderId) if encoderId.isdigit() else 1
         self.metadataMaxBytes = metadataMaxBytes
         self.customDimensions = [CustomDimension(**dim) for dim in customDimensions]
         self.filterAttributes = [FilterAttribute(**attr) for attr in filterAttributes]
 
     def to_dict(self):
         return {
             "id": self.corpus_id,
             "name": self.name,
             "description": self.description,
-            "dtProvision": self.dtProvision,
+            "dtProvision": self.dtProvision, # ommit if there's an issue ?
             "enabled": self.enabled,
             "swapQenc": self.swapQenc,
             "swapIenc": self.swapIenc,
             "textless": self.textless,
             "encrypted": self.encrypted,
             "encoderId": self.encoderId,
             "metadataMaxBytes": self.metadataMaxBytes,
```

### Comparing `vectara-cli-0.1.8/vectara_cli/defaults.py` & `vectara-cli-0.1.9/vectara_cli/defaults.py`

 * *Files identical despite different names*

### Comparing `vectara-cli-0.1.8/vectara_cli/main.py` & `vectara-cli-0.1.9/vectara_cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-# vectara_cli/main.py
-from .defaults import CorpusDefaults
-
-import sys
+ # ./main.py
+import sys 
 from vectara_cli.commands import (
     nerdspan_upsert_folder,
-    set_api_keys,
+    index_text,
     index_document,
     query,
     create_corpus,
     delete_corpus,
     span_enhance_folder,
     upload_document,
     upload_enriched_text,
     span_text,
     rebel_upsert_folder,
 )
-
 from vectara_cli.config_manager import ConfigManager
-from vectara_cli.core import VectaraClient
-
-
-def get_vectara_client():
-    try:
-        customer_id, api_key = ConfigManager.get_api_keys()
-        return VectaraClient(customer_id, api_key)
-    except ValueError as e:
-        print(e)
-        sys.exit(1)
-
+# from vectara_cli.commands.set_api_keys import main as set_api_keys_main
+from vectara_cli.utils import get_vectara_client , set_api_keys as set_api_keys_main
 
 def print_help():
     help_text = """
     Usage: vectara-cli <command> [arguments]
 
     Commands:
     set-api-keys <customer_id> <api_key> - Set the API keys for Vectara client.
@@ -46,48 +34,45 @@
     nerdspan-upsert-folder <args> - Process and upload documents in a folder using the nerdspan model.
     rebel-upsert-folder <args> - Perform advanced upsert for a folder using the rebel model.
 
     Use 'vectara-cli help' to display this help message.
     """
     print(help_text)
 
-
 def main():
-    
     if len(sys.argv) < 2 or sys.argv[1] in ("help", "--help", "-h"):
         print_help()
         return
-    
+
     command = sys.argv[1]
-    args = sys.argv[2:] 
+    args = sys.argv[1:] 
 
     if command == "set-api-keys":
-        set_api_keys.main(args)
+        set_api_keys_main(args)
     else:
-        vectara_client = get_vectara_client()
-
-        if command == "index-document":
-            index_document.main(args, vectara_client)
-        elif command == "query":
-            query.main(args, vectara_client)
-        elif command == "create-corpus":
-            create_corpus.main(args, vectara_client)
-        elif command == "delete-corpus":
-            delete_corpus.main(args, vectara_client)
-        elif command == "span-text":
-            span_text.main(args, vectara_client)
-        elif command == "span-enhance-folder":
-            span_enhance_folder.main(args, vectara_client)
-        elif command == "upload-document":
-            upload_document.main(args, vectara_client)
-        elif command == "upload-enriched-text":
-            upload_enriched_text.main(args, vectara_client)
-        elif command == "nerdspan-upsert-folder":
-            nerdspan_upsert_folder.main(args, vectara_client)
-        elif command == "rebel-upsert-folder":
-            rebel_upsert_folder.main(args, vectara_client)
-        else:
-            print(f"Unknown command: {command}")
-
+        try:
+            vectara_client = get_vectara_client()
+            command_mapping = {
+                "index-document": index_document.main,
+                "query": query.main,
+                "create-corpus": create_corpus.main,
+                "delete-corpus": delete_corpus.main,
+                "span-text": span_text.main,
+                "span-enhance-folder": span_enhance_folder.main,
+                "upload-document": upload_document.main,
+                "upload-enriched-text": upload_enriched_text.main,
+                "nerdspan-upsert-folder": nerdspan_upsert_folder.main,
+                "rebel-upsert-folder": rebel_upsert_folder.main,
+                "index-text": index_text.main,
+            }
+
+            if command in command_mapping:
+                command_mapping[command](args, vectara_client)
+            else:
+                print(f"Unknown command: {command}")
+                print_help()
+        except ValueError as e:
+            print(e)
+            sys.exit(1)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `vectara-cli-0.1.8/vectara_cli.egg-info/PKG-INFO` & `vectara-cli-0.1.9/vectara_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: A CLI tool for interacting with the Vectara platform, including advanced text processing and indexing features.
 Home-page: https://git.tonic-ai.com/releases/vectara-cli
 Author: Tonic-AI
 Author-email: team@tonic-ai.com
 License: MIT
 Keywords: vectara search-engine document-indexing text-analysis information-retrieval natural-language-processing cli-tool data-science machine-learning text-processing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vectara-cli-0.1.8/vectara_cli.egg-info/SOURCES.txt` & `vectara-cli-0.1.9/vectara_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 vectara_cli/config_manager.py
 vectara_cli/core.py
 vectara_cli/corpus_data.py
 vectara_cli/custom_dimension.py
 vectara_cli/defaults.py
 vectara_cli/filter_attribute.py
 vectara_cli/main.py
+vectara_cli/utils.py
 vectara_cli.egg-info/PKG-INFO
 vectara_cli.egg-info/SOURCES.txt
 vectara_cli.egg-info/dependency_links.txt
 vectara_cli.egg-info/entry_points.txt
 vectara_cli.egg-info/requires.txt
 vectara_cli.egg-info/top_level.txt
 vectara_cli/advanced/__init__.py
@@ -21,15 +22,15 @@
 vectara_cli/advanced/noncommercial/__init__.py
 vectara_cli/advanced/noncommercial/nerdspan.py
 vectara_cli/advanced/noncommercial/rebel.py
 vectara_cli/commands/__init__.py
 vectara_cli/commands/create_corpus.py
 vectara_cli/commands/delete_corpus.py
 vectara_cli/commands/index_document.py
+vectara_cli/commands/index_text.py
 vectara_cli/commands/nerdspan_upsert_folder.py
 vectara_cli/commands/query.py
 vectara_cli/commands/rebel_upsert_folder.py
-vectara_cli/commands/set_api_keys.py
 vectara_cli/commands/span_enhance_folder.py
 vectara_cli/commands/span_text.py
 vectara_cli/commands/upload_document.py
 vectara_cli/commands/upload_enriched_text.py
```

