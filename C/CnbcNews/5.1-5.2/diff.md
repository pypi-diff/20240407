# Comparing `tmp/CnbcNews-5.1.tar.gz` & `tmp/CnbcNews-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CnbcNews-5.1.tar", last modified: Sat Apr  6 20:20:15 2024, max compression
+gzip compressed data, was "CnbcNews-5.2.tar", last modified: Sun Apr  7 20:48:12 2024, max compression
```

## Comparing `CnbcNews-5.1.tar` & `CnbcNews-5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 20:20:15.452462 CnbcNews-5.1/
-drwxrwxrwx   0        0        0        0 2024-04-06 20:20:15.338256 CnbcNews-5.1/CnbcNews/
--rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-5.1/CnbcNews/__init__.py
--rw-rw-rw-   0        0        0     4593 2024-04-06 17:59:40.000000 CnbcNews-5.1/CnbcNews/main.py
-drwxrwxrwx   0        0        0        0 2024-04-06 20:20:15.442234 CnbcNews-5.1/CnbcNews.egg-info/
--rw-rw-rw-   0        0        0     2723 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       31 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 20:20:15.000000 CnbcNews-5.1/CnbcNews.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2723 2024-04-06 20:20:15.449762 CnbcNews-5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2625 2024-04-06 20:14:06.000000 CnbcNews-5.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 20:20:15.453457 CnbcNews-5.1/setup.cfg
--rw-rw-rw-   0        0        0      579 2024-04-06 20:20:08.000000 CnbcNews-5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:48:12.684251 CnbcNews-5.2/
+drwxrwxrwx   0        0        0        0 2024-04-07 20:48:12.651233 CnbcNews-5.2/CnbcNews/
+-rw-rw-rw-   0        0        0       44 2024-04-06 16:37:01.000000 CnbcNews-5.2/CnbcNews/__init__.py
+-rw-rw-rw-   0        0        0     4903 2024-04-07 20:39:27.000000 CnbcNews-5.2/CnbcNews/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:48:12.677947 CnbcNews-5.2/CnbcNews.egg-info/
+-rw-rw-rw-   0        0        0     2723 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 20:48:12.000000 CnbcNews-5.2/CnbcNews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2723 2024-04-07 20:48:12.682226 CnbcNews-5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2625 2024-04-06 20:14:06.000000 CnbcNews-5.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 20:48:12.685240 CnbcNews-5.2/setup.cfg
+-rw-rw-rw-   0        0        0      579 2024-04-07 20:48:03.000000 CnbcNews-5.2/setup.py
```

### Comparing `CnbcNews-5.1/CnbcNews/main.py` & `CnbcNews-5.2/CnbcNews/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import json
 import pandas as pd
 from bs4 import BeautifulSoup
 import requests
-import csv
+import argparse
 import os
 import time
 
 def getLinks(field, number, page_number=1):
     article_urls = []
     while len(article_urls) < number:
         url = f"https://www.cnbc.com/{field}/?page={page_number}"
@@ -31,15 +30,15 @@
     if field not in ['technology', 'politics', 'tv', 'business', 'markets', 'investing']:
         print("Invalid field. Please provide one of the following sections: 'technology', 'politics', 'tv', 'business', 'markets', 'investing'.")
         return
     
     print(f"crawling {field} articles ...")
     articles_url = getLinks(field, number)
     articles_df = pd.DataFrame({"url":articles_url})
-    le = len(articles_df)
+    
     for i in range(number):
         response = requests.get(articles_df.iloc[i].url)
         article_page = BeautifulSoup(response.content, "html.parser")
         article_headline = article_page.find("h1", class_="ArticleHeader-headline")
         article_body = article_page.find("div", class_="ArticleBody-articleBody")
         article_author = article_page.find("a", class_="Author-authorName")
         article_header = article_page.find(id="main-article-header")
@@ -87,19 +86,26 @@
     """
     for field in fields: 
         getArticles(field=field, number=number)
         time.sleep(timeout)
 
 
 def main():
-    import sys
-    if len(sys.argv)==4:
-        getArticles(sys.argv[1], int(sys.argv[2]), json.loads(sys.argv[3].lower()))
-    elif len(sys.argv)==3:
-        getArticles(sys.argv[1], int(sys.argv[2]))
-    elif len(sys.argv)==2:
-        getArticles(sys.argv[1])
+    parser = argparse.ArgumentParser(description="CnbcNews Cnbc article retrieval tool by Ahmed Bendrioua")
+    parser.add_argument("field", help="Field/category of articles to retrieve from CNBC")
+    parser.add_argument("--number", "-n", type=int, help="Number of articles to retrieve")
+    parser.add_argument("--dropna", "-d", action="store_true", help="Drop rows with missing values")
+
+    args = parser.parse_args()
+
+    field = args.field
+    number = args.number
+    dropna = args.dropna
+
+    if number is not None and dropna is not None:
+        getArticles(field, number, dropna)
+    elif number is not None:
+        getArticles(field, number)
     else:
-        print("please provide the field ! exemple : CnbcNews-getArticles technology")
-
+        getArticles(field)
 if __name__ == "__main__":
     main()
```

### Comparing `CnbcNews-5.1/CnbcNews.egg-info/PKG-INFO` & `CnbcNews-5.2/CnbcNews.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 5.1
+Version: 5.2
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-5.1/PKG-INFO` & `CnbcNews-5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CnbcNews
-Version: 5.1
+Version: 5.2
 Description-Content-Type: text/markdown
 
 # **CnbcNews** #
 
 [![PyPI version](https://img.shields.io/pypi/v/CnbcNews.svg)](https://pypi.org/project/CnbcNews/)
 <!-- [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XX272QZV9A2FN&source=url) -->
```

### Comparing `CnbcNews-5.1/README.md` & `CnbcNews-5.2/README.md`

 * *Files identical despite different names*

### Comparing `CnbcNews-5.1/setup.py` & `CnbcNews-5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CnbcNews',
-    version='5.1',
+    version='5.2',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
         'pandas',
     ],
     entry_points={
```

