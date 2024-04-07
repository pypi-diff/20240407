# Comparing `tmp/owmpy-0.4.1.tar.gz` & `tmp/owmpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owmpy-0.4.1.tar", last modified: Wed Nov 16 21:42:56 2022, max compression
+gzip compressed data, was "owmpy-1.0.0.tar", last modified: Sun Apr  7 13:32:03 2024, max compression
```

## Comparing `owmpy-0.4.1.tar` & `owmpy-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,39 @@
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.674922 owmpy-0.4.1/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1081 2022-03-26 09:52:06.000000 owmpy-0.4.1/LICENSE
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1447 2022-11-16 21:42:56.674922 owmpy-0.4.1/PKG-INFO
--rw-r--r--   0 ernie     (1000) ernie     (1000)      920 2022-11-16 21:42:54.000000 owmpy-0.4.1/README.md
--rw-r--r--   0 ernie     (1000) ernie     (1000)      222 2022-11-15 14:58:17.000000 owmpy-0.4.1/pyproject.toml
--rw-r--r--   0 ernie     (1000) ernie     (1000)      651 2022-11-16 21:42:56.674922 owmpy-0.4.1/setup.cfg
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.672922 owmpy-0.4.1/src/
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.673922 owmpy-0.4.1/src/owmpy/
--rw-r--r--   0 ernie     (1000) ernie     (1000)      197 2022-11-16 21:39:59.000000 owmpy-0.4.1/src/owmpy/__init__.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.674922 owmpy-0.4.1/src/owmpy/current/
--rw-r--r--   0 ernie     (1000) ernie     (1000)       48 2022-03-26 09:52:06.000000 owmpy-0.4.1/src/owmpy/current/__init__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1211 2022-11-16 21:38:28.000000 owmpy-0.4.1/src/owmpy/current/_classes.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)     3004 2022-11-16 21:38:51.000000 owmpy-0.4.1/src/owmpy/current/response.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.674922 owmpy-0.4.1/src/owmpy/utils/
--rw-r--r--   0 ernie     (1000) ernie     (1000)       68 2022-03-26 09:52:06.000000 owmpy-0.4.1/src/owmpy/utils/__init__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)      727 2022-11-16 21:35:59.000000 owmpy-0.4.1/src/owmpy/utils/_classes.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)     2531 2022-11-15 14:56:54.000000 owmpy-0.4.1/src/owmpy/utils/units.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-11-16 21:42:56.673922 owmpy-0.4.1/src/owmpy.egg-info/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1447 2022-11-16 21:42:56.000000 owmpy-0.4.1/src/owmpy.egg-info/PKG-INFO
--rw-r--r--   0 ernie     (1000) ernie     (1000)      367 2022-11-16 21:42:56.000000 owmpy-0.4.1/src/owmpy.egg-info/SOURCES.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)        1 2022-11-16 21:42:56.000000 owmpy-0.4.1/src/owmpy.egg-info/dependency_links.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)        6 2022-11-16 21:42:56.000000 owmpy-0.4.1/src/owmpy.egg-info/top_level.txt
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.425948 owmpy-1.0.0/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1081 2024-04-07 10:00:37.000000 owmpy-1.0.0/LICENSE
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       25 2024-04-07 13:21:34.000000 owmpy-1.0.0/MANIFEST.in
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 13:32:03.425948 owmpy-1.0.0/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      778 2024-04-07 12:42:49.000000 owmpy-1.0.0/README.md
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.418948 owmpy-1.0.0/owmpy/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      261 2024-04-07 12:56:00.000000 owmpy-1.0.0/owmpy/__init__.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.420948 owmpy-1.0.0/owmpy/core/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       76 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/core/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       40 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/core/api_exception.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      795 2024-04-07 12:48:31.000000 owmpy-1.0.0/owmpy/core/base_client.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.421948 owmpy-1.0.0/owmpy/current/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       58 2024-04-07 12:34:14.000000 owmpy-1.0.0/owmpy/current/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      962 2024-04-07 12:34:08.000000 owmpy-1.0.0/owmpy/current/client.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.423948 owmpy-1.0.0/owmpy/current/response/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      202 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/current/response/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      108 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/clouds.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      176 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/coord.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      903 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/main.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       98 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/current/response/rain.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      947 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/response.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      328 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/sys.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      481 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/weather.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      317 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/current/response/wind.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.424948 owmpy-1.0.0/owmpy/utils/
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      130 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/utils/__init__.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      218 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/utils/short_long.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     2187 2024-04-07 12:13:58.000000 owmpy-1.0.0/owmpy/utils/standard_units.py
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      451 2024-04-07 12:13:57.000000 owmpy-1.0.0/owmpy/utils/units.py
+drwxrwxr-x   0 ernie     (1000) ernie     (1000)        0 2024-04-07 13:32:03.424948 owmpy-1.0.0/owmpy.egg-info/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1243 2024-04-07 13:32:03.000000 owmpy-1.0.0/owmpy.egg-info/PKG-INFO
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      752 2024-04-07 13:32:03.000000 owmpy-1.0.0/owmpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        1 2024-04-07 13:32:03.000000 owmpy-1.0.0/owmpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       31 2024-04-07 13:32:03.000000 owmpy-1.0.0/owmpy.egg-info/requires.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)        6 2024-04-07 13:32:03.000000 owmpy-1.0.0/owmpy.egg-info/top_level.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)      231 2024-04-07 10:21:28.000000 owmpy-1.0.0/pyproject.toml
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       36 2024-04-07 10:39:25.000000 owmpy-1.0.0/requirements.txt
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)       38 2024-04-07 13:32:03.425948 owmpy-1.0.0/setup.cfg
+-rw-rw-r--   0 ernie     (1000) ernie     (1000)     1069 2024-04-07 13:31:41.000000 owmpy-1.0.0/setup.py
```

### Comparing `owmpy-0.4.1/LICENSE` & `owmpy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owmpy-0.4.1/PKG-INFO` & `owmpy-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 0.4.1
-Summary: An open-sourced wrapper to interact with the OpenWeatherMap API
+Version: 1.0.0
+Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
-Project-URL: Bug Tracker, https://github.com/ernieIzde8ski/open_weather_mappy/issues
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.7.4
+Requires-Dist: pydantic>=1.9.0
 
 # Open Weather Mappy
 
-Wrapper to interact with the [Open Weather Map](https://openweathermap.org/api) Current Weather Data API. Install from pip under the name `owmpy`.
+A wrapper for the [Open Weather Map API](https://openweathermap.org/api).
+
+## Installation
+
+`pip install owmpy`
 
 ## Usage
 
-Import the class and make requests.
+Import the API and make requests.
 
 ```py
 import asyncio
 from os import getenv
 
-from owmpy.current import CurrentWeather
+from owmpy.current import Client
 
 
 async def main():
     # Get a weather token from openweathermap.org
-    async with CurrentWeather(appid=getenv("WEATHER_TOKEN")) as weather:
+    async with Client(appid="YOUR_API_TOKEN") as weather:
         response = await weather.get((0, 0))
-        print(response)
+    print(response)
 
 
 if __name__ == "__main__":
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    loop.run_until_complete(main())
+    asyncio.run(main())
 ```
 
 Optionally, you can supply your own ClientSession:
 
 ```py
 import aiohttp
-weather = CurrentWeather(appid="token", client=aiohttp.ClientSession())
+weather = Client("YOUR_API_TOKEN", client_session=aiohttp.ClientSession())
 ```
 
 ## Building
 
 <!-- for when I inevitably forget again -->
 
 ```sh
```

### Comparing `owmpy-0.4.1/src/owmpy.egg-info/PKG-INFO` & `owmpy-1.0.0/owmpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: owmpy
-Version: 0.4.1
-Summary: An open-sourced wrapper to interact with the OpenWeatherMap API
+Version: 1.0.0
+Summary: A wrapper for the OpenWeatherMap API
 Home-page: https://github.com/ernieIzde8ski/open_weather_mappy
 Author: Ernest Izdebski
-Project-URL: Bug Tracker, https://github.com/ernieIzde8ski/open_weather_mappy/issues
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.7.4
+Requires-Dist: pydantic>=1.9.0
 
 # Open Weather Mappy
 
-Wrapper to interact with the [Open Weather Map](https://openweathermap.org/api) Current Weather Data API. Install from pip under the name `owmpy`.
+A wrapper for the [Open Weather Map API](https://openweathermap.org/api).
+
+## Installation
+
+`pip install owmpy`
 
 ## Usage
 
-Import the class and make requests.
+Import the API and make requests.
 
 ```py
 import asyncio
 from os import getenv
 
-from owmpy.current import CurrentWeather
+from owmpy.current import Client
 
 
 async def main():
     # Get a weather token from openweathermap.org
-    async with CurrentWeather(appid=getenv("WEATHER_TOKEN")) as weather:
+    async with Client(appid="YOUR_API_TOKEN") as weather:
         response = await weather.get((0, 0))
-        print(response)
+    print(response)
 
 
 if __name__ == "__main__":
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    loop.run_until_complete(main())
+    asyncio.run(main())
 ```
 
 Optionally, you can supply your own ClientSession:
 
 ```py
 import aiohttp
-weather = CurrentWeather(appid="token", client=aiohttp.ClientSession())
+weather = Client("YOUR_API_TOKEN", client_session=aiohttp.ClientSession())
 ```
 
 ## Building
 
 <!-- for when I inevitably forget again -->
 
 ```sh
```

