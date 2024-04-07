# Comparing `tmp/iolite_client-0.6.1.tar.gz` & `tmp/iolite_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iolite_client-0.6.1.tar", max compression
+gzip compressed data, was "iolite_client-0.7.0.tar", max compression
```

## Comparing `iolite_client-0.6.1.tar` & `iolite_client-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-11-01 09:23:31.968398 iolite_client-0.6.1/LICENSE.md
--rw-r--r--   0        0        0     3978 2023-11-01 09:23:31.968398 iolite_client-0.6.1/README.md
--rw-r--r--   0        0        0      131 2023-11-01 09:23:31.968398 iolite_client-0.6.1/iolite_client/__init__.py
--rwxr-xr-x   0        0        0    10885 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/client.py
--rw-r--r--   0        0        0     2755 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/entity.py
--rw-r--r--   0        0        0     3202 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/entity_factory.py
--rw-r--r--   0        0        0      346 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/exceptions.py
--rw-r--r--   0        0        0     4093 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/heating_scheduler.py
--rw-r--r--   0        0        0     8629 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/oauth_handler.py
--rw-r--r--   0        0        0     3087 2023-11-01 09:23:31.972398 iolite_client-0.6.1/iolite_client/request_handler.py
--rw-r--r--   0        0        0     1010 2023-11-01 09:24:06.926606 iolite_client-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 iolite_client-0.6.1/setup.py
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 iolite_client-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-07 18:46:24.922356 iolite_client-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     3978 2024-04-07 18:46:24.922356 iolite_client-0.7.0/README.md
+-rw-r--r--   0        0        0      131 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/__init__.py
+-rwxr-xr-x   0        0        0    11079 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/client.py
+-rw-r--r--   0        0        0     3989 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/entity.py
+-rw-r--r--   0        0        0     4757 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/entity_factory.py
+-rw-r--r--   0        0        0      346 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/exceptions.py
+-rw-r--r--   0        0        0     4093 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/heating_scheduler.py
+-rw-r--r--   0        0        0     8928 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/oauth_handler.py
+-rw-r--r--   0        0        0     3089 2024-04-07 18:46:24.922356 iolite_client-0.7.0/iolite_client/request_handler.py
+-rw-r--r--   0        0        0     1010 2024-04-07 18:46:53.754643 iolite_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 iolite_client-0.7.0/setup.py
+-rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 iolite_client-0.7.0/PKG-INFO
```

### Comparing `iolite_client-0.6.1/LICENSE.md` & `iolite_client-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iolite_client-0.6.1/README.md` & `iolite_client-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python IOLite Client
 
 ![CI](https://github.com/inverse/python-iolite-client/workflows/CI/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/a38c5dbfc12247c893b4f39db4fac2b2)](https://www.codacy.com/manual/inverse/python-iolite-client?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=inverse/python-iolite-client&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/inverse/python-iolite-client/branch/master/graph/badge.svg?token=26LC98A22C)](https://codecov.io/gh/inverse/python-iolite-client)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/decode-config)
+[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/iolite-client)
 ![PyPI downloads](https://img.shields.io/pypi/dm/iolite-client?label=pypi%20downloads)
 [![License](https://img.shields.io/github/license/inverse/python-iolite-client.svg)](LICENSE)
 
 
 Python client for [IOLite's][0] remote API.
 
 The client has basic functionality such as the authentication layer, some basic command models, and a client to change the
```

### Comparing `iolite_client-0.6.1/iolite_client/client.py` & `iolite_client-0.7.0/iolite_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -300,13 +300,16 @@
         await asyncio.create_task(self._fetch_application(requests))
         await asyncio.create_task(self._fetch_heating())
 
     def discover(self):
         """Discovers the entities registered within the heating system."""
         asyncio.run(self.async_discover())
 
-    async def async_set_temp(self, device, temp: float):
-        request = self.request_handler.get_action_request(device, temp)
+    async def async_set_property(self, device, property: str, value: float):
+        request = self.request_handler.get_action_request(device, property, value)
         await asyncio.create_task(self._fetch_application([request]))
 
-    def set_temp(self, device, temp: float):
-        asyncio.run(self.async_set_temp(device, temp))
+    def set_temp(self, device, value: float):
+        asyncio.run(self.async_set_property(device, "heatingTemperatureSetting", value))
+
+    def set_blind_level(self, device, value: float):
+        asyncio.run(self.async_set_property(device, "blindLevel", value))
```

### Comparing `iolite_client-0.6.1/iolite_client/entity.py` & `iolite_client-0.7.0/iolite_client/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,42 @@
         return cls.__name__.lower()
 
 
 class Switch(Device):
     pass
 
 
+class Blind(Device):
+    def __init__(
+        self,
+        identifier: str,
+        name: str,
+        place_identifier: str,
+        manufacturer: str,
+        blind_level: int,
+    ):
+        super().__init__(identifier, name, place_identifier, manufacturer)
+        self.blind_level = blind_level
+
+
+class HumiditySensor(Device):
+    def __init__(
+        self,
+        identifier: str,
+        name: str,
+        place_identifier: str,
+        manufacturer: str,
+        current_env_temp: float,
+        humidity_level: float,
+    ):
+        super().__init__(identifier, name, place_identifier, manufacturer)
+        self.current_env_temp = current_env_temp
+        self.humidity_level = humidity_level
+
+
 class Lamp(Device):
     pass
 
 
 class RadiatorValve(Device):
     def __init__(
         self,
@@ -49,22 +77,39 @@
         super().__init__(identifier, name, place_identifier, manufacturer)
         self.valve_position = valve_position
         self.heating_mode = heating_mode
         self.battery_level = battery_level
         self.current_env_temp = current_env_temp
 
 
+class InFloorValve(Device):
+    def __init__(
+        self,
+        identifier: str,
+        name: str,
+        place_identifier: str,
+        manufacturer: str,
+        current_env_temp: float,
+        heating_temperature_setting: float,
+        device_status: str,
+    ):
+        super().__init__(identifier, name, place_identifier, manufacturer)
+        self.heating_temperature_setting = heating_temperature_setting
+        self.device_status = device_status
+        self.current_env_temp = current_env_temp
+
+
 class Heating(Entity):
     def __init__(
         self,
         identifier: str,
         name: str,
         current_temp: float,
         target_temp: float,
-        window_open: bool,
+        window_open: Optional[bool],
     ):
         super().__init__(identifier, name)
         self.current_temp = current_temp
         self.target_temp = target_temp
         self.window_open = window_open
```

### Comparing `iolite_client-0.6.1/iolite_client/entity_factory.py` & `iolite_client-0.7.0/iolite_client/entity_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-from iolite_client.entity import Device, Heating, Lamp, RadiatorValve, Room, Switch
+from iolite_client.entity import (
+    Blind,
+    Device,
+    Heating,
+    HumiditySensor,
+    InFloorValve,
+    Lamp,
+    RadiatorValve,
+    Room,
+    Switch,
+)
 from iolite_client.exceptions import UnsupportedDeviceError
 
 
 def create_room(payload: dict) -> Room:
     entity_class = payload.get("class")
     identifier = payload.get("id")
 
@@ -38,22 +48,23 @@
     return _create_device(identifier, payload["typeName"], payload)
 
 
 def create_heating(payload: dict) -> Heating:
     return Heating(
         payload["id"],
         payload["name"],
-        payload["currentTemperature"],
+        payload.get("currentTemperature", None),
         payload["targetTemperature"],
-        payload["windowOpen"],
+        payload.get("windowOpen", None),
     )
 
 
 def _create_device(identifier: str, type_name: str, payload: dict):
     place_identifier = payload["placeIdentifier"]
+    model_name = payload.get("modelName", None)
     if type_name == "Lamp":
         return Lamp(
             identifier,
             payload["friendlyName"],
             place_identifier,
             payload["manufacturer"],
         )
@@ -69,29 +80,69 @@
             identifier,
             payload["friendlyName"],
             place_identifier,
             payload["manufacturer"],
         )
     elif type_name == "Heater":
         properties = payload["properties"]
+        current_env_temp = _get_prop(properties, "currentEnvironmentTemperature")
+
+        if model_name is not None and model_name.startswith("38de6001c3ad"):
+            heating_temperature_setting = _get_prop(
+                properties, "heatingTemperatureSetting"
+            )
+            device_status = _get_prop(properties, "deviceStatus")
+            return InFloorValve(
+                identifier,
+                payload["friendlyName"],
+                place_identifier,
+                payload["manufacturer"],
+                current_env_temp,
+                heating_temperature_setting,
+                device_status,
+            )
+
+        else:
+            battery_level = _get_prop(properties, "batteryLevel")
+            heating_mode = _get_prop(properties, "heatingMode")
+            valve_position = _get_prop(properties, "valvePosition")
+
+            return RadiatorValve(
+                identifier,
+                payload["friendlyName"],
+                place_identifier,
+                payload["manufacturer"],
+                current_env_temp,
+                battery_level,
+                heating_mode,
+                valve_position,
+            )
+    elif type_name == "Blind":
+        properties = payload["properties"]
+        blind_level = _get_prop(properties, "blindLevel")
 
+        return Blind(
+            identifier,
+            payload["friendlyName"],
+            place_identifier,
+            payload["manufacturer"],
+            blind_level,
+        )
+    elif type_name == "HumiditySensor":
+        properties = payload["properties"]
         current_env_temp = _get_prop(properties, "currentEnvironmentTemperature")
-        battery_level = _get_prop(properties, "batteryLevel")
-        heating_mode = _get_prop(properties, "heatingMode")
-        valve_position = _get_prop(properties, "valvePosition")
+        humidity_level = _get_prop(properties, "humidityLevel")
 
-        return RadiatorValve(
+        return HumiditySensor(
             identifier,
             payload["friendlyName"],
             place_identifier,
             payload["manufacturer"],
             current_env_temp,
-            battery_level,
-            heating_mode,
-            valve_position,
+            humidity_level,
         )
     else:
         raise UnsupportedDeviceError(type_name, identifier, payload)
 
 
 def _get_prop(properties: list, key: str):
     """
```

### Comparing `iolite_client-0.6.1/iolite_client/heating_scheduler.py` & `iolite_client-0.7.0/iolite_client/heating_scheduler.py`

 * *Files identical despite different names*

### Comparing `iolite_client-0.6.1/iolite_client/oauth_handler.py` & `iolite_client-0.7.0/iolite_client/oauth_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 BASE_URL = "https://remote.iolite.de"
 CLIENT_ID = "deuwo_mia_app"
 
 
 class OAuthHandlerHelper:
     @staticmethod
-    def get_access_token_query(code: str, name: str) -> str:
+    def get_access_token_query(code: str, name: str, client_id: str) -> str:
         return urlencode(
             {
-                "client_id": CLIENT_ID,
+                "client_id": client_id,
                 "grant_type": "authorization_code",
                 "code": code,
                 "name": name,
             }
         )
 
     @staticmethod
-    def get_new_access_token_query(refresh_token: str) -> str:
+    def get_new_access_token_query(refresh_token: str, client_id: str) -> str:
         return urlencode(
             {
-                "client_id": CLIENT_ID,
+                "client_id": client_id,
                 "grant_type": "refresh_token",
                 "refresh_token": refresh_token,
             }
         )
 
     @staticmethod
     def get_sid_query(access_token: str) -> str:
@@ -49,39 +49,42 @@
         expires_at = time.time() + token["expires_in"]
         token.update({"expires_at": expires_at})
         del token["expires_in"]
         return token
 
 
 class OAuthHandler:
-    def __init__(self, username: str, password: str):
+    def __init__(self, username: str, password: str, client_id: str = CLIENT_ID):
         self.username = username
         self.password = password
+        self.client_id = client_id
 
     def get_access_token(self, code: str, name: str) -> dict:
         """
         Get access token.
         :param code: The pairing code
         :param name: The name of the device being paired
         :return:
         """
-        query = OAuthHandlerHelper.get_access_token_query(code, name)
+        query = OAuthHandlerHelper.get_access_token_query(code, name, self.client_id)
         response = requests.post(
             f"{BASE_URL}/ui/token?{query}", auth=(self.username, self.password)
         )
         response.raise_for_status()
         return OAuthHandlerHelper.add_expires_at(json.loads(response.text))
 
     def get_new_access_token(self, refresh_token: str) -> dict:
         """
         Get new access token
         :param refresh_token: The refresh token
         :return: dict containing access token, and new refresh token
         """
-        query = OAuthHandlerHelper.get_new_access_token_query(refresh_token)
+        query = OAuthHandlerHelper.get_new_access_token_query(
+            refresh_token, self.client_id
+        )
         response = requests.post(
             f"{BASE_URL}/ui/token?{query}", auth=(self.username, self.password)
         )
         response.raise_for_status()
         return OAuthHandlerHelper.add_expires_at(json.loads(response.text))
 
     def get_sid(self, access_token: str) -> str:
@@ -96,42 +99,49 @@
         )
         response.raise_for_status()
         return json.loads(response.text).get("SID")
 
 
 class AsyncOAuthHandler:
     def __init__(
-        self, username: str, password: str, web_session: aiohttp.ClientSession
+        self,
+        username: str,
+        password: str,
+        web_session: aiohttp.ClientSession,
+        client_id: str = CLIENT_ID,
     ):
         self.username = username
         self.password = password
         self.web_session = web_session
+        self.client_id = client_id
 
     async def get_access_token(self, code: str, name: str) -> dict:
         """
         Get access token.
         :param code: The pairing code
         :param name: The name of the device being paired
         :return:
         """
-        query = OAuthHandlerHelper.get_access_token_query(code, name)
+        query = OAuthHandlerHelper.get_access_token_query(code, name, self.client_id)
         response = await self.web_session.post(
             f"{BASE_URL}/ui/token?{query}",
             auth=aiohttp.BasicAuth(self.username, self.password),
         )
         response.raise_for_status()
         return OAuthHandlerHelper.add_expires_at(await response.json())
 
     async def get_new_access_token(self, refresh_token: str) -> dict:
         """
         Get new access token
         :param refresh_token: The refresh token
         :return: dict containing access token, and new refresh token
         """
-        query = OAuthHandlerHelper.get_new_access_token_query(refresh_token)
+        query = OAuthHandlerHelper.get_new_access_token_query(
+            refresh_token, self.client_id
+        )
         response = await self.web_session.post(
             f"{BASE_URL}/ui/token?{query}",
             auth=aiohttp.BasicAuth(self.username, self.password),
         )
         response.raise_for_status()
         return OAuthHandlerHelper.add_expires_at(await response.json())
```

### Comparing `iolite_client-0.6.1/iolite_client/request_handler.py` & `iolite_client-0.7.0/iolite_client/request_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,26 +30,26 @@
                 "callback": "",
                 "minimumUpdateInterval": 100,
             },
         )
 
         return request
 
-    def get_action_request(self, device_id: str, temp: float) -> dict:
+    def get_action_request(self, device_id: str, property: str, value: float) -> dict:
         request = self._build_request(
             ClassMap.ActionRequest.value,
             {
                 "modelID": "http://iolite.de#Environment",
                 "class": ClassMap.ActionRequest.value,
-                "objectQuery": f"devices[id='{device_id}']/properties[name='heatingTemperatureSetting']",
+                "objectQuery": f"devices[id='{device_id}']/properties[name='{property}']",
                 "actionName": "requestValueUpdate",
                 "parameters": [
                     {
                         "class": "ValueParameter",
-                        "value": temp,
+                        "value": value,
                     }
                 ],
             },
         )
 
         return request
```

### Comparing `iolite_client-0.6.1/pyproject.toml` & `iolite_client-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iolite-client"
-version = "0.6.1"
+version = "0.7.0"
 description = "API client for interacting with IOLite's remote API"
 authors = ["Malachi Soord <me@malachisoord.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/inverse/python-iolite-client"
 homepage = "https://github.com/inverse/python-iolite-client"
```

### Comparing `iolite_client-0.6.1/setup.py` & `iolite_client-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4,<4.0.0', 'requests', 'single-source>=0.2,<0.4', 'websockets']
 
 setup_kwargs = {
     'name': 'iolite-client',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': "API client for interacting with IOLite's remote API",
-    'long_description': '# Python IOLite Client\n\n![CI](https://github.com/inverse/python-iolite-client/workflows/CI/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/a38c5dbfc12247c893b4f39db4fac2b2)](https://www.codacy.com/manual/inverse/python-iolite-client?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=inverse/python-iolite-client&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/gh/inverse/python-iolite-client/branch/master/graph/badge.svg?token=26LC98A22C)](https://codecov.io/gh/inverse/python-iolite-client)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/decode-config)\n![PyPI downloads](https://img.shields.io/pypi/dm/iolite-client?label=pypi%20downloads)\n[![License](https://img.shields.io/github/license/inverse/python-iolite-client.svg)](LICENSE)\n\n\nPython client for [IOLite\'s][0] remote API.\n\nThe client has basic functionality such as the authentication layer, some basic command models, and a client to change the\nheating intervals are available.\n\nBuild by reverse engineering the [Deutsche Wohnen][2] [MIA Android App][1] and subsequently their remote API.\n\nRead the following [short post][3] on how that was achieved.\n\nUsed in making the [IOLite Custom Component](https://github.com/inverse/home-assistant-iolite-component) for Home Assistant.\n\n## Requirements\n\n-   Python 3.7+\n-   [Poetry][4]\n\n## Getting credentials\n\nOpen your Deutsche Wohnen tablet and begin pairing device process. Scan the QR code with your QR-Scanner and instead of\nopening the QR code in your browser, copy it\'s content. You\'ll get the following payload:\n\n```json\n{\n  "webApp": "/ui/",\n  "code": "<redacted>",\n  "basicAuth": "<redacted>"\n}\n```\n\n-   `basicAuth` contains base64 encoded HTTP basic username and password. Decode this to get the `:` separated `user:pass`.\n-   `code` is the pairing code\n\nYou can decode the credentials using the `scripts/get_credentials.py` script. e.g.\n\n```bash\n python scripts/get_credentials.py \'{"webApp":"/ui/","code":"<redacted>","basicAuth":"<redacted>"}\'\n```\n\n## Development\n\n-   Init your virtualenv environment (`poetry install`)\n-   Copy `.env.example` to `.env`\n-   Decode credentials (`poetry run python scripts/get_credentials.py <basic-auth-value>`)\n-   Add your credentials to `.env` following the above process\n\nThe [pre-commit][5] framework is used enforce some linting and style compliance on CI.\n\nTo get the same behaviour locally you can run `pre-commit install` within your activated venv.\n\nAlternatively to run manually you can run `pre-commit run -a`.\n\n## Access remote UI\n\nRun `poetry run python scripts/example.py` and copy the URL to your browser of choice.\n\nYou will need the HTTP basic credentials you defined earlier within the `.env` file.\n\nBe sure to run `poetry install -E dev` to get the required dependencies for this.\n\n## Usage example\n\nA jupyter notebook showcasing the heating interval scheduler can be found in `notebooks/Heating Scheduler.ipynb`. To\naccess the notebook install [jupyter notebook or jupyter lab](https://jupyter.org/install.html) into the virtual environment and run the notebook:\n\n```sh\npoetry shell\npip install notebook\njupyter notebook\n```\n\nIf running the notebook gives you a `ModuleNotFoundError`, you may fix this issue by changing the notebook\'s kernel (following [this StackOverflow post](https://stackoverflow.com/a/47296960/50913)):\n\n```sh\npoetry shell\npython -m ipykernel install --user --name=`basename $VIRTUAL_ENV`\n```\n\nThen switch the kernel in the notebook\'s top menu under: _Kernel > Change Kernel_.\n\n## Licence\n\nMIT\n\n[0]: https://iolite.de/\n\n[1]: https://play.google.com/store/apps/details?id=de.iolite.client.android.mia\n\n[2]: https://deutsche-wohnen.com/\n\n[3]: https://www.malachisoord.com/2020/08/06/reverse-engineering-iolite-remote-api/\n\n[4]: https://python-poetry.org/\n\n[5]: https://pre-commit.com/\n',
+    'long_description': '# Python IOLite Client\n\n![CI](https://github.com/inverse/python-iolite-client/workflows/CI/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/a38c5dbfc12247c893b4f39db4fac2b2)](https://www.codacy.com/manual/inverse/python-iolite-client?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=inverse/python-iolite-client&amp;utm_campaign=Badge_Grade)\n[![codecov](https://codecov.io/gh/inverse/python-iolite-client/branch/master/graph/badge.svg?token=26LC98A22C)](https://codecov.io/gh/inverse/python-iolite-client)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/iolite-client)\n![PyPI downloads](https://img.shields.io/pypi/dm/iolite-client?label=pypi%20downloads)\n[![License](https://img.shields.io/github/license/inverse/python-iolite-client.svg)](LICENSE)\n\n\nPython client for [IOLite\'s][0] remote API.\n\nThe client has basic functionality such as the authentication layer, some basic command models, and a client to change the\nheating intervals are available.\n\nBuild by reverse engineering the [Deutsche Wohnen][2] [MIA Android App][1] and subsequently their remote API.\n\nRead the following [short post][3] on how that was achieved.\n\nUsed in making the [IOLite Custom Component](https://github.com/inverse/home-assistant-iolite-component) for Home Assistant.\n\n## Requirements\n\n-   Python 3.7+\n-   [Poetry][4]\n\n## Getting credentials\n\nOpen your Deutsche Wohnen tablet and begin pairing device process. Scan the QR code with your QR-Scanner and instead of\nopening the QR code in your browser, copy it\'s content. You\'ll get the following payload:\n\n```json\n{\n  "webApp": "/ui/",\n  "code": "<redacted>",\n  "basicAuth": "<redacted>"\n}\n```\n\n-   `basicAuth` contains base64 encoded HTTP basic username and password. Decode this to get the `:` separated `user:pass`.\n-   `code` is the pairing code\n\nYou can decode the credentials using the `scripts/get_credentials.py` script. e.g.\n\n```bash\n python scripts/get_credentials.py \'{"webApp":"/ui/","code":"<redacted>","basicAuth":"<redacted>"}\'\n```\n\n## Development\n\n-   Init your virtualenv environment (`poetry install`)\n-   Copy `.env.example` to `.env`\n-   Decode credentials (`poetry run python scripts/get_credentials.py <basic-auth-value>`)\n-   Add your credentials to `.env` following the above process\n\nThe [pre-commit][5] framework is used enforce some linting and style compliance on CI.\n\nTo get the same behaviour locally you can run `pre-commit install` within your activated venv.\n\nAlternatively to run manually you can run `pre-commit run -a`.\n\n## Access remote UI\n\nRun `poetry run python scripts/example.py` and copy the URL to your browser of choice.\n\nYou will need the HTTP basic credentials you defined earlier within the `.env` file.\n\nBe sure to run `poetry install -E dev` to get the required dependencies for this.\n\n## Usage example\n\nA jupyter notebook showcasing the heating interval scheduler can be found in `notebooks/Heating Scheduler.ipynb`. To\naccess the notebook install [jupyter notebook or jupyter lab](https://jupyter.org/install.html) into the virtual environment and run the notebook:\n\n```sh\npoetry shell\npip install notebook\njupyter notebook\n```\n\nIf running the notebook gives you a `ModuleNotFoundError`, you may fix this issue by changing the notebook\'s kernel (following [this StackOverflow post](https://stackoverflow.com/a/47296960/50913)):\n\n```sh\npoetry shell\npython -m ipykernel install --user --name=`basename $VIRTUAL_ENV`\n```\n\nThen switch the kernel in the notebook\'s top menu under: _Kernel > Change Kernel_.\n\n## Licence\n\nMIT\n\n[0]: https://iolite.de/\n\n[1]: https://play.google.com/store/apps/details?id=de.iolite.client.android.mia\n\n[2]: https://deutsche-wohnen.com/\n\n[3]: https://www.malachisoord.com/2020/08/06/reverse-engineering-iolite-remote-api/\n\n[4]: https://python-poetry.org/\n\n[5]: https://pre-commit.com/\n',
     'author': 'Malachi Soord',
     'author_email': 'me@malachisoord.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/inverse/python-iolite-client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `iolite_client-0.6.1/PKG-INFO` & `iolite_client-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iolite-client
-Version: 0.6.1
+Version: 0.7.0
 Summary: API client for interacting with IOLite's remote API
 Home-page: https://github.com/inverse/python-iolite-client
 License: MIT
 Author: Malachi Soord
 Author-email: me@malachisoord.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 
 # Python IOLite Client
 
 ![CI](https://github.com/inverse/python-iolite-client/workflows/CI/badge.svg)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/a38c5dbfc12247c893b4f39db4fac2b2)](https://www.codacy.com/manual/inverse/python-iolite-client?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=inverse/python-iolite-client&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/inverse/python-iolite-client/branch/master/graph/badge.svg?token=26LC98A22C)](https://codecov.io/gh/inverse/python-iolite-client)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/decode-config)
+[![PyPI version](https://badge.fury.io/py/iolite-client.svg)](https://badge.fury.io/py/iolite-client)
 ![PyPI downloads](https://img.shields.io/pypi/dm/iolite-client?label=pypi%20downloads)
 [![License](https://img.shields.io/github/license/inverse/python-iolite-client.svg)](LICENSE)
 
 
 Python client for [IOLite's][0] remote API.
 
 The client has basic functionality such as the authentication layer, some basic command models, and a client to change the
```

