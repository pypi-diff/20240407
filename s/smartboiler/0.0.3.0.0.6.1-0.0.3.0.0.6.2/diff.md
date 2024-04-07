# Comparing `tmp/smartboiler-0.0.3.0.0.6.1.tar.gz` & `tmp/smartboiler-0.0.3.0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.6.1.tar", last modified: Sat Apr  6 09:20:04 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.6.2.tar", last modified: Sun Apr  7 19:17:51 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.6.1.tar` & `smartboiler-0.0.3.0.0.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.836211 smartboiler-0.0.3.0.0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.836211 smartboiler-0.0.3.0.0.6.1/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/src/smartboiler/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/src/smartboiler/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/web_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-06 09:20:02.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:20:04.840211 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 09:20:04.000000 smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-07 19:17:49.000000 smartboiler-0.0.3.0.0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.461532 smartboiler-0.0.3.0.0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36881 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22887 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36915 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42745 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-07 19:17:48.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:17:51.465532 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 19:17:51.000000 smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.6.1/PKG-INFO` & `smartboiler-0.0.3.0.0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.6.1
+Version: 0.0.3.0.0.6.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.6.1/README.md` & `smartboiler-0.0.3.0.0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/setup.py` & `smartboiler-0.0.3.0.0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.6.1',  # Required
+    version='0.0.3.0.0.6.2',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/boiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
         len_of_df = len(prediction_of_consumption)
 
         for i in range(len_of_df, 0, -1):
             time_to_consumption_minutes = (i * 60) - 30
 
             sum_of_consumption = (
-                prediction_of_consumption.iloc[:i].sum().values[0]
+                sum(prediction_of_consumption[:i])
                 - boiler_kWh_above_set
             ) + self.get_kWh_loss_in_time(time_minutes=time_to_consumption_minutes, tmp_act=tmp_act) 
 
             unavailible_minutes = actual_schedule.iloc[:i]["unavailable_minutes"].sum()
             time_needed_to_heat = (
                 self.time_needed_to_heat_up_minutes(consumption_kWh=sum_of_consumption)
             )
```

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/command_line.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/command_line.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/data_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,31 +152,30 @@
             "measurement": "°C",
         },
         "boiler_relay_status": {
             "sql_query": f'SELECT last("value") AS "boiler_relay_status" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "entity_id"=\'{self.relay_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(null)',
             "measurement": "state",
         },
         "device_longitude": {
-            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(linear)',
+            "sql_query": f'SELECT mean("longitude") AS "mean_longitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
             "measurement": "state",
         },
         "device_latitude": {
-            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(linear)',
+            "sql_query": f'SELECT mean("latitude") AS "mean_latitude" FROM "{self.db_name}"."autogen"."state" WHERE time > {left_time_interval} AND time <= {right_time_interval} AND "domain"=\'device_tracker\' AND "entity_id"=\'{self.device_tracker_entity_id}\' GROUP BY time({group_by_time_interval}) FILL(previous)',
             "measurement": "state",
         },
         
     } 
 
     def haversine_dist(self, x1, x2, y1, y2):
         return haversine((x1, x2), (y1, y2), unit="km")
 
     # Data Processing
 
     def extract_features_from_longitude_latitude(self, df_old):
-        home_coords = (self.home_latitude, self.home_longitude)
         #drop na in columns mean_latitude and mean_longitude
         df = df_old.copy()
         
         df = df.dropna(subset=["mean_latitude", "mean_longitude"])
         df.loc[:,"distance_from_home"] = np.vectorize(self.haversine_dist)(
             df["mean_latitude"],
             df["mean_longitude"],
@@ -221,16 +220,16 @@
         result = self.dataframe_client.query(query)
         return result
 
     def get_df_from_queries(self, queries):
         df_all_list = []
         # iterate over key an value in data
         for key, value in queries.items():
-            # get data from influxdb
 
+            # print(value["sql_query"])
             result = self.dataframe_client.query(value["sql_query"])[
                 value["measurement"]
             ]
             df = pd.DataFrame(result)
             df_all_list.append(df)
 
         df = pd.concat(df_all_list, axis=1)
@@ -241,15 +240,15 @@
         df = df.resample("1min").mean()
         # df = df.reset_index(drop=True)
         df["consumed_heat_kJ"] = (
             df["water_flow_L_per_minute_mean"]
             * (df["water_temperature_mean"] - 10)
             * 4.186
             * 0.6
-        )
+        )  
 
         df = self.extract_features_from_longitude_latitude(df)
         # all value in speed larger than 200 set to 0
         df.loc[df["speed"] > 200, "speed"] = 0
 
         df = df.groupby(pd.Grouper(freq="60T"))
         df = df.agg(
@@ -304,26 +303,24 @@
         queries = self.get_database_queries(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
         df_all = self.get_df_from_queries(queries)
         df_all = self.process_kWh_water_consumption(df_all)
         df_all.index = df_all.index.tz_localize(None)
-        df_all, _ = self.transform_data_for_ml(df_all, predicted_column="longtime_mean")
+        df_all, datetimes = self.transform_data_for_ml(df_all, predicted_column="longtime_mean")
 
-        return df_all
+        return df_all, datetimes
 
-    def write_forecast_to_influxdb(self, df, measurement_name):
+    def write_forecast_to_influxdb(self, forecast_list, measurement_name):
         current_time = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
 
-        df.index = df.index.astype(str)
 
-        # Create dictionary
-        result_dict = df.squeeze().to_dict()
-        print(f'Writing forecast to influxdb: {result_dict}')
+       # create a dict from list with keys from 0
+        result_dict = dict(enumerate(forecast_list, 0))
         # Create a dictionary
         measurement_dict = {
             "measurement": "prediction",
             "time": current_time,
             "fields": result_dict,
         }
 
@@ -377,15 +374,15 @@
 
         df.loc[:, "weekday"] = df.index.weekday
         df.loc[:, "hour"] = df.index.hour
         # df.loc[:, "minute"] = df.index.minute
         df.loc[:, "minute"] = 0
 
         # delete rows with weekday nan
-        df = df.dropna(subset=["weekday"])
+        # df = df.dropna(subset=["weekday"])
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].fillna(0)
 
         # fill negative values with 0
         df["consumed_heat_kWh"] = df["consumed_heat_kWh"].clip(lower=0)
 
         # fill na in df based on column
         df["temperature"] = df[f"outside_temperature_mean"].fillna(method="ffill")
@@ -425,61 +422,65 @@
         df['last_3_week_max'] = df['last_3_week_max'].fillna(method='ffill')
         
         df['last_3_week_min'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).min().reset_index(level=[0,1], drop=True)
         df['last_3_week_min'] = df['last_3_week_min'].fillna(method='ffill')
         
         df['last_3_week_skew'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).skew().reset_index(level=[0,1], drop=True)
         df['last_3_week_skew'] = df['last_3_week_skew'].fillna(method='ffill')
+        #fill 
         
         df['last_3_week_median'] = df.groupby([df.index.weekday, df.index.hour])['consumed_heat_kWh'].rolling(window=3, min_periods=1).median().reset_index(level=[0,1], drop=True)
         df['last_3_week_median'] = df['last_3_week_median'].fillna(method='ffill') 
         
+        
+        
+        df_reverse = df.iloc[::-1]
+
+        nan_indices = df_reverse[df_reverse['last_3_week_skew'].isna()].index
+
+        for index in nan_indices:
+
+            rolling_skew = df_reverse.loc[index:, 'consumed_heat_kWh'].rolling(window=3, min_periods=1).skew()
+            rolling_std = df_reverse.loc[index:, 'consumed_heat_kWh'].rolling(window=3, min_periods=1).std()
+            df_reverse.loc[index:, 'last_3_week_skew'] = np.where(df_reverse.loc[index:, 'last_3_week_skew'].isna(), rolling_skew, df_reverse.loc[index:, 'last_3_week_skew'])
+            df_reverse.loc[index:, 'last_3_week_std'] = np.where(df_reverse.loc[index:, 'last_3_week_std'].isna(), rolling_std, df_reverse.loc[index:, 'last_3_week_std'])
+
+        df['last_3_week_skew'] = df_reverse['last_3_week_skew'].iloc[::-1]
+        df['last_3_week_std'] = df_reverse['last_3_week_std'].iloc[::-1]
+        
+        
         df = df.drop(columns=["consumed_heat_kWh"])
         # transform weekday, minute, hour to sin cos
         df["weekday_sin"] = np.sin(2 * df["weekday"] * np.pi / 7)
         df["weekday_cos"] = np.cos(2 * df["weekday"] * np.pi / 7)
 
         df["hour_sin"] = np.sin(2 * df["hour"] * np.pi / 24)
         df["hour_cos"] = np.cos(2 * df["hour"] * np.pi / 24)
 
         df["minute_sin"] = np.sin(2 * df["minute"] * np.pi / 60)
         df["minute_cos"] = np.cos(2 * df["minute"] * np.pi / 60)
 
         df = df[
             [
                 "longtime_mean",
-                
-                
-                # "last_3_week_mean",
-                # "last_3_week_median",
                 "last_3_week_skew",
                 "last_3_week_std",
-                # "last_3_week_min",
-                # "last_3_week_max",
-                
-                
-                # "longtime_min",
-                # "longtime_max",
                 "distance_from_home",
-                # # "speed",
                 "speed_towards_home",
                 "count",
                 "heading_to_home_sin",
                 "heading_to_home_cos",
-                # "mean_latitude",
-                # "mean_longitude",
-                # "temperature",
-                # "humidity",
-                # "wind_speed",
+                "temperature",
+                "humidity",
+                "wind_speed",
                 "weekday_sin",
                 "weekday_cos",
                 "hour_sin",
                 "hour_cos",
-                "minute_sin",
-                "minute_cos",
+
             ]
         ]
         # df = df[
         #     [
         #         predicted_column,
         #         "weekday_sin",
         #         "weekday_cos",
```

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/forecast.py`

 * *Files 16% similar despite different names*

```diff
@@ -199,52 +199,52 @@
         SS_res = K.sum(K.square(y_true - y_pred))
         SS_tot = K.sum(K.square(y_true - K.mean(y_true)))
         return 1 - SS_res / (SS_tot + K.epsilon())
 
     def build_model(self):
 
         model = Sequential()
-        model.add(Input(shape=(None, 13)))
-
+        model.add(Input(shape=(None, 14)))       
+     
         # Add LSTM layer
         model.add(LSTM(100))
         model.add(Dense(1))
 
         self.model = model
         self.model.compile(loss="mae", optimizer="adam")
         return model
 
-    def fit_model(self):
-        pass
 
-        # self.model.save(self.model_path)
 
     def add_empty_row(self, df, date_time, predicted_value):
 
         last_row_values = df.iloc[-1].values
+        prev_week_values = df.iloc[-24 * 7].values
 
         new_row_df = pd.DataFrame(
             columns=df.columns,
             data=[
                 [
-                    predicted_value,
-                    last_row_values[1],
-                    last_row_values[2],
-                    last_row_values[3],
-                    last_row_values[4],
-                    last_row_values[5],
-                    last_row_values[6],
-                    last_row_values[7],
+                    predicted_value,# longtime_mean
+                    prev_week_values[1], # 3 week skew
+                    prev_week_values[2], # 3 weeak std
+                    last_row_values[3], # distance_from_home
+                    last_row_values[4], # speed_towards_home
+                    last_row_values[5], # count
+                    last_row_values[6], # heading to home sin
+                    last_row_values[7], # heading to home cos
+                    last_row_values[8], # temperature
+                    last_row_values[9], # humidity
+                    last_row_values[10], # wind_speed
                     
                     np.sin(2 * np.pi * date_time.weekday() / 7),
                     np.cos(2 * np.pi * date_time.weekday() / 7),
                     np.sin(2 * np.pi * date_time.hour / 24),
                     np.cos(2 * np.pi * date_time.hour / 24),
-                    np.sin(2 * np.pi * date_time.minute / 60),
-                    np.cos(2 * np.pi * date_time.minute / 60),
+
                 ]
             ],
         )
         df = pd.concat([df, new_row_df], ignore_index=True)
         df = df.reset_index(drop=True)
 
         return df
@@ -310,89 +310,101 @@
     ):
         # Define the indices for the different predictions and truths
         if left_time_interval is None:
             left_time_interval = datetime.now() - timedelta(days=30)
         if right_time_interval is None:
             right_time_interval = datetime.now()
 
-        forecast_future = pd.DataFrame()
-
-        df_all = self.dataHandler.get_data_for_prediction(
+        df_all, datetimes = self.dataHandler.get_data_for_prediction(
             left_time_interval=left_time_interval,
             right_time_interval=right_time_interval,
         )
 
         num_targets = len(self.predicted_columns)
         len_columns = len(df_all.columns)
         forecast_future = pd.DataFrame()
 
         # print last row of df all
 
-        forecast_future = pd.DataFrame()
-        
+        forecast_future = []
+            
         current_forecast_begin_date = right_time_interval + timedelta(hours=1)
-
+        
         df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
         current_forecast_begin_date += timedelta(hours=1)
 
         # prediction for next 6 hours
         for i in range(0, 6):
 
-                        
-            df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
-            current_forecast_begin_date += timedelta(hours=1)
-
-            df_test_norm = df_all.reset_index(drop=True).dropna().copy()
+            df_test_norm = df_all.reset_index(drop=True).copy()
 
             # df_test_norm = df_test_zuka.copy()
             df_test_norm[df_test_norm.columns] = self.scaler.transform(df_test_norm)
-
+            
+            
+            
+            df_test_norm = df_test_norm[-self.lookback*4:]
             test_gen = self.mul_generator(
                 dataframe=df_test_norm,
                 target_names=self.predicted_columns,
                 lookback=self.lookback,
                 delay=self.delay,
                 min_index=0,
                 max_index=None,
                 step=1,
                 shuffle=False,
-                batch_size=df_test_norm.shape[0],
+                batch_size=self.batch_size,
             )
             
-            (X, y_truth) = next(test_gen)
+            last_batch = next(test_gen)
+
+            # Step 3: Extract the last batch of features (X_batch) and target values (y_truth_batch)
+            (X_batch, y_truth) = last_batch
+            
             
+
+            # Step 4: Make predictions with your model on the last batch
             num_targets = len(self.predicted_columns)
             len_columns = len(df_test_norm.columns)
             num_features = len_columns - num_targets
             
-            y_pred = self.model.predict(X, verbose=0)
+            y_truth_concat = np.concatenate(
+                (y_truth, np.zeros((y_truth.shape[0], num_features))), axis=1
+            )
+            y_truth_concat = self.scaler.inverse_transform(y_truth_concat)
+            
+            y_truth_inv = y_truth_concat[-1, 0]
+            
+            y_pred = self.model.predict(X_batch, verbose=0)
             y_pred_inv = np.concatenate(
                 (y_pred, np.zeros((y_pred.shape[0], num_features))), axis=1
             )
 
             y_pred_inv = self.scaler.inverse_transform(y_pred_inv)
             # get last predicted value
             y_pred_inv = y_pred_inv[-1, 0]
             # y_pred_inv[0] is min 0
             if y_pred_inv < 0:
                 y_pred_inv = 0
+                
+            if (i == 0):
+                print("y_pred_inv: ", y_pred_inv)
+                print("y_truth_inv: ", y_truth_inv)
 
             # set last longtimemean value
-            df_all.iloc[-2, df_all.columns.get_loc("longtime_mean")] = y_pred_inv
+            df_all.iloc[-1, df_all.columns.get_loc("longtime_mean")] = y_pred_inv
 
             # df_all = df_all[1:]
 
-            forecast_future = pd.concat(
-                [
-                    forecast_future,
-                    df_all.iloc[[-2], df_all.columns.get_loc("longtime_mean")],
-                ],
-                axis=0,
-            )
-            forecast_future = forecast_future.reset_index(drop=True)
+            forecast_future.append(y_pred_inv)
+            
+            
+            df_all = self.add_empty_row(df_all, current_forecast_begin_date, 0)
+            current_forecast_begin_date += timedelta(hours=1)
+            
         # create a dataframe with forecast and datetime as index
         self.dataHandler.write_forecast_to_influxdb(
             forecast_future, "prediction_longtime_mean"
         )
         return forecast_future
 
 
@@ -404,9 +416,8 @@
         "root",
         "shelly1pm_34945475a969",
         "esphome_web_c771e8_tmp3",
     )
     forecast = Forecast(dataHandler)
     forecast.train_model()
     forecast.build_model()
-    forecast.fit_model()
     forecast.get_forecast_next_steps(30)
```

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/machine_learning_forecaster.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/optimization.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/optimization.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/static/style.css` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/static/style.css`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/templates/index.html` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/templates/index.html`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/utils.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/utils.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/web_server.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/web_server.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.6.1
+Version: 0.0.3.0.0.6.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.6.1/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.6.2/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

