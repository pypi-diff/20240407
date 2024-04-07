# Comparing `tmp/legal_citation_parser-0.1.4.tar.gz` & `tmp/legal_citation_parser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.1.4.tar", last modified: Sat Apr  6 22:35:38 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.1.5.tar", last modified: Sun Apr  7 01:26:01 2024, max compression
```

## Comparing `legal_citation_parser-0.1.4.tar` & `legal_citation_parser-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.4/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2409 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.4/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.003444 legal_citation_parser-0.1.4/legal_citation_parser/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2024-04-06 21:22:24.000000 legal_citation_parser-0.1.4/legal_citation_parser/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.4/legal_citation_parser/canlii_constants.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6246 2024-04-06 21:18:46.000000 legal_citation_parser-0.1.4/legal_citation_parser/canlii_rules.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      959 2024-04-06 21:18:22.000000 legal_citation_parser-0.1.4/legal_citation_parser/citation_parser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.4/legal_citation_parser/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.003444 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2409 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      806 2024-04-06 22:35:27.000000 legal_citation_parser-0.1.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.5/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1940 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1606 2024-04-07 00:44:19.000000 legal_citation_parser-0.1.5/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/legal_citation_parser/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2024-04-06 23:11:08.000000 legal_citation_parser-0.1.5/legal_citation_parser/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.5/legal_citation_parser/canlii_constants.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6799 2024-04-06 23:56:27.000000 legal_citation_parser-0.1.5/legal_citation_parser/canlii_rules.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2024-04-07 01:23:43.000000 legal_citation_parser-0.1.5/legal_citation_parser/citation_parser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.5/legal_citation_parser/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1940 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-07 01:26:01.000000 legal_citation_parser-0.1.5/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-07 01:26:01.210785 legal_citation_parser-0.1.5/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      702 2024-04-07 01:25:55.000000 legal_citation_parser-0.1.5/setup.py
```

### Comparing `legal_citation_parser-0.1.4/LICENSE` & `legal_citation_parser-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.4/legal_citation_parser/canlii_constants.py` & `legal_citation_parser-0.1.5/legal_citation_parser/canlii_constants.py`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.4/legal_citation_parser/canlii_rules.py` & `legal_citation_parser-0.1.5/legal_citation_parser/canlii_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+"""
+Rule set for parsing CanLII citations and constructing CanLII URLs, as well as neutral citations.
+"""
+
 import re
 
 from .canlii_constants import (
     COURT_HIERARCHY_CRIMINAL,
     COURT_LEVEL_MAPPING,
     PROVINCE_TERRITORY_ABBREVIATIONS,
 )
 
 from .utils import check_url
 
-# CanLII functions
-
 def court_code_corrector(court_code):
     """
-    Assorted tools for standardizing court codes. I'll continue to add them as I encounter them.
+    Court code fine-tuning function to ensure consistency in the court code format.
+
+    Args:
+        court_code (str): The court code to correct.
+
+    Returns:
+        str: The corrected court code.
     """
 
     court_code = court_code.lower()
 
     # Correct for older decisions that use "NWT" instead of "NT"
     if "nwt" in court_code:
         court_code = court_code.replace("nwt", "nt")
@@ -109,15 +117,15 @@
         court_name = None
         jurisdiction = None
 
     # Construct the citation information dictionary
     citation_info = {
         "uid": uid,
         "style_of_cause": style_of_cause,
-        "citation": citation,
+        "atomic_citation": citation,
         "citation_type": citation_type,
         "scr_citation": scr_citation,
         "year": year,
         "court": court_code,
         "decision_number": decision_number,
         "jurisdiction": jurisdiction,
         "court_name": court_name,
@@ -175,8 +183,18 @@
     ]
 
     if jurisdiction == "qc":  # Prioritize French URLs for Quebec decisions
         urls.reverse()
     for url in urls:
         if check_url(url):
             return url
-    return None
+    return None
+# Path: legal_citation_parser/canlii_constants.py
+# Compare this snippet from legal_citation_parser/__init__.py:
+# from .citation_parser import parse_citation
+#
+# __all__ = ['parse_citation']
+# Compare this snippet from setup.py:
+# from setuptools import setup, find_packages
+#
+# # read the contents of your README file one level up
+# from os import path
```

### Comparing `legal_citation_parser-0.1.4/legal_citation_parser/citation_parser.py` & `legal_citation_parser-0.1.5/legal_citation_parser/citation_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """
 This Python module provides tools for extracting metadata information from legal citation strings.
 
 """
 
-#from canlii_rules import canlii_citation_parser
-
 from .canlii_rules import canlii_citation_parser
 
-# Main code
-
-def parse_citation(citation: str, citation_type="canlii") -> dict:
+def parse_citation(
+    citation: str, citation_type: str = "canlii", include_url: bool = False
+) -> dict:
     """
     Parses a citation string to extract key information about the court case.
 
     Args:
         citation (str): The citation string to parse.
         type (str): The type of citation to parse. Default is "canlii".
 
     Returns:
         dict: A dictionary containing the parsed information, including the style of cause,
         citation, citation type (neutral or CanLII), year, court code, decision number,
         jurisdiction, court name, and court level.
     """
 
     if citation_type == "canlii":
-        return canlii_citation_parser(citation)
+        return canlii_citation_parser(citation, include_url=include_url)
 
     elif "CanLII" in citation:
         return canlii_citation_parser(citation)
 
     else:
         return None
```

### Comparing `legal_citation_parser-0.1.4/legal_citation_parser/utils.py` & `legal_citation_parser-0.1.5/legal_citation_parser/utils.py`

 * *Files identical despite different names*

