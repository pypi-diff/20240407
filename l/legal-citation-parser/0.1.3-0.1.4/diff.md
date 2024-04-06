# Comparing `tmp/legal_citation_parser-0.1.3.tar.gz` & `tmp/legal_citation_parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.1.3.tar", last modified: Sat Apr  6 21:24:48 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.1.4.tar", last modified: Sat Apr  6 22:35:38 2024, max compression
```

## Comparing `legal_citation_parser-0.1.3.tar` & `legal_citation_parser-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:24:48.469960 legal_citation_parser-0.1.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.3/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 21:24:48.469960 legal_citation_parser-0.1.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.3/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:24:48.469960 legal_citation_parser-0.1.3/legal_citation_parser/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2024-04-06 21:22:24.000000 legal_citation_parser-0.1.3/legal_citation_parser/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.3/legal_citation_parser/canlii_constants.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     6246 2024-04-06 21:18:46.000000 legal_citation_parser-0.1.3/legal_citation_parser/canlii_rules.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      959 2024-04-06 21:18:22.000000 legal_citation_parser-0.1.3/legal_citation_parser/citation_parser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.3/legal_citation_parser/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 21:24:48.469960 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      205 2024-04-06 21:24:48.000000 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-06 21:24:48.000000 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 21:24:48.000000 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 21:24:48.000000 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-06 21:24:48.000000 legal_citation_parser-0.1.3/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 21:24:48.469960 legal_citation_parser-0.1.3/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      299 2024-04-06 21:24:30.000000 legal_citation_parser-0.1.3/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.1.4/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2409 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2019 2024-04-06 19:14:15.000000 legal_citation_parser-0.1.4/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.003444 legal_citation_parser-0.1.4/legal_citation_parser/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       74 2024-04-06 21:22:24.000000 legal_citation_parser-0.1.4/legal_citation_parser/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    32460 2024-04-06 18:41:34.000000 legal_citation_parser-0.1.4/legal_citation_parser/canlii_constants.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6246 2024-04-06 21:18:46.000000 legal_citation_parser-0.1.4/legal_citation_parser/canlii_rules.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      959 2024-04-06 21:18:22.000000 legal_citation_parser-0.1.4/legal_citation_parser/citation_parser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      537 2024-04-06 20:05:11.000000 legal_citation_parser-0.1.4/legal_citation_parser/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-06 22:35:38.003444 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2409 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-06 22:35:37.000000 legal_citation_parser-0.1.4/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-06 22:35:38.007444 legal_citation_parser-0.1.4/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      806 2024-04-06 22:35:27.000000 legal_citation_parser-0.1.4/setup.py
```

### Comparing `legal_citation_parser-0.1.3/LICENSE` & `legal_citation_parser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.3/README.md` & `legal_citation_parser-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.3/legal_citation_parser/canlii_constants.py` & `legal_citation_parser-0.1.4/legal_citation_parser/canlii_constants.py`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.3/legal_citation_parser/canlii_rules.py` & `legal_citation_parser-0.1.4/legal_citation_parser/canlii_rules.py`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.3/legal_citation_parser/citation_parser.py` & `legal_citation_parser-0.1.4/legal_citation_parser/citation_parser.py`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.1.3/legal_citation_parser/utils.py` & `legal_citation_parser-0.1.4/legal_citation_parser/utils.py`

 * *Files identical despite different names*

