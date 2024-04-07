# Comparing `tmp/bestnlp-1.0.3-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6746 bytes, number of entries: 9
+Zip file size: 6758 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
--rw-r--r--  2.0 unx     7284 b- defN 24-Apr-07 05:48 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx     4165 b- defN 24-Apr-07 06:23 bestnlp/similar_word_discovery.py
+-rw-r--r--  2.0 unx     7301 b- defN 24-Apr-07 06:43 bestnlp/new_word_discovery.py
+-rw-r--r--  2.0 unx     4182 b- defN 24-Apr-07 06:43 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
 -rw-r--r--  2.0 unx      842 b- defN 24-Apr-03 02:41 bestnlp/utils.py
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/RECORD
-9 files, 17598 bytes uncompressed, 5504 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/RECORD
+9 files, 17632 bytes uncompressed, 5516 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.3.dist-info/METADATA
+Filename: bestnlp-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.3.dist-info/WHEEL
+Filename: bestnlp-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.3.dist-info/top_level.txt
+Filename: bestnlp-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.3.dist-info/RECORD
+Filename: bestnlp-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/new_word_discovery.py

```diff
@@ -1,14 +1,14 @@
 import random
 import math
 import pandas as pd
 import jieba.posseg as jieba
 import re
 import os
-import utils
+import bestnlp.utils as utils
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 
 
 class NewWordDiscovery():
```

## bestnlp/similar_word_discovery.py

```diff
@@ -1,9 +1,9 @@
 # import pandas as pd
-import utils
+import bestnlp.utils as utils
 
 
 class SimilarWordDiscovery():
     """
     search dataframe
     time  keyword  user_id
```

