# Comparing `tmp/whereabouts-0.3.5.tar.gz` & `tmp/whereabouts-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whereabouts-0.3.5.tar", max compression
+gzip compressed data, was "whereabouts-0.3.6.tar", max compression
```

## Comparing `whereabouts-0.3.5.tar` & `whereabouts-0.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1065 2024-03-02 05:09:14.320026 whereabouts-0.3.5/LICENSE
--rw-r--r--   0        0        0     2758 2024-04-07 00:02:49.532122 whereabouts-0.3.5/README.md
--rw-r--r--   0        0        0      548 2024-04-07 04:44:02.654891 whereabouts-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     8051 2024-03-02 07:08:18.716238 whereabouts-0.3.5/whereabouts/AddressLoader.py
--rw-r--r--   0        0        0     5767 2024-03-02 05:09:14.321615 whereabouts-0.3.5/whereabouts/GNAFLoader.py
--rw-r--r--   0        0        0     6024 2024-04-07 01:08:47.529463 whereabouts-0.3.5/whereabouts/Matcher.py
--rw-r--r--   0        0        0     1892 2024-03-02 05:09:14.321835 whereabouts-0.3.5/whereabouts/MatcherPipeline.py
--rw-r--r--   0        0        0        0 2024-03-02 05:09:14.321876 whereabouts-0.3.5/whereabouts/__init__.py
--rw-r--r--   0        0        0      522 2024-03-02 05:09:14.321988 whereabouts-0.3.5/whereabouts/__main__.py
--rw-r--r--   0        0        0        0 2024-03-02 05:09:14.322676 whereabouts-0.3.5/whereabouts/models/__init__.py
--rw-r--r--   0        0        0      798 2024-03-02 05:09:14.322852 whereabouts-0.3.5/whereabouts/queries/create_addrtext.sql
--rw-r--r--   0        0        0     1072 2024-03-02 05:09:14.322950 whereabouts-0.3.5/whereabouts/queries/create_geocoder_tables.sql
--rw-r--r--   0        0        0      387 2024-03-02 05:09:14.323068 whereabouts-0.3.5/whereabouts/queries/create_indexes.sql
--rw-r--r--   0        0        0       84 2024-03-02 05:09:14.323185 whereabouts-0.3.5/whereabouts/queries/create_indexes_skipphrase.sql
--rw-r--r--   0        0        0      900 2024-03-02 05:09:14.323299 whereabouts-0.3.5/whereabouts/queries/create_phrases.sql
--rw-r--r--   0        0        0      829 2024-03-02 05:09:14.323393 whereabouts-0.3.5/whereabouts/queries/create_skipphrases.sql
--rw-r--r--   0        0        0      131 2024-03-02 05:09:14.323485 whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step1.sql
--rw-r--r--   0        0        0      440 2024-03-02 05:09:14.323576 whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step2.sql
--rw-r--r--   0        0        0      527 2024-03-09 04:06:11.104110 whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step2b.sql
--rw-r--r--   0        0        0      550 2024-03-02 05:09:14.323806 whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step3.sql
--rw-r--r--   0        0        0      298 2024-03-02 05:09:14.323904 whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step4.sql
--rw-r--r--   0        0        0      847 2024-03-02 05:09:14.324037 whereabouts-0.3.5/whereabouts/queries/create_trigramphrases.sql
--rw-r--r--   0        0        0     4043 2024-03-02 05:09:14.324196 whereabouts-0.3.5/whereabouts/queries/geocoder_query_skipphrase.sql
--rw-r--r--   0        0        0     4402 2024-03-02 05:09:14.324298 whereabouts-0.3.5/whereabouts/queries/geocoder_query_standard.sql
--rw-r--r--   0        0        0     4037 2024-03-02 05:09:14.324387 whereabouts-0.3.5/whereabouts/queries/geocoder_query_standard2.sql
--rw-r--r--   0        0        0     4831 2024-03-02 05:09:14.324469 whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigram.sql
--rw-r--r--   0        0        0     4856 2024-03-02 05:09:14.324555 whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigramb.sql
--rw-r--r--   0        0        0     4479 2024-03-02 05:09:14.324657 whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigramb2.sql
--rw-r--r--   0        0        0      107 2024-03-02 05:09:14.324880 whereabouts-0.3.5/whereabouts/queries/phrase_inverted.sql
--rw-r--r--   0        0        0      117 2024-03-02 05:09:14.324965 whereabouts-0.3.5/whereabouts/queries/skipphrase_inverted.sql
--rw-r--r--   0        0        0      130 2024-03-02 05:09:14.325054 whereabouts-0.3.5/whereabouts/queries/trigramphrase_inverted.sql
--rw-r--r--   0        0        0     5356 2024-04-07 04:43:01.888010 whereabouts-0.3.5/whereabouts/utils.py
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 whereabouts-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-02 05:09:14.320026 whereabouts-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2758 2024-04-07 00:02:49.532122 whereabouts-0.3.6/README.md
+-rw-r--r--   0        0        0      548 2024-04-07 04:48:45.797158 whereabouts-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     8051 2024-03-02 07:08:18.716238 whereabouts-0.3.6/whereabouts/AddressLoader.py
+-rw-r--r--   0        0        0     5767 2024-03-02 05:09:14.321615 whereabouts-0.3.6/whereabouts/GNAFLoader.py
+-rw-r--r--   0        0        0     6024 2024-04-07 01:08:47.529463 whereabouts-0.3.6/whereabouts/Matcher.py
+-rw-r--r--   0        0        0     1892 2024-03-02 05:09:14.321835 whereabouts-0.3.6/whereabouts/MatcherPipeline.py
+-rw-r--r--   0        0        0        0 2024-03-02 05:09:14.321876 whereabouts-0.3.6/whereabouts/__init__.py
+-rw-r--r--   0        0        0      522 2024-03-02 05:09:14.321988 whereabouts-0.3.6/whereabouts/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-02 05:09:14.322676 whereabouts-0.3.6/whereabouts/models/__init__.py
+-rw-r--r--   0        0        0      798 2024-03-02 05:09:14.322852 whereabouts-0.3.6/whereabouts/queries/create_addrtext.sql
+-rw-r--r--   0        0        0     1072 2024-03-02 05:09:14.322950 whereabouts-0.3.6/whereabouts/queries/create_geocoder_tables.sql
+-rw-r--r--   0        0        0      387 2024-03-02 05:09:14.323068 whereabouts-0.3.6/whereabouts/queries/create_indexes.sql
+-rw-r--r--   0        0        0       84 2024-03-02 05:09:14.323185 whereabouts-0.3.6/whereabouts/queries/create_indexes_skipphrase.sql
+-rw-r--r--   0        0        0      900 2024-03-02 05:09:14.323299 whereabouts-0.3.6/whereabouts/queries/create_phrases.sql
+-rw-r--r--   0        0        0      829 2024-03-02 05:09:14.323393 whereabouts-0.3.6/whereabouts/queries/create_skipphrases.sql
+-rw-r--r--   0        0        0      131 2024-03-02 05:09:14.323485 whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step1.sql
+-rw-r--r--   0        0        0      440 2024-03-02 05:09:14.323576 whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step2.sql
+-rw-r--r--   0        0        0      527 2024-03-09 04:06:11.104110 whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step2b.sql
+-rw-r--r--   0        0        0      550 2024-03-02 05:09:14.323806 whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step3.sql
+-rw-r--r--   0        0        0      298 2024-03-02 05:09:14.323904 whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step4.sql
+-rw-r--r--   0        0        0      847 2024-03-02 05:09:14.324037 whereabouts-0.3.6/whereabouts/queries/create_trigramphrases.sql
+-rw-r--r--   0        0        0     4043 2024-03-02 05:09:14.324196 whereabouts-0.3.6/whereabouts/queries/geocoder_query_skipphrase.sql
+-rw-r--r--   0        0        0     4402 2024-03-02 05:09:14.324298 whereabouts-0.3.6/whereabouts/queries/geocoder_query_standard.sql
+-rw-r--r--   0        0        0     4037 2024-03-02 05:09:14.324387 whereabouts-0.3.6/whereabouts/queries/geocoder_query_standard2.sql
+-rw-r--r--   0        0        0     4831 2024-03-02 05:09:14.324469 whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigram.sql
+-rw-r--r--   0        0        0     4856 2024-03-02 05:09:14.324555 whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigramb.sql
+-rw-r--r--   0        0        0     4479 2024-03-02 05:09:14.324657 whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigramb2.sql
+-rw-r--r--   0        0        0      107 2024-03-02 05:09:14.324880 whereabouts-0.3.6/whereabouts/queries/phrase_inverted.sql
+-rw-r--r--   0        0        0      117 2024-03-02 05:09:14.324965 whereabouts-0.3.6/whereabouts/queries/skipphrase_inverted.sql
+-rw-r--r--   0        0        0      130 2024-03-02 05:09:14.325054 whereabouts-0.3.6/whereabouts/queries/trigramphrase_inverted.sql
+-rw-r--r--   0        0        0     5356 2024-04-07 04:43:01.888010 whereabouts-0.3.6/whereabouts/utils.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 whereabouts-0.3.6/PKG-INFO
```

### Comparing `whereabouts-0.3.5/LICENSE` & `whereabouts-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/README.md` & `whereabouts-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/pyproject.toml` & `whereabouts-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whereabouts"
-version = "0.3.5"
+version = "0.3.6"
 description = "Open source geocoding in Python"
 authors = ["alex2718 <ajlee3141@gmail.com>"]
 readme = "README.md"
 keywords = ['geocoding', 'geospatial', 'record linkage']
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `whereabouts-0.3.5/whereabouts/AddressLoader.py` & `whereabouts-0.3.6/whereabouts/AddressLoader.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/GNAFLoader.py` & `whereabouts-0.3.6/whereabouts/GNAFLoader.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/Matcher.py` & `whereabouts-0.3.6/whereabouts/Matcher.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/MatcherPipeline.py` & `whereabouts-0.3.6/whereabouts/MatcherPipeline.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/__main__.py` & `whereabouts-0.3.6/whereabouts/__main__.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_addrtext.sql` & `whereabouts-0.3.6/whereabouts/queries/create_addrtext.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_geocoder_tables.sql` & `whereabouts-0.3.6/whereabouts/queries/create_geocoder_tables.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_phrases.sql` & `whereabouts-0.3.6/whereabouts/queries/create_phrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_skipphrases.sql` & `whereabouts-0.3.6/whereabouts/queries/create_skipphrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step2b.sql` & `whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step2b.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_trigram_index_step3.sql` & `whereabouts-0.3.6/whereabouts/queries/create_trigram_index_step3.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/create_trigramphrases.sql` & `whereabouts-0.3.6/whereabouts/queries/create_trigramphrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_skipphrase.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_skipphrase.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_standard.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_standard.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_standard2.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_standard2.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigram.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigram.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigramb.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigramb.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/queries/geocoder_query_trigramb2.sql` & `whereabouts-0.3.6/whereabouts/queries/geocoder_query_trigramb2.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/whereabouts/utils.py` & `whereabouts-0.3.6/whereabouts/utils.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.5/PKG-INFO` & `whereabouts-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whereabouts
-Version: 0.3.5
+Version: 0.3.6
 Summary: Open source geocoding in Python
 Keywords: geocoding,geospatial,record linkage
 Author: alex2718
 Author-email: ajlee3141@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

