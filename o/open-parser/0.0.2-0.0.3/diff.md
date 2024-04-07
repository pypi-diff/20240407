# Comparing `tmp/open_parser-0.0.2.tar.gz` & `tmp/open_parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_parser-0.0.2.tar", max compression
+gzip compressed data, was "open_parser-0.0.3.tar", max compression
```

## Comparing `open_parser-0.0.2.tar` & `open_parser-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-14 16:22:06.153815 open_parser-0.0.2/README.md
--rw-r--r--   0        0        0       89 2024-04-03 07:26:52.527095 open_parser-0.0.2/open_parser/__init__.py
--rw-r--r--   0        0        0     3267 2024-04-03 06:56:01.777124 open_parser-0.0.2/open_parser/base.py
--rw-r--r--   0        0        0      394 2024-04-03 07:26:48.860556 open_parser-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 open_parser-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1419 2024-04-06 00:51:24.943032 open_parser-0.0.3/README.md
+-rw-r--r--   0        0        0       89 2024-04-07 02:41:57.793424 open_parser-0.0.3/open_parser/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-07 02:39:17.470054 open_parser-0.0.3/open_parser/base.py
+-rw-r--r--   0        0        0      394 2024-04-07 02:41:57.794218 open_parser-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 open_parser-0.0.3/PKG-INFO
```

### Comparing `open_parser-0.0.2/open_parser/base.py` & `open_parser-0.0.3/open_parser/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         self._request_header = {"x-api-key": apiKey}
 
     def extract(self, file_path):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path)
         result = self._request_file_extraction(user_id, job_id, s3_key)
         return result["file_content"]
 
-    def parse(self, file_path, prompt):
+    def parse(self, file_path, prompt, mode="advanced"):
         user_id, job_id, s3_key = self._request_and_upload_by_apiKey(file_path, prompt)
-        result = self._request_info_extraction(user_id, job_id, s3_key)
+        result = self._request_info_extraction(user_id, job_id, s3_key, mode)
         return result["results"]
 
     def _error_handler(self, response):
         if response.status_code == 403:
             raise Exception("Invalid API Key")
         elif response.status_code == 429:
             raise Exception("API Key limit exceeded")
@@ -73,19 +73,22 @@
 
         if response.status_code == 200:
             print("Extraction success.")
             return json.loads(response.json()["result"])
 
         self._error_handler(response)
 
-    def _request_info_extraction(self, user_id, job_id, s3_key):
+    def _request_info_extraction(self, user_id, job_id, s3_key, mode):
+        if mode not in ["advanced", "basic"]:
+            raise ValueError("Invalid mode. Choose either 'advanced' or 'basic'.")
         payload = {
             "userId": user_id,
             "jobId": job_id,
             "fileKey": s3_key,
+            "extract": True if mode == "advanced" else False,
         }
         response = requests.post(
             self._parseurl, headers=self._request_header, json=payload
         )
 
         if response.status_code == 200:
             print("Extraction success.")
```

