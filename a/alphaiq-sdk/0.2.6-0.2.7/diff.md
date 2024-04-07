# Comparing `tmp/alphaiq-sdk-0.2.6.tar.gz` & `tmp/alphaiq-sdk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaiq-sdk-0.2.6.tar", last modified: Fri Mar 29 00:05:45 2024, max compression
+gzip compressed data, was "alphaiq-sdk-0.2.7.tar", last modified: Sun Apr  7 21:52:30 2024, max compression
```

## Comparing `alphaiq-sdk-0.2.6.tar` & `alphaiq-sdk-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 00:05:45.647444 alphaiq-sdk-0.2.6/
--rw-rw-rw-   0        0        0     7865 2024-03-29 00:05:45.646062 alphaiq-sdk-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     7293 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 00:05:45.603301 alphaiq-sdk-0.2.6/alphaiq_sdk/
--rw-rw-rw-   0        0        0       37 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/__init__.py
--rw-rw-rw-   0        0        0      520 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/client.py
--rw-rw-rw-   0        0        0     1606 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/generative.py
--rw-rw-rw-   0        0        0     2362 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/mapping.py
--rw-rw-rw-   0        0        0     1595 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/models.py
--rw-rw-rw-   0        0        0     1840 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/alphaiq_sdk/signals.py
-drwxrwxrwx   0        0        0        0 2024-03-29 00:05:45.645838 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/
--rw-rw-rw-   0        0        0     7865 2024-03-29 00:05:45.000000 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-03-29 00:05:45.000000 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 00:05:45.000000 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-03-29 00:05:45.000000 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-29 00:05:45.000000 alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      735 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 00:05:45.648466 alphaiq-sdk-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 00:05:45.643581 alphaiq-sdk-0.2.6/test/
--rw-rw-rw-   0        0        0     1314 2024-03-28 21:26:59.000000 alphaiq-sdk-0.2.6/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.962014 alphaiq-sdk-0.2.7/
+-rw-rw-rw-   0        0        0     7865 2024-04-07 21:52:30.961016 alphaiq-sdk-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7293 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.944016 alphaiq-sdk-0.2.7/alphaiq_sdk/
+-rw-rw-rw-   0        0        0       37 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/__init__.py
+-rw-rw-rw-   0        0        0      520 2024-04-04 16:33:26.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/client.py
+-rw-rw-rw-   0        0        0     1578 2024-04-07 21:50:10.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/generative.py
+-rw-rw-rw-   0        0        0     2538 2024-04-07 21:50:10.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/mapping.py
+-rw-rw-rw-   0        0        0     1595 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/models.py
+-rw-rw-rw-   0        0        0     1840 2024-03-28 23:57:31.000000 alphaiq-sdk-0.2.7/alphaiq_sdk/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.961016 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/
+-rw-rw-rw-   0        0        0     7865 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 21:52:30.000000 alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      735 2024-04-07 21:52:07.000000 alphaiq-sdk-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 21:52:30.963014 alphaiq-sdk-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 21:52:30.960018 alphaiq-sdk-0.2.7/test/
+-rw-rw-rw-   0        0        0     2025 2024-04-04 15:51:38.000000 alphaiq-sdk-0.2.7/test/test.py
```

### Comparing `alphaiq-sdk-0.2.6/PKG-INFO` & `alphaiq-sdk-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphaiq-sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Access AlphaIQ quantitative linguistics signals and generative content
 Author-email: AlphaIQ <contact@alphaiq.ai>
 Project-URL: GitHub, https://github.com/alphaiq-ai/python-sdk
 Keywords: risk,AI,fintech,investing,NLP,GenAI
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `alphaiq-sdk-0.2.6/README.md` & `alphaiq-sdk-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk/client.py` & `alphaiq-sdk-0.2.7/alphaiq_sdk/client.py`

 * *Files identical despite different names*

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk/generative.py` & `alphaiq-sdk-0.2.7/alphaiq_sdk/generative.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         url = self.host_url + f"/generative/company/spinsights/reportContent/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response 
 
     def get_spinsights_report_pdf(self, ticker: str):
 
-        url = self.host_url + f"/company/spinsights/reportPDF/{ticker}"
+        url = self.host_url + f"/pdf/spinsights/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response 
 
     def get_compass_explorer_question_answer(self, ticker: str):
 
         url = self.host_url + f"/generative/company/compass/questionContent/{ticker}"
@@ -38,12 +38,12 @@
         url = self.host_url + f"/generative/company/compass/reportContent/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response 
     
     def get_compass_report_pdf(self, ticker: str):
 
-        url = self.host_url + f"/company/compass/reportPDF/{ticker}"
+        url = self.host_url + f"/pdf/compass/{ticker}"
 
         response = requests.get(url, headers=self.headers).json()
         return response
```

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk/mapping.py` & `alphaiq-sdk-0.2.7/alphaiq_sdk/mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,18 @@
         optional_args = {
             'consilienceId': kwargs.get('consilienceId', None),
             'ticker': kwargs.get('ticker', None),
             'cik': kwargs.get('cik', None),
             'lei': kwargs.get('lei', None),
             'isin': kwargs.get('isin', None),
             'cusip': kwargs.get('cusip', None),
-            'sedol': kwargs.get('sedol', None)
+            'sedol': kwargs.get('sedol', None),
+            'figi': kwargs.get('figi',None),
+            'compositeFigi': kwargs.get('compositeFigi',None),
+            'shareClassFigi': kwargs.get('shareClassFigi',None)
         }
 
         # Checking if at least one optional argument is present
         if not any(optional_args.values()):
             raise ValueError("One and only one company identifier argument must be provided.")
 
         url = self.host_url + "/mapping/companyIdentifierMapping?"
```

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk/models.py` & `alphaiq-sdk-0.2.7/alphaiq_sdk/models.py`

 * *Files identical despite different names*

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk/signals.py` & `alphaiq-sdk-0.2.7/alphaiq_sdk/signals.py`

 * *Files identical despite different names*

### Comparing `alphaiq-sdk-0.2.6/alphaiq_sdk.egg-info/PKG-INFO` & `alphaiq-sdk-0.2.7/alphaiq_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphaiq-sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Access AlphaIQ quantitative linguistics signals and generative content
 Author-email: AlphaIQ <contact@alphaiq.ai>
 Project-URL: GitHub, https://github.com/alphaiq-ai/python-sdk
 Keywords: risk,AI,fintech,investing,NLP,GenAI
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `alphaiq-sdk-0.2.6/pyproject.toml` & `alphaiq-sdk-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphaiq-sdk"
-version = "0.2.6"
+version = "0.2.7"
 description = "Access AlphaIQ quantitative linguistics signals and generative content"
 readme = "README.md"
 authors = [{ name = "AlphaIQ", email = "contact@alphaiq.ai" }]
 
 classifiers = [
     "Programming Language :: Python",
 ]
```

### Comparing `alphaiq-sdk-0.2.6/test/test.py` & `alphaiq-sdk-0.2.7/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import example_functions as aiq
 import csv
+import uuid
+from datetime import date
 
 def to_csv(output_checks):
-    with open('output_checks.csv', mode='w', newline='', encoding='utf-8') as file:
-        fieldnames = ['output', 'outcome']
+    today_date = date.today()
+    random_string = str(uuid.uuid4().hex)[:8]  # You can adjust the length as needed
+    filename = f'output_checks_{today_date}_{random_string}.csv'
+    with open(filename, mode='w', newline='', encoding='utf-8') as file:
+        fieldnames = ['function','output', 'outcome']
         writer = csv.DictWriter(file, fieldnames=fieldnames)
 
         writer.writeheader()
         for check in output_checks:
             writer.writerow(check)
 
 function_list = [
     aiq.get_quant_linguistics_signals(),
     aiq.get_bulk_signals(),
     aiq.get_bulk_signals_yearly(),
     aiq.get_models_spindex(),
     aiq.get_bulk_model(),
-    aiq.get_company_identifiers_map(),
+    aiq.get_company_identifiers_map_compositeFigi(),
+    aiq.get_company_identifiers_map_cik(),
+    aiq.get_company_identifiers_map_consilienceId(),
+    aiq.get_company_identifiers_map_cusip(),
+    aiq.get_company_identifiers_map_figi(),
+    aiq.get_company_identifiers_map_isin(),
+    aiq.get_company_identifiers_map_lei(),
+    aiq.get_company_identifiers_map_shareClassFigi(),
+    aiq.get_company_identifiers_map_ticker(),
     aiq.get_spindex_factors_map(),
     aiq.get_bulk_mapping(),
     aiq.get_compass_questions_map(),
     aiq.get_spinsights_explorer_spindex_summary(),
     aiq.get_spinsights_report_content(),
     aiq.get_spinsights_report_pdf(),
     aiq.get_compass_explorer_question_answer(),
@@ -29,16 +42,18 @@
 ]
 
 output_checks= []
 i=0
 for function in function_list:
     i+=1
     print(f'Trying function --> {i}')
-    if "data" in function:
+    if "message" in function[0]:
+        outcome = 'Fail'
+    elif "data" in function[0]:
         outcome = 'Pass'
-    elif "errors" in function:
+    elif "errors" in function[0]:
         outcome = 'Fail'
-    output_checks.append({'output':function, 'outcome': outcome})
+    output_checks.append({'function':function[1],'output':function[0], 'outcome': outcome})
 
 # print(f'Result of tests: {output_checks}')
 
 to_csv(output_checks)
```

