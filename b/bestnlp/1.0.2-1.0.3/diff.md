# Comparing `tmp/bestnlp-1.0.2-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6629 bytes, number of entries: 9
+Zip file size: 6746 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
--rw-r--r--  2.0 unx     7287 b- defN 24-Mar-29 09:38 bestnlp/new_word_discovery.py
--rw-r--r--  2.0 unx     3620 b- defN 24-Apr-03 06:50 bestnlp/similar_word_discovery.py
+-rw-r--r--  2.0 unx     7284 b- defN 24-Apr-07 05:48 bestnlp/new_word_discovery.py
+-rw-r--r--  2.0 unx     4165 b- defN 24-Apr-07 06:23 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
 -rw-r--r--  2.0 unx      842 b- defN 24-Apr-03 02:41 bestnlp/utils.py
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-03 06:57 bestnlp-1.0.2.dist-info/RECORD
-9 files, 17024 bytes uncompressed, 5387 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-07 06:38 bestnlp-1.0.3.dist-info/RECORD
+9 files, 17598 bytes uncompressed, 5504 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.2.dist-info/METADATA
+Filename: bestnlp-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.2.dist-info/WHEEL
+Filename: bestnlp-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.2.dist-info/top_level.txt
+Filename: bestnlp-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.2.dist-info/RECORD
+Filename: bestnlp-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bestnlp/new_word_discovery.py

```diff
@@ -22,17 +22,14 @@
             for line in f:
                 temp = line.strip().split()
                 word, freq = temp[0], int(temp[1])
                 di[word] = freq
         return di
 
 
-
-
-
     def calculate_idf(self, idf_list):
         idf_di = dict()
         for sentence_word_set in idf_list:
             for word in sentence_word_set:
                 if word not in idf_di:
                     idf_di[word] = 0
                 idf_di[word] += 1
```

## bestnlp/similar_word_discovery.py

```diff
@@ -1,14 +1,12 @@
-import pandas as pd
+# import pandas as pd
 import utils
 
 
 class SimilarWordDiscovery():
-
-
     """
     search dataframe
     time  keyword  user_id
 
     click dataframe
     time  keyword  user_id  item_id
     """
@@ -77,8 +75,27 @@
 # print(res)
 # print(len(res))
 # for elem in res:
 #     print(elem)
 
 
 
+# search_df = pd.read_excel("search.xlsx")
+# click_df = pd.read_excel("click.xlsx")
+# print(search_df)
+# print(click_df)
+#
+# search_df.rename(columns={"search_term":"keyword", "distinct_id":"user_id"}, inplace=True)
+# click_df["keyword"] = click_df["url"].apply(lambda x: str(x)[6:])
+# click_df.rename(columns={"distinct_id":"user_id", "article_number":"item_id"}, inplace=True)
+#
+# swd = SimilarWordDiscovery()
+# res = swd.find_similar(search_df, click_df, threshold=100)
+# print(res)
+# print(len(res))
+# for elem in res:
+#     print(elem)
+
+
+
+
```

## Comparing `bestnlp-1.0.2.dist-info/RECORD` & `bestnlp-1.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 bestnlp/__init__.py,sha256=yWr8dJQkCu83EoT_iYfJ_XAO1EFHFvZz47Wud_dClzM,239
-bestnlp/new_word_discovery.py,sha256=jxl9GwUW2cB3r8FfOvSBiFKeRKIV8UcRw7ezaLuEXEQ,7287
-bestnlp/similar_word_discovery.py,sha256=oXbX1L-P-0mDm7-SMELZF1A4jHe4kePtjFlrNWS1vA0,3620
+bestnlp/new_word_discovery.py,sha256=KHkUAtrWj_57BvyYjG7mGxSIu9tOTzrRdjblQUz_RkU,7284
+bestnlp/similar_word_discovery.py,sha256=Tacn93NIpOxJZlQJBTVYwH35ckSuU3SrlIdEmPdfVbM,4165
 bestnlp/similar_word_discovery_embedding.py,sha256=HsoxJomebHNlB9JyNfGghGSPJ6FJ4X0eAvRnbTUUmf8,4004
 bestnlp/utils.py,sha256=g8F8OjAFl2Fkwn6WyppxHdreeBnN9bVwBFqNUa1Wfww,842
-bestnlp-1.0.2.dist-info/METADATA,sha256=SMQ5DEAn4Q-WKZRjmBCNNFrBoQJhNphN9m4P6jhqJsU,213
-bestnlp-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bestnlp-1.0.2.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
-bestnlp-1.0.2.dist-info/RECORD,,
+bestnlp-1.0.3.dist-info/METADATA,sha256=heOzibPOJVwZ8ORP9Zlqr7mY78PHHAT-1KYeKtUKUzY,245
+bestnlp-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bestnlp-1.0.3.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
+bestnlp-1.0.3.dist-info/RECORD,,
```

