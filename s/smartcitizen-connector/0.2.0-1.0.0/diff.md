# Comparing `tmp/smartcitizen-connector-0.2.0.tar.gz` & `tmp/smartcitizen-connector-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen-connector-0.2.0.tar", last modified: Wed Dec 21 13:36:10 2022, max compression
+gzip compressed data, was "smartcitizen-connector-1.0.0.tar", last modified: Sun Apr  7 15:53:08 2024, max compression
```

## Comparing `smartcitizen-connector-0.2.0.tar` & `smartcitizen-connector-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,37 @@
-drwxr-xr-x   0 macoscar   (501) staff       (20)        0 2022-12-21 13:36:10.917794 smartcitizen-connector-0.2.0/
--rw-r--r--   0 macoscar   (501) staff       (20)    35149 2022-10-20 14:08:33.000000 smartcitizen-connector-0.2.0/LICENSE
--rw-r--r--   0 macoscar   (501) staff       (20)       69 2022-11-16 16:38:46.000000 smartcitizen-connector-0.2.0/MANIFEST.in
--rw-r--r--   0 macoscar   (501) staff       (20)     1730 2022-12-21 13:36:10.918022 smartcitizen-connector-0.2.0/PKG-INFO
--rw-r--r--   0 macoscar   (501) staff       (20)      598 2022-11-16 16:36:16.000000 smartcitizen-connector-0.2.0/README.md
--rw-r--r--   0 macoscar   (501) staff       (20)       79 2022-12-21 13:36:10.918839 smartcitizen-connector-0.2.0/setup.cfg
--rw-r--r--   0 macoscar   (501) staff       (20)     1729 2022-12-21 13:35:44.000000 smartcitizen-connector-0.2.0/setup.py
-drwxr-xr-x   0 macoscar   (501) staff       (20)        0 2022-12-21 13:36:10.620280 smartcitizen-connector-0.2.0/src/
-drwxr-xr-x   0 macoscar   (501) staff       (20)        0 2022-12-21 13:36:10.623468 smartcitizen-connector-0.2.0/src/smartcitizen_connector/
--rw-r--r--   0 macoscar   (501) staff       (20)      285 2022-12-02 10:24:35.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector/__init__.py
--rw-r--r--   0 macoscar   (501) staff       (20)     2004 2022-12-02 10:34:00.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector/models.py
--rw-r--r--   0 macoscar   (501) staff       (20)    30980 2022-12-21 13:35:35.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector/smartcitizen_connector.py
-drwxr-xr-x   0 macoscar   (501) staff       (20)        0 2022-12-21 13:36:10.917320 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/
--rw-r--r--   0 macoscar   (501) staff       (20)     1730 2022-12-21 13:36:09.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 macoscar   (501) staff       (20)      426 2022-12-21 13:36:10.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 macoscar   (501) staff       (20)        1 2022-12-21 13:36:09.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 macoscar   (501) staff       (20)       48 2022-12-21 13:36:09.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 macoscar   (501) staff       (20)       23 2022-12-21 13:36:09.000000 smartcitizen-connector-0.2.0/src/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24197 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.046855 smartcitizen-connector-1.0.0/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-07 15:53:03.000000 smartcitizen-connector-1.0.0/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:53:08.050855 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 15:53:08.000000 smartcitizen-connector-1.0.0/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen-connector-0.2.0/LICENSE` & `smartcitizen-connector-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen-connector-0.2.0/setup.py` & `smartcitizen-connector-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,37 +12,47 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="0.2.0",
+    version="1.0.0",
     description="Python connector to download information collected in SmartCitizen API",
-    author="Óscar González",
+    author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
     project_urls=PROJECT_URLS,
-    py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     python_requires=">=3.6",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: Unix",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Utilities",
         "Natural Language :: English",
     ],
-    install_requires=["pydantic", "requests", "pandas", "timezonefinder", "urllib3"],
+    install_requires=["pydantic",
+        "requests",
+        "pandas",
+        "timezonefinder",
+        "urllib3",
+        "aiohttp",
+        "aiohttp-retry",
+        "termcolor",
+        "tqdm"],
+    setup_requires=['wheel'],
+    zip_safe=False
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `smartcitizen-connector-0.2.0/src/smartcitizen_connector/models.py` & `smartcitizen-connector-1.0.0/smartcitizen_connector/models/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,117 @@
 from datetime import datetime
 from typing import Optional, List
 from pydantic import BaseModel
 
+class Measurement(BaseModel):
+    id: int
+    name: str
+    description: str
+
+class Metric(BaseModel):
+    id: Optional[int] = None
+    name: str
+    description: Optional[str] = ''
+    module: Optional[str] = "scdata.device.process"
+    function: str
+    unit: Optional[str] = ''
+    post: Optional[bool] = False
+    args: Optional[dict] = None
+    kwargs: Optional[dict] = None
+
 class Sensor(BaseModel):
     id: int
-    name: Optional[str] = None
-    description: Optional[str] = None
+    name: str
+    description: str
     unit: Optional[str] = None
+    measurement_id: Optional[int] = None
+    measurement: Optional[Measurement] = None
+    value: Optional[float] = None
+    prev_value: Optional[float] = None
+    last_reading_at: Optional[datetime] = None
+    tags: Optional[List[str]] = []
+    default_key: Optional[str] = []
 
 class Kit(BaseModel):
     id: int
-    slug: Optional[str] = None
-    name: Optional[str] = None
-    description: Optional[str] = None
-    created_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
+    slug: str
+    name: str
+    description: str
+    created_at: datetime
+    updated_at: datetime
     sensors: Optional[List[Sensor]] = None
 
 class Owner(BaseModel):
     id: int
-    username: Optional[str] = None
-    username: Optional[str] = None
+    username: str
+    role: Optional[str] = ""
+    devices: Optional[List[str]] = None
 
 class Location(BaseModel):
+    city: str
+    country_code: str
+    country: str
+    exposure: Optional[str] = None
+    elevation: Optional[float] = None
+    geohash: Optional[str] = None
     latitude: Optional[float] = None
     longitude: Optional[float] = None
-    city: Optional[str] = None
-    country_code: Optional[str] = None
+
+class HardwareInfo(BaseModel):
+    id: str
+    mac: str
+    time: str
+    esp_bd: str
+    hw_ver: str
+    sam_bd: str
+    esp_ver: str
+    sam_ver: str
+    rcause: Optional[str] = None
+
+class HardwareVersion(BaseModel):
+    from_date: Optional[datetime] = None
+    to_date: Optional[datetime] = None
+    ids: Optional[dict] = None
+
+class HardwarePostprocessing(BaseModel):
+    blueprint_url: Optional[str] = None
+    description: Optional[str] = None
+    versions: Optional[List[HardwareVersion]] = None
+    forwarding: Optional[str] = None
+
+class Postprocessing(BaseModel):
+    id: int
+    blueprint_url: Optional[str] = None
+    hardware_url: Optional[str] = None
+    forwarding_params: Optional[int] = None
+    meta: Optional[str] = None
+    latest_postprocessing: Optional[datetime] = None
+    created_at: datetime
+    updated_at: datetime
 
 class Data(BaseModel):
-    location: Optional[Location]= None
     sensors: Optional[List[Sensor]] = None
 
-class DeviceSummary(BaseModel):
-    id: int
-    name: Optional[str] = None
-    description: Optional[str] = None
-    added_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
-    last_reading_at: Optional[datetime] = None
-    owner_id: Optional[int] = None
-    owner_username: Optional[str] = None
-    user_tags: Optional[List] = None
-    system_tags: Optional[List] = None
-    state: Optional[str] = None
-    kit_id: Optional[float] = None
-    latitude: Optional[float] = None
-    longitude: Optional[float] = None
-    city: Optional[str] = None
-    country_code: Optional[str] = None
+class Notifications(BaseModel):
+    low_battery: bool
+    stopped_publishing: bool
 
 class Device(BaseModel):
     id: int
-    name: Optional[str] = None
-    description: Optional[str] = None
-    added_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
+    uuid: str
+    name: str
+    description: str
+    state: str
+    postprocessing: Optional[Postprocessing] = None
+    hardware_info: Optional[HardwareInfo] = None
+    system_tags: List[str]
+    user_tags: List[str]
+    is_private: bool
+    notify: Notifications
     last_reading_at: Optional[datetime] = None
-    data: Optional[Data] = None
-    owner: Optional[Owner] = None
-    owner_id: Optional[int] = None
-    owner_username: Optional[str] = None
-    user_tags: Optional[List] = None
-    system_tags: Optional[List] = None
-    state: Optional[str] = None
+    created_at: Optional[datetime] = None
+    updated_at: datetime
+    owner: Owner
+    data: Data
+    location: Optional[Location]= None
     kit: Optional[Kit] = None
+    device_token: Optional[str] = ''
```

