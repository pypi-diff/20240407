# Comparing `tmp/holboxai-0.7.tar.gz` & `tmp/holboxai-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holboxai-0.7.tar", last modified: Wed Apr  3 11:38:32 2024, max compression
+gzip compressed data, was "holboxai-0.8.tar", last modified: Sun Apr  7 17:18:12 2024, max compression
```

## Comparing `holboxai-0.7.tar` & `holboxai-0.8.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:38:32.925701 holboxai-0.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2024-04-03 11:38:32.925701 holboxai-0.7/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-03 11:38:32.925701 holboxai-0.7/holboxai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      430 2024-04-03 08:13:44.640509 holboxai-0.7/holboxai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3417 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/csv_query.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4294 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/docs_query.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/relevant_docs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1875 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/s3_reader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3462 2024-04-03 08:13:44.640509 holboxai-0.7/holboxai/sentiment_analysis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2024-04-02 11:16:14.723187 holboxai-0.7/holboxai/test1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3414 2024-04-03 09:38:52.606504 holboxai-0.7/holboxai/text2image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-03-13 17:29:34.327798 holboxai-0.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2076 2024-04-03 11:38:07.729687 holboxai-0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-07 17:18:12.341013 holboxai-0.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2024-04-07 17:18:12.341013 holboxai-0.8/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-07 17:18:12.341013 holboxai-0.8/holboxai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      499 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3417 2024-04-02 11:16:14.723187 holboxai-0.8/holboxai/csv_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4294 2024-04-02 11:16:14.723187 holboxai-0.8/holboxai/docs_query.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7447 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/name_entity_recognition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-04-02 11:16:14.723187 holboxai-0.8/holboxai/relevant_docs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/s3_reader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6780 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/sentiment_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/summarizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3018 2024-04-07 16:33:52.059765 holboxai-0.8/holboxai/test1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3414 2024-04-03 09:38:52.606504 holboxai-0.8/holboxai/text2image.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2024-04-07 17:15:31.380946 holboxai-0.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2185 2024-04-07 17:18:06.777011 holboxai-0.8/setup.py
```

### Comparing `holboxai-0.7/PKG-INFO` & `holboxai-0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: holboxai
-Version: 0.7
+Version: 0.8
 Summary: HolboxAI package
 Home-page: https://github.com/springtownAdmin/holboxai
 Author: Sahil Khatri
 Author-email: sahil.khatri@holbox.ai
 License: MIT
-Download-URL: https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_08.tar.gz
-Description: Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries.
+Download-URL: https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_09.tar.gz
+Description: Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries. This README provides a detailed guide on how to install and use the various features of HolboxAI.
 Keywords: GenAI,Custom,holbox
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `holboxai-0.7/holboxai/csv_query.py` & `holboxai-0.8/holboxai/csv_query.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.7/holboxai/docs_query.py` & `holboxai-0.8/holboxai/docs_query.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.7/holboxai/relevant_docs.py` & `holboxai-0.8/holboxai/relevant_docs.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.7/holboxai/s3_reader.py` & `holboxai-0.8/holboxai/s3_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import boto3
 from langchain_community.document_loaders import S3DirectoryLoader
-
+from langchain_community.document_loaders import S3FileLoader
 class S3DocReader:
     """
     A class for reading documents from an S3 bucket using the S3DirectoryLoader.
 
     This class initializes a boto3 session to interact with AWS S3 services and provides
     a method to retrieve documents from a specified S3 bucket.
 
@@ -20,15 +20,15 @@
         try:
             # Initialize a boto3 session to interact with AWS services
             session = boto3.Session()
         except Exception as e:
             # Print the exception if the session initialization fails
             print(e)
     
-    def get_bucket(self, bucket_name: str):
+    def get_docs(self, bucket_name: str):
         """
         Retrieves documents from the specified S3 bucket.
 
         Args:
             bucket_name (str): The name of the S3 bucket from which to retrieve documents.
 
         Returns:
@@ -41,14 +41,23 @@
             docs = loader.load()
             return docs
         except Exception as e:
             # Return the exception if an error occurs during document retrieval
             print(e)
             return e
         
+    
+    def get_file(self,bucket_name,file_name):
+        try:
+            loader = S3FileLoader(bucket_name ,file_name)
+            doc_file = loader.load()
+            return doc_file
+    
+        except Exception as e :
+            return e
```

### Comparing `holboxai-0.7/holboxai/text2image.py` & `holboxai-0.8/holboxai/text2image.py`

 * *Files identical despite different names*

### Comparing `holboxai-0.7/setup.py` & `holboxai-0.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from distutils.core import setup
+
+def read_requirements():
+    with open('requirements.txt') as req:
+        return req.read().splitlines()
+      
+with open('README.md') as f:
+    readme = f.read()
+
 setup(
   name = 'holboxai',         # How you named your package folder (MyLib)
   packages = ['holboxai'],   # Chose the same as "name"
-  version = '0.7',      # Start with a small number and increase it with every change you make
+  version = '0.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'HolboxAI package',   # Give a short description about your library
-  long_description = 'Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries.',
+  long_description="Welcome to HolboxAI, a comprehensive AI package designed to enhance your data processing and creative capabilities. HolboxAI offers a range of functionalities including text-to-image generation, running textual queries on documents stored in your S3 bucket, and generating insights from natural language queries. This README provides a detailed guide on how to install and use the various features of HolboxAI.",
+  long_description_content_type='text/markdown',
   author = 'Sahil Khatri',                   # Type in your name
   author_email = 'sahil.khatri@holbox.ai',      # Type in your E-Mail
   url = 'https://github.com/springtownAdmin/holboxai',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_08.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/springtownAdmin/holboxai/archive/refs/tags/v_09.tar.gz',    # I explain this later on
   keywords = ['GenAI', 'Custom', 'holbox'],   # Keywords that define your package best
-  install_requires=[          
-          'diffusers',
-          'flask',
-          'boto3',
-          'langchain',
-          'langchain_community',
-          'unstructured[pdf]',
-          'unstructured[docx]',
-          'pandasai',
-      ],
+  install_requires=read_requirements(),
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.8',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.9',
```

