# Comparing `tmp/webscout-1.2.5.tar.gz` & `tmp/webscout-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.5.tar", last modified: Wed Apr  3 11:23:06 2024, max compression
+gzip compressed data, was "webscout-1.2.6.tar", last modified: Sun Apr  7 08:19:59 2024, max compression
```

## Comparing `webscout-1.2.5.tar` & `webscout-1.2.6.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.843877 webscout-1.2.5/
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.392882 webscout-1.2.5/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.439873 webscout-1.2.5/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.484888 webscout-1.2.5/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.521883 webscout-1.2.5/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.5/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.5/LICENSE.md
--rw-rw-rw-   0        0        0    22262 2024-04-03 11:23:06.834878 webscout-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    20120 2024-04-03 11:20:24.000000 webscout-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 11:23:06.844883 webscout-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2757 2024-04-03 11:21:10.000000 webscout-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.726903 webscout-1.2.5/webscout/
--rw-rw-rw-   0        0        0    57984 2024-04-03 10:46:54.000000 webscout-1.2.5/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.5/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/LLM.py
--rw-rw-rw-   0        0        0      507 2024-04-03 10:48:19.000000 webscout-1.2.5/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.5/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/models.py
--rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-03 11:19:15.000000 webscout-1.2.5/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.5/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-03 11:23:06.818894 webscout-1.2.5/webscout.egg-info/
--rw-rw-rw-   0        0        0    22262 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2024-04-03 11:23:05.000000 webscout-1.2.5/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 11:23:04.000000 webscout-1.2.5/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:59.081478 webscout-1.2.6/
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:57.976422 webscout-1.2.6/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.019423 webscout-1.2.6/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.231903 webscout-1.2.6/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.303830 webscout-1.2.6/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.6/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0    24247 2024-04-07 08:19:59.063517 webscout-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    22072 2024-04-07 08:14:49.000000 webscout-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 08:19:59.082479 webscout-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2790 2024-04-07 06:24:18.000000 webscout-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:58.966784 webscout-1.2.6/webscout/
+-rw-rw-rw-   0        0        0    57985 2024-04-06 15:11:56.000000 webscout-1.2.6/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.6/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/LLM.py
+-rw-rw-rw-   0        0        0      547 2024-04-07 06:11:57.000000 webscout-1.2.6/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.6/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/models.py
+-rw-rw-rw-   0        0        0    20232 2024-04-07 08:02:09.000000 webscout-1.2.6/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-07 07:49:31.000000 webscout-1.2.6/webscout/version.py
+-rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.6/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:19:59.056465 webscout-1.2.6/webscout.egg-info/
+-rw-rw-rw-   0        0        0    24247 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      965 2024-04-07 08:19:57.000000 webscout-1.2.6/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 08:19:56.000000 webscout-1.2.6/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.5/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.2.6/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.2.6/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/networks/filepath_converter.py` & `webscout-1.2.6/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/networks/google_searcher.py` & `webscout-1.2.6/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/networks/network_configs.py` & `webscout-1.2.6/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.2.6/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/utilsdw/enver.py` & `webscout-1.2.6/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/DeepWEBS/utilsdw/logger.py` & `webscout-1.2.6/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/LICENSE.md` & `webscout-1.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/PKG-INFO` & `webscout-1.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.5
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Version: 1.2.6
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -52,26 +52,26 @@
 
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Also containes AI models that you can use
+Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
+  - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
@@ -214,15 +214,63 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 
+## Transcriber
+The transcriber function in webscout is a handy tool that transcribes YouTube videos. Here's an example code demonstrating its usage:
+```python
+import sys
+from webscout import transcriber
+
+def extract_transcript(video_id):
+    """Extracts the transcript from a YouTube video."""
+    try:
+        transcript_list = transcriber.list_transcripts(video_id)
+        for transcript in transcript_list:
+            transcript_text_list = transcript.fetch()
+            lang = transcript.language
+            transcript_text = ""
+            if transcript.language_code == 'en':
+                for line in transcript_text_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+            elif transcript.is_translatable:
+                english_transcript_list = transcript.translate('en').fetch()
+                for line in english_transcript_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+        print("Transcript extraction failed. Please check the video URL.")
+    except Exception as e:
+        print(f"Error: {e}")
+
+def main():
+    video_url = input("Enter the video link: ")
+
+    if video_url:
+        video_id = video_url.split("=")[1]
+        print("Video URL:", video_url)
+        submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '':
+            print("Extracting Transcript...")
+            transcript = extract_transcript(video_id)
+            print('Transcript:')
+            print(transcript)
+            print("__________________________________________________________________________________")
+        elif submit.lower() == 'exit':
+            print("Exiting...")
+            sys.exit()
+        else:
+            print("Invalid input. Please try again.")
 
+if __name__ == "__main__":
+    main()
+```
 ## DeepWEBS: Advanced Web Searches
 
 `DeepWEBS` is a standalone feature designed to perform advanced web searches with enhanced capabilities. It is particularly powerful in extracting relevant information directly from webpages and Search engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which provides a broader range of search functionalities, `DeepWEBS` is specifically tailored for in-depth web searches.
 
 ### Activating DeepWEBS
 
 To utilize the `DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This is designed to be used independently of the `WEBS` , offering a focused approach to web searches.
```

#### html2text {}

```diff
@@ -1,96 +1,97 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.5 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.6 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
-"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
+now can transcribe yt videos Author: OEvortex Author-email:
+helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
+URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
+Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
+github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
+youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Description-Content-Type: text/
+markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
+lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
+Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
+Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
+Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
+Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
+Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
+# webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models Also containes AI models that you can use
- ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
+you.com, etc Also containes AI models and now can transcribe yt videos ## Table
+of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
+      [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-[Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
- Example](#usage-example) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
+Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
+  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
+before-using-deepwebs) - [Usage Example](#usage-example) - [WEBS and AsyncWEBS
+ classes](#webs-and-asyncwebs-classes) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+ yepcom) - [usage of webscout.AI](#usage-of-webscoutai) - [1. `PhindSearch` -
+Search using Phind.com](#1-phindsearch---search-using-phindcom) - [2. `YepChat`
+ - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-
+ 8x7b-powered-by-yepchat) - [3. `You.com` - search with you.com](#3-youcom---
+ search-with-youcom) - [4. `Gemini` - search with google gemini](#4-gemini---
+   search-with-google-gemini) - [usage of image generator from Webscout.AI]
+ (#usage-of-image-generator-from-webscoutai) - [5. `Prodia` - make image using
+  prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat
+  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
+Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
+ - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-
+koboldia--) - [usage of special .LLM file from webscout (webscout.LLM)](#usage-
+   of-special-llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -110,26 +111,46 @@
  Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
  for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
 Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
   for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
  Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-  To TOP](#TOP) ## DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone
- feature designed to perform advanced web searches with enhanced capabilities.
- It is particularly powerful in extracting relevant information directly from
-webpages and Search engine, focusing exclusively on text (web) searches. Unlike
-    the `WEBS` , which provides a broader range of search functionalities,
- `DeepWEBS` is specifically tailored for in-depth web searches. ### Activating
- DeepWEBS To utilize the `DeepWEBS` feature, you must first create an instance
- of the `DeepWEBS` . This is designed to be used independently of the `WEBS` ,
-offering a focused approach to web searches. ### Point to remember before using
- `DeepWEBS` As `DeepWEBS` is designed to extract relevant information directly
-from webpages and Search engine, It extracts html from webpages and saves them
-         to folder named files in `DeepWEBS` that can be found at `C:
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+for line in transcript_text_list: transcript_text += " " + line["text"] return
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+transcript_text += " " + line["text"] return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
+("__________________________________________________________________________________")
+   elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
+ ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
+DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
+ perform advanced web searches with enhanced capabilities. It is particularly
+ powerful in extracting relevant information directly from webpages and Search
+engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
+provides a broader range of search functionalities, `DeepWEBS` is specifically
+  tailored for in-depth web searches. ### Activating DeepWEBS To utilize the
+`DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This
+    is designed to be used independently of the `WEBS` , offering a focused
+  approach to web searches. ### Point to remember before using `DeepWEBS` As
+ `DeepWEBS` is designed to extract relevant information directly from webpages
+  and Search engine, It extracts html from webpages and saves them to folder
+              named files in `DeepWEBS` that can be found at `C:
 \Users\Username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-
   packages\Python311\site-packages\DeepWEBS` ### Usage Example Here's a basic
 example of how to use the `DeepWEBS` : ```python from webscout import DeepWEBS
 def perform_web_search(query): # Initialize the DeepWEBS class D = DeepWEBS() #
  Set up the search parameters search_params = D.DeepSearch( queries=[query], #
  Query to search result_num=5, # Number of search results safe=True, # Enable
  SafeSearch types=["web"], # Search type: web extract_webpage=True, # True for
```

### Comparing `webscout-1.2.5/README.md` & `webscout-1.2.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Also containes AI models that you can use
+Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
+  - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
@@ -162,15 +162,63 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 
+## Transcriber
+The transcriber function in webscout is a handy tool that transcribes YouTube videos. Here's an example code demonstrating its usage:
+```python
+import sys
+from webscout import transcriber
+
+def extract_transcript(video_id):
+    """Extracts the transcript from a YouTube video."""
+    try:
+        transcript_list = transcriber.list_transcripts(video_id)
+        for transcript in transcript_list:
+            transcript_text_list = transcript.fetch()
+            lang = transcript.language
+            transcript_text = ""
+            if transcript.language_code == 'en':
+                for line in transcript_text_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+            elif transcript.is_translatable:
+                english_transcript_list = transcript.translate('en').fetch()
+                for line in english_transcript_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+        print("Transcript extraction failed. Please check the video URL.")
+    except Exception as e:
+        print(f"Error: {e}")
+
+def main():
+    video_url = input("Enter the video link: ")
+
+    if video_url:
+        video_id = video_url.split("=")[1]
+        print("Video URL:", video_url)
+        submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '':
+            print("Extracting Transcript...")
+            transcript = extract_transcript(video_id)
+            print('Transcript:')
+            print(transcript)
+            print("__________________________________________________________________________________")
+        elif submit.lower() == 'exit':
+            print("Exiting...")
+            sys.exit()
+        else:
+            print("Invalid input. Please try again.")
 
+if __name__ == "__main__":
+    main()
+```
 ## DeepWEBS: Advanced Web Searches
 
 `DeepWEBS` is a standalone feature designed to perform advanced web searches with enhanced capabilities. It is particularly powerful in extracting relevant information directly from webpages and Search engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which provides a broader range of search functionalities, `DeepWEBS` is specifically tailored for in-depth web searches.
 
 ### Activating DeepWEBS
 
 To utilize the `DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This is designed to be used independently of the `WEBS` , offering a focused approach to web searches.
```

#### html2text {}

```diff
@@ -1,69 +1,69 @@
 # webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models Also containes AI models that you can use
- ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
+you.com, etc Also containes AI models and now can transcribe yt videos ## Table
+of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
+      [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-[Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
- Example](#usage-example) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
+Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
+  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
+before-using-deepwebs) - [Usage Example](#usage-example) - [WEBS and AsyncWEBS
+ classes](#webs-and-asyncwebs-classes) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+ yepcom) - [usage of webscout.AI](#usage-of-webscoutai) - [1. `PhindSearch` -
+Search using Phind.com](#1-phindsearch---search-using-phindcom) - [2. `YepChat`
+ - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-
+ 8x7b-powered-by-yepchat) - [3. `You.com` - search with you.com](#3-youcom---
+ search-with-youcom) - [4. `Gemini` - search with google gemini](#4-gemini---
+   search-with-google-gemini) - [usage of image generator from Webscout.AI]
+ (#usage-of-image-generator-from-webscoutai) - [5. `Prodia` - make image using
+  prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat
+  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
+Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
+ - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-
+koboldia--) - [usage of special .LLM file from webscout (webscout.LLM)](#usage-
+   of-special-llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -83,26 +83,46 @@
  Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
  for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
 Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
   for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
  Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-  To TOP](#TOP) ## DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone
- feature designed to perform advanced web searches with enhanced capabilities.
- It is particularly powerful in extracting relevant information directly from
-webpages and Search engine, focusing exclusively on text (web) searches. Unlike
-    the `WEBS` , which provides a broader range of search functionalities,
- `DeepWEBS` is specifically tailored for in-depth web searches. ### Activating
- DeepWEBS To utilize the `DeepWEBS` feature, you must first create an instance
- of the `DeepWEBS` . This is designed to be used independently of the `WEBS` ,
-offering a focused approach to web searches. ### Point to remember before using
- `DeepWEBS` As `DeepWEBS` is designed to extract relevant information directly
-from webpages and Search engine, It extracts html from webpages and saves them
-         to folder named files in `DeepWEBS` that can be found at `C:
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+for line in transcript_text_list: transcript_text += " " + line["text"] return
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+transcript_text += " " + line["text"] return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
+("__________________________________________________________________________________")
+   elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
+ ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
+DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
+ perform advanced web searches with enhanced capabilities. It is particularly
+ powerful in extracting relevant information directly from webpages and Search
+engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
+provides a broader range of search functionalities, `DeepWEBS` is specifically
+  tailored for in-depth web searches. ### Activating DeepWEBS To utilize the
+`DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This
+    is designed to be used independently of the `WEBS` , offering a focused
+  approach to web searches. ### Point to remember before using `DeepWEBS` As
+ `DeepWEBS` is designed to extract relevant information directly from webpages
+  and Search engine, It extracts html from webpages and saves them to folder
+              named files in `DeepWEBS` that can be found at `C:
 \Users\Username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-
   packages\Python311\site-packages\DeepWEBS` ### Usage Example Here's a basic
 example of how to use the `DeepWEBS` : ```python from webscout import DeepWEBS
 def perform_web_search(query): # Initialize the DeepWEBS class D = DeepWEBS() #
  Set up the search parameters search_params = D.DeepSearch( queries=[query], #
  Query to search result_num=5, # Number of search results safe=True, # Enable
  SafeSearch types=["web"], # Search type: web extract_webpage=True, # True for
```

### Comparing `webscout-1.2.5/setup.py` & `webscout-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.5", 
-    description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models",
+    version="1.2.6", 
+    description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `webscout-1.2.5/webscout/AI.py` & `webscout-1.2.6/webscout/AI.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from webscout.AIutel import Optimizers
 from webscout.AIutel import Conversation
 from webscout.AIutel import AwesomePrompts
 from webscout.AIbase import Provider
 from Helpingai_T2 import Perplexity
 from typing import Any
 import logging
-#------------------------------------------------------OpenGPT-----------------------------------------------------------
+#------------------------------------------------------KOBOLDAI-----------------------------------------------------------
 class KOBOLDAI(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         temperature: float = 1,
         top_p: float = 1,
```

### Comparing `webscout-1.2.5/webscout/AIbase.py` & `webscout-1.2.6/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/AIutel.py` & `webscout-1.2.6/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/DWEBS.py` & `webscout-1.2.6/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/HelpingAI.py` & `webscout-1.2.6/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/LLM.py` & `webscout-1.2.6/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/cli.py` & `webscout-1.2.6/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/models.py` & `webscout-1.2.6/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/utils.py` & `webscout-1.2.6/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/webscout_search.py` & `webscout-1.2.6/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout/webscout_search_async.py` & `webscout-1.2.6/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.5/webscout.egg-info/PKG-INFO` & `webscout-1.2.6/webscout.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.5
-Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
+Version: 1.2.6
+Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -52,26 +52,26 @@
 
 #  webscout
 <p align="center">
 
 <a href="#"><img alt="Python version" src="https://img.shields.io/pypi/pyversions/webscout"/></a>
 <a href="https://pepy.tech/project/webscout"><img alt="Downloads" src="https://static.pepy.tech/badge/webscout"></a>
 
-Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Also containes AI models that you can use
+Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 
 
 ## Table of Contents
 - [webscout](#webscout)
   - [Table of Contents](#table-of-contents)
   - [Install](#install)
   - [CLI version](#cli-version)
   - [CLI version of webscout.AI](#cli-version-of-webscoutai)
   - [CLI to use LLM](#cli-to-use-llm)
   - [Regions](#regions)
+  - [Transcriber](#transcriber)
   - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-searches)
     - [Activating DeepWEBS](#activating-deepwebs)
     - [Point to remember before using `DeepWEBS`](#point-to-remember-before-using-deepwebs)
     - [Usage Example](#usage-example)
   - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-classes)
   - [Exceptions](#exceptions)
   - [usage of webscout](#usage-of-webscout)
@@ -214,15 +214,63 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 
+## Transcriber
+The transcriber function in webscout is a handy tool that transcribes YouTube videos. Here's an example code demonstrating its usage:
+```python
+import sys
+from webscout import transcriber
+
+def extract_transcript(video_id):
+    """Extracts the transcript from a YouTube video."""
+    try:
+        transcript_list = transcriber.list_transcripts(video_id)
+        for transcript in transcript_list:
+            transcript_text_list = transcript.fetch()
+            lang = transcript.language
+            transcript_text = ""
+            if transcript.language_code == 'en':
+                for line in transcript_text_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+            elif transcript.is_translatable:
+                english_transcript_list = transcript.translate('en').fetch()
+                for line in english_transcript_list:
+                    transcript_text += " " + line["text"]
+                return transcript_text
+        print("Transcript extraction failed. Please check the video URL.")
+    except Exception as e:
+        print(f"Error: {e}")
+
+def main():
+    video_url = input("Enter the video link: ")
+
+    if video_url:
+        video_id = video_url.split("=")[1]
+        print("Video URL:", video_url)
+        submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '':
+            print("Extracting Transcript...")
+            transcript = extract_transcript(video_id)
+            print('Transcript:')
+            print(transcript)
+            print("__________________________________________________________________________________")
+        elif submit.lower() == 'exit':
+            print("Exiting...")
+            sys.exit()
+        else:
+            print("Invalid input. Please try again.")
 
+if __name__ == "__main__":
+    main()
+```
 ## DeepWEBS: Advanced Web Searches
 
 `DeepWEBS` is a standalone feature designed to perform advanced web searches with enhanced capabilities. It is particularly powerful in extracting relevant information directly from webpages and Search engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which provides a broader range of search functionalities, `DeepWEBS` is specifically tailored for in-depth web searches.
 
 ### Activating DeepWEBS
 
 To utilize the `DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This is designed to be used independently of the `WEBS` , offering a focused approach to web searches.
```

#### html2text {}

```diff
@@ -1,96 +1,97 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.5 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.6 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
-DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models
-Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
-"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" # webscout
+DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
+now can transcribe yt videos Author: OEvortex Author-email:
+helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
+URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
+Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
+github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
+youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier: Topic
+:: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Description-Content-Type: text/
+markdown License-File: LICENSE.md Requires-Dist: docstring_inheritance>=2.1.2
+Requires-Dist: click>=8.1.7 Requires-Dist: curl_cffi>=0.6.0b7 Requires-Dist:
+lxml>=5.1.0 Requires-Dist: nest-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3
+Requires-Dist: tqdm>=4.64.0 Requires-Dist: webdriver-manager>=3.5.4 Requires-
+Dist: halo>=0.0.31 Requires-Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-
+Dist: python-dotenv Requires-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify Requires-Dist: pydantic Requires-Dist: requests
+Requires-Dist: sse_starlette Requires-Dist: termcolor Requires-Dist: tiktoken
+Requires-Dist: tldextract Requires-Dist: orjson Provides-Extra: dev Requires-
+Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
+# webscout
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for words, documents, images, videos, news,
 maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com,
-you.com, etc Also containes AI models Also containes AI models that you can use
- ## Table of Contents - [webscout](#webscout) - [Table of Contents](#table-of-
-contents) - [Install](#install) - [CLI version](#cli-version) - [CLI version of
+you.com, etc Also containes AI models and now can transcribe yt videos ## Table
+of Contents - [webscout](#webscout) - [Table of Contents](#table-of-contents) -
+      [Install](#install) - [CLI version](#cli-version) - [CLI version of
 webscout.AI](#cli-version-of-webscoutai) - [CLI to use LLM](#cli-to-use-llm) -
-[Regions](#regions) - [DeepWEBS: Advanced Web Searches](#deepwebs-advanced-web-
- searches) - [Activating DeepWEBS](#activating-deepwebs) - [Point to remember
-  before using `DeepWEBS`](#point-to-remember-before-using-deepwebs) - [Usage
- Example](#usage-example) - [WEBS and AsyncWEBS classes](#webs-and-asyncwebs-
-classes) - [Exceptions](#exceptions) - [usage of webscout](#usage-of-webscout)
-  - [1. `text()` - text search by DuckDuckGo.com and Yep.com](#1-text---text-
-  search-by-duckduckgocom-and-yepcom) - [2. `answers()` - instant answers by
-DuckDuckGo.com and Yep.com](#2-answers---instant-answers-by-duckduckgocom-and-
-  yepcom) - [3. `images()` - image search by DuckDuckGo.com and Yep.com](#3-
-  images---image-search-by-duckduckgocom-and-yepcom) - [4. `videos()` - video
-  search by DuckDuckGo.com](#4-videos---video-search-by-duckduckgocom) - [5.
-`news()` - news search by DuckDuckGo.com and yep.com](#5-news---news-search-by-
- duckduckgocom-and-yepcom) - [6. `maps()` - map search by DuckDuckGo.com and]
- (#6-maps---map-search-by-duckduckgocom-and) - [7. `translate()` - translation
-by DuckDuckGo.com and Yep.com](#7-translate---translation-by-duckduckgocom-and-
-yepcom) - [8. `suggestions()` - suggestions by DuckDuckGo.com and Yep.com](#8-
-suggestions---suggestions-by-duckduckgocom-and-yepcom) - [usage of webscout.AI]
-   (#usage-of-webscoutai) - [1. `PhindSearch` - Search using Phind.com](#1-
- phindsearch---search-using-phindcom) - [2. `YepChat` - Chat with mistral 8x7b
-powered by yepchat](#2-yepchat---chat-with-mistral-8x7b-powered-by-yepchat) -
-  [3. `You.com` - search with you.com](#3-youcom---search-with-youcom) - [4.
-`Gemini` - search with google gemini](#4-gemini---search-with-google-gemini) -
-  [usage of image generator from Webscout.AI](#usage-of-image-generator-from-
- webscoutai) - [5. `Prodia` - make image using prodia](#5-prodia---make-image-
-  using-prodia) - [6. `BlackBox` - Search/chat With BlackBox](#6-blackbox---
-  searchchat-with-blackbox) - [7. `PERPLEXITY` - Search With PERPLEXITY](#7-
- perplexity---search-with-perplexity) - [8. `OpenGPT` - chat With OPENGPT](#8-
-  opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-koboldia--) - [usage of
-  special .LLM file from webscout (webscout.LLM)](#usage-of-special-llm-file-
- from-webscout-webscoutllm) - [`LLM`](#llm) ## Install ```python pip install -
-   U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
--------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | ## CLI version of
-webscout.AI | Command | Description | |----------------------------------------
--------|-----------------------------------------------------------------------
-  ---------------------------------| | `python -m webscout.AI phindsearch --
-  prompt "your search query"` | CLI function to perform a search query using
-Webscout.AI's Phindsearch feature. | | `python -m webscout.AI yepchat --message
-   "your_message_here"` | CLI function to send a message using Webscout.AI's
-         Yepchat feature. | | `python -m webscout.AI youchat --prompt
-  "your_prompt_here"` | CLI function to generate a response based on a prompt
-   using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini --
-  message "tell me about gemma 7b"` | CLI function to get information about a
+  [Regions](#regions) - [Transcriber](#transcriber) - [DeepWEBS: Advanced Web
+Searches](#deepwebs-advanced-web-searches) - [Activating DeepWEBS](#activating-
+  deepwebs) - [Point to remember before using `DeepWEBS`](#point-to-remember-
+before-using-deepwebs) - [Usage Example](#usage-example) - [WEBS and AsyncWEBS
+ classes](#webs-and-asyncwebs-classes) - [Exceptions](#exceptions) - [usage of
+ webscout](#usage-of-webscout) - [1. `text()` - text search by DuckDuckGo.com
+and Yep.com](#1-text---text-search-by-duckduckgocom-and-yepcom) - [2. `answers
+  ()` - instant answers by DuckDuckGo.com and Yep.com](#2-answers---instant-
+    answers-by-duckduckgocom-and-yepcom) - [3. `images()` - image search by
+  DuckDuckGo.com and Yep.com](#3-images---image-search-by-duckduckgocom-and-
+ yepcom) - [4. `videos()` - video search by DuckDuckGo.com](#4-videos---video-
+  search-by-duckduckgocom) - [5. `news()` - news search by DuckDuckGo.com and
+ yep.com](#5-news---news-search-by-duckduckgocom-and-yepcom) - [6. `maps()` -
+map search by DuckDuckGo.com and](#6-maps---map-search-by-duckduckgocom-and) -
+[7. `translate()` - translation by DuckDuckGo.com and Yep.com](#7-translate---
+translation-by-duckduckgocom-and-yepcom) - [8. `suggestions()` - suggestions by
+DuckDuckGo.com and Yep.com](#8-suggestions---suggestions-by-duckduckgocom-and-
+ yepcom) - [usage of webscout.AI](#usage-of-webscoutai) - [1. `PhindSearch` -
+Search using Phind.com](#1-phindsearch---search-using-phindcom) - [2. `YepChat`
+ - Chat with mistral 8x7b powered by yepchat](#2-yepchat---chat-with-mistral-
+ 8x7b-powered-by-yepchat) - [3. `You.com` - search with you.com](#3-youcom---
+ search-with-youcom) - [4. `Gemini` - search with google gemini](#4-gemini---
+   search-with-google-gemini) - [usage of image generator from Webscout.AI]
+ (#usage-of-image-generator-from-webscoutai) - [5. `Prodia` - make image using
+  prodia](#5-prodia---make-image-using-prodia) - [6. `BlackBox` - Search/chat
+  With BlackBox](#6-blackbox---searchchat-with-blackbox) - [7. `PERPLEXITY` -
+Search With PERPLEXITY](#7-perplexity---search-with-perplexity) - [8. `OpenGPT`
+ - chat With OPENGPT](#8-opengpt---chat-with-opengpt) - [9. `KOBOLDIA` -](#9-
+koboldia--) - [usage of special .LLM file from webscout (webscout.LLM)](#usage-
+   of-special-llm-file-from-webscout-webscoutllm) - [`LLM`](#llm) ## Install
+   ```python pip install -U webscout ``` ## CLI version ```python3 python -
+m webscout --help ``` | Command | Description | |------------------------------
+-------------|-----------------------------------------------------------------
+--------------------------------------| | python -m webscout answers -k Text |
+    CLI function to perform an answers search using Webscout. | | python -
+  m webscout images -k Text | CLI function to perform an images search using
+Webscout. | | python -m webscout maps -k Text | CLI function to perform a maps
+ search using Webscout. | | python -m webscout news -k Text | CLI function to
+  perform a news search using Webscout. | | python -m webscout suggestions -
+   k Text | CLI function to perform a suggestions search using Webscout. | |
+ python -m webscout text -k Text | CLI function to perform a text search using
+ Webscout. | | python -m webscout translate -k Text | CLI function to perform
+   translate using Webscout. | | python -m webscout version | A command-line
+   interface command that prints and returns the version of the program. | |
+  python -m webscout videos -k Text | CLI function to perform a videos search
+using DuckDuckGo API. | ## CLI version of webscout.AI | Command | Description |
+|-----------------------------------------------|------------------------------
+ --------------------------------------------------------------------------| |
+`python -m webscout.AI phindsearch --prompt "your search query"` | CLI function
+to perform a search query using Webscout.AI's Phindsearch feature. | | `python
+-m webscout.AI yepchat --message "your_message_here"` | CLI function to send a
+message using Webscout.AI's Yepchat feature. | | `python -m webscout.AI youchat
+ --prompt "your_prompt_here"` | CLI function to generate a response based on a
+prompt using Webscout.AI's Youchat feature. | | `python -m webscout.AI gemini -
+ -message "tell me about gemma 7b"` | CLI function to get information about a
  specific topic using Webscout.AI's Gemini feature. | | `python -m webscout.AI
  prodia --prompt "car"` | CLI function to generate content related to a prompt
  using Webscout.AI's Prodia feature. | | `python -m webscout.AI blackboxai --
       prompt "Your prompt here"` | CLI function to perform a search using
 Webscout.AI's Blackbox search feature. | | `python -m webscout.AI perplexity --
       prompt "Your prompt here"` | CLI function to perform a search using
  Webscout.AI's PERPLEXITY feature. | | `python -m webscout.AI opengpt --prompt
@@ -110,26 +111,46 @@
  Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
  for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
 Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
   for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
  Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
  for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
  States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
-  To TOP](#TOP) ## DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone
- feature designed to perform advanced web searches with enhanced capabilities.
- It is particularly powerful in extracting relevant information directly from
-webpages and Search engine, focusing exclusively on text (web) searches. Unlike
-    the `WEBS` , which provides a broader range of search functionalities,
- `DeepWEBS` is specifically tailored for in-depth web searches. ### Activating
- DeepWEBS To utilize the `DeepWEBS` feature, you must first create an instance
- of the `DeepWEBS` . This is designed to be used independently of the `WEBS` ,
-offering a focused approach to web searches. ### Point to remember before using
- `DeepWEBS` As `DeepWEBS` is designed to extract relevant information directly
-from webpages and Search engine, It extracts html from webpages and saves them
-         to folder named files in `DeepWEBS` that can be found at `C:
+ To TOP](#TOP) ## Transcriber The transcriber function in webscout is a handy
+tool that transcribes YouTube videos. Here's an example code demonstrating its
+       usage: ```python import sys from webscout import transcriber def
+    extract_transcript(video_id): """Extracts the transcript from a YouTube
+  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
+transcript in transcript_list: transcript_text_list = transcript.fetch() lang =
+ transcript.language transcript_text = "" if transcript.language_code == 'en':
+for line in transcript_text_list: transcript_text += " " + line["text"] return
+  transcript_text elif transcript.is_translatable: english_transcript_list =
+    transcript.translate('en').fetch() for line in english_transcript_list:
+transcript_text += " " + line["text"] return transcript_text print("Transcript
+ extraction failed. Please check the video URL.") except Exception as e: print
+  (f"Error: {e}") def main(): video_url = input("Enter the video link: ") if
+ video_url: video_id = video_url.split("=")[1] print("Video URL:", video_url)
+submit = input("Press 'Enter' to get the transcript or type 'exit' to quit: ")
+        if submit == '': print("Extracting Transcript...") transcript =
+   extract_transcript(video_id) print('Transcript:') print(transcript) print
+("__________________________________________________________________________________")
+   elif submit.lower() == 'exit': print("Exiting...") sys.exit() else: print
+ ("Invalid input. Please try again.") if __name__ == "__main__": main() ``` ##
+DeepWEBS: Advanced Web Searches `DeepWEBS` is a standalone feature designed to
+ perform advanced web searches with enhanced capabilities. It is particularly
+ powerful in extracting relevant information directly from webpages and Search
+engine, focusing exclusively on text (web) searches. Unlike the `WEBS` , which
+provides a broader range of search functionalities, `DeepWEBS` is specifically
+  tailored for in-depth web searches. ### Activating DeepWEBS To utilize the
+`DeepWEBS` feature, you must first create an instance of the `DeepWEBS` . This
+    is designed to be used independently of the `WEBS` , offering a focused
+  approach to web searches. ### Point to remember before using `DeepWEBS` As
+ `DeepWEBS` is designed to extract relevant information directly from webpages
+  and Search engine, It extracts html from webpages and saves them to folder
+              named files in `DeepWEBS` that can be found at `C:
 \Users\Username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.11_qbz5n2kfra8p0\LocalCache\local-
   packages\Python311\site-packages\DeepWEBS` ### Usage Example Here's a basic
 example of how to use the `DeepWEBS` : ```python from webscout import DeepWEBS
 def perform_web_search(query): # Initialize the DeepWEBS class D = DeepWEBS() #
  Set up the search parameters search_params = D.DeepSearch( queries=[query], #
  Query to search result_num=5, # Number of search results safe=True, # Enable
  SafeSearch types=["web"], # Search type: web extract_webpage=True, # True for
```

### Comparing `webscout-1.2.5/webscout.egg-info/SOURCES.txt` & `webscout-1.2.6/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 webscout/HelpingAI.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
 webscout/cli.py
 webscout/exceptions.py
 webscout/models.py
+webscout/transcriber.py
 webscout/utils.py
 webscout/version.py
 webscout/webscout_search.py
 webscout/webscout_search_async.py
 webscout.egg-info/PKG-INFO
 webscout.egg-info/SOURCES.txt
 webscout.egg-info/dependency_links.txt
```

