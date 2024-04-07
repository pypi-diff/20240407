# Comparing `tmp/seastate-0.1.2.tar.gz` & `tmp/seastate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seastate-0.1.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `seastate-0.1.2.tar` & `seastate-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,36 @@
--rw-r--r--   0        0        0     1060 2022-06-27 10:51:31.498468 seastate-0.1.2/LICENSE
--rw-r--r--   0        0        0     2077 2022-07-18 07:40:58.086363 seastate-0.1.2/README.md
--rw-r--r--   0        0        0      631 2022-07-18 11:11:18.450226 seastate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-27 10:51:31.498685 seastate-0.1.2/seastate/__init__.py
--rw-r--r--   0        0        0        0 2022-06-27 10:51:31.498755 seastate-0.1.2/seastate/api/__init__.py
--rw-r--r--   0        0        0     3418 2022-07-17 13:35:36.630402 seastate-0.1.2/seastate/api/api_mediator.py
--rw-r--r--   0        0        0     5506 2022-07-17 13:30:06.972999 seastate-0.1.2/seastate/api/datasources.py
--rw-r--r--   0        0        0    10694 2022-07-17 13:31:37.245098 seastate-0.1.2/seastate/api/noaa_ndbc.py
--rw-r--r--   0        0        0     4131 2022-07-17 13:32:08.245487 seastate-0.1.2/seastate/api/noaa_tidesandcurrents.py
--rw-r--r--   0        0        0     4250 2022-07-17 14:23:04.436778 seastate-0.1.2/seastate/api/rest_adapter.py
--rw-r--r--   0        0        0       44 2022-06-30 18:27:04.326653 seastate-0.1.2/seastate/exceptions.py
--rw-r--r--   0        0        0     1997 2022-07-17 13:36:01.913313 seastate-0.1.2/seastate/models.py
--rw-r--r--   0        0        0     4710 2022-07-17 17:43:53.743787 seastate-0.1.2/seastate/seastate.py
--rw-r--r--   0        0        0      826 2022-07-16 17:56:52.087262 seastate-0.1.2/seastate/utils.py
--rw-r--r--   0        0        0     2927 2022-07-18 11:11:29.767532 seastate-0.1.2/setup.py
--rw-r--r--   0        0        0     2946 2022-07-18 11:11:29.767783 seastate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 seastate-0.2.0/.flake8
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 seastate-0.2.0/Makefile
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 seastate-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/exceptions.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/models.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/settings.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/__init__.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/api_mediator.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/base.py
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/noaa_ndbc.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/noaa_tidesandcurrents.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/rest_adapter.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/__init__.py
+-rw-r--r--   0        0        0   179607 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/noaa_ndbc.json
+-rw-r--r--   0        0        0    96988 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/noaa_tidesandcurrents.json
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/factories.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_seastate.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_seastate_regression.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_api_mediator.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_noaa_ndbc.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_noaa_tidesandcurrents.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_rest_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/test___init__.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/test_parsers.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 seastate-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 seastate-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 seastate-0.2.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 seastate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 seastate-0.2.0/PKG-INFO
```

### Comparing `seastate-0.1.2/LICENSE` & `seastate-0.2.0/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ivo
+Copyright (c) 2024 Ivo Rivetta
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `seastate-0.1.2/README.md` & `seastate-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,114 @@
-# Seastate
+# seastate
 
 ## Summary
+
 Collect ocean measurement data based on location and timeframe
 
 **Features**
+
 - Closest active station is selected for each measurement
 - Reaches into secondary historical archives when required
-- Returns pandas dataframe compatible lists
+- Returns pandas dataframe compatible dictionaries
 - Available measurements: Tide, wind, water temp, air temp, air pressure, conductivity and swell information
 - Datasources: NOAA NDBC, NOAA Tides and Currents
 
 ## Installing
+
 `pip install seastate`
 
 ## Quick start
+
 ```
-from seastate.seastate import SeaState
+from seastate import SeaState
 from datetime import datetime
 
 # make SeaState object for specific location
 san_diego = SeaState(32,-117)
 
 # retrieve measurements for today
-san_diego_today = san_diego.measurements_from_date_range(datetime.today())
+san_diego_today = san_diego.from_date_range(datetime.today())
 
-san_diego_today['tide'] -> [{t: time, v: value, s: stdev]
+san_diego_today['tide'] -> [{t: time, v: value, s: stdev}]
 san_diego_today['wind']-> [{t: time, v: value, d: direction, g: gust}]
 san_diego_today['water_temp']-> [{t: time, v: value}]
 san_diego_today['air_temp']-> [{t: time, v: value}]
 san_diego_today['air_press']-> [{t: time, v: value}]
 san_diego_today['wave']-> [{t: time, v: Wave Height, dpd: Dominant Period, mwd: dpd Direction}]
-san_diego_today['conductivity']-> [{t: time, v: value}] 
+san_diego_today['conductivity']-> [{t: time, v: value}]
 ```
+
 Measurement details for NDBC are [here](https://www.ndbc.noaa.gov/measdes.shtml) and for Tides and Currents [here](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html)
 
+## API reference
+
+Useful metadata can be accessed through the SeaState object
+
+```
+san_diego = SeaState(32,-117)
+
+# Each measurement has an entry point
+san_diego.tide
+-> (api.mediator Object)
+
+# The valid keys are:
+valid_measurements = {
+    'tide',
+    'wind',
+    'water_temp',
+    'air_temp',
+    'air_press',
+    'wave',
+    'conductivity',
+}
+
+
+# the original lat/lon are available
+san_diego.lat
+-> 32
+san_diego.tide._target_lon
+-> 32
+
+# the distance of each measurement station to target gps
+san_diego.tide.distance
+-> xyz kilometers
+
+# and other useful exposed api keys
+san_diego.tide.station.name
+san_diego.tide.station.id
+san_diego.tide.station.lat
+san_diego.tide.station.lon
+
+```
+
 ## Measurement x API breakdown
-| Measurement | T&C | NDBC |
-| ---: | :---: | :---: |
-|tide | y | y |
-|wind | y | y |
-|water_temp | y | y |
-|air_temp | y | y |
-|air_press | y | y |
-|wave |  | y |
-|conductivity | y |  |
+
+|  Measurement | T&C | NDBC |
+| -----------: | :-: | :--: |
+|         tide |  y  |  y   |
+|         wind |  y  |  y   |
+|   water_temp |  y  |  y   |
+|     air_temp |  y  |  y   |
+|    air_press |  y  |  y   |
+|         wave |     |  y   |
+| conductivity |  y  |      |
 
 ## More Examples
+
 ### Measurements for past 30 days
+
 ```
-from seastate.seastate import SeaState
+from seastate import SeaState
 from datetime import datetime, timedelta
 
 start = datetime.today()-timedelta(days=30)
 end = datetime.today()
 san_diego_past_30 = san_diego.measurements_from_date_range(start,end)
 ```
+
 ### Hourly Slices
+
 ```
 san_diego_past_30_hourly = san_diego.hourly(start,end) # this returns a single reading per hour
 # experimental feature
 # no guarantee between APIs that readings will align or exist in all cases
 ```
```

### Comparing `seastate-0.1.2/seastate/api/api_mediator.py` & `seastate-0.2.0/seastate/api/api_mediator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,132 @@
+from typing import Union
 from dataclasses import field
 import logging
 
-from seastate.api.datasources import DataSources
+from seastate.data import STATIONS
 from seastate.exceptions import SeaStateException
 from seastate.models import Station
 from seastate.utils import haversine
+from seastate.api.base import BaseApi
+from seastate.api.noaa_ndbc import NdbcApi
+from seastate.api.noaa_tidesandcurrents import TidesAndCurrentsApi
+from abc import ABC, abstractmethod
+
+
+class BaseMediator(ABC):
+    """Implements utils for finding nearest station and API for that station"""
+
+    def __init__(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def station(self) -> Station:
+        pass
+
+    @abstractmethod
+    def api(self) -> BaseApi:
+        pass
+
+    @abstractmethod
+    def distance(self) -> float:
+        pass
 
-class ApiMediator:
-    def __init__(self, measurement: str, lat: float, lon: float, exclude: list = field(default_factory=list), ssl_verify: bool = True, logger: logging.Logger = None):
-        """Constructor for configured api endpoint based on measurement type, gps coordinates and exclude filters 
-        """
-        self._ssl_verify = ssl_verify
-        self._logger = logger or logging.getLogger(__name__)
-        self._target_lat = lat
-        self._target_lon = lon
-        self.exclude = exclude
-        self.measurement = measurement
-        self.station = self.nearest_station() # nearest_station handles the selection logic
-        self.api = self.station.api
-        self.distance = haversine(self._target_lat,self._target_lon, self.station.lat, self.station.lon)
-        
-    ## Properties
     @property
-    def _target_lat(self):
+    def _target_lat(self) -> None:
         return self.__target_lat
-    
+
     @_target_lat.setter
-    def _target_lat(self,value):
-        #  Latitudes are in range of -90 to 90
+    def _target_lat(self, value) -> None:
+        #  Latitudes exist in range of -90 to 90
         if -90 <= value <= 90:
             self.__target_lat = value
         else:
             raise SeaStateException("Latitude must be between -90 and 90 degrees")
-    
+
     @property
-    def _target_lon(self):
+    def _target_lon(self) -> None:
         return self.__target_lon
-    
+
     @_target_lon.setter
-    def _target_lon(self,value):
-        #  Longitudes are in range of -180 to 180
+    def _target_lon(self, value) -> None:
+        #  Longitudes exist in range of -180 to 180
         if -180 <= value <= 180:
             self.__target_lon = value
         else:
             raise SeaStateException("Longitude must be between -180 and 180 degrees")
 
-    # # Methods
-    def nearest_station(self) -> Station:
-        # if measurement
-        # Return dict of stations
-        # n<2000 so just return them all
-        try:
-            # Grab all stations
-            stations = DataSources().all()
-        except (KeyError) as e:
-            raise SeaStateException("Error retrieving stations") from e
-
-        # Find station closest to input coordinates using haversine
-        # and is active for specified measurement
-        min_ptr = float('inf') # Initialize minimum pointer
-        for eval_station in stations:
+    def _nearest_station(self) -> Station:
+        """
+        Find station that:
+        - is closest to input coordinates using haversine method
+        - is collecting the measurement at present (active)
+        """
+        station = None
+        min_ptr = float("inf")  # Initialize minimum pointer at inf
+        for eval_station in STATIONS:
             # skip if station is in exclude list
             if eval_station.id in self.exclude:
                 continue
             # skip if eval_station is inactive
             if not eval_station.is_active:
                 continue
             # skip if station does not support measurement
             if not eval_station.is_supported(self.measurement):
                 continue
             # compute distance between SeaState target coords and current station
-            new_val = haversine(self._target_lat, self._target_lon, eval_station.lat, eval_station.lon)
+            new_val = haversine(
+                self._target_lat, self._target_lon, eval_station.lat, eval_station.lon
+            )
             # if closer, update new minimum
             if new_val < min_ptr:
                 min_ptr = new_val
                 station = eval_station
         return station
 
 
+class ApiMediator(BaseMediator):
+    """_summary_"""
 
-if __name__ == '__main__':
-    api = ApiMediator('Tide',32,-117) # testing San Diego for tide
+    def __init__(
+        self,
+        measurement: str,
+        lat: float,
+        lon: float,
+        exclude: list = field(default_factory=list),
+        logger: logging.Logger = None,
+    ):
+        self._target_lat = lat
+        self._target_lon = lon
+        self.measurement = measurement
+        self.exclude = exclude
+        # self._register_mediator(self)
+        self._logger = logger or logging.getLogger(__name__)
+
+    @property
+    def station(self) -> Station:
+        return self._nearest_station()
+
+    @property
+    def api(self) -> Union[NdbcApi, TidesAndCurrentsApi]:
+        if self.station.api == "noaa_ndbc":
+            return NdbcApi()
+        elif self.station.api == "noaa_tidesandcurrents":
+            return TidesAndCurrentsApi()
+        else:
+            raise SeaStateException("Unsupported API")
+
+    @property
+    def distance(self) -> float:
+        return haversine(
+            self._target_lat, self._target_lon, self.station.lat, self.station.lon
+        )
+
+
+if __name__ == "__main__":
+    api = ApiMediator("Tide", 32, -117)  # testing San Diego for tide
     # Station should have tide as a valid measurement
     assert api.station.tide
     assert api.station.is_supported(api.measurement)
     # out of bound lat/lon should throw errors
-    
-    # testing wind
-    api = ApiMediator('Wind',32,-117) # testing San Diego for tide
 
+    # testing wind
+    api = ApiMediator("Wind", 32, -117)  # testing San Diego for tide
```

### Comparing `seastate-0.1.2/seastate/api/datasources.py` & `seastate-0.2.0/seastate/data/parsers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,139 @@
+import json
 import logging
+from dataclasses import asdict
 from typing import List
 
 import defusedxml.minidom
+
 from seastate.api.noaa_ndbc import NdbcApi
 from seastate.api.noaa_tidesandcurrents import TidesAndCurrentsApi
 from seastate.api.rest_adapter import RestAdapter
 from seastate.exceptions import SeaStateException
 from seastate.models import Station
 
 
-class DataSources:
+class StationParser:
     def __init__(self, logger: logging.Logger = None):
         self._logger = logger or logging.getLogger(__name__)
-        
-    def all(self) -> List[Station]:
-        """Convenience function for all stations
 
-        Returns:
-            List[Station]: _description_
-        """
-        stations = self.ndbc_stations()
-        stations += self.tides_and_currents_stations()
-        return stations
-    
-    def ndbc_stations(self) -> List[Station]:
-        """Parse a text table
+    @staticmethod
+    def from_jsons(jsons: str) -> List[Station]:
+        """Parses a json string into a list of Station objects"""
+        return [Station(**x) for x in json.loads(jsons)]
+
+    @staticmethod
+    def to_jsons(stations: List[Station]) -> str:
+        """Parses a list of Station object into a json str"""
+        return json.dumps([asdict(x) for x in stations])
 
-        Returns:
-            List[Station]: _description_
+    def noaa_ndbc(self) -> List[Station]:
+        """
+        Calls the ndbc endpoint
+        summarizes all observations and parses the station metadata
         """
         # todo: refactor this spaghetti code
         # check station status by retrieving latest measurements from all stations
-        result = RestAdapter('www.ndbc.noaa.gov/').get('data/latest_obs/latest_obs.txt')
-        
+        result = RestAdapter("www.ndbc.noaa.gov/").get("data/latest_obs/latest_obs.txt")
+
         # loop through text lines and test if station is ouputting specified measurement
         stations = []
-        for i, value in enumerate(result.data.split('\n')):
+        for i, value in enumerate(result.data.split("\n")):
             # skipping 2 header lines
             if i == 0 or i == 1:
-                continue #skip header and unit lines
-            
+                continue  # skip header and unit lines
+
             # split current line by delimiter and clear empty values
-            line = value.split(' ')    
-            while ' ' in line:
-                line.remove(' ')
-            while '' in line:
-                line.remove('')
-            
+            line = value.split(" ")
+            while " " in line:
+                line.remove(" ")
+            while "" in line:
+                line.remove("")
+
             # skip corrupted lines
             if len(line) != 22:
                 self._logger.info("No station info in this line: " + str(line))
                 continue
 
             # parse stationID, gps, and confirm active measurement sources
             # 'MM' is NOAA's notation for missing measurement
-            temp_station = {
-                'id': line[0],
-                'lat': float(line[1]),
-                'lon': float(line[2]),
-                'api': NdbcApi(),
-                'tide': True if line[21] != 'MM' else False,
-                'wind': True if line[8] != 'MM' else False,
-                'water_temp': True if line[18] != 'MM' else False,
-                'air_temp': True if line[17] != 'MM' else False,
-                'air_press': True if line[15] != 'MM' else False,
-                'wave': True if line[11] != 'MM' else False,
+            tmp_station = {
+                "id": line[0],
+                "lat": float(line[1]),
+                "lon": float(line[2]),
+                "api": NdbcApi().id,
+                "tide": True if line[21] != "MM" else False,
+                "wind": True if line[8] != "MM" else False,
+                "water_temp": True if line[18] != "MM" else False,
+                "air_temp": True if line[17] != "MM" else False,
+                "air_press": True if line[15] != "MM" else False,
+                "wave": True if line[11] != "MM" else False,
             }
-            
+
             # construct station with temp var
-            stations.append(Station(**temp_station))
-        
+            stations.append(Station(**tmp_station))
+
         # return list of stations
         return stations
 
-    def tides_and_currents_stations(self) -> List[Station]:
-        """Parse xml doc
-
-        Raises:
-            SeaStateException: _description_
-
-        Returns:
-            List[Station]: _description_
+    def noaa_tidesandcurrents(self) -> List[Station]:
+        """
+        Calls the tnc endpoint
+        summarizes all stations and parses their metadata
         """
         # todo: refactor this spaghetti code
         # TidesAndCurrent station capabilities are kept here
-        result = RestAdapter('opendap.co-ops.nos.noaa.gov/').get('stations/stationsXML.jsp')
-        
+        result = RestAdapter("opendap.co-ops.nos.noaa.gov/").get(
+            "stations/stationsXML.jsp"
+        )
+
         # parse xml elements safely with defusedxml -> []
         dom = defusedxml.minidom.parseString(result.data)
-        station_elements = dom.getElementsByTagName('station')
-        
+        station_elements = dom.getElementsByTagName("station")
+
         # traverse station elements to build Station objects
         stations = []
         for line in station_elements:
-            temp_station = {}
+            tmp_station = {}
             # parse station metadata into temporary dict
             try:
-                temp_station['name'] = line.getAttribute('name')
-                temp_station['id'] = line.getAttribute('ID')
-                temp_station['lat'] = float(line.getElementsByTagName('lat')[0].firstChild.nodeValue)
-                temp_station['lon'] = float(line.getElementsByTagName('long')[0].firstChild.nodeValue)
-                temp_station['api'] = TidesAndCurrentsApi()
-            except (IndexError) as e:
+                tmp_station["name"] = line.getAttribute("name")
+                tmp_station["id"] = line.getAttribute("ID")
+                tmp_station["lat"] = float(
+                    line.getElementsByTagName("lat")[0].firstChild.nodeValue
+                )
+                tmp_station["lon"] = float(
+                    line.getElementsByTagName("long")[0].firstChild.nodeValue
+                )
+                tmp_station["api"] = TidesAndCurrentsApi().id
+            except IndexError as e:
                 # Faulty station, skip station node
                 self._logger.warn(e + str(line))
                 continue
-            
+
             # separate loop to parse individual measurements
-            for m in line.getElementsByTagName('parameter'):
-                name = m.attributes['name'].value
-                status = True if m.attributes['status'].value == '1' else False
-                if 'Water Level' in name and status:
-                    temp_station['tide'] = True
-                elif 'Winds' in name and status:
-                    temp_station['wind'] = True
+            for m in line.getElementsByTagName("parameter"):
+                name = m.attributes["name"].value
+                status = True if m.attributes["status"].value == "1" else False
+                if "Water Level" in name and status:
+                    tmp_station["tide"] = True
+                elif "Winds" in name and status:
+                    tmp_station["wind"] = True
                     # todo: wind dir and gust may or may not be true
-                elif 'Air Temp' in name and status:
-                    temp_station['air_temp'] = True
-                elif 'Water Temp' in name and status:
-                    temp_station['water_temp'] = True
-                elif 'Air Pressure' in name and status:
-                    temp_station['air_press'] = True
-                elif 'Conductivity' in name and status:
-                    temp_station['conductivity'] = True
+                elif "Air Temp" in name and status:
+                    tmp_station["air_temp"] = True
+                elif "Water Temp" in name and status:
+                    tmp_station["water_temp"] = True
+                elif "Air Pressure" in name and status:
+                    tmp_station["air_press"] = True
+                elif "Conductivity" in name and status:
+                    tmp_station["conductivity"] = True
 
             # construct station with temp var
-            stations.append(Station(**temp_station))
-            
+            stations.append(Station(**tmp_station))
+
         # Check parsing was succesful
         if len(stations) == 0:
-            raise SeaStateException("No stations successfully parsed, please submit issue")
+            raise SeaStateException(
+                "No stations successfully parsed, please submit issue"
+            )
         return stations
-
-if __name__ == '__main__':
-    tnc = DataSources().tides_and_currents_stations()
-    ndbc = DataSources().ndbc_stations()
```

### Comparing `seastate-0.1.2/seastate/api/noaa_ndbc.py` & `seastate-0.2.0/seastate/api/noaa_ndbc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 import logging
 from datetime import datetime, timedelta
-from typing import Dict, List
+from typing import Dict, Union
 
+from seastate.api.base import BaseApi
 from seastate.api.rest_adapter import RestAdapter
 from seastate.exceptions import SeaStateException
+from seastate.models import Result
 
-class NdbcApi:
-    def __init__(self, api_key: str = '', ssl_verify: bool = True, logger: logging.Logger = None):
-        """Constructor for NdbcApi, composed with RestAdapter 
-
-        Args:
-            api_key (str, optional): Not used here. Defaults to ''.
-            ssl_verify (bool, optional): Defaults to True.
-            logger (logging.Logger, optional): Pass explictly else will be created with __name__.
-        """
+
+class NdbcApi(BaseApi):
+    def __init__(self, logger: logging.Logger = None):
+        """Constructor for NdbcApi, composed with RestAdapter"""
         self._logger = logger or logging.getLogger(__name__)
-        self._rest_adapter = RestAdapter('www.ndbc.noaa.gov', api_key, ssl_verify, logger)
-        
-    def measurements_from_date_range(self, measurement:str, station_id:str, start:datetime, end: datetime) -> List[Dict]:
-        """Returns Result for stationID and datetime start and end
-
-        Args:
-            station (str): station ID.
-            start (datetime): start datetime.
-            end (datetime): end datetime.
-
-        Raises:
-            SeaStateException: _description_
-
-        Returns:
-            Result: _description_
-        """
-        # todo refactor this spaghetti code
+        self._adapter = RestAdapter("www.ndbc.noaa.gov")
+
+    def _build_parse_key(self, measurement: str = None) -> Union[str, list[str], None]:
         measurement = measurement.lower()
-        if 'tide' in measurement:
-            measurement_key = ['TIDE']
-        elif 'wind' in measurement:
-            measurement_key = ['WSPD','SPD']
+        if "tide" in measurement:
+            key = ["TIDE"]
+        elif "wind" in measurement:
+            key = ["WSPD", "SPD"]
             # additional wind information handled when unpacking
-        elif 'water_temp' in measurement:
-            measurement_key = ['WTMP']
-        elif 'air_temp' in measurement:
-            measurement_key = ['ATMP']
-        elif 'air_press' in measurement:
-            measurement_key = ['PRES','BARO','BAR']
-        elif 'wave' in measurement:
-            measurement_key = ['WVHT','H0']
+        elif "water_temp" in measurement:
+            key = ["WTMP"]
+        elif "air_temp" in measurement:
+            key = ["ATMP"]
+        elif "air_press" in measurement:
+            key = ["PRES", "BARO", "BAR"]
+        elif "wave" in measurement:
+            key = ["WVHT", "H0"]
             # additional swell information handled when unpacking
-        elif 'conductivity' in measurement:
-            raise SeaStateException("Unsupported measurement requested, please report issue")
+        elif "conductivity" in measurement:
+            raise SeaStateException(
+                "Unsupported measurement requested, please report issue"
+            )
         else:
-            raise SeaStateException("Unsupported measurement requested, please report issue")
-        
+            raise SeaStateException(
+                "Unsupported measurement requested, please report issue"
+            )
+        return key
+
+    def _build_endpoint(
+        self, measurement: str, station_id: str, start: datetime, end: datetime
+    ) -> (str, Dict):
         # Collect endpoints needed to cover daterange
         endpoints = []
         # daterange spans realtime endpoint (45 days)
         archive_cutoff_date = datetime.today() - timedelta(days=45)
         if start > archive_cutoff_date or end > archive_cutoff_date:
             # "realtime" endpoint covers prev 45 days
             endpoints += [f"data/realtime2/{station_id}.txt"]
@@ -69,157 +60,217 @@
             # use January if start year precedes the archive cutoff year
             # else use start month
             start_range = 1 if start.year < archive_cutoff_date.year else start.month
             # end of range will be up to cutoff
             # duplicates to be filtered downstream
             end_range = archive_cutoff_date.month
             # Endpoint uses month number and abbreviated month designations (%b)
-            requested_months = [(str(x), datetime(1,x,1).strftime("%b")) for x in range(start_range,end_range)]
-            endpoints += [f"view_text_file.php?filename={station_id}{x}{datetime.today().year}.txt.gz&dir=data/stdmet/{y}/" for x, y in requested_months]
+            requested_months = [
+                (str(x), datetime(1, x, 1).strftime("%b"))
+                for x in range(start_range, end_range)
+            ]
+            endpoints += [
+                f"view_text_file.php?filename= \
+                    {station_id}{x}{datetime.today().year} \
+                        .txt.gz&dir=data/stdmet/{y}/"
+                for x, y in requested_months
+            ]
         # daterange spans prior years
-        # 
+        #
         if start < archive_cutoff_date and start.year < datetime.today().year:
             # if end year is this year, handled upstream
             # else, it is a prior year and needs to be included
             end_range = end.year if end.year == datetime.today().year else end.year + 1
-            requested_years = [str(x) for x in range(start.year,end_range)]
-            endpoints += [f"view_text_file.php?filename={station_id}h{x}.txt.gz&dir=data/historical/stdmet/" for x in requested_years]
+            requested_years = [str(x) for x in range(start.year, end_range)]
+            endpoints += [
+                f"view_text_file.php?filename= \
+                    {station_id}h{x} \
+                        .txt.gz&dir=data/historical/stdmet/"
+                for x in requested_years
+            ]
+        return endpoints, None
+
+    def _parse_result(
+        self, result: list[Result], start: datetime, end: datetime, measurement: str
+    ) -> list[Dict]:
+        # unpack list of results to text
+        tmp = ""
+        for res in result:
+            tmp += res.data
 
-        result = ''
-        for endpoint in endpoints:
-            try:
-                res = self._rest_adapter.get(endpoint=endpoint)
-            except (SeaStateException) as e:
-                self._logger.warning(f"{str(e)} for {endpoint}")
-                continue
-            result += res.data
-                
-        
         # unpack text result
         # realtime ndbc reports are a text file with previous 45 days of measurements
         # archival are a years worth
         # todo: unpack text file into t: and v:
         data = []
-        for i, value in enumerate(result.split('\n')):
+        for i, value in enumerate(tmp.split("\n")):
             # turn str to list
-            # known anomaly: 2 space characters sometimes delimiting 
-            line = value.replace('  ', ' ').split(' ')
-            while ' ' in line:
-                line.remove(' ') #remove blanks
-            while '' in line:
-                line.remove('') #remove blanks
-            
+            # known anomaly: 2 space characters sometimes delimiting
+            line = value.replace("  ", " ").split(" ")
+            while " " in line:
+                line.remove(" ")  # remove blanks
+            while "" in line:
+                line.remove("")  # remove blanks
+
             # handle corrupted lines
             if len(line) == 0:
                 self._logger.info(f"ignoring line #{i}:{str(line)}")
                 continue
-            
+
             # handle header lines
-            if line[0] in ['#YY', 'YY']:
+            if line[0] in ["#YY", "YY"]:
                 # header row starts with #YY in realtime, YY in archive
                 header = line
                 # strip '#' from '#YY'
-                header[0] = header[0].strip('#')
+                header[0] = header[0].strip("#")
                 continue
-            elif line[0] in ['#yr']:
+            elif line[0] in ["#yr"]:
                 # skipping units line
                 continue
 
-            
             # ignore lines outside of daterange
             # archive files sometimes use 95 instead of 1995
-            if not (start.year <= int(line[0]) <= end.year) and not (abs(start.year % 100) <= int(line[0]) <= abs(end.year % 100)):
+            if not (start.year <= int(line[0]) <= end.year) and not (
+                abs(start.year % 100) <= int(line[0]) <= abs(end.year % 100)
+            ):
                 # 4 digit year representation
                 continue
             if not start.month <= int(line[1]) <= end.month:
                 continue
             if not start.day <= int(line[2]) <= end.day:
                 continue
-            
+
             # line is in requested daterange
             # parse timestamp
             timestamp = datetime(
-                year=int(line[0] if len(line[0])==4 else '19' + line[0]), #rebuild dates with archive format
+                year=int(
+                    line[0] if len(line[0]) == 4 else "19" + line[0]
+                ),  # rebuild dates with archive format
                 month=int(line[1]),
                 day=int(line[2]),
                 hour=int(line[3]),
-                minute=int(line[4] if 'mm' in header else 0) # archival format is hourly
-                ).isoformat(sep= ' ')
+                minute=int(
+                    line[4] if "mm" in header else 0
+                ),  # archival format is hourly
+            ).isoformat(sep=" ")
             # parse measurement column
             # because of changes in the source api column names over the years
             # we try to unpack with the possible variants
             # details here: https://www.ndbc.noaa.gov/measdes.shtml
             temp_data = {}
             # unpack time and main value
-            for key in measurement_key:
+            for key in self._build_parse_key(measurement):
                 try:
-                    temp_data['t'] = timestamp
-                    temp_data['v'] = line[header.index(key)]
-                except (KeyError, ValueError) as e:
+                    temp_data["t"] = timestamp
+                    temp_data["v"] = line[header.index(key)]
+                except (KeyError, ValueError):
                     pass
             # check for success before continuing
             if len(temp_data) < 2:
                 self._logger.error(value)
                 raise SeaStateException("NdbcApi unpacking error, please report issue")
             # wind sometimes has direction and gust data
-            if 'wind' in measurement:
+            if "wind" in measurement:
                 # for wind direction:
-                for key in ['WDIR', 'WD','DIR']:
+                for key in ["WDIR", "WD", "DIR"]:
                     try:
                         temp = line[header.index(key)]
-                        temp_data['d'] = temp if temp and '999' not in temp and 'MM' not in temp else None # 999 for direction
+                        temp_data["d"] = (
+                            temp
+                            if temp and "999" not in temp and "MM" not in temp
+                            else None
+                        )  # 999 for direction
                     except Exception as e:
                         self._logger.debug(f"{e} for {measurement}")
                 # For wind gust:
-                for key in ['GST', 'GSP']:
+                for key in ["GST", "GSP"]:
                     try:
                         temp = line[header.index(key)]
-                        temp_data['g'] = temp if temp and '99' not in temp and 'MM' not in temp else None # 99 for decimal
+                        temp_data["g"] = (
+                            temp
+                            if temp and "99" not in temp and "MM" not in temp
+                            else None
+                        )  # 99 for decimal
                     except Exception as e:
                         self._logger.debug(f"{e} for {measurement}")
             # wave sometimes has period and direction
-            if 'wave' in measurement:
+            if "wave" in measurement:
                 # for dominant wave period:
-                for key in ['DPD','DOMPD']:
+                for key in ["DPD", "DOMPD"]:
                     try:
                         temp = line[header.index(key)]
-                        temp_data['dpd'] = temp if temp and '99' not in temp and 'MM' not in temp else None  # 99 for decimal
+                        temp_data["dpd"] = (
+                            temp
+                            if temp and "99" not in temp and "MM" not in temp
+                            else None
+                        )  # 99 for decimal
                     except Exception as e:
                         self._logger.debug(f"{e} for {measurement}")
                 # For dominant wave direction:
-                for key in ['MWD']:
+                for key in ["MWD"]:
                     try:
                         temp = line[header.index(key)]
-                        temp_data['mwd'] = temp if temp and '999' not in temp and 'MM' not in temp else None # 999 for direction
+                        temp_data["mwd"] = (
+                            temp
+                            if temp and "999" not in temp and "MM" not in temp
+                            else None
+                        )  # 999 for direction
                     except Exception as e:
                         self._logger.debug(f"{e} for {measurement}")
                 # For average wave period
-                for key in ['APD','AVP']:
+                for key in ["APD", "AVP"]:
                     try:
                         temp = line[header.index(key)]
-                        temp_data['apd'] = temp if temp and '99' not in temp and 'MM' not in temp else None
+                        temp_data["apd"] = (
+                            temp
+                            if temp and "99" not in temp and "MM" not in temp
+                            else None
+                        )
                     except Exception as e:
                         self._logger.debug(f"{e} for {measurement}")
             data.append(temp_data)
-            
+
         # log warning if no data recovered for daterange
         if len(data) == 0:
-            self._logger.warning(f"No {measurement} data recovered for daterange: {str(start.date())} : {str(end.date())}")
+            self._logger.warning(
+                f"No {measurement} data recovered for daterange:\
+                    {str(start.date())} : {str(end.date())}"
+            )
 
         # todo: scrub duplicates between cutoff month and realtime
         return data
 
-        
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     api = NdbcApi()
     # check daterange within realtime
-    # result = api.hourly('wind',46224,datetime.today(),datetime.today()-timedelta(days=2))
-    
+    # result = api.hourly(
+    #     "wind",
+    #     46224,
+    #     datetime.today(),
+    #     datetime.today() - timedelta(days=2),
+    # )
+
     # check daterange for request only in prior years
-    # result = api.hourly('wind',46224,datetime.today()-timedelta(days=2*365+30),datetime.today()-timedelta(days=1*365+30))
+    # result = api.hourly(
+    #     "wind",
+    #     46224,
+    #     datetime.today() - timedelta(days=2 * 365 + 30),
+    #     datetime.today() - timedelta(days=1 * 365 + 30),
+    # )
 
     # check daterange spanning archive and realtime, into prior year
-    # result = api.hourly('wind',46224,datetime.today()-timedelta(days=365+30),datetime.today())
-    
+    # result = api.hourly(
+    #     "wind",
+    #     46224,
+    #     datetime.today() - timedelta(days=365 + 30),
+    #     datetime.today(),
+    # )
+
     # check old archive with different headers
     # check date format
-    result = api.hourly('air_press',42040,datetime(1996,2,1),datetime(1996,2,2))
+    result = api.hourly(
+        "air_press",
+        42040,
+        datetime(1996, 2, 1),
+        datetime(1996, 2, 2),
+    )
```

### Comparing `seastate-0.1.2/seastate/api/noaa_tidesandcurrents.py` & `seastate-0.2.0/seastate/api/noaa_tidesandcurrents.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,101 @@
 import logging
 from datetime import datetime
-from typing import Dict, List
+from typing import Dict, Union
 
+from seastate.api.base import BaseApi
 from seastate.api.rest_adapter import RestAdapter
 from seastate.exceptions import SeaStateException
+from seastate.models import Result
 
-class TidesAndCurrentsApi:
-    def __init__(self, api_key: str = '', ssl_verify: bool = True, logger: logging.Logger = None):
-        """Constructor for TidesAndCurrentsApi, composed with RestAdapter 
-
-        Args:
-            api_key (str, optional): Not used here. Defaults to ''.
-            ssl_verify (bool, optional): Defaults to True.
-            logger (logging.Logger, optional): Pass explictly else will be created with __name__.
-        """
+
+class TidesAndCurrentsApi(BaseApi):
+    def __init__(self, logger: logging.Logger = None):
+        """Constructor for TidesAndCurrentsApi, composed with RestAdapter"""
         self._logger = logger or logging.getLogger(__name__)
-        self._rest_adapter = RestAdapter('api.tidesandcurrents.noaa.gov', api_key, ssl_verify, logger)
-        
-    def measurements_from_date_range(self, measurement:str, station_id:str, start:datetime, end: datetime) -> List[Dict]:
-        """Returns Result for station ID and datetime start and end. Args should be validated externally
-
-        Args:
-            measurement (str): measurement type can be tide|wind|water_temp|air_temp|air_press|conductivity|tide_prediction.
-            station_id (str): Station ID.
-            start (datetime): start datetime.
-            end (datetime): end datetime.
-
-        Raises:
-            SeaStateException: _description_
-
-        Returns:
-            Result: _description_
-        """
-        
-        # each measurement type will have a different endpoint "product" param and key to unpack response
+        self._adapter = RestAdapter("api.tidesandcurrents.noaa.gov")
+
+    def _build_parse_key(self, measurement: str = None) -> Union[str, list[str], None]:
+        return "data"
+
+    def _build_endpoint(
+        self, measurement: str, station_id: str, start: datetime, end: datetime
+    ) -> (str, Dict):
+        # each measurement type will have a different endpoint "product" param
         # always test str on lowercase casting
         measurement = measurement.lower()
-        if 'tide' in measurement:
-            product = 'water_level'
-            measurement_key = 'data'
-        elif 'wind' in measurement:
-            product = 'wind'
-            measurement_key = 'data'
-        elif 'water_temp' in measurement:
-            product = 'water_temperature'
-            measurement_key = 'data'
-        elif 'air_temp' in measurement:
-            product = 'air_temperature'
-            measurement_key = 'data'
-        elif 'air_press' in measurement:
-            product = 'air_pressure'
-            measurement_key = 'data'
-        elif 'wave' in measurement:
+        if "tide" in measurement:
+            product = "water_level"
+        elif "wind" in measurement:
+            product = "wind"
+        elif "water_temp" in measurement:
+            product = "water_temperature"
+        elif "air_temp" in measurement:
+            product = "air_temperature"
+        elif "air_press" in measurement:
+            product = "air_pressure"
+        elif "wave" in measurement:
             raise SeaStateException("Unsupported measurement requested")
-        elif 'conductivity' in measurement:
-            product = 'conductivity'
-            measurement_key = 'data'
+        elif "conductivity" in measurement:
+            product = "conductivity"
         else:
             raise SeaStateException("Unsupported measurement requested")
 
         # formatting datetime to endpoint param
         begin_date = f"{start.year}{start.month:02}{start.day:02}"
         end_date = f"{end.year}{end.month:02}{end.day:02}"
-        
+
         ep_params = {
-            'begin_date': begin_date,
-            'end_date': end_date,
-            'station': str(station_id),
-            'product': product,
-            'interval': 'h',
-            'datum': 'MTL',
-            'units': 'metric',
-            'time_zone': 'lst_ldt',
-            'application': 'seastate',
-            'format': 'json',
+            "begin_date": begin_date,
+            "end_date": end_date,
+            "station": str(station_id),
+            "product": product,
+            "interval": "h",
+            "datum": "MTL",
+            "units": "metric",
+            "time_zone": "lst_ldt",  # todo: local time or gmt? what is ndbc doing?
+            "application": "seastate",
+            "format": "json",
         }
-        
+
         # Call endpoint
-        endpoint='api/prod/datagetter?'
-        result = self._rest_adapter.get(endpoint=endpoint,ep_params=ep_params)
-        
+        endpoint = "api/prod/datagetter?"
+        return endpoint, ep_params
+
+    def _parse_result(
+        self, result: list[Result], start: datetime, end: datetime, measurement: str
+    ) -> list[Dict]:
         # unpack to return specified measurement
-        # since TidesAndCurrents returns 1 product per endpoint, no need to parse, just unpack Json
+        # since TidesAndCurrents returns 1 product per endpoint:
+        # -> minimal parsing, just unpack Json
         # details here: https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html
-        # 
+        #
+        if len(result) > 1:
+            raise SeaStateException(
+                "TidesAndCurrentsApi doesn't support multiple results"
+            )
         try:
-            data = result.data[measurement_key]
-        except (KeyError) as e:
-            self._logger.error(result.data)
+            parse_key = self._build_parse_key(measurement)
+            if result[0].data.get("error"):
+                self._logger.error("TidesAndCurrentsApi error, returning empty data")
+                self._logger.error(f"{measurement}:{result[0].data}")
+                return []
+            data = result[0].data[parse_key]
+        except KeyError as e:
+            self._logger.exception(result.data)
             raise SeaStateException("TidesAndCurrentsApi unpacking error") from e
-        
+
         if len(data) == 0:
-            raise SeaStateException("No data retrieved")
-        
+            self._logger.warning(
+                f"No {measurement} data recovered for daterange:\
+                    {str(start.date())} : {str(end.date())}"
+            )
+
         return data
 
-        
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     api = TidesAndCurrentsApi()
-    result = api.hourly('wind',9410230, datetime.today(),datetime.today())
+    result = api.hourly("wind", 9410230, datetime.today(), datetime.today())
     print(result)
-    result = api.hourly(9410230, datetime.today(),datetime.today(),'air_temp')
-    result = api.hourly(9410230, datetime.today(),datetime.today(),'water_temp')
+    result = api.hourly(9410230, datetime.today(), datetime.today(), "air_temp")
+    result = api.hourly(9410230, datetime.today(), datetime.today(), "water_temp")
```

### Comparing `seastate-0.1.2/seastate/api/rest_adapter.py` & `seastate-0.2.0/seastate/api/rest_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,112 @@
 import logging
-from json import JSONDecodeError
-from typing import Dict
+from typing import Dict, Union
 
 import requests
 import requests.packages
+from requests_cache import CachedSession
 from seastate.exceptions import SeaStateException
 from seastate.models import Result
 
+
 class RestAdapter:
-    def __init__(self, hostname: str, api_key: str = '', ssl_verify: bool = True, logger: logging.Logger = None):
+    session = CachedSession("seastate_cache", backend="filesystem", use_cache_dir=True)
+
+    def __init__(
+        self,
+        hostname: str,
+        api_key: str = None,
+        ssl_verify: bool = True,
+        logger: logging.Logger = None,
+    ):
         """Constructor for RestAdapter, supports GET
 
         Args:
             hostname (str): hostname for http request
             api_key (str, optional): Defaults to ''.
             ssl_verify (bool, optional): Defaults to True.
-            logger (logging.Logger, optional): Pass explictly else will be created with __name__.
         """
         self._logger = logger or logging.getLogger(__name__)
         self.url = f"https://{hostname}/"
         self._api_key = api_key
         self._ssl_verify = ssl_verify
         if not ssl_verify:
             requests.packages.urllib3.disable_warnings()
-            
-    def _do(self, http_method, endpoint:str, ep_params: Dict = None, data: Dict = None ) -> Result:
+
+    def _do(
+        self, http_method: str, endpoint: str, ep_params: Dict = None, data: Dict = None
+    ) -> Result:
         """HTTP request contructor convenience method
 
         Args:
             http_method (_type_): GET, POST, DELETE
             endpoint (str): target endpoint
             ep_params (Dict, optional): http parameters. Defaults to None.
             data (Dict, optional): POST data. Defaults to None.
 
-        Raises:
-            SeaStateException: _description_
-            SeaStateException: _description_
-            SeaStateException: _description_
-
         Returns:
             Result: Simplified http.Response object with:
                 status_code
                 message
                 data
         """
         full_url = self.url + endpoint
-        headers = {'x-api-key': self._api_key}
+        headers = {"x-api-key": self._api_key}
         log_line_pre = f"method={http_method}, url={full_url}, params={ep_params}"
         log_line_post = "result: success={}, status_code={}, message={}"
         # Log HTTP params and try HTTP request
         try:
             self._logger.debug(msg=log_line_pre)
-            response = requests.request(
+            # response = requests.request(
+            response = self.session.request(
                 method=http_method,
                 url=full_url,
                 verify=self._ssl_verify,
                 headers=headers,
                 params=ep_params,
-                json=data)
-        except requests.exceptions.RequestException as e:
-            self._logger.error(msg=str(e))
+                json=data,
+            )
+        except Exception as e:
+            self._logger.exception(msg=str(e))
             raise SeaStateException("Request Failed") from e
         # Parse JSON ouput to Python object or return failed Result on exception
         try:
-            if '.txt' in full_url.lower():
+            if ".txt" in full_url.lower():
                 # handle txt based files from nonRest endpoints
                 data_out = response.text
-            elif 'xml' in full_url.lower():
+            elif "xml" in full_url.lower():
                 # handle xml files from nonRest endpoints
                 data_out = response.text
-            elif any(x in full_url.lower() for x in ['spec','.sw']):
+            elif any(x in full_url.lower() for x in ["spec", ".sw"]):
                 # handle the 7 different spectral file extensions
                 data_out = response.text
             else:
                 # handle a restful endpoint
                 data_out = response.json()
-        except (ValueError) as e:
+        except ValueError as e:
             self._logger.error(msg=log_line_post.format(False, None, e))
             raise SeaStateException("Bad JSON in Response") from e
         is_success = 299 >= response.status_code >= 200
-        log_line = log_line_post.format(is_success, response.status_code, response.reason)
+        log_line = log_line_post.format(
+            is_success, response.status_code, response.reason
+        )
         # if status code in 200-299 range, return Result, else raise exception
         if is_success:
             self._logger.debug(msg=log_line)
             return Result(response.status_code, message=response.reason, data=data_out)
         self._logger.error(msg=log_line)
         raise SeaStateException(f"{response.status_code}: {response.reason}")
 
-
-    def get(self, endpoint: str, ep_params: Dict = None) -> Result:
+    def get(self, endpoint: str, ep_params: Union[Dict, None] = None) -> Result:
         """GET method for RestAdapter
 
         Args:
             endpoint (str): target endpoint
             ep_params (Dict, optional): key:value API parameters. Defaults to None.
 
         Returns:
             Result: Simplified Response object with:
                 status_code
                 message
                 data
         """
-        return self._do(http_method='GET', endpoint=endpoint, ep_params=ep_params)
+        return self._do(http_method="GET", endpoint=endpoint, ep_params=ep_params)
```

### Comparing `seastate-0.1.2/seastate/models.py` & `seastate-0.2.0/seastate/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 from dataclasses import dataclass, field
-from typing import List, Dict, Any
+from typing import List, Dict
+from seastate.settings import MEASUREMENTS
 
-# the implemented measurements for 
-valid_measurements = {
-    'tide',
-    'wind',
-    'water_temp',
-    'air_temp',
-    'air_press',
-    'wave',
-    'conductivity',
-}
 
 @dataclass
 class Result:
     """Simplified requests.Response returned from RestAdapter
 
     Args:
         status_code (int): HTTP Status
         message (str, optional): Human readable result. Defaults to ''.
         data (List[Dict], optional): Python list of Dicts. Defaults to None.
     """
+
     status_code: int
-    message: str = ''
+    message: str = None
     data: List[Dict] = field(default_factory=list)
-    
+
     def __post__init__(self, data):
-        self.data = data if data else [] #init data if dne
+        self.data = data if data else []  # init data if dne
+
 
 @dataclass
 class Station:
     id: str
     lat: float
     lon: float
-    api: Any
+    api: str
+    name: str = None
     tide: bool = False
     wind: bool = False
     water_temp: bool = False
     air_temp: bool = False
     air_press: bool = False
     wave: bool = False
     conductivity: bool = False
     is_active: bool = False
-    name: str = ''
-    
+
     def __post_init__(self):
         # toggle if self.is_active
         if len(self.supported_measurements()) > 0:
             self.is_active = True
-            
-    def supported_measurements(self) -> List[str]:
-        """Return list of supported measurements for station
-
-        Returns:
-            List[str]: _description_
-        """
-        # 
+
+    def supported_measurements(self) -> tuple[str]:
+        """Return list of supported measurements for station"""
+        #
         supported = []
-        for key in valid_measurements:
+        for key in MEASUREMENTS:
             if self.__getattribute__(key):
                 supported.append(key)
-        return supported
-        
-    def is_supported(self, value:str) -> bool:
+        return tuple(supported)
+
+    def is_supported(self, value: str) -> bool:
         # Implemented this to always run comparison on lower case casting of strings
         for x in self.supported_measurements():
             if value in x:
                 return True
         return False
-        
-        
-if __name__ == '__main__':
-    # Result tests
-    test = Result(200)
-    
-    # Station Tests
-    test = Station()
-    # test internal methods
```

### Comparing `seastate-0.1.2/seastate/seastate.py` & `seastate-0.2.0/seastate/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,179 @@
 import logging
 from datetime import datetime, timedelta
 from typing import Dict, Union
 
 from seastate.api.api_mediator import ApiMediator
+from seastate.settings import MEASUREMENTS
+
 
 class SeaState:
-    def __init__(self, lat: float, lon: float, exclude: list=[], logger: logging.Logger = None):
+    def __init__(
+        self, lat: float, lon: float, exclude: list = [], logger: logging.Logger = None
+    ):
         self._logger = logger or logging.getLogger(__name__)
         self.lat = float(lat)
         self.lon = float(lon)
         self.exclude = list(exclude)
-        self.tide = ApiMediator('tide', self.lat, self.lon, self.exclude)
-        self.wind = ApiMediator('wind', self.lat, self.lon, self.exclude)
-        self.water_temp = ApiMediator('water_temp', self.lat, self.lon, self.exclude)
-        self.air_temp = ApiMediator('air_temp', self.lat, self.lon, self.exclude)
-        self.air_press = ApiMediator('air_press', self.lat, self.lon, self.exclude)
-        self.wave = ApiMediator('wave', self.lat, self.lon, self.exclude)
-        self.conductivity = ApiMediator('conductivity', self.lat, self.lon, self.exclude)
-        
-    def measurements_from_date_range(self, start: datetime = None, end: Union[datetime, timedelta] = None) -> Dict:
+        self.mediator_map = {}
+        self._set_api_mediators()
+
+    @property
+    def _requested_measurements(self) -> tuple:
+        return (x for x in MEASUREMENTS if x not in self.exclude)
+
+    def _build_date_range(
+        self, start: Union[datetime, None], end: Union[datetime, timedelta, None]
+    ) -> tuple[datetime, datetime]:
+        """
+        Builds date range to fullest days possible,
+        with start and end at midnight and (midnight - 1)
+        """
         # Process timeframe
         # todo: handle iso date strings
         # todo: handle bad date strings
-        if start and end: # all values provided, handle endpoint
+        if start and end:  # all values provided
             # end can be declared relative to start as a timedelta
             if isinstance(end, timedelta):
                 end = start + end
-        elif start and not end: # no end provided, return same day as start
+        elif start and not end:  # no end provided, return same day as start
             end = start
-        elif not start and not end: # nothing provided, return today
-            start = datetime.today()
-            end = datetime.today()
-            
+        elif not start and not end:  # nothing provided, return today
+            start = end = datetime.today()
+
         # remove microseconds to pass comparison tests
         # remove hours and minutes from start
-        # set hours and minutes to end of day for start
-        if isinstance(start,datetime):
+        # set hours and minutes to end of day for end
+        if isinstance(start, datetime):
             start = start.replace(microsecond=0)
-            start = start.replace(hour=0, minute=0)
-        if isinstance(end,datetime):
+            start = start.replace(hour=0, minute=0, second=0)
+        if isinstance(end, datetime):
             end = end.replace(microsecond=0)
-            end = end.replace(hour=23, minute=0)
-            
+            end = end.replace(hour=23, minute=59, second=59)
+
         # log warning if end is before start
         if end < start:
             self._logger.warning("end is after start")
-        
-        # Get data
+
+        return start, end
+
+    def _get_mediator(self, measurement: str) -> ApiMediator:
+        return self.__getattribute__(measurement)
+
+    def _set_mediator(self, measurement: str) -> None:
+        if measurement in self.exclude:
+            self.__setattr__(measurement, None)
+        else:
+            tmp = ApiMediator(measurement, self.lat, self.lon, self.exclude)
+            # add attribute
+            self.__setattr__(measurement, tmp)
+            # register mediator to map
+            self.mediator_map[measurement] = tmp
+
+    def _set_api_mediators(self) -> None:
+        """set APIMediator as attribute for all implemented measurements"""
+        for measurement in MEASUREMENTS:
+            self._set_mediator(measurement)
+
+    def _get_data(self, key: str, start: datetime, end: datetime) -> list[Dict]:
+        mediator = self._get_mediator(key)
         data = {}
-        #todo: have a class property that summarizes the active apis for this list
-        for api_key in ['tide', 'wind', 'water_temp', 'air_temp', 'air_press', 'wave', 'conductivity']:
-            # access the configured api to generate response with hourly method 
-            data[api_key] = self.__getattribute__(api_key).api.measurements_from_date_range(
-                measurement = self.__getattribute__(api_key).measurement,
-                station_id = self.__getattribute__(api_key).station.id,
-                start = start,
-                end = end)
+        data = mediator.api.measurement_from_date_range(
+            measurement=mediator.measurement,
+            station_id=mediator.station.id,
+            start=start,
+            end=end,
+        )
         return data
 
-    def hourly(self, start: datetime = None, end: Union[datetime, timedelta] = None) -> Dict:
-        """Convenience method to return 1 sample per hour for each api
-
-        Args:
-            start (datetime, optional): _description_. Defaults to None.
-            end (Union[datetime, timedelta], optional): _description_. Defaults to None.
+    def from_date_range(
+        self,
+        start: Union[datetime, None] = None,
+        end: Union[datetime, timedelta, None] = None,
+    ) -> Dict:
+        # process timeframe
+        start, end = self._build_date_range(start, end)
+
+        # makes an api call for each measurement,
+        # the idea is that the cache absorbs duplicate calls
+        # and the actual data is small so it's ok to reprocess
+        data = {
+            key: self._get_data(key, start, end) for key in self._requested_measurements
+        }
+
+        # previously, i manually built a dict with 7 api calls
+        # for each measurement
+        # get attribute.api
+        # call api.from_date_range on measurement, station, start, end
+        # gets measurement again
+        # gets staion again
+        # data = {}
+        # for measurement_key in MEASUREMENTS:
+        #     # access the configured api to generate response with hourly method
+        #     data[measurement_key] = self.__getattribute__(
+        #         measurement_key
+        #     ).api.measurement_from_date_range(
+        #         measurement=self.__getattribute__(measurement_key).measurement,
+        #         station_id=self.__getattribute__(measurement_key).station.id,
+        #         start=start,
+        #         end=end,
+        #     )
+        return data
 
-        Returns:
-            Dict: _description_
-        """
-        data_all = self.measurements_from_date_range(start,end)
-        data= {}
+    def hourly(
+        self,
+        start: Union[datetime, None] = None,
+        end: Union[datetime, timedelta, None] = None,
+    ) -> Dict:
+        """Convenience method to return 1 sample per hour for each api"""
+        data_all = self.from_date_range(start, end)
+        data = {}
         for key in data_all:
             # find the first minute within the hour
-            # the apis typically use the same minute 
+            # the apis typically use the same minute
             first_minute = 0
-            while datetime.fromisoformat(data_all[key][0]['t']).minute != first_minute:
+            while datetime.fromisoformat(data_all[key][0]["t"]).minute != first_minute:
                 first_minute += 1
-                # prevent endless loop 
+                # prevent endless loop
                 if first_minute == 60:
                     data[key] = []
                     break
             # keep one reading per hour
-            data[key] = [x for x in data_all[key] if datetime.fromisoformat(x['t']).minute == first_minute]
+            data[key] = [
+                x
+                for x in data_all[key]
+                if datetime.fromisoformat(x["t"]).minute == first_minute
+            ]
         return data
-    
-if __name__ == '__main__':
-    api = SeaState(32,-117)
-    start = datetime(2022,7,5)
-    end = datetime(2022,7,5)
-    a = api.hourly(start,end)
-    
+
+    def measurements_from_date_range(
+        self, start: datetime = None, end: Union[datetime, timedelta] = None
+    ) -> Dict:
+        self._logger.warning(
+            "measurements_from_date_range() is deprecated,\
+                use from_date_range() instead"
+        )
+        return self.from_date_range(start, end)
+
+
+if __name__ == "__main__":
+    api = SeaState(32, -117)
+    start = datetime(2023, 9, 5)
+    end = datetime(2023, 9, 5)
+    data = api.from_date_range(start, end)
+    a = api.hourly(start, end)
+
     # check daterange within realtime
     # result = api.hourly(datetime.today()-timedelta(days=2),datetime.today())
-    
+
     # # check daterange for request only in prior years
-    # result = api.hourly(datetime.today()-timedelta(days=2*365+30),datetime.today()-timedelta(days=1*365+30))
+    # result = api.hourly(
+    #     datetime.today() - timedelta(days=2 * 365 + 30),
+    #     datetime.today() - timedelta(days=1 * 365 + 30),
+    # )
 
     # # check daterange spanning archive and realtime, into prior year
     # result = api.hourly(datetime.today()-timedelta(days=365+30),datetime.today())
-    
+
     # # check old archive with different headers
     # # check date format
     # result = api.hourly('air_press',42040,datetime(1996,2,1),datetime(1996,2,2))
-
```

### Comparing `seastate-0.1.2/seastate/utils.py` & `seastate-0.2.0/seastate/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 
+
 def haversine(lat1: float, lon1: float, lat2: float, lon2: float) -> float:
-    """ Returns distance in km using haversine method
+    """Returns distance in km using haversine method
 
     Args:
         lat1 (float): Coordinate in decimal degrees
         lon1 (float): Coordinate in decimal degrees
         lat2 (float): Coordinate in decimal degrees
         lon2 (float): Coordinate in decimal degrees
 
@@ -16,12 +17,12 @@
     lat1, lon1, lat2, lon2 = map(np.radians, [lat1, lon1, lat2, lon2])
 
     # Calculate deltas
     dlat = lat2 - lat1
     dlon = lon2 - lon1
 
     # Haversine method for measuring distance on a sphere
-    a = np.sin(dlat/2.0)**2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon/2.0)**2
+    a = np.sin(dlat / 2.0) ** 2 + np.cos(lat1) * np.cos(lat2) * np.sin(dlon / 2.0) ** 2
     c = 2 * np.arcsin(np.sqrt(a))
-    
+
     km = 6367 * c
     return km
```

### Comparing `seastate-0.1.2/PKG-INFO` & `seastate-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,129 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: seastate
-Version: 0.1.2
-Summary: Collect ocean measurement data based on location and timeframe
-Home-page: https://github.com/ivorivetta/seastate
-License: MIT
-Author: Ivo
-Author-email: ivorivetta@users.noreply.github.com
-Requires-Python: >=3.8,<4
+Version: 0.2.0
+Summary: Collect ocean measurements for location and timeframe. Integrates NDBC and TidesAndCurrents datasources.
+Project-URL: Homepage, https://github.com/ivorivetta/seastate
+Project-URL: Issues, https://github.com/ivorivetta/seastate/issues
+Author-email: Ivo Rivetta <ivo@ivorivetta.com>
+License-File: LICENSE
+Keywords: api,currents,data,forecast,marine,ndbc,ocean,tides,weather
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
-Project-URL: Bug Tracker, https://github.com/ivorivetta/seastate/issues
-Project-URL: Repository, https://github.com/ivorivetta/seastate
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 
-# Seastate
+# seastate
 
 ## Summary
+
 Collect ocean measurement data based on location and timeframe
 
 **Features**
+
 - Closest active station is selected for each measurement
 - Reaches into secondary historical archives when required
-- Returns pandas dataframe compatible lists
+- Returns pandas dataframe compatible dictionaries
 - Available measurements: Tide, wind, water temp, air temp, air pressure, conductivity and swell information
 - Datasources: NOAA NDBC, NOAA Tides and Currents
 
 ## Installing
+
 `pip install seastate`
 
 ## Quick start
+
 ```
-from seastate.seastate import SeaState
+from seastate import SeaState
 from datetime import datetime
 
 # make SeaState object for specific location
 san_diego = SeaState(32,-117)
 
 # retrieve measurements for today
-san_diego_today = san_diego.measurements_from_date_range(datetime.today())
+san_diego_today = san_diego.from_date_range(datetime.today())
 
-san_diego_today['tide'] -> [{t: time, v: value, s: stdev]
+san_diego_today['tide'] -> [{t: time, v: value, s: stdev}]
 san_diego_today['wind']-> [{t: time, v: value, d: direction, g: gust}]
 san_diego_today['water_temp']-> [{t: time, v: value}]
 san_diego_today['air_temp']-> [{t: time, v: value}]
 san_diego_today['air_press']-> [{t: time, v: value}]
 san_diego_today['wave']-> [{t: time, v: Wave Height, dpd: Dominant Period, mwd: dpd Direction}]
-san_diego_today['conductivity']-> [{t: time, v: value}] 
+san_diego_today['conductivity']-> [{t: time, v: value}]
 ```
+
 Measurement details for NDBC are [here](https://www.ndbc.noaa.gov/measdes.shtml) and for Tides and Currents [here](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html)
 
+## API reference
+
+Useful metadata can be accessed through the SeaState object
+
+```
+san_diego = SeaState(32,-117)
+
+# Each measurement has an entry point
+san_diego.tide
+-> (api.mediator Object)
+
+# The valid keys are:
+valid_measurements = {
+    'tide',
+    'wind',
+    'water_temp',
+    'air_temp',
+    'air_press',
+    'wave',
+    'conductivity',
+}
+
+
+# the original lat/lon are available
+san_diego.lat
+-> 32
+san_diego.tide._target_lon
+-> 32
+
+# the distance of each measurement station to target gps
+san_diego.tide.distance
+-> xyz kilometers
+
+# and other useful exposed api keys
+san_diego.tide.station.name
+san_diego.tide.station.id
+san_diego.tide.station.lat
+san_diego.tide.station.lon
+
+```
+
 ## Measurement x API breakdown
-| Measurement | T&C | NDBC |
-| ---: | :---: | :---: |
-|tide | y | y |
-|wind | y | y |
-|water_temp | y | y |
-|air_temp | y | y |
-|air_press | y | y |
-|wave |  | y |
-|conductivity | y |  |
+
+|  Measurement | T&C | NDBC |
+| -----------: | :-: | :--: |
+|         tide |  y  |  y   |
+|         wind |  y  |  y   |
+|   water_temp |  y  |  y   |
+|     air_temp |  y  |  y   |
+|    air_press |  y  |  y   |
+|         wave |     |  y   |
+| conductivity |  y  |      |
 
 ## More Examples
+
 ### Measurements for past 30 days
+
 ```
-from seastate.seastate import SeaState
+from seastate import SeaState
 from datetime import datetime, timedelta
 
 start = datetime.today()-timedelta(days=30)
 end = datetime.today()
 san_diego_past_30 = san_diego.measurements_from_date_range(start,end)
 ```
+
 ### Hourly Slices
+
 ```
 san_diego_past_30_hourly = san_diego.hourly(start,end) # this returns a single reading per hour
 # experimental feature
 # no guarantee between APIs that readings will align or exist in all cases
 ```
-
```

