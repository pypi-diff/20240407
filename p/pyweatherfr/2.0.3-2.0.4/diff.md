# Comparing `tmp/pyweatherfr-2.0.3.tar.gz` & `tmp/pyweatherfr-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-2.0.3.tar", last modified: Sat Apr  6 21:22:54 2024, max compression
+gzip compressed data, was "pyweatherfr-2.0.4.tar", last modified: Sun Apr  7 12:27:08 2024, max compression
```

## Comparing `pyweatherfr-2.0.3.tar` & `pyweatherfr-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:22:54.232503 pyweatherfr-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 21:22:54.232503 pyweatherfr-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:22:54.228503 pyweatherfr-2.0.3/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    35183 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:22:54.232503 pyweatherfr-2.0.3/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 21:22:54.000000 pyweatherfr-2.0.3/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:22:54.232503 pyweatherfr-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 21:22:50.000000 pyweatherfr-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36004 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 12:27:08.000000 pyweatherfr-2.0.4/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:27:08.607322 pyweatherfr-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-07 12:26:59.000000 pyweatherfr-2.0.4/setup.py
```

### Comparing `pyweatherfr-2.0.3/LICENSE.txt` & `pyweatherfr-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.3/PKG-INFO` & `pyweatherfr-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.3
+Version: 2.0.4
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.3/README.md` & `pyweatherfr-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.3/pyweatherfr/args.py` & `pyweatherfr-2.0.4/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-2.0.3/pyweatherfr/pyweatherfr.py` & `pyweatherfr-2.0.4/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,16 @@
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         current_weather_code,
         snowfall,
         relative_humidity_2m,
+        sunshine_duration,
+        cloud_cover       
     ) = specific_day(latitude, longitude, compute_args().jour)
     data = []
     for h in range(0, 24):
         warning = ""
         if (
             compute_args().jour == 0
             and 0 < h - int(datetime.datetime.now().strftime("%H")) <= 1
@@ -208,14 +210,15 @@
         pression = f"{surface_pressure[h]:.1f}Hpa"
         if surface_pressure[h] >= WARNING_HP:
             warning = warning + " " + ELEPHANT
         if surface_pressure[h] <= WARNING_BP:
             warning = warning + " " + PLUME
         weather, emojiweather = traduction(current_weather_code[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
+        soleil_nuage = f"{sunshine_duration[h]/60:.0f}% / {cloud_cover[h]:.0f}%"
         if compute_args().nocolor:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -226,14 +229,15 @@
                     weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
+                    soleil_nuage,
                 ]
             )
         else:
             data.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
@@ -246,39 +250,42 @@
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
                     direction,
                     pression,
                     humidity,
+                    soleil_nuage,
                     warning,
                 ]
             )
 
     if compute_args().nocolor:
         headers = [
             "date",
             "temps",
             "température (ressenties)",
             "précipitations",
             "vent (rafales)",
             "direction",
             "pression",
             "humidité",
+            "soleil / nuage"
         ]
     else:
         headers = [
             "date",
             "temps",
             "température (ressenties)",
             "précipitations",
             "vent (rafales)",
             "direction",
             "pression",
             "humidité",
+            "soleil / nuage",            
             "warnings",
         ]
 
     if data != []:
         if compute_args().condensate:
             table = columnar(data, no_borders=True, wrap_max=0)
         else:
@@ -479,19 +486,20 @@
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
         daily_wind_direction_10m_dominant,
         weather_code,
         snowfall,
         precipitation_hours,
+        sunshine_duration,
     ) = resume(latitude, longitude)
     data2 = []
     for i in [0, 1, 2, 3]:
         warning = ""
-        pluie = f"{daily_precipitation_sum[i]:.1f}mm ({precipitation_hours[i]:.1f}h)"
+        pluie = f"{daily_precipitation_sum[i]:.1f}mm"
         if snowfall[i] >= WARNING_SNOW:
             warning = warning + " " + SNOW
         elif daily_precipitation_sum[i] >= WARNING_RAIN:
             warning = warning + " " + RAIN
         temp = f"{daily_temperature_2m_min[i]:.1f}° ({daily_apparent_temperature_min[i]:.1f}°) -> {daily_temperature_2m_max[i]:.1f}° ({daily_apparent_temperature_max[i]:.1f}°)"
         if (
             daily_temperature_2m_min[i] <= WARNING_FROID
@@ -512,15 +520,15 @@
         vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
         direction=calculer_direction(daily_wind_direction_10m_dominant[i])
 
 
         vent = vent
         if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
             warning = warning + " " + WIND
-
+        duree = f"{precipitation_hours[i]:.0f}h / {sunshine_duration[i]/3600:.0f}h"
         if compute_args().nocolor:
             data2.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
                         )
@@ -528,23 +536,25 @@
                         "%Y-%m-%d",
                     ),
                     weather,
                     temp,
                     pluie,
                     vent,
                     direction,
+                    duree
                 ]
             )
             headers = [
                 "date",
                 "temps",
                 "température",
                 "précipitations",
                 "vent (rafales)",
                 "direction",
+                "pluie/soleil"
             ]
         else:
             data2.append(
                 [
                     datetime.datetime.strftime(
                         datetime.datetime.now().replace(
                             hour=0, minute=0, second=0, microsecond=0
@@ -553,24 +563,26 @@
                         "%Y-%m-%d",
                     ),
                     emojiweather + " " + weather,
                     temp,
                     pluie,
                     vent,
                     direction,
+                    duree,
                     warning,
                 ]
             )
             headers = [
                 "date",
                 "temps",
                 "température",
                 "précipitations",
                 "vent (rafales)",
                 "direction",
+                "pluie/soleil",
                 "warning",
             ]
 
     if data2 != []:
         if compute_args().condensate:
             table = columnar(data2, no_borders=True, wrap_max=0)
         else:
@@ -892,15 +904,16 @@
             "apparent_temperature_min",
             "precipitation_sum",
             "wind_speed_10m_max",
             "wind_gusts_10m_max",
             "wind_direction_10m_dominant",
             "weather_code",
             "snowfall_sum",
-            "precipitation_hours"
+            "precipitation_hours",
+            "sunshine_duration"
         ],
     }
     responses = openmeteo.weather_api(url, params=params)
 
     # Process first location. Add a for-loop for multiple locations or weather models
     response = responses[0]
 
@@ -913,28 +926,30 @@
     daily_precipitation_sum = daily.Variables(4).ValuesAsNumpy()
     daily_wind_speed_10m_max = daily.Variables(5).ValuesAsNumpy()
     daily_wind_gusts_10m_max = daily.Variables(6).ValuesAsNumpy()
     daily_wind_direction_10m_dominant = daily.Variables(7).ValuesAsNumpy()
     weather_code = daily.Variables(8).ValuesAsNumpy()
     snowfall = daily.Variables(9).ValuesAsNumpy()
     precipitation_hours= daily.Variables(10).ValuesAsNumpy()
+    sunshine_duration= daily.Variables(11).ValuesAsNumpy()
     date_debut = pd.to_datetime(daily.Time(), unit="s", utc=True)
     return (
         date_debut,
         daily_temperature_2m_min,
         daily_temperature_2m_max,
         daily_apparent_temperature_min,
         daily_apparent_temperature_max,
         daily_precipitation_sum,
         daily_wind_speed_10m_max,
         daily_wind_gusts_10m_max,
         daily_wind_direction_10m_dominant,
         weather_code,
         snowfall,
         precipitation_hours,
+        sunshine_duration
     )
 
 
 def specific_day(latitude, longitude, day):
     cache_session = requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
@@ -952,14 +967,16 @@
             "wind_speed_10m",
             "wind_gusts_10m",
             "wind_direction_10m",
             "pressure_msl",
             "weather_code",
             "snowfall",
             "relative_humidity_2m",
+            "sunshine_duration",
+            "cloud_cover" 
         ],
         "start_date": (datetime.datetime.now() + datetime.timedelta(days=day)).strftime(
             "%Y-%m-%d"
         ),
         "end_date": (
             datetime.datetime.now() + datetime.timedelta(days=day + 1)
         ).strftime("%Y-%m-%d"),
@@ -977,26 +994,30 @@
     hourly_wind_speed_10m = hourly.Variables(3).ValuesAsNumpy()
     hourly_wind_gusts_10m = hourly.Variables(4).ValuesAsNumpy()
     hourly_wind_direction_10m = hourly.Variables(5).ValuesAsNumpy()
     surface_pressure = hourly.Variables(6).ValuesAsNumpy()
     weather_code = hourly.Variables(7).ValuesAsNumpy()
     snowfall = hourly.Variables(8).ValuesAsNumpy()
     relative_humidity_2m = hourly.Variables(9).ValuesAsNumpy()
+    sunshine_duration = hourly.Variables(10).ValuesAsNumpy()
+    cloud_cover = hourly.Variables(11).ValuesAsNumpy()
     return (
         hourly_temperature_2m,
         hourly_apparent_temperature,
         hourly_precipitation,
         hourly_wind_speed_10m,
         hourly_wind_gusts_10m,
         hourly_wind_direction_10m,
         surface_pressure,
         weather_code,
         snowfall,
         relative_humidity_2m,
-    )
+        sunshine_duration,
+        cloud_cover
+                )
 
 
 def current(latitude, longitude):
     cache_session = requests_cache.CachedSession(
         get_user_config_directory_pyweather() + ".cache", expire_after=3600
     )
     retry_session = retry(cache_session, retries=5, backoff_factor=0.2)
```

### Comparing `pyweatherfr-2.0.3/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-2.0.4/pyweatherfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 2.0.3
+Version: 2.0.4
 Summary: pyweatherfr displays weather forecast for a given town in France
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-2.0.3/setup.py` & `pyweatherfr-2.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="2.0.3",
+    version="2.0.4",
     description="pyweatherfr displays weather forecast for a given town in France",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

