# Comparing `tmp/rdfhelpers-0.6.2.tar.gz` & `tmp/rdfhelpers-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdfhelpers-0.6.2.tar", last modified: Sun Mar 31 12:32:05 2024, max compression
+gzip compressed data, was "rdfhelpers-0.6.3.tar", last modified: Sat Apr  6 22:24:37 2024, max compression
```

## Comparing `rdfhelpers-0.6.2.tar` & `rdfhelpers-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-03-31 12:32:05.475914 rdfhelpers-0.6.2/
--rw-r--r--   0 ora        (502) staff       (20)     1530 2022-06-20 11:30:36.000000 rdfhelpers-0.6.2/LICENSE
--rw-r--r--   0 ora        (502) staff       (20)     1243 2024-03-31 12:32:05.475775 rdfhelpers-0.6.2/PKG-INFO
--rw-r--r--   0 ora        (502) staff       (20)      813 2022-11-24 09:55:26.000000 rdfhelpers-0.6.2/README.md
--rw-r--r--   0 ora        (502) staff       (20)      104 2022-06-20 12:10:06.000000 rdfhelpers-0.6.2/pyproject.toml
--rw-r--r--   0 ora        (502) staff       (20)      549 2024-03-31 12:32:05.476431 rdfhelpers-0.6.2/setup.cfg
-drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-03-31 12:32:05.466597 rdfhelpers-0.6.2/src/
-drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-03-31 12:32:05.472961 rdfhelpers-0.6.2/src/rdfhelpers/
--rw-r--r--   0 ora        (502) staff       (20)     1527 2023-09-19 00:45:45.000000 rdfhelpers-0.6.2/src/rdfhelpers/__init__.py
--rw-r--r--   0 ora        (502) staff       (20)     7491 2024-03-31 11:56:38.000000 rdfhelpers-0.6.2/src/rdfhelpers/cbd.py
--rw-r--r--   0 ora        (502) staff       (20)     3611 2023-10-24 23:12:19.000000 rdfhelpers-0.6.2/src/rdfhelpers/constructor.py
--rw-r--r--   0 ora        (502) staff       (20)     7304 2023-09-19 00:45:45.000000 rdfhelpers-0.6.2/src/rdfhelpers/labels.py
--rw-r--r--   0 ora        (502) staff       (20)     6328 2022-12-18 10:27:46.000000 rdfhelpers-0.6.2/src/rdfhelpers/rdfhelpers.py
--rw-r--r--   0 ora        (502) staff       (20)     7058 2024-03-31 12:25:45.000000 rdfhelpers-0.6.2/src/rdfhelpers/templated.py
-drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-03-31 12:32:05.475272 rdfhelpers-0.6.2/src/rdfhelpers.egg-info/
--rw-r--r--   0 ora        (502) staff       (20)     1243 2024-03-31 12:32:05.000000 rdfhelpers-0.6.2/src/rdfhelpers.egg-info/PKG-INFO
--rw-r--r--   0 ora        (502) staff       (20)      355 2024-03-31 12:32:05.000000 rdfhelpers-0.6.2/src/rdfhelpers.egg-info/SOURCES.txt
--rw-r--r--   0 ora        (502) staff       (20)        1 2024-03-31 12:32:05.000000 rdfhelpers-0.6.2/src/rdfhelpers.egg-info/dependency_links.txt
--rw-r--r--   0 ora        (502) staff       (20)       11 2024-03-31 12:32:05.000000 rdfhelpers-0.6.2/src/rdfhelpers.egg-info/top_level.txt
+drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-04-06 22:24:37.002603 rdfhelpers-0.6.3/
+-rw-r--r--   0 ora        (502) staff       (20)     1530 2022-06-20 11:30:36.000000 rdfhelpers-0.6.3/LICENSE
+-rw-r--r--   0 ora        (502) staff       (20)     1243 2024-04-06 22:24:37.002441 rdfhelpers-0.6.3/PKG-INFO
+-rw-r--r--   0 ora        (502) staff       (20)      813 2022-11-24 09:55:26.000000 rdfhelpers-0.6.3/README.md
+-rw-r--r--   0 ora        (502) staff       (20)      104 2022-06-20 12:10:06.000000 rdfhelpers-0.6.3/pyproject.toml
+-rw-r--r--   0 ora        (502) staff       (20)      549 2024-04-06 22:24:37.003496 rdfhelpers-0.6.3/setup.cfg
+drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-04-06 22:24:36.957089 rdfhelpers-0.6.3/src/
+drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-04-06 22:24:36.966901 rdfhelpers-0.6.3/src/rdfhelpers/
+-rw-r--r--   0 ora        (502) staff       (20)     1527 2023-09-19 00:45:45.000000 rdfhelpers-0.6.3/src/rdfhelpers/__init__.py
+-rw-r--r--   0 ora        (502) staff       (20)     7491 2024-03-31 11:56:38.000000 rdfhelpers-0.6.3/src/rdfhelpers/cbd.py
+-rw-r--r--   0 ora        (502) staff       (20)     3611 2023-10-24 23:12:19.000000 rdfhelpers-0.6.3/src/rdfhelpers/constructor.py
+-rw-r--r--   0 ora        (502) staff       (20)     7166 2024-04-06 22:19:07.000000 rdfhelpers-0.6.3/src/rdfhelpers/labels.py
+-rw-r--r--   0 ora        (502) staff       (20)     6328 2022-12-18 10:27:46.000000 rdfhelpers-0.6.3/src/rdfhelpers/rdfhelpers.py
+-rw-r--r--   0 ora        (502) staff       (20)     7058 2024-03-31 12:25:45.000000 rdfhelpers-0.6.3/src/rdfhelpers/templated.py
+drwxr-xr-x   0 ora        (502) staff       (20)        0 2024-04-06 22:24:37.001794 rdfhelpers-0.6.3/src/rdfhelpers.egg-info/
+-rw-r--r--   0 ora        (502) staff       (20)     1243 2024-04-06 22:24:36.000000 rdfhelpers-0.6.3/src/rdfhelpers.egg-info/PKG-INFO
+-rw-r--r--   0 ora        (502) staff       (20)      355 2024-04-06 22:24:36.000000 rdfhelpers-0.6.3/src/rdfhelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 ora        (502) staff       (20)        1 2024-04-06 22:24:36.000000 rdfhelpers-0.6.3/src/rdfhelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 ora        (502) staff       (20)       11 2024-04-06 22:24:36.000000 rdfhelpers-0.6.3/src/rdfhelpers.egg-info/top_level.txt
```

### Comparing `rdfhelpers-0.6.2/LICENSE` & `rdfhelpers-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/PKG-INFO` & `rdfhelpers-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhelpers
-Version: 0.6.2
+Version: 0.6.3
 Summary: Useful stuff when programming with RDFLib
 Home-page: https://gitlab.com/somanyaircraft/rdfhelpers
 Author-email: ora@somanyaircraft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `rdfhelpers-0.6.2/README.md` & `rdfhelpers-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/setup.cfg` & `rdfhelpers-0.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rdfhelpers
-version = 0.6.2
+version = 0.6.3
 author_email = ora@somanyaircraft.com
 description = Useful stuff when programming with RDFLib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/somanyaircraft/rdfhelpers
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/__init__.py` & `rdfhelpers-0.6.3/src/rdfhelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/cbd.py` & `rdfhelpers-0.6.3/src/rdfhelpers/cbd.py`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/constructor.py` & `rdfhelpers-0.6.3/src/rdfhelpers/constructor.py`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/labels.py` & `rdfhelpers-0.6.3/src/rdfhelpers/labels.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,31 +33,29 @@
 #
 # Cache the values of rdfs:label (and sub-properties thereof) for faster access. Select
 # either all vertices with a label (the default) or customize vertex selection.
 class LabelCache:
     def __init__(self, db, label_query=None, selector=None, language="en", prepopulate=False):
         self.db = db
         self.label_query = label_query or self.LABELQUERY
-        self.selector = selector or "?res ?p ?o"
+        self.selector = selector
         self.language = language
         self._labels = dict()
         self._search_index = collections.defaultdict(set)
         if prepopulate:
             self.repopulate()
 
     LABELQUERY = '''
         SELECT ?r ?label {
+            ?label_prop rdfs:subPropertyOf* rdfs:label .
             $selector
+            $resource ?label_prop ?real_label
             BIND ($resource AS ?r)
-            ?label_prop rdfs:subPropertyOf* rdfs:label
             OPTIONAL { ?r skos:prefLabel ?pref_label }
-            OPTIONAL { ?r skos:altLabel ?alt_label }
-            OPTIONAL { ?r ?label_prop ?real_label }
-            OPTIONAL { ?r dc:title ?other_label }
-            BIND (COALESCE(?pref_label, ?real_label, ?alt_label, ?other_label) AS ?label)
+            BIND (COALESCE(?pref_label, ?real_label) AS ?label)
             FILTER ((str(lang(?label)) = "") || langMatches(lang(?label), "$language"))
         }
         $limit
     '''
 
     ALLLABELSQUERY = '''
         SELECT DISTINCT ?label {
@@ -79,15 +77,15 @@
             resource = URIRef(resource)
         label = self._labels.get(resource, None)
         if label:
             return label
         else:
             label = None
             for _, lb in Templated.query(self.db, self.label_query,
-                                         resource=resource, selector=None, limit="LIMIT 1",
+                                         resource=resource, selector=self.selector, limit="LIMIT 1",
                                          language=self.language):
                 label = lb
                 self.updateSearchIndex(resource, label)
                 break
             if label is None:
                 label = self.makeQName(resource)
             if label is not None:
@@ -145,15 +143,15 @@
 # SKOS CONCEPT LABEL CACHING
 #
 # Similar to regular label caching, but the default selection of vertices includes only the
 # concepts of a specified concept scheme. Also provides a mapping from labels to concepts.
 class SKOSLabelCache(LabelCache):
     def __init__(self, db, scheme, selector=None):
         self._concepts = dict()
-        selector = Templated.convert(selector or "?res skos:broader*/^skos:hasTopConcept $scheme",
+        selector = Templated.convert(selector or "?res skos:broader*/^skos:hasTopConcept $scheme .",
                                      {"scheme": scheme})
         super().__init__(db, selector=selector)
 
     def invalidateLabel(self, resource):
         label = self.getLabel(resource)
         super().invalidateLabel(resource)
         self._concepts[label] = None
```

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/rdfhelpers.py` & `rdfhelpers-0.6.3/src/rdfhelpers/rdfhelpers.py`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers/templated.py` & `rdfhelpers-0.6.3/src/rdfhelpers/templated.py`

 * *Files identical despite different names*

### Comparing `rdfhelpers-0.6.2/src/rdfhelpers.egg-info/PKG-INFO` & `rdfhelpers-0.6.3/src/rdfhelpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdfhelpers
-Version: 0.6.2
+Version: 0.6.3
 Summary: Useful stuff when programming with RDFLib
 Home-page: https://gitlab.com/somanyaircraft/rdfhelpers
 Author-email: ora@somanyaircraft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

