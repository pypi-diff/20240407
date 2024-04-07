# Comparing `tmp/LocalSolarWatt-0.6.1.tar.gz` & `tmp/LocalSolarWatt-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/SolarWattEnergyManagerAPI/SolarWattEnergyManagerAPI/dist/.tmp-t8_xbclc/LocalSolarWatt-0.6.1.tar", last modified: Fri Mar 10 16:33:28 2023, max compression
+gzip compressed data, was "LocalSolarWatt-0.7.tar", last modified: Sun Apr  7 14:17:26 2024, max compression
```

## Comparing `LocalSolarWatt-0.6.1.tar` & `LocalSolarWatt-0.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/energy_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/my_reserve.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/LocalSolarWatt/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-10 16:33:28.000000 LocalSolarWatt-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-10 16:33:19.000000 LocalSolarWatt-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:17:26.144686 LocalSolarWatt-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:17:26.144686 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 14:17:26.000000 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-07 14:17:26.000000 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:17:26.000000 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 14:17:26.000000 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 14:17:26.000000 LocalSolarWatt-0.7/LocalSolarWatt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-07 14:17:26.144686 LocalSolarWatt-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:17:26.144686 LocalSolarWatt-0.7/local_solar_watt/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/energy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/local_solar_watt/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 14:17:26.144686 LocalSolarWatt-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-07 14:17:22.000000 LocalSolarWatt-0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `LocalSolarWatt-0.6.1/LICENSE.txt` & `LocalSolarWatt-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LocalSolarWatt-0.6.1/LocalSolarWatt/api_client.py` & `LocalSolarWatt-0.7/local_solar_watt/api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from abc import ABC, abstractmethod
-import requests
-import logging
-import json
-
-
-class ApiClient(ABC):
-    _API_PATH = ''
-    _DEVICE_NAME = ''
-    _HEADERS = {'Accept': 'application/json'}
-    _LOGGER = None
-
-    def __init__(self, host: str, logger=None):
-        if not host:
-            raise ValueError('Invalid host')
-        self._API_URL = "http://" + host + self._API_PATH
-        if not logger:
-            self._LOGGER = logging.getLogger(__name__)
-
-    def set_log_level(self, log_level):
-        if isinstance(log_level, str):
-            numeric_level = getattr(logging, log_level.upper(), None)
-            if not isinstance(numeric_level, int):
-                raise ValueError('Invalid log level: %s' % log_level)
-        if not (isinstance(log_level, int) or isinstance(log_level, str)):
-            raise ValueError('Invalid log level: %s' % log_level)
-
-        self._LOGGER.setLevel(log_level)
-
-    def _call_API(self):
-        try:
-            response = requests.get(self._API_URL, headers=self._HEADERS)
-            if response.status_code == 200:
-                return response.json()
-            else:
-                logging.error(f"Failed to communicate with the {self._DEVICE_NAME} API")
-        except requests.exceptions.RequestException as e:
-            logging.error(f"Failed to communicate with {self._DEVICE_NAME} API")
-            logging.debug(f"HTTP Error code: {repr(e)}")
-        except json.decoder.JSONDecodeError as e:
-            logging.error(f"Failed to communicate with the {self._DEVICE_NAME} API")
-            logging.debug(f"JSON decode error: {repr(e)}")
-        return None
-
-    @abstractmethod
-    def test_connection(self):
-        pass
-
-    @abstractmethod
-    def pull_data(self):
-        pass
+from abc import ABC, abstractmethod
+import requests
+import logging
+import json
+
+
+class ApiClient(ABC):
+    _API_PATH = ''
+    _DEVICE_NAME = ''
+    _HEADERS = {'Accept': 'application/json'}
+    _LOGGER = None
+
+    def __init__(self, host: str, logger=None):
+        if not host:
+            raise ValueError('Invalid host')
+        self._API_URL = "http://" + host + self._API_PATH
+        if not logger:
+            self._LOGGER = logging.getLogger(__name__)
+
+    def set_log_level(self, log_level):
+        if isinstance(log_level, str):
+            numeric_level = getattr(logging, log_level.upper(), None)
+            if not isinstance(numeric_level, int):
+                raise ValueError('Invalid log level: %s' % log_level)
+        if not (isinstance(log_level, int) or isinstance(log_level, str)):
+            raise ValueError('Invalid log level: %s' % log_level)
+
+        self._LOGGER.setLevel(log_level)
+
+    def _call_api(self):
+        try:
+            response = requests.get(self._API_URL, headers=self._HEADERS)
+            if response.status_code == 200:
+                return response.json()
+            else:
+                logging.error(f"Failed to communicate with the {self._DEVICE_NAME} API")
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Failed to communicate with {self._DEVICE_NAME} API")
+            logging.debug(f"HTTP Error code: {repr(e)}")
+        except json.decoder.JSONDecodeError as e:
+            logging.error(f"Failed to communicate with the {self._DEVICE_NAME} API")
+            logging.debug(f"JSON decode error: {repr(e)}")
+        return None
+
+    @abstractmethod
+    def test_connection(self):
+        pass
+
+    @abstractmethod
+    def pull_data(self):
+        pass
```

### Comparing `LocalSolarWatt-0.6.1/LocalSolarWatt.egg-info/PKG-INFO` & `LocalSolarWatt-0.7/LocalSolarWatt.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 Metadata-Version: 2.1
 Name: LocalSolarWatt
-Version: 0.6.1
-Summary: python api wrapper for solar watt devices
+Version: 0.7
+Summary: python api wrapper for solar watt device api
 Home-page: https://github.com/AlgorithmicEntropy/SolarWattEnergyManagerAPI
-Download-URL: https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_061.tar.gz
+Download-URL: https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_070.tar.gz
 Author: AlgorithmicEntropy
 License: MIT
 Keywords: IOT,Solar,Local
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
 
 # LocalSolarWatt
 A python3 library to access the data of solar watt devices via local api  
 Disclaimer: This library uses an unofficial local api and could therefore break at any point
 
 # Overview
-The package wraps both the kiwigrid energy manager api and the myReserve api.  
+The package uses the kiwigrid api provided by your solar watt energy manager device.  
 Data available:
-  - energy manager: current power, energy counters, diagnostics
-  - my reserve: hex status codes, current power (same as web interface)
+  - Real time power values from inverter, AC sensor and battery (if exists)
+  - Long term energy statistics
 
-As the myReserve api only returns small amount of data and gets polled by the web interface anyway,  
-it is the preferred option for realtime data.  
-Polling the energy manager to often could lead to reliability issues (untested).
+This library does some preprocessing by extracting relevant fields and grouping them by device class.  
+For now this mostly includes data I deem usefully for the integration with home assistant.
+
+Note: Polling the energy manager with a very high interval often could lead to reliability issues (untested).
+
+# Supported devices
+As I only have access to one installation and the api is as far as I'm aware not documented by SolarWatt, I can not guarantee that this library works with your setup.  
+If you encounter issues with your concrete setup, feel free to open a new issue.  
+The raw json data is available via `http://YOUR_DEVICE_IP/rest/kiwigrid/wizard/devices`  
+If you can provide the raw json dump, I can try to add support for your device.  
+**Important Note**: This data does contain some sensitive information (especially for the "Location" device), so make sure to remove any sensitive data before sharing.
 
 ## Installation
 
 ```
 pip install LocalSolarWatt
 ```
 
 ## Usage
 ```
-from LocalSolarWatt import EnergyManager, MyReserve, WorkUnits
+from local_solar_watt import Api, WorkUnits, DeviceClass
 
 # create a new api objects
-energy_api = EnergyManager('hostname or ip')
-my_reserve_api = MyReserve('hostname or ip')
+energy_api = Api('hostname or ip')
 
 # optional, change work units to Wh instead of kWh
-from SolarWattEnergyManagerAPI.units import WorkUnit
-api = EnergyManager('hostname or ip', work_unit=WorkUnits.Wh)
+api = Api('hostname or ip', work_unit=WorkUnits.Wh)
 
-# below functions work on both energy manager and my reserve
 # optional, change log level
 api.set_log_level('WARNING')
 
 # test the connection (returns bool based on success)
 status, data = api.test_connection()
 
-# pull data from the device (retuirn dictionary with power values)
+# pull data from the device (returns only selected power values, grouped by device class)
 print(api.pull_data())
+
+# You can also pull the raw json data for your own parsing needs
+print(api.pull_raw())
 ```
 
 # Tests:
 If you want to run the tests locally make sure to set the following environment variables to correct IPs / hostnames
 ```
 ENERGY_MANAGER_HOST
-MY_RESERVE_HOST
 ```
```

### Comparing `LocalSolarWatt-0.6.1/PKG-INFO` & `LocalSolarWatt-0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 Metadata-Version: 2.1
 Name: LocalSolarWatt
-Version: 0.6.1
-Summary: python api wrapper for solar watt devices
+Version: 0.7
+Summary: python api wrapper for solar watt device api
 Home-page: https://github.com/AlgorithmicEntropy/SolarWattEnergyManagerAPI
-Download-URL: https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_061.tar.gz
+Download-URL: https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_070.tar.gz
 Author: AlgorithmicEntropy
 License: MIT
 Keywords: IOT,Solar,Local
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
 
 # LocalSolarWatt
 A python3 library to access the data of solar watt devices via local api  
 Disclaimer: This library uses an unofficial local api and could therefore break at any point
 
 # Overview
-The package wraps both the kiwigrid energy manager api and the myReserve api.  
+The package uses the kiwigrid api provided by your solar watt energy manager device.  
 Data available:
-  - energy manager: current power, energy counters, diagnostics
-  - my reserve: hex status codes, current power (same as web interface)
+  - Real time power values from inverter, AC sensor and battery (if exists)
+  - Long term energy statistics
 
-As the myReserve api only returns small amount of data and gets polled by the web interface anyway,  
-it is the preferred option for realtime data.  
-Polling the energy manager to often could lead to reliability issues (untested).
+This library does some preprocessing by extracting relevant fields and grouping them by device class.  
+For now this mostly includes data I deem usefully for the integration with home assistant.
+
+Note: Polling the energy manager with a very high interval often could lead to reliability issues (untested).
+
+# Supported devices
+As I only have access to one installation and the api is as far as I'm aware not documented by SolarWatt, I can not guarantee that this library works with your setup.  
+If you encounter issues with your concrete setup, feel free to open a new issue.  
+The raw json data is available via `http://YOUR_DEVICE_IP/rest/kiwigrid/wizard/devices`  
+If you can provide the raw json dump, I can try to add support for your device.  
+**Important Note**: This data does contain some sensitive information (especially for the "Location" device), so make sure to remove any sensitive data before sharing.
 
 ## Installation
 
 ```
 pip install LocalSolarWatt
 ```
 
 ## Usage
 ```
-from LocalSolarWatt import EnergyManager, MyReserve, WorkUnits
+from local_solar_watt import Api, WorkUnits, DeviceClass
 
 # create a new api objects
-energy_api = EnergyManager('hostname or ip')
-my_reserve_api = MyReserve('hostname or ip')
+energy_api = Api('hostname or ip')
 
 # optional, change work units to Wh instead of kWh
-from SolarWattEnergyManagerAPI.units import WorkUnit
-api = EnergyManager('hostname or ip', work_unit=WorkUnits.Wh)
+api = Api('hostname or ip', work_unit=WorkUnits.Wh)
 
-# below functions work on both energy manager and my reserve
 # optional, change log level
 api.set_log_level('WARNING')
 
 # test the connection (returns bool based on success)
 status, data = api.test_connection()
 
-# pull data from the device (retuirn dictionary with power values)
+# pull data from the device (returns only selected power values, grouped by device class)
 print(api.pull_data())
+
+# You can also pull the raw json data for your own parsing needs
+print(api.pull_raw())
 ```
 
 # Tests:
 If you want to run the tests locally make sure to set the following environment variables to correct IPs / hostnames
 ```
 ENERGY_MANAGER_HOST
-MY_RESERVE_HOST
 ```
```

### Comparing `LocalSolarWatt-0.6.1/setup.py` & `LocalSolarWatt-0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='LocalSolarWatt',
-    packages=['LocalSolarWatt'],
-    version='0.6.1',
+    packages=['local_solar_watt'],
+    version='0.7',
     license='MIT',
-    description='python api wrapper for solar watt devices',
+    description='python api wrapper for solar watt device api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='AlgorithmicEntropy',
     url='https://github.com/AlgorithmicEntropy/SolarWattEnergyManagerAPI',
-    download_url='https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_061.tar.gz',
+    download_url='https://github.com/SebastianWallat/SolarWattEnergyManagerAPI/archive/v_070.tar.gz',
     keywords=['IOT', 'Solar', 'Local'],
     install_requires=[
         'requests',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

