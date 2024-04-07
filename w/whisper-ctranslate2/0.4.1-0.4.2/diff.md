# Comparing `tmp/whisper-ctranslate2-0.4.1.tar.gz` & `tmp/whisper-ctranslate2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.4.1.tar", last modified: Fri Feb 23 22:06:33 2024, max compression
+gzip compressed data, was "whisper-ctranslate2-0.4.2.tar", last modified: Sun Apr  7 16:36:12 2024, max compression
```

## Comparing `whisper-ctranslate2-0.4.1.tar` & `whisper-ctranslate2-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-02-23 22:06:33.861340 whisper-ctranslate2-0.4.1/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.4.1/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6872 2024-02-23 22:06:33.861340 whisper-ctranslate2-0.4.1/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.1/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-02-23 22:06:33.862340 whisper-ctranslate2-0.4.1/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-02-22 18:55:15.000000 whisper-ctranslate2-0.4.1/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-02-23 22:06:33.859340 whisper-ctranslate2-0.4.1/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-02-23 22:06:33.860340 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14776 2024-02-23 21:48:18.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/commandline.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3321 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/diarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/live_old.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6772 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-02-21 19:47:57.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8977 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10130 2024-02-23 21:25:54.000000 whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-02-23 22:06:33.861340 whisper-ctranslate2-0.4.1/tests/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.1/tests/testdiarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper-ctranslate2-0.4.1/tests/testlive.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper-ctranslate2-0.4.1/tests/testwriters.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-02-23 22:06:33.861340 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/
--rw-r--r--   0 jordi     (1000) jordi     (1000)     6872 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-02-23 22:06:33.000000 whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.4.2/LICENSE
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.2/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-04-07 16:36:12.127792 whisper-ctranslate2-0.4.2/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-04-07 16:35:05.000000 whisper-ctranslate2-0.4.2/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.125792 whisper-ctranslate2-0.4.2/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.125792 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14776 2024-02-23 21:48:18.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/commandline.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3567 2024-04-07 16:26:12.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/diarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live_old.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6772 2024-04-07 16:09:16.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-02-23 22:08:01.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8977 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10130 2024-04-07 16:09:16.000000 whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.126792 whisper-ctranslate2-0.4.2/tests/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.2/tests/testdiarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper-ctranslate2-0.4.2/tests/testlive.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper-ctranslate2-0.4.2/tests/testwriters.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-04-07 16:36:12.126792 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-04-07 16:36:12.000000 whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.4.1/LICENSE` & `whisper-ctranslate2-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/PKG-INFO` & `whisper-ctranslate2-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -12,16 +12,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: faster-whisper>=1.0.0
+Requires-Dist: ctranslate2
+Requires-Dist: tqdm
+Requires-Dist: sounddevice
+Requires-Dist: numpy
+Provides-Extra: dev
+Requires-Dist: flake8==6.*; extra == "dev"
+Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: nose2; extra == "dev"
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
 
 Whisper command line client compatible with original [OpenAI client](https://github.com/openai/whisper) based on CTranslate2.
```

### Comparing `whisper-ctranslate2-0.4.1/README.md` & `whisper-ctranslate2-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/setup.py` & `whisper-ctranslate2-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/commandline.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/commandline.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/diarization.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/diarization.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,23 @@
     def unload_model(self):
         del self.model
         torch.cuda.empty_cache()
 
     def _load_model(self):
         model_name = "pyannote/speaker-diarization-3.1"
         device = torch.device(self.device)
-        self.model = Pipeline.from_pretrained(
+        model_handle = Pipeline.from_pretrained(
             model_name, use_auth_token=self.use_auth_token
-        ).to(device)
+        )
+        if model_handle is None:
+            raise ValueError(
+                f"The token Hugging Face token '{self.use_auth_token}' for diarization is not valid or you did not accept the EULA"
+            )
+
+        self.model = model_handle.to(device)
 
     def run_model(self, audio: str):
         self._load_model()
         audio = decode_audio(audio)
         audio_data = {
             "waveform": torch.from_numpy(audio[None, :]),
             "sample_rate": 16000,
```

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/live_old.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/live_old.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.4.2/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/tests/testdiarization.py` & `whisper-ctranslate2-0.4.2/tests/testdiarization.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/tests/testlive.py` & `whisper-ctranslate2-0.4.2/tests/testlive.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/tests/testwriters.py` & `whisper-ctranslate2-0.4.2/tests/testwriters.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -12,16 +12,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: faster-whisper>=1.0.0
+Requires-Dist: ctranslate2
+Requires-Dist: tqdm
+Requires-Dist: sounddevice
+Requires-Dist: numpy
+Provides-Extra: dev
+Requires-Dist: flake8==6.*; extra == "dev"
+Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: nose2; extra == "dev"
 
 [![PyPI version](https://img.shields.io/pypi/v/whisper-ctranslate2.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/whisper-ctranslate2/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/whisper-ctranslate2.svg)](https://pypistats.org/packages/whisper-ctranslate2)
 
 # Introduction
 
 Whisper command line client compatible with original [OpenAI client](https://github.com/openai/whisper) based on CTranslate2.
```

### Comparing `whisper-ctranslate2-0.4.1/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.4.2/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

