# Comparing `tmp/forcealign-1.1.3.tar.gz` & `tmp/forcealign-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcealign-1.1.3.tar", last modified: Sat Apr  6 23:08:31 2024, max compression
+gzip compressed data, was "forcealign-1.1.4.tar", last modified: Sun Apr  7 04:01:18 2024, max compression
```

## Comparing `forcealign-1.1.3.tar` & `forcealign-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 23:08:31.891863 forcealign-1.1.3/
--rw-r--r--   0 luke       (501) staff       (20)     1067 2024-03-18 13:49:23.000000 forcealign-1.1.3/LICENSE
--rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-06 23:08:31.891109 forcealign-1.1.3/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)     3864 2024-04-05 18:03:54.000000 forcealign-1.1.3/README.md
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 23:08:31.887748 forcealign-1.1.3/forcealign/
--rw-r--r--   0 luke       (501) staff       (20)       34 2024-03-18 15:39:18.000000 forcealign-1.1.3/forcealign/__init__.py
--rw-r--r--   0 luke       (501) staff       (20)     7287 2024-04-06 23:07:40.000000 forcealign-1.1.3/forcealign/forcealign.py
--rw-r--r--   0 luke       (501) staff       (20)        0 2024-04-05 18:05:30.000000 forcealign-1.1.3/forcealign/util.py
-drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-06 23:08:31.890489 forcealign-1.1.3/forcealign.egg-info/
--rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-06 23:08:31.000000 forcealign-1.1.3/forcealign.egg-info/PKG-INFO
--rw-r--r--   0 luke       (501) staff       (20)      262 2024-04-06 23:08:31.000000 forcealign-1.1.3/forcealign.egg-info/SOURCES.txt
--rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-06 23:08:31.000000 forcealign-1.1.3/forcealign.egg-info/dependency_links.txt
--rw-r--r--   0 luke       (501) staff       (20)       59 2024-04-06 23:08:31.000000 forcealign-1.1.3/forcealign.egg-info/requires.txt
--rw-r--r--   0 luke       (501) staff       (20)       11 2024-04-06 23:08:31.000000 forcealign-1.1.3/forcealign.egg-info/top_level.txt
--rw-r--r--   0 luke       (501) staff       (20)       38 2024-04-06 23:08:31.892004 forcealign-1.1.3/setup.cfg
--rw-r--r--   0 luke       (501) staff       (20)      969 2024-04-06 23:08:02.000000 forcealign-1.1.3/setup.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 04:01:18.105636 forcealign-1.1.4/
+-rw-r--r--   0 luke       (501) staff       (20)     1067 2024-03-18 13:49:23.000000 forcealign-1.1.4/LICENSE
+-rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-07 04:01:18.105081 forcealign-1.1.4/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)     3864 2024-04-05 18:03:54.000000 forcealign-1.1.4/README.md
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 04:01:18.101760 forcealign-1.1.4/forcealign/
+-rw-r--r--   0 luke       (501) staff       (20)       34 2024-03-18 15:39:18.000000 forcealign-1.1.4/forcealign/__init__.py
+-rw-r--r--   0 luke       (501) staff       (20)     7353 2024-04-07 04:00:38.000000 forcealign-1.1.4/forcealign/forcealign.py
+-rw-r--r--   0 luke       (501) staff       (20)        0 2024-04-05 18:05:30.000000 forcealign-1.1.4/forcealign/util.py
+drwxr-xr-x   0 luke       (501) staff       (20)        0 2024-04-07 04:01:18.104363 forcealign-1.1.4/forcealign.egg-info/
+-rw-r--r--   0 luke       (501) staff       (20)     4528 2024-04-07 04:01:17.000000 forcealign-1.1.4/forcealign.egg-info/PKG-INFO
+-rw-r--r--   0 luke       (501) staff       (20)      262 2024-04-07 04:01:18.000000 forcealign-1.1.4/forcealign.egg-info/SOURCES.txt
+-rw-r--r--   0 luke       (501) staff       (20)        1 2024-04-07 04:01:17.000000 forcealign-1.1.4/forcealign.egg-info/dependency_links.txt
+-rw-r--r--   0 luke       (501) staff       (20)       59 2024-04-07 04:01:17.000000 forcealign-1.1.4/forcealign.egg-info/requires.txt
+-rw-r--r--   0 luke       (501) staff       (20)       11 2024-04-07 04:01:17.000000 forcealign-1.1.4/forcealign.egg-info/top_level.txt
+-rw-r--r--   0 luke       (501) staff       (20)       38 2024-04-07 04:01:18.105734 forcealign-1.1.4/setup.cfg
+-rw-r--r--   0 luke       (501) staff       (20)      969 2024-04-07 04:00:53.000000 forcealign-1.1.4/setup.py
```

### Comparing `forcealign-1.1.3/LICENSE` & `forcealign-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `forcealign-1.1.3/PKG-INFO` & `forcealign-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcealign
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python library for forced alignment of English text to English audio.
 Home-page: https://github.com/lukerbs/forcealign
 Author: Luke Kerbs
 Keywords: force align,forced alignment,audio segmentation,audio forced alignment,python forced alignment,phoneme,generate subtitles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forcealign-1.1.3/README.md` & `forcealign-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `forcealign-1.1.3/forcealign/forcealign.py` & `forcealign-1.1.4/forcealign/forcealign.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,16 +264,19 @@
 
 
 def get_breath_idx(transcript):
 	transcript = transcript.replace('—',' ')
 	transcript = alpha_with_punct(transcript).upper().split()
 	idxs = []
 	for i in range(len(transcript)-1):
-		if "," in transcript[i] or "." in transcript[i]:
+		if "," in transcript[i]:
 			idxs.append(i+1)
+		elif "." in transcript[i] and random.choice([True, False, False]):
+			idxs.append(i+1)
+
 	return idxs
 
 def alpha_with_punct(text):
 	return re.sub(r'[^a-zA-Z\s,.]', '', text)
```

### Comparing `forcealign-1.1.3/forcealign.egg-info/PKG-INFO` & `forcealign-1.1.4/forcealign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcealign
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python library for forced alignment of English text to English audio.
 Home-page: https://github.com/lukerbs/forcealign
 Author: Luke Kerbs
 Keywords: force align,forced alignment,audio segmentation,audio forced alignment,python forced alignment,phoneme,generate subtitles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forcealign-1.1.3/setup.py` & `forcealign-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='forcealign',
-    version='1.1.3',
+    version='1.1.4',
     packages=find_packages(),
     install_requires=['torch==2.2.1', 'torchaudio==2.2.1', 'pydub==0.25.1', 'g2p-en==2.1.0'],
     author='Luke Kerbs',
     description='A Python library for forced alignment of English text to English audio.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lukerbs/forcealign',
```

