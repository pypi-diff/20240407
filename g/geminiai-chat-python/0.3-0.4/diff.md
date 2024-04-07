# Comparing `tmp/geminiai-chat-python-0.3.tar.gz` & `tmp/geminiai-chat-python-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geminiai-chat-python-0.3.tar", last modified: Thu Mar 28 12:02:47 2024, max compression
+gzip compressed data, was "geminiai-chat-python-0.4.tar", last modified: Sun Apr  7 02:52:47 2024, max compression
```

## Comparing `geminiai-chat-python-0.3.tar` & `geminiai-chat-python-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-03-28 12:02:47.192444 geminiai-chat-python-0.3/
-drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-03-28 12:02:47.181177 geminiai-chat-python-0.3/GeminiAIChat/
--rwxrwxrwx   0 momin     (1000) momin     (1000)      146 2024-03-28 00:43:02.000000 geminiai-chat-python-0.3/GeminiAIChat/.env
--rwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-03-26 00:37:57.000000 geminiai-chat-python-0.3/GeminiAIChat/__init__.py
--rwxrwxrwx   0 momin     (1000) momin     (1000)      533 2024-03-28 11:14:09.000000 geminiai-chat-python-0.3/GeminiAIChat/core.py
--rwxrwxrwx   0 momin     (1000) momin     (1000)     1296 2024-03-28 11:30:48.000000 geminiai-chat-python-0.3/GeminiAIChat/process.py
--rwxrwxrwx   0 momin     (1000) momin     (1000)     1618 2024-03-28 12:02:47.191781 geminiai-chat-python-0.3/PKG-INFO
--rwxrwxrwx   0 momin     (1000) momin     (1000)     1121 2024-03-28 11:51:06.000000 geminiai-chat-python-0.3/README.md
-drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-03-28 12:02:47.190352 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/
--rwxrwxrwx   0 momin     (1000) momin     (1000)     1618 2024-03-28 12:02:47.000000 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/PKG-INFO
--rwxrwxrwx   0 momin     (1000) momin     (1000)      325 2024-03-28 12:02:47.000000 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/SOURCES.txt
--rwxrwxrwx   0 momin     (1000) momin     (1000)        1 2024-03-28 12:02:47.000000 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/dependency_links.txt
--rwxrwxrwx   0 momin     (1000) momin     (1000)       20 2024-03-28 12:02:47.000000 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/requires.txt
--rwxrwxrwx   0 momin     (1000) momin     (1000)       13 2024-03-28 12:02:47.000000 geminiai-chat-python-0.3/geminiai_chat_python.egg-info/top_level.txt
--rwxrwxrwx   0 momin     (1000) momin     (1000)       38 2024-03-28 12:02:47.192744 geminiai-chat-python-0.3/setup.cfg
--rwxrwxrwx   0 momin     (1000) momin     (1000)     1903 2024-03-28 11:28:07.000000 geminiai-chat-python-0.3/setup.py
+drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-04-07 02:52:47.761776 geminiai-chat-python-0.4/
+drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-04-07 02:52:47.736314 geminiai-chat-python-0.4/GeminiAIChat/
+-rwxrwxrwx   0 momin     (1000) momin     (1000)      146 2024-03-28 00:43:02.000000 geminiai-chat-python-0.4/GeminiAIChat/.env
+-rwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-03-26 00:37:57.000000 geminiai-chat-python-0.4/GeminiAIChat/__init__.py
+-rwxrwxrwx   0 momin     (1000) momin     (1000)      527 2024-04-07 02:47:57.000000 geminiai-chat-python-0.4/GeminiAIChat/core.py
+-rwxrwxrwx   0 momin     (1000) momin     (1000)     1296 2024-03-28 11:30:48.000000 geminiai-chat-python-0.4/GeminiAIChat/process.py
+-rwxrwxrwx   0 momin     (1000) momin     (1000)     1946 2024-04-07 02:52:47.760940 geminiai-chat-python-0.4/PKG-INFO
+-rwxrwxrwx   0 momin     (1000) momin     (1000)     1121 2024-03-28 11:51:06.000000 geminiai-chat-python-0.4/README.md
+drwxrwxrwx   0 momin     (1000) momin     (1000)        0 2024-04-07 02:52:47.759128 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/
+-rwxrwxrwx   0 momin     (1000) momin     (1000)     1946 2024-04-07 02:52:47.000000 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/PKG-INFO
+-rwxrwxrwx   0 momin     (1000) momin     (1000)      325 2024-04-07 02:52:47.000000 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/SOURCES.txt
+-rwxrwxrwx   0 momin     (1000) momin     (1000)        1 2024-04-07 02:52:47.000000 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/dependency_links.txt
+-rwxrwxrwx   0 momin     (1000) momin     (1000)       51 2024-04-07 02:52:47.000000 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/requires.txt
+-rwxrwxrwx   0 momin     (1000) momin     (1000)       13 2024-04-07 02:52:47.000000 geminiai-chat-python-0.4/geminiai_chat_python.egg-info/top_level.txt
+-rwxrwxrwx   0 momin     (1000) momin     (1000)       38 2024-04-07 02:52:47.762094 geminiai-chat-python-0.4/setup.cfg
+-rwxrwxrwx   0 momin     (1000) momin     (1000)     2264 2024-04-07 02:51:51.000000 geminiai-chat-python-0.4/setup.py
```

### Comparing `geminiai-chat-python-0.3/GeminiAIChat/core.py` & `geminiai-chat-python-0.4/GeminiAIChat/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,12 +6,12 @@
             raise ValueError("read doc get free api key \n  -> https://github.com/MominIqbal-1234/geminiai-chat-python")
         self.api = api
         self.getRes = GET(self.api)
 
     def prompt(self,prompt):
         self.getRes.sendResponse(prompt)
         
-    def response(self):
+    def response_(self):
         return self.getRes.retrieveShortResponse()
 
-    def detailsResponse(self):
+    def response(self):
         return self.getRes.retrieveDetailResponse()
```

### Comparing `geminiai-chat-python-0.3/GeminiAIChat/process.py` & `geminiai-chat-python-0.4/GeminiAIChat/process.py`

 * *Files identical despite different names*

### Comparing `geminiai-chat-python-0.3/PKG-INFO` & `geminiai-chat-python-0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-Metadata-Version: 2.1
-Name: geminiai-chat-python
-Version: 0.3
-Summary: GeminiAI-Chat enables easy integration of AI Chat functionalities into Python projects.
-Home-page: UNKNOWN
-Author: mominiqbal1234
-Author-email: <mominiqbal1214@gmail.com>
-License: UNKNOWN
-Keywords: geminiai-chat-python,python,geminiai-chat,geminiai
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
+from setuptools import setup, find_packages
 
 
+
+VERSION = '0.4'
+DESCRIPTION = "GeminiAI-Chat enables easy integration of AI Chat functionalities into Python projects."
+
+
+# Setting up
+setup(
+    name="geminiai-chat-python",
+    version=VERSION,
+    author="mominiqbal1234",
+    author_email="<mominiqbal1214@gmail.com>",
+    description=DESCRIPTION,
+    long_description="""
     
+### Downloads geminiai-chat-python
+[![Downloads](https://static.pepy.tech/badge/geminiai-chat-python)](https://pepy.tech/project/geminiai-chat-python)
+
 ![image](https://github.com/MominIqbal-1234/geminiai-chat-python/assets/61788052/15e838f4-d6ff-41da-b2b1-366c72c30107)
 
 GeminiAI-Chat – the revolutionary Python library designed to power up your applications with advanced conversational AI capabilities
 GeminiAI-Chat, developers can effortlessly integrate AI-driven chat functionalities into their projects,
 # How to install geminiai-chat
 
 ```python
-pip install geminiai-chat-python
+pip install geminiai-chat-python --upgrade
 ```
 # Documentation
 GeminiAI-Chat offers a seamless way to incorporate intelligent, responsive AI chat features
 ```python
 from GeminiAIChat.core import API
 
 
-res = API("your_api_key")
-res.prompt("what is python programing language")
+res = API("your_api_key") # https://aistudio.google.com/app/apikey
+res.prompt("what is python")
 print(res.response())
-print(res.detailsResponse())
 
 ```
+## Get API KEY
+https://aistudio.google.com/app/apikey
+![image](https://github.com/MominIqbal-1234/geminiai-chat-python/assets/61788052/6b573d4a-5d3d-4370-96dc-eca0d327292f)
 
 
 
 # Issues
 https://github.com/MominIqbal-1234/geminiai-chat-python/issues
 
 
@@ -51,9 +53,24 @@
 
 
 
 Check Our Site : https://mefiz.com/about </br>
 Developed by : Momin Iqbal
 
 
-    
 
+    """,
+    long_description_content_type="text/markdown",
+    packages=find_packages(),
+    include_package_data=True,
+    package_data={'': ['.env']},
+    install_requires=["httpx","google-generativeai","google-api-python-client"],
+    keywords=['geminiai-chat-python','python', 'geminiai-chat', 'geminiai'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

### Comparing `geminiai-chat-python-0.3/README.md` & `geminiai-chat-python-0.4/README.md`

 * *Files identical despite different names*

