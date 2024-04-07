# Comparing `tmp/avrotize-1.0.2.tar.gz` & `tmp/avrotize-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.0.2.tar` & `avrotize-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    18924 2024-04-03 18:00:30.051725 avrotize-1.0.2/README.md
--rw-r--r--   0        0        0       65 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-03 18:00:38.623702 avrotize-1.0.2/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/asn1toavro.py
--rw-r--r--   0        0        0     9463 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotize.py
--rw-r--r--   0        0        0    18100 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotoproto.py
--rw-r--r--   0        0        0     9514 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12136 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91241 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-03 18:00:30.051725 avrotize-1.0.2/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15532 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-03 18:00:30.055725 avrotize-1.0.2/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-03 18:00:30.055725 avrotize-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    19591 1970-01-01 00:00:00.000000 avrotize-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    18924 2024-04-07 09:39:19.835150 avrotize-1.0.3/README.md
+-rw-r--r--   0        0        0      924 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-07 09:39:23.979235 avrotize-1.0.3/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0     9463 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotize.py
+-rw-r--r--   0        0        0    18100 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0     9514 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12136 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91241 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15532 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-07 09:39:19.835150 avrotize-1.0.3/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-07 09:39:19.839150 avrotize-1.0.3/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-07 09:39:19.839150 avrotize-1.0.3/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-07 09:39:19.839150 avrotize-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    19591 1970-01-01 00:00:00.000000 avrotize-1.0.3/PKG-INFO
```

### Comparing `avrotize-1.0.2/README.md` & `avrotize-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/asn1toavro.py` & `avrotize-1.0.3/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotize.py` & `avrotize-1.0.3/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotojsons.py` & `avrotize-1.0.3/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotokusto.py` & `avrotize-1.0.3/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotoparquet.py` & `avrotize-1.0.3/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotoproto.py` & `avrotize-1.0.3/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrototsql.py` & `avrotize-1.0.3/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/avrotoxsd.py` & `avrotize-1.0.3/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/common.py` & `avrotize-1.0.3/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/dependency_resolver.py` & `avrotize-1.0.3/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/generic/generic.avsc` & `avrotize-1.0.3/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/jsonstoavro.py` & `avrotize-1.0.3/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/kconnect.json` & `avrotize-1.0.3/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/kstructtoavro.py` & `avrotize-1.0.3/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/proto2parser.py` & `avrotize-1.0.3/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/proto3parser.py` & `avrotize-1.0.3/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototoavro.py` & `avrotize-1.0.3/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/any.avsc` & `avrotize-1.0.3/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/api.avsc` & `avrotize-1.0.3/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/duration.avsc` & `avrotize-1.0.3/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/field_mask.avsc` & `avrotize-1.0.3/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/struct.avsc` & `avrotize-1.0.3/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/timestamp.avsc` & `avrotize-1.0.3/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/type.avsc` & `avrotize-1.0.3/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/prototypes/wrappers.avsc` & `avrotize-1.0.3/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/avrotize/xsdtoavro.py` & `avrotize-1.0.3/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/pyproject.toml` & `avrotize-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.0.2/PKG-INFO` & `avrotize-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

