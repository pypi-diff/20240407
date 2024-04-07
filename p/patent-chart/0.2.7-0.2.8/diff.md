# Comparing `tmp/patent_chart-0.2.7.tar.gz` & `tmp/patent_chart-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_chart-0.2.7.tar", max compression
+gzip compressed data, was "patent_chart-0.2.8.tar", max compression
```

## Comparing `patent_chart-0.2.7.tar` & `patent_chart-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-04-03 22:16:17.760177 patent_chart-0.2.7/patent_chart/__init__.py
--rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.7/patent_chart/citation.py
--rw-r--r--   0        0        0     1759 2024-04-04 16:56:23.070248 patent_chart-0.2.7/patent_chart/data_structures.py
--rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.7/patent_chart/embeddings.py
--rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.7/patent_chart/evaluation.py
--rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.7/patent_chart/filtering.py
--rw-r--r--   0        0        0    37060 2024-04-05 03:16:24.398048 patent_chart-0.2.7/patent_chart/generator.py
--rw-r--r--   0        0        0     3249 2024-04-04 16:55:39.837226 patent_chart-0.2.7/patent_chart/google_patents.py
--rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.7/patent_chart/integrationtests.py
--rw-r--r--   0        0        0    64508 2024-04-02 04:43:42.390709 patent_chart-0.2.7/patent_chart/parser.py
--rw-r--r--   0        0        0     4518 2024-04-05 02:43:11.615256 patent_chart-0.2.7/patent_chart/pinecone.py
--rw-r--r--   0        0        0     5277 2024-04-04 03:03:09.786061 patent_chart-0.2.7/patent_chart/ranking.py
--rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.7/patent_chart/redis_utils.py
--rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.7/patent_chart/requests_utils.py
--rw-r--r--   0        0        0     5931 2024-04-04 03:03:09.787023 patent_chart-0.2.7/patent_chart/search_index.py
--rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.7/patent_chart/settings.py
--rw-r--r--   0        0        0    31579 2024-04-02 04:43:42.392082 patent_chart-0.2.7/patent_chart/tests.py
--rw-r--r--   0        0        0     6106 2024-04-04 03:49:22.349201 patent_chart-0.2.7/patent_chart/uspto_parse.py
--rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.7/patent_chart/utils.py
--rw-r--r--   0        0        0     1082 2024-04-05 03:18:45.504490 patent_chart-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 patent_chart-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-02 22:00:15.933827 patent_chart-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 22:16:17.760177 patent_chart-0.2.8/patent_chart/__init__.py
+-rw-r--r--   0        0        0     3440 2024-02-02 22:00:15.821601 patent_chart-0.2.8/patent_chart/citation.py
+-rw-r--r--   0        0        0     1759 2024-04-06 03:36:49.841147 patent_chart-0.2.8/patent_chart/data_structures.py
+-rw-r--r--   0        0        0     1843 2024-02-02 22:00:15.871024 patent_chart-0.2.8/patent_chart/embeddings.py
+-rw-r--r--   0        0        0     2811 2024-02-02 22:00:15.824681 patent_chart-0.2.8/patent_chart/evaluation.py
+-rw-r--r--   0        0        0      498 2024-02-02 22:00:15.823970 patent_chart-0.2.8/patent_chart/filtering.py
+-rw-r--r--   0        0        0    37060 2024-04-06 03:36:49.842435 patent_chart-0.2.8/patent_chart/generator.py
+-rw-r--r--   0        0        0    11496 2024-04-07 17:08:25.982481 patent_chart-0.2.8/patent_chart/google_patents.py
+-rw-r--r--   0        0        0     3838 2024-02-02 22:00:15.872576 patent_chart-0.2.8/patent_chart/integrationtests.py
+-rw-r--r--   0        0        0    64508 2024-04-02 04:43:42.390709 patent_chart-0.2.8/patent_chart/parser.py
+-rw-r--r--   0        0        0     4536 2024-04-07 17:09:21.646564 patent_chart-0.2.8/patent_chart/pinecone.py
+-rw-r--r--   0        0        0     5277 2024-04-06 03:36:49.846114 patent_chart-0.2.8/patent_chart/ranking.py
+-rw-r--r--   0        0        0      591 2024-02-02 22:00:15.820971 patent_chart-0.2.8/patent_chart/redis_utils.py
+-rw-r--r--   0        0        0     5103 2024-02-02 22:00:15.870154 patent_chart-0.2.8/patent_chart/requests_utils.py
+-rw-r--r--   0        0        0     5931 2024-04-06 03:36:49.847015 patent_chart-0.2.8/patent_chart/search_index.py
+-rw-r--r--   0        0        0      567 2024-02-20 15:54:25.646442 patent_chart-0.2.8/patent_chart/settings.py
+-rw-r--r--   0        0        0    31579 2024-04-02 04:43:42.392082 patent_chart-0.2.8/patent_chart/tests.py
+-rw-r--r--   0        0        0     6106 2024-04-06 03:51:00.343412 patent_chart-0.2.8/patent_chart/uspto_parse.py
+-rw-r--r--   0        0        0     1825 2024-02-02 22:00:15.871782 patent_chart-0.2.8/patent_chart/utils.py
+-rw-r--r--   0        0        0     1082 2024-04-07 17:22:09.343062 patent_chart-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 patent_chart-0.2.8/PKG-INFO
```

### Comparing `patent_chart-0.2.7/patent_chart/citation.py` & `patent_chart-0.2.8/patent_chart/citation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/data_structures.py` & `patent_chart-0.2.8/patent_chart/data_structures.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/embeddings.py` & `patent_chart-0.2.8/patent_chart/embeddings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/evaluation.py` & `patent_chart-0.2.8/patent_chart/evaluation.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/generator.py` & `patent_chart-0.2.8/patent_chart/generator.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/integrationtests.py` & `patent_chart-0.2.8/patent_chart/integrationtests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/parser.py` & `patent_chart-0.2.8/patent_chart/parser.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/pinecone.py` & `patent_chart-0.2.8/patent_chart/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,25 +87,25 @@
 
     if not vectors:
         raise IndexError("No claim embeddings to index")
 
     claims_index.upsert(vectors)
 
 
-# @retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
-def query_spec_embedding(query: list[float], top_k: int, filter: dict | None = None):
-    return spec_index.query(query, top_k=top_k, filter=filter)['matches']
+@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
+def query_spec_embedding(query: list[float], top_k: int, filter: dict | None = None, **kwargs):
+    return spec_index.query(query, top_k=top_k, filter=filter, **kwargs)['matches']
 
 
 @retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
 def get_claim_embeddings_by_patent_doc_id(patent_doc_id:str):
-    ids = claims_index.list(prefix=patent_doc_id)
+    ids = list(claims_index.list(prefix=patent_doc_id))
     if not ids:
         return []
-    ids = list(ids)[0]
+    ids = ids[0]
     records = claims_index.fetch(ids)
     return records['vectors']
 
 
 def get_claim_embeddings_values_by_patent_doc_id(patent_doc_id:str):
     values = []
     records = get_claim_embeddings_by_patent_doc_id(patent_doc_id)
@@ -113,18 +113,18 @@
         record_values = records[record]['values']
         values.append(record_values)
     return values
 
 
 @retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(6), reraise=True)
 def get_spec_embeddings_by_patent_doc_id(patent_doc_id:str):
-    ids = spec_index.list(prefix=patent_doc_id)
+    ids = list(spec_index.list(prefix=patent_doc_id))
     if not ids:
         return []
-    ids = list(ids)[0]
+    ids = ids[0]
     records = spec_index.fetch(ids)
     return records['vectors']
 
 
 def get_spec_embeddings_values_by_patent_doc_id(patent_doc_id:str):
     values = []
     records = get_spec_embeddings_by_patent_doc_id(patent_doc_id)
```

### Comparing `patent_chart-0.2.7/patent_chart/ranking.py` & `patent_chart-0.2.8/patent_chart/ranking.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/redis_utils.py` & `patent_chart-0.2.8/patent_chart/redis_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/requests_utils.py` & `patent_chart-0.2.8/patent_chart/requests_utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/search_index.py` & `patent_chart-0.2.8/patent_chart/search_index.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/settings.py` & `patent_chart-0.2.8/patent_chart/settings.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/tests.py` & `patent_chart-0.2.8/patent_chart/tests.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/uspto_parse.py` & `patent_chart-0.2.8/patent_chart/uspto_parse.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/patent_chart/utils.py` & `patent_chart-0.2.8/patent_chart/utils.py`

 * *Files identical despite different names*

### Comparing `patent_chart-0.2.7/pyproject.toml` & `patent_chart-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent-chart"
-version = "0.2.7"
+version = "0.2.8"
 description = "Automated invalidity contention charts"
 authors = ["Josh Hedtke"]
 license = "Proprietary"
 readme = "README.md"
 
 exclude = ["experiments.ipynb"]
```

### Comparing `patent_chart-0.2.7/PKG-INFO` & `patent_chart-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patent-chart
-Version: 0.2.7
+Version: 0.2.8
 Summary: Automated invalidity contention charts
 License: Proprietary
 Author: Josh Hedtke
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

