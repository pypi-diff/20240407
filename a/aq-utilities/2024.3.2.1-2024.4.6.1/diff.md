# Comparing `tmp/aq_utilities-2024.3.2.1.tar.gz` & `tmp/aq_utilities-2024.4.6.1.tar.gz`

## Comparing `aq_utilities-2024.3.2.1.tar` & `aq_utilities-2024.4.6.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/requirements.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/config/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/config/data.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/__init__.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/psql.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/daily_stations/__init__.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/daily_stations/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/failures/__init__.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/failures/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/hourly_data/__init__.py
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/hourly_data/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/processing/__init__.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/processing/filter_stations.py
--rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/processing/reindex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/stations_info/__init__.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/data/stations_info/psql.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/engine/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/aq_utilities/engine/psql.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/LICENSE.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/README.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aq_utilities-2024.3.2.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/config/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/config/data.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/__init__.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/psql.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/remote.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/test_psql.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/test_remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/__init__.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/failures/__init__.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/failures/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/__init__.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/__init__.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/filter_stations.py
+-rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/reindex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/__init__.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/psql.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/psql.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/test_psql.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/LICENSE.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/PKG-INFO
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/__init__.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from aq_utilities.data.daily_stations.psql import daily_stations_to_postgres, load_daily_stations
 from aq_utilities.data.hourly_data.psql import hourly_predictions_to_postgres
 from aq_utilities.data.hourly_data.psql import hourly_features_to_postgres
 from aq_utilities.data.hourly_data.psql import hourly_data_to_postgres
 from aq_utilities.data.hourly_data.psql import load_hourly_data
 from aq_utilities.data.hourly_data.psql import load_hourly_feature
+from aq_utilities.data.hourly_data.psql import load_hourly_features
 from aq_utilities.data.stations_info.psql import stations_info_to_postgres
 from aq_utilities.data.stations_info.psql import load_stations_info
 from aq_utilities.data.failures.psql import write_failure_to_postgres
 from aq_utilities.data.psql import get_max_timestamp, get_min_timestamp
 from aq_utilities.data.processing.filter_stations import *
 from aq_utilities.data.processing.reindex import *
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/remote.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/remote.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/daily_stations/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/psql.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,21 +81,26 @@
     return 0
 
 
 def load_daily_stations(
     engine: "sqlalchemy.engine.base.Engine",
     table_name: str = "daily_stations",
     query_date: str = "2022-01-01",
-    aqsid: Union[List[str], None] = None,
+    selected_aqsids: Union[List[str], None] = None,
     measurements: Union[List[str], None] = None,
     verbose: bool = False,
 ) -> pd.DataFrame:
     # get the station information for these stations from the database
-    aqsid = ",".join(f"'{s}'" for s in aqsid) if aqsid is not None else None
-    aqsid_override = f" AND d.aqsid IN ({aqsid})" if aqsid is not None else ""
+    if selected_aqsids is not None:
+        assert len(selected_aqsids) > 0, "selected_aqsids must have at least one aqsid if provided"
+        assert isinstance(selected_aqsids, list), "selected_aqsids must be a list"
+        aqsid = ",".join(f"'{s}'" for s in selected_aqsids)
+        aqsid_override = f" AND d.aqsid IN ({aqsid})"
+    else:
+        aqsid_override = ""
     # make a measurements filter if measurements are provided
     measurements = ",".join(f"'{m}'" for m in measurements) if measurements is not None else None
     measurements_override = f" AND d.parameters && ARRAY[{measurements}]" if measurements is not None else ""
     
     query = f"SELECT d.aqsid, d.latitude, d.longitude FROM {table_name} AS d WHERE d.timestamp = '{query_date}'{aqsid_override}{measurements_override} GROUP BY d.aqsid, d.latitude, d.longitude ORDER BY d.aqsid;"
 
     if verbose: print(f"[{datetime.now()}] executing query: {query}")
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/failures/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/failures/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/hourly_data/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/psql.py`

 * *Files 17% similar despite different names*

```diff
@@ -135,21 +135,21 @@
 
 def load_hourly_data(
     engine: "sqlalchemy.engine.base.Engine",
     table_name: str = "hourly_data",
     features: List[str] = ["PM2.5"],
     start_time: str = "2020-01-01",
     end_time: str = "2024-01-01",
-    aqsid_filter: Union[List[str], None] = None,
+    aqsids_filter: Union[List[str], None] = None,
     verbose: bool = False,
 ) -> pd.DataFrame:
     """Load the dataframe from the database."""
     measurements = ",".join(f"'{m}'" for m in features)
-    aqsid_filter = ",".join(f"'{a}'" for a in aqsid_filter) if aqsid_filter is not None else None
-    aqsid_override = f"AND d.aqsid IN ({aqsid_filter})" if aqsid_filter is not None else ""
+    aqsids_filter = ",".join(f"'{a}'" for a in aqsids_filter) if aqsids_filter is not None else None
+    aqsid_override = f"AND d.aqsid IN ({aqsids_filter})" if aqsids_filter is not None else ""
     query = f"SELECT d.aqsid, d.timestamp, d.measurement, d.value FROM {table_name} AS d WHERE d.timestamp >= '{start_time}' AND d.timestamp < '{end_time}' AND d.measurement IN ({measurements}) {aqsid_override} GROUP BY d.aqsid, d.timestamp, d.measurement, d.value ORDER BY d.timestamp;"
 
     if verbose: print(f"[{datetime.now()}] executing query: {query}")
 
     # execute the query
     with engine.connect() as conn:
         query_start = time.time()
@@ -161,36 +161,76 @@
             )
 
     if verbose: print(f"[{datetime.now()}] dataframe shape: {df.shape}")
 
     return df
 
 
+def load_hourly_features(
+    engine: "sqlalchemy.engine.base.Engine",
+    table_name: str = "hourly_features",
+    features: List[str] = ["PM2.5"],
+    start_time: str = "2020-01-01",
+    end_time: str = "2024-01-01",
+    h3_indices_filter: Union[List[str], None] = None,
+    aqsids_filter: Union[List[str], None] = None,
+    verbose: bool = False,
+) -> pd.DataFrame:
+    """Load the dataframe from the database."""
+    # build filter for measurements
+    measurement_filter = ",".join(f"'{m}'" for m in features)
+    # build filter for aqsid (station ids)
+    aqsids_filter = ",".join(f"'{a}'" for a in aqsids_filter) if aqsids_filter is not None else None
+    aqsids_filter_override = f" AND d.aqsid IN ({aqsids_filter})" if aqsids_filter is not None else ""
+    # build filter for h3 index
+    h3_indices_filter = ",".join(f"'{a}'" for a in h3_indices_filter) if h3_indices_filter is not None else None
+    h3_indices_filter_override = f" AND d.h3_index IN ({h3_indices_filter})" if h3_indices_filter is not None else ""
+    
+    # build the query
+    query = f"SELECT d.aqsid, d.h3_index, d.timestamp, d.measurement, d.value FROM {table_name} AS d WHERE d.timestamp >= '{start_time}' AND d.timestamp < '{end_time}' AND d.measurement IN ({measurement_filter}){aqsids_filter_override}{h3_indices_filter_override} GROUP BY d.aqsid, d.h3_index, d.timestamp, d.measurement, d.value ORDER BY d.timestamp;"
+
+    if verbose: print(f"[{datetime.now()}] executing query: {query}")
+
+    # execute the query
+    with engine.connect() as conn:
+        query_start = time.time()
+        df = pd.read_sql_query(text(query), conn)
+        query_end = time.time()
+        if verbose:
+            print(
+                f"[{datetime.now()}] query executed in {query_end - query_start:.2f} seconds"
+            )
+
+    if verbose: print(f"[{datetime.now()}] dataframe shape: {df.shape}")
+
+    return df
+
+
 def load_hourly_feature(
     engine: "sqlalchemy.engine.base.Engine",
     table_name: str = "hourly_features",
     feature: str = "PM2.5",
     start_time: str = "2020-01-01",
     end_time: str = "2024-01-01",
     h3_indices_filter: Union[List[str], None] = None,
     aqsids_filter: Union[List[str], None] = None,
     verbose: bool = False,
 ) -> pd.DataFrame:
     """Load the dataframe from the database."""
     # build filter for measurements
-    measurement_filter = f"'{feature}'"
+    measurement_filter =f"'{feature}'"
     # build filter for aqsid (station ids)
     aqsids_filter = ",".join(f"'{a}'" for a in aqsids_filter) if aqsids_filter is not None else None
     aqsids_filter_override = f" AND d.aqsid IN ({aqsids_filter})" if aqsids_filter is not None else ""
     # build filter for h3 index
     h3_indices_filter = ",".join(f"'{a}'" for a in h3_indices_filter) if h3_indices_filter is not None else None
     h3_indices_filter_override = f" AND d.h3_index IN ({h3_indices_filter})" if h3_indices_filter is not None else ""
     
     # build the query
-    query = f"SELECT d.h3_index, d.timestamp, d.value FROM {table_name} AS d WHERE d.timestamp >= '{start_time}' AND d.timestamp < '{end_time}' AND d.measurement IN ({measurement_filter}){aqsids_filter_override}{h3_indices_filter_override} GROUP BY d.h3_index, d.timestamp, d.measurement, d.value ORDER BY d.timestamp;"
+    query = f"SELECT d.aqsid, d.h3_index, d.timestamp, d.value FROM {table_name} AS d WHERE d.timestamp >= '{start_time}' AND d.timestamp < '{end_time}' AND d.measurement IN ({measurement_filter}){aqsids_filter_override}{h3_indices_filter_override} GROUP BY d.aqsid, d.h3_index, d.timestamp, d.measurement, d.value ORDER BY d.timestamp;"
 
     if verbose: print(f"[{datetime.now()}] executing query: {query}")
 
     # execute the query
     with engine.connect() as conn:
         query_start = time.time()
         df = pd.read_sql_query(text(query), conn)
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/processing/filter_stations.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/processing/filter_stations.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,44 @@
     
     if verbose:
         print(f"[{datetime.now()}] Returning {len(stations_info)} stations.")  
 
     return stations_info
 
 
+def filter_lat_lon_in_bounding_box(
+        stations_info: pd.DataFrame,
+        lat_min: float = 24.9493,
+        lat_max: float = 49.5904,
+        lon_min: float = -125.0011,
+        lon_max: float = 	-66.9326,
+        lat_col_name: str = "latitude",
+        lon_col_name: str = "longitude",
+        verbose: bool = False,
+    ) -> pd.DataFrame:
+    """Filter stations based on lat-lon locations."""
+    if verbose:
+        print(f"[{datetime.now()}] Filtering from {len(stations_info)} stations.")
+
+    # apply the lat-lon bounding box filter
+    if verbose:
+        print(f"[{datetime.now()}] Removing stations outside of the bounding box.")
+    stations_info = stations_info[
+        (stations_info[lat_col_name] >= lat_min) &
+        (stations_info[lat_col_name] <= lat_max) &
+        (stations_info[lon_col_name] >= lon_min) &
+        (stations_info[lon_col_name] <= lon_max)
+    ]
+    
+    if verbose:
+        print(f"[{datetime.now()}] Returning {len(stations_info)} stations.")  
+
+    return stations_info
+
+
 def round_station_lat_lon(
         stations_info: pd.DataFrame,
         round_lat_lon: Union[int, None] = 2,
         lat_col_name: str = "latitude",
         lon_col_name: str = "longitude",
         verbose: bool = False,
     ) -> pd.DataFrame:
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/processing/reindex.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/processing/reindex.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/data/stations_info/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/psql.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,20 +102,25 @@
     return 0
 
 
 def load_stations_info(
     engine: "sqlalchemy.engine.base.Engine",
     table_name: str = "stations_info",
     query_date: str = "2022-01-01",
-    aqsid: Union[List[str], None] = None,
+    selected_aqsids: Union[List[str], None] = None,
     verbose: bool = False,
 ) -> pd.DataFrame:
     # get the station information for these stations from the database
-    aqsid = ",".join(f"'{s}'" for s in aqsid) if aqsid is not None else None
-    aqsid_override = f"AND d.aqsid IN ({aqsid})" if aqsid is not None else ""
+    if selected_aqsids is not None:
+        assert len(selected_aqsids) > 0, "selected_aqsids must have at least one aqsid if provided"
+        assert isinstance(selected_aqsids, list), "selected_aqsids must be a list"
+        aqsid = ",".join(f"'{s}'" for s in selected_aqsids)
+        aqsid_override = f"AND d.aqsid IN ({aqsid})"
+    else:
+        aqsid_override = ""
     query = f"SELECT d.aqsid, d.latitude, d.longitude, d.elevation FROM {table_name} AS d WHERE d.timestamp = '{query_date}' {aqsid_override} GROUP BY d.aqsid, d.latitude, d.longitude, d.elevation ORDER BY d.aqsid;"
 
     if verbose: print(f"[{datetime.now()}] executing query: {query}")
 
     with engine.connect() as conn:
         query_start = time.time()
         df_stations = pd.read_sql_query(text(query), conn)
```

### Comparing `aq_utilities-2024.3.2.1/aq_utilities/engine/psql.py` & `aq_utilities-2024.4.6.1/aq_utilities/engine/psql.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,7 +23,12 @@
             execution_options={"isolation_level": "AUTOCOMMIT"},
             connect_args={"sslmode": "require"},
             pool_size=10,
             max_overflow=10,
             pool_timeout=30,
         )
     return ENGINE
+
+def reset_engine():
+    global ENGINE
+    ENGINE = None
+    return ENGINE
```

### Comparing `aq_utilities-2024.3.2.1/LICENSE.md` & `aq_utilities-2024.4.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.3.2.1/pyproject.toml` & `aq_utilities-2024.4.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-utilities"
-version="2024.3.2.1"
+version="2024.04.06.1"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Data utilities for air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
```

### Comparing `aq_utilities-2024.3.2.1/PKG-INFO` & `aq_utilities-2024.4.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aq-utilities
-Version: 2024.3.2.1
+Version: 2024.4.6.1
 Summary: Data utilities for air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: earth-systems,geometric-deep-learning,graph-neural-networks
 Classifier: License :: OSI Approved :: MIT License
```

