# Comparing `tmp/bestnlp-1.0.1-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 3511 bytes, number of entries: 6
--rw-r--r--  2.0 unx      113 b- defN 23-Jul-21 08:28 bestnlp/__init__.py
--rw-r--r--  2.0 unx     7561 b- defN 23-Jul-28 09:00 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx      213 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Jul-28 09:47 bestnlp-1.0.1.dist-info/RECORD
-6 files, 8444 bytes uncompressed, 2681 bytes compressed:  68.2%
+Zip file size: 6629 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
+-rw-r--r--  2.0 unx     7287 b- defN 24-Mar-29 09:38 bestnlp/new_word_discovery.py
+-rw-r--r--  2.0 unx     3620 b- defN 24-Apr-03 06:50 bestnlp/similar_word_discovery.py
+-rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
+-rw-r--r--  2.0 unx      842 b- defN 24-Apr-03 02:41 bestnlp/utils.py
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/RECORD
+9 files, 17024 bytes uncompressed, 5387 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
 Filename: bestnlp/__init__.py
 Comment: 
 
 Filename: bestnlp/new_word_discovery.py
 Comment: 
 
-Filename: bestnlp-1.0.1.dist-info/METADATA
+Filename: bestnlp/similar_word_discovery.py
 Comment: 
 
-Filename: bestnlp-1.0.1.dist-info/WHEEL
+Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
-Filename: bestnlp-1.0.1.dist-info/top_level.txt
+Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.1.dist-info/RECORD
+Filename: bestnlp-1.0.2.dist-info/METADATA
+Comment: 
+
+Filename: bestnlp-1.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: bestnlp-1.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: bestnlp-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/__init__.py

```diff
@@ -1,4 +1,7 @@
 from bestnlp.new_word_discovery import NewWordDiscovery
-
 nwd = NewWordDiscovery()
-new_words = nwd.extract_keyword
+new_words = nwd.extract_keyword
+
+from bestnlp.similar_word_discovery import SimilarWordDiscovery
+swd = SimilarWordDiscovery()
+similar_words = swd.find_similar
```

## bestnlp/new_word_discovery.py

```diff
@@ -1,13 +1,14 @@
 import random
 import math
 import pandas as pd
 import jieba.posseg as jieba
 import re
 import os
+import utils
 
 _get_module_path = lambda path: os.path.normpath(os.path.join(os.getcwd(),
                                                  os.path.dirname(__file__), path))
 
 
 class NewWordDiscovery():
 
@@ -21,22 +22,15 @@
             for line in f:
                 temp = line.strip().split()
                 word, freq = temp[0], int(temp[1])
                 di[word] = freq
         return di
 
 
-    def read_txt(self, filename):
-        sentences = []
-        with open(filename, "r") as f:
-            for line in f:
-                res = re.split("[,，。.、;；\'\"\(\)“（）【】\[\]\?？:：!！\s+]", line)
-                sentences.extend(res)
-        sentences = list(set(sentences))
-        return sentences
+
 
 
     def calculate_idf(self, idf_list):
         idf_di = dict()
         for sentence_word_set in idf_list:
             for word in sentence_word_set:
                 if word not in idf_di:
@@ -44,16 +38,16 @@
                 idf_di[word] += 1
         l = len(idf_list)
         for word in idf_di:
             idf_di[word] = math.log(l/(idf_di[word] + 1))
         return idf_di
 
 
-    def get_filter_word(self, freq_di, threshold=500, filename="dict.txt"):
-        jieba_dict = self._read_jieba_dict(filename)
+    def get_filter_word(self, freq_di, threshold=500):
+        jieba_dict = self._read_jieba_dict()
         filter_words = set()
         for word in freq_di:
             word = "".join(word)
             if jieba_dict.get(word, 0) > threshold:
                 filter_words.add(word)
         return filter_words
 
@@ -139,16 +133,14 @@
            if word == "":
                res -= freq/num * math.log2(freq/num)
            else:
                res -= freq/num * math.log2(freq/num)
        return res
 
 
-
-
     def L_entropy(self, freq_di, threshold=0, percent=10):
         di = dict()
         for word in freq_di:
             if len(word) > 1:
                 l_e = self.entropy(freq_di[word]["left"])
                 r_e = self.entropy(freq_di[word]["right"])
                 final_entropy = min(l_e, r_e) * math.log(max(l_e, r_e) + math.e, math.e)
@@ -157,15 +149,15 @@
         di = sorted(di.items(), key=lambda x: x[1][0], reverse=True)
         di = di[:int(len(freq_di) * percent / 100)]
         di = {key: value for key, value in di}
         return di
 
 
     def extract_keyword(self, filename, k_min=2, k_max=5, mode="word", min_freq=5, entropy_percent=20, ami_percent=20, write_mode=True, write_name="details.csv"):
-        sentences = self.read_txt(filename)
+        sentences = utils.read_txt(filename)
         write_df = {"word":[], "ami":[], "entropy":[], "l_e":[], "r_e":[], "pos":[], "freq":[], "idf":[], "score":[]}
         freq_di, word_num, idf_di = self.calculate_frequency(sentences, k_min, k_max, mode)
         entropy_di = self.L_entropy(freq_di, percent=entropy_percent)
         print(len(entropy_di))
         ami_di = self.ami(freq_di, word_num, percent=ami_percent)
         print(len(ami_di))
         structure_di = self.structure(freq_di)
@@ -183,15 +175,16 @@
                 write_df["l_e"].append(entropy_di[name][1])
                 write_df["r_e"].append(entropy_di[name][2])
                 write_df["pos"].append("_".join(freq_di[name]["pos"]))
                 write_df["freq"].append(freq_di[name]["freq"])
                 write_df["idf"].append(idf)
                 write_df["score"].append(final_di[name])
         if write_mode:
-            pd.DataFrame.from_dict(write_df).to_csv(write_name)
+            write_df = pd.DataFrame.from_dict(write_df).sort_values("score", ascending=False)
+            write_df.to_csv(write_name)
 
 
 
 
 # nwd = NewWordDiscovery()
 # nwd.extract_keyword("三体.txt", k_min=2, k_max=7, mode="char", min_freq=7, entropy_percent=20, ami_percent=20, write_name="char.csv", write_mode=True)
```

