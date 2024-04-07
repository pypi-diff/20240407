# Comparing `tmp/whereabouts-0.3.2.tar.gz` & `tmp/whereabouts-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whereabouts-0.3.2.tar", max compression
+gzip compressed data, was "whereabouts-0.3.3.tar", max compression
```

## Comparing `whereabouts-0.3.2.tar` & `whereabouts-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-12-12 00:22:26.847084 whereabouts-0.3.2/LICENSE
--rw-r--r--   0        0        0     2268 2023-12-12 00:22:26.847084 whereabouts-0.3.2/README.md
--rw-r--r--   0        0        0      463 2024-02-18 05:28:35.358537 whereabouts-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8051 2024-02-11 04:37:10.521583 whereabouts-0.3.2/whereabouts/AddressLoader.py
--rw-r--r--   0        0        0     5767 2024-02-11 02:24:00.537007 whereabouts-0.3.2/whereabouts/GNAFLoader.py
--rw-r--r--   0        0        0     5840 2024-02-18 02:25:40.763083 whereabouts-0.3.2/whereabouts/Matcher.py
--rw-r--r--   0        0        0     1892 2024-01-28 00:12:55.226202 whereabouts-0.3.2/whereabouts/MatcherPipeline.py
--rw-r--r--   0        0        0        0 2024-02-11 01:13:26.602537 whereabouts-0.3.2/whereabouts/__init__.py
--rw-r--r--   0        0        0      522 2024-02-11 10:26:05.011589 whereabouts-0.3.2/whereabouts/__main__.py
--rw-r--r--   0        0        0        0 2024-02-11 06:39:21.341963 whereabouts-0.3.2/whereabouts/models/__init__.py
--rw-r--r--   0        0        0      798 2024-01-17 10:42:09.172003 whereabouts-0.3.2/whereabouts/queries/create_addrtext.sql
--rw-r--r--   0        0        0     1072 2024-01-22 05:56:25.371741 whereabouts-0.3.2/whereabouts/queries/create_geocoder_tables.sql
--rw-r--r--   0        0        0      386 2024-01-27 23:48:15.954411 whereabouts-0.3.2/whereabouts/queries/create_indexes.sql
--rw-r--r--   0        0        0       84 2024-01-22 06:49:42.710580 whereabouts-0.3.2/whereabouts/queries/create_indexes_skipphrase.sql
--rw-r--r--   0        0        0      900 2024-01-09 22:09:52.271511 whereabouts-0.3.2/whereabouts/queries/create_phrases.sql
--rw-r--r--   0        0        0      829 2024-01-22 08:27:20.317973 whereabouts-0.3.2/whereabouts/queries/create_skipphrases.sql
--rw-r--r--   0        0        0      131 2023-12-12 00:22:26.847084 whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step1.sql
--rw-r--r--   0        0        0      440 2024-02-11 00:35:54.729154 whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step2.sql
--rw-r--r--   0        0        0      527 2024-02-02 01:52:41.540482 whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step2b.sql
--rw-r--r--   0        0        0      550 2024-01-05 05:23:30.379820 whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step3.sql
--rw-r--r--   0        0        0      298 2024-01-22 06:49:56.698353 whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step4.sql
--rw-r--r--   0        0        0      847 2023-12-12 00:22:26.847084 whereabouts-0.3.2/whereabouts/queries/create_trigramphrases.sql
--rw-r--r--   0        0        0     4043 2024-01-22 08:19:58.311762 whereabouts-0.3.2/whereabouts/queries/geocoder_query_skipphrase.sql
--rw-r--r--   0        0        0     4402 2024-01-21 12:15:30.954964 whereabouts-0.3.2/whereabouts/queries/geocoder_query_standard.sql
--rw-r--r--   0        0        0     4037 2024-02-18 05:10:37.131220 whereabouts-0.3.2/whereabouts/queries/geocoder_query_standard2.sql
--rw-r--r--   0        0        0     4831 2024-02-01 21:33:25.198306 whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigram.sql
--rw-r--r--   0        0        0     4856 2024-02-01 21:44:58.531696 whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigramb.sql
--rw-r--r--   0        0        0     4479 2024-02-18 05:10:33.742972 whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigramb2.sql
--rw-r--r--   0        0        0      162 2023-12-12 00:22:26.847084 whereabouts-0.3.2/whereabouts/queries/load_addresses.sql
--rw-r--r--   0        0        0      107 2024-01-10 10:03:47.860485 whereabouts-0.3.2/whereabouts/queries/phrase_inverted.sql
--rw-r--r--   0        0        0      117 2024-01-22 08:29:21.699348 whereabouts-0.3.2/whereabouts/queries/skipphrase_inverted.sql
--rw-r--r--   0        0        0     4638 2024-02-18 02:23:48.043121 whereabouts-0.3.2/whereabouts/queries/testing.py
--rw-r--r--   0        0        0     5607 2024-01-22 05:42:54.779020 whereabouts-0.3.2/whereabouts/queries/testing.sql
--rw-r--r--   0        0        0      130 2024-01-22 06:29:21.726251 whereabouts-0.3.2/whereabouts/queries/trigramphrase_inverted.sql
--rw-r--r--   0        0        0     4771 2024-02-11 10:15:35.285776 whereabouts-0.3.2/whereabouts/utils.py
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 whereabouts-0.3.2/setup.py
--rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 whereabouts-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-02 05:09:14.320026 whereabouts-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2758 2024-04-07 00:02:49.532122 whereabouts-0.3.3/README.md
+-rw-r--r--   0        0        0      460 2024-04-07 04:36:50.063158 whereabouts-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8051 2024-03-02 07:08:18.716238 whereabouts-0.3.3/whereabouts/AddressLoader.py
+-rw-r--r--   0        0        0     5767 2024-03-02 05:09:14.321615 whereabouts-0.3.3/whereabouts/GNAFLoader.py
+-rw-r--r--   0        0        0     6024 2024-04-07 01:08:47.529463 whereabouts-0.3.3/whereabouts/Matcher.py
+-rw-r--r--   0        0        0     1892 2024-03-02 05:09:14.321835 whereabouts-0.3.3/whereabouts/MatcherPipeline.py
+-rw-r--r--   0        0        0        0 2024-03-02 05:09:14.321876 whereabouts-0.3.3/whereabouts/__init__.py
+-rw-r--r--   0        0        0      522 2024-03-02 05:09:14.321988 whereabouts-0.3.3/whereabouts/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-02 05:09:14.322676 whereabouts-0.3.3/whereabouts/models/__init__.py
+-rw-r--r--   0        0        0      798 2024-03-02 05:09:14.322852 whereabouts-0.3.3/whereabouts/queries/create_addrtext.sql
+-rw-r--r--   0        0        0     1072 2024-03-02 05:09:14.322950 whereabouts-0.3.3/whereabouts/queries/create_geocoder_tables.sql
+-rw-r--r--   0        0        0      387 2024-03-02 05:09:14.323068 whereabouts-0.3.3/whereabouts/queries/create_indexes.sql
+-rw-r--r--   0        0        0       84 2024-03-02 05:09:14.323185 whereabouts-0.3.3/whereabouts/queries/create_indexes_skipphrase.sql
+-rw-r--r--   0        0        0      900 2024-03-02 05:09:14.323299 whereabouts-0.3.3/whereabouts/queries/create_phrases.sql
+-rw-r--r--   0        0        0      829 2024-03-02 05:09:14.323393 whereabouts-0.3.3/whereabouts/queries/create_skipphrases.sql
+-rw-r--r--   0        0        0      131 2024-03-02 05:09:14.323485 whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step1.sql
+-rw-r--r--   0        0        0      440 2024-03-02 05:09:14.323576 whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step2.sql
+-rw-r--r--   0        0        0      527 2024-03-09 04:06:11.104110 whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step2b.sql
+-rw-r--r--   0        0        0      550 2024-03-02 05:09:14.323806 whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step3.sql
+-rw-r--r--   0        0        0      298 2024-03-02 05:09:14.323904 whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step4.sql
+-rw-r--r--   0        0        0      847 2024-03-02 05:09:14.324037 whereabouts-0.3.3/whereabouts/queries/create_trigramphrases.sql
+-rw-r--r--   0        0        0     4043 2024-03-02 05:09:14.324196 whereabouts-0.3.3/whereabouts/queries/geocoder_query_skipphrase.sql
+-rw-r--r--   0        0        0     4402 2024-03-02 05:09:14.324298 whereabouts-0.3.3/whereabouts/queries/geocoder_query_standard.sql
+-rw-r--r--   0        0        0     4037 2024-03-02 05:09:14.324387 whereabouts-0.3.3/whereabouts/queries/geocoder_query_standard2.sql
+-rw-r--r--   0        0        0     4831 2024-03-02 05:09:14.324469 whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigram.sql
+-rw-r--r--   0        0        0     4856 2024-03-02 05:09:14.324555 whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigramb.sql
+-rw-r--r--   0        0        0     4479 2024-03-02 05:09:14.324657 whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigramb2.sql
+-rw-r--r--   0        0        0      107 2024-03-02 05:09:14.324880 whereabouts-0.3.3/whereabouts/queries/phrase_inverted.sql
+-rw-r--r--   0        0        0      117 2024-03-02 05:09:14.324965 whereabouts-0.3.3/whereabouts/queries/skipphrase_inverted.sql
+-rw-r--r--   0        0        0      130 2024-03-02 05:09:14.325054 whereabouts-0.3.3/whereabouts/queries/trigramphrase_inverted.sql
+-rw-r--r--   0        0        0     5355 2024-04-07 04:33:57.516233 whereabouts-0.3.3/whereabouts/utils.py
+-rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 whereabouts-0.3.3/PKG-INFO
```

### Comparing `whereabouts-0.3.2/LICENSE` & `whereabouts-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/README.md` & `whereabouts-0.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,28 @@
 Once Poetry is installed and you are in the project directory:
 
 ```
 poetry shell
 poetry install
 ```
 
+## Create a geocoder database
+To start geocoding, a geocoding database has to be created, which uses a reference dataset containing addresses and corresponding latitude, longitude values.
+
+The reference file should be a single csv file with at least three fields: the complete address, latitude, longitude. These fields should be specified in a `setup.yml` file. An example is included.
+
+Once the `setup.yml` is created and a reference dataset is available, the geocoding database can be created using the `setup_geocoder` function from whereabouts.utils.
+
 The current process for using Australian data from the GNAF is as follows:
 1) Download the latest version of GNAF core from https://geoscape.com.au/data/g-naf-core/
 2) Update the `setup.yml` file to point to the location of the GNAF core file
 3) Finally, setup the geocoder. This creates the required reference tables
 
 ```
-python setup_geocoder.py
+python -m whereabouts setup_geocoder setup.yml
 ```
 
 To use address data from another country, the file should have the following columns:
 
 | Column name | Description |
 | ----------- | ----------- |
 | ADDRESS_DETAIL_PID | Unique identifier for address |
@@ -41,16 +48,14 @@
 | ADDRESS_SITE_NAME | Name of the site. This is usually null |
 | LOCALITY_NAME | Name of the suburb or locality |
 | POSTCODE | Postcode of address |
 | STATE | State 
 | LATITUDE | Latitude of geocoded address |
 | LONGITUDE | Longitude of geocoded address |
 
-Note that by default the file should be pipe-separated, i.e., use '|' as the delimitor.
-
 ## Examples
 
 Geocode a list of addresses 
 ```
 from whereabouts.Matcher import Matcher
 
 matcher = Matcher(db_name='gnaf_au')
```

### Comparing `whereabouts-0.3.2/whereabouts/AddressLoader.py` & `whereabouts-0.3.3/whereabouts/AddressLoader.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/GNAFLoader.py` & `whereabouts-0.3.3/whereabouts/GNAFLoader.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/Matcher.py` & `whereabouts-0.3.3/whereabouts/Matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,24 +50,26 @@
         Args
         ----
         db_name (str): name of database
         how (str): geocoding type to use
         threshold (float): when to classify geocoded result as a match 
         """
         # check that model is in folder
-        path_to_models = importlib.resources.path('whereabouts', '') / 'models'
-        path_to_models = str(path_to_models)
+        with importlib.resources.path('whereabouts', '') as whereabouts_path:
+            path_to_models = Path(whereabouts_path) / 'models'
 
         db_names = os.listdir(path_to_models)
-        db_names = [db_name[:-3] for db_name in db_names]
+        db_names = [db_name[:-3] for db_name in db_names if db_name[-3:] == '.db']
         if db_name in db_names:
             self.con = duckdb.connect(database=f'{path_to_models}/{db_name}.db')
         else:
             print(f"Could not find database {db_name}")
-
+            print(f"The following geocoding databases are installed:")
+            for db_name in db_names:
+                print(f'{db_name}')
         try:    
             self.con.create_function('list_overlap', list_overlap)
             self.con.create_function('numeric_overlap', numeric_overlap)
             self.con.create_function('ngram_jaccard', ngram_jaccard)
         except:
             pass
       #  self.tree = KDTree(self.reference_data[['latitude', 'longitude']].values)
```

### Comparing `whereabouts-0.3.2/whereabouts/MatcherPipeline.py` & `whereabouts-0.3.3/whereabouts/MatcherPipeline.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/__main__.py` & `whereabouts-0.3.3/whereabouts/__main__.py`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_addrtext.sql` & `whereabouts-0.3.3/whereabouts/queries/create_addrtext.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_geocoder_tables.sql` & `whereabouts-0.3.3/whereabouts/queries/create_geocoder_tables.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_phrases.sql` & `whereabouts-0.3.3/whereabouts/queries/create_phrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_skipphrases.sql` & `whereabouts-0.3.3/whereabouts/queries/create_skipphrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step2b.sql` & `whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step2b.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_trigram_index_step3.sql` & `whereabouts-0.3.3/whereabouts/queries/create_trigram_index_step3.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/create_trigramphrases.sql` & `whereabouts-0.3.3/whereabouts/queries/create_trigramphrases.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_skipphrase.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_skipphrase.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_standard.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_standard.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_standard2.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_standard2.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigram.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigram.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigramb.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigramb.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/queries/geocoder_query_trigramb2.sql` & `whereabouts-0.3.3/whereabouts/queries/geocoder_query_trigramb2.sql`

 * *Files identical despite different names*

### Comparing `whereabouts-0.3.2/whereabouts/utils.py` & `whereabouts-0.3.3/whereabouts/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess 
 import requests 
 import yaml
 import os
 from .AddressLoader import AddressLoader
 import importlib.resources
+from time import time
 
 def get_unmatched(results, threshold):
     """
     Given results (outputs from Matcher), filter out those that are correctly matched and
     those that are not.
     """
     # unmatched are those below threshold in similarity value
@@ -73,15 +74,19 @@
         db_name = details['data']['db_name']
         db_folder = details['data']['folder']
         states = details['geocoder']['states']
         matchers = details['geocoder']['matchers']
     except:
         print("Some details missing from configuration file")
 
+
+    t1 = time()
+    print("Creating reference database")
     # create the database
+    db_name += '.db'
     addressloader = AddressLoader(db_name)
     
     print("Create geocoder tables")
     addressloader.create_geocoder_tables()
     if states:
         for state in states:
             addressloader.load_data(details, state_names=[state])
@@ -115,31 +120,44 @@
     addressloader.export_database(db_folder)
 
     # delete the old db file
     os.remove(db_name)
 
     print("Importing database")
     del(addressloader)
-    path_to_model = importlib.resources.path('whereabouts', '') / 'models'
+    path_to_model = importlib.resources.files('whereabouts') / 'models'
     path_to_model = str(path_to_model)
 
     addressloader = AddressLoader(f'{path_to_model}/{db_name}')
     addressloader.import_database(db_folder)
     
     # remove all files created in export of db
     for filename in os.listdir(db_folder):
         os.remove(f'{db_folder}/{filename}')
     os.rmdir(db_folder)
+    t2 = time()
+    printf(f'Created reference database in {t2-t1}s.')
 
 def remove_database(db_name):
     """
     Remove a database from the folder of databases
 
     db_name (str): title of database (without the extension of folder path)
     """
-    path_to_model = importlib.resources.path('whereabouts', '') / 'models'
+    path_to_model = importlib.resources.files('whereabouts') / 'models'
     path_to_model = str(path_to_model)
     all_dbs = os.listdir(path_to_model)
     if f'{db_name}.db' in all_dbs:
         os.remove(f'{path_to_model}/{db_name}.db')
     else:
         print(f"Could not database with name {db_name}")
+
+def list_databases():
+    """
+    List all the reference databases that have been installed
+    """
+    path_to_models = importlib.resources.files('whereabouts') / 'models'
+    path_to_models = str(path_to_models)
+    all_dbs = [filename[:-4] for filename in os.listdir(path_to_models if filename.endswith('.db'))]
+    print('The following reference databases are installed')
+    for db in all_dbs:
+        print(db)
```

### Comparing `whereabouts-0.3.2/PKG-INFO` & `whereabouts-0.3.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whereabouts
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: alex2718
 Author-email: ajlee3141@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: duckdb (==0.9.2)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: duckdb (==0.10.0)
 Requires-Dist: fastparquet (>=2023.7.0,<2024.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openpyxl (>=3.1.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pyarrow (==14.0.1)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Whereabouts
@@ -41,21 +42,28 @@
 Once Poetry is installed and you are in the project directory:
 
 ```
 poetry shell
 poetry install
 ```
 
+## Create a geocoder database
+To start geocoding, a geocoding database has to be created, which uses a reference dataset containing addresses and corresponding latitude, longitude values.
+
+The reference file should be a single csv file with at least three fields: the complete address, latitude, longitude. These fields should be specified in a `setup.yml` file. An example is included.
+
+Once the `setup.yml` is created and a reference dataset is available, the geocoding database can be created using the `setup_geocoder` function from whereabouts.utils.
+
 The current process for using Australian data from the GNAF is as follows:
 1) Download the latest version of GNAF core from https://geoscape.com.au/data/g-naf-core/
 2) Update the `setup.yml` file to point to the location of the GNAF core file
 3) Finally, setup the geocoder. This creates the required reference tables
 
 ```
-python setup_geocoder.py
+python -m whereabouts setup_geocoder setup.yml
 ```
 
 To use address data from another country, the file should have the following columns:
 
 | Column name | Description |
 | ----------- | ----------- |
 | ADDRESS_DETAIL_PID | Unique identifier for address |
@@ -63,16 +71,14 @@
 | ADDRESS_SITE_NAME | Name of the site. This is usually null |
 | LOCALITY_NAME | Name of the suburb or locality |
 | POSTCODE | Postcode of address |
 | STATE | State 
 | LATITUDE | Latitude of geocoded address |
 | LONGITUDE | Longitude of geocoded address |
 
-Note that by default the file should be pipe-separated, i.e., use '|' as the delimitor.
-
 ## Examples
 
 Geocode a list of addresses 
 ```
 from whereabouts.Matcher import Matcher
 
 matcher = Matcher(db_name='gnaf_au')
```

