# Comparing `tmp/fyta_cli-0.3.4.tar.gz` & `tmp/fyta_cli-0.3.5.tar.gz`

## Comparing `fyta_cli-0.3.4.tar` & `fyta_cli-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/src/fyta_cli/__init__.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/src/fyta_cli/fyta_client.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/src/fyta_cli/fyta_connector.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/src/fyta_cli/fyta_exceptions.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/src/fyta_cli/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/__init__.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_client.py
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_connector.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/fyta_exceptions.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/src/fyta_cli/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 fyta_cli-0.3.5/PKG-INFO
```

### Comparing `fyta_cli-0.3.4/.github/workflows/pylint.yml` & `fyta_cli-0.3.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.4/.github/workflows/python-publish.yml` & `fyta_cli-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.4/.github/workflows/ruff.yml` & `fyta_cli-0.3.5/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.4/src/fyta_cli/fyta_client.py` & `fyta_cli-0.3.5/src/fyta_cli/fyta_client.py`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.4/src/fyta_cli/fyta_connector.py` & `fyta_cli-0.3.5/src/fyta_cli/fyta_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Connector class to manage access to FYTA API."""
 
-from datetime import datetime
+from datetime import datetime, UTC
 from typing import Any
 from zoneinfo import ZoneInfo
 
 from .fyta_client import Client
 from .utils import safe_get
 
 PLANT_STATUS = {
@@ -35,15 +35,15 @@
         self.password: str = password
         self.client = Client(email, password, access_token, expiration)
         self.online: bool = False
         self.plant_list: dict[int, str] = {}
         self.plants: dict[int, dict[str, Any]] = {}
         self.access_token: str = access_token
         self.expiration: datetime | None = expiration
-        self.timezone: ZoneInfo = datetime.UTC if tz == "" else ZoneInfo(tz)
+        self.timezone: ZoneInfo = UTC if tz == "" else ZoneInfo(tz)
 
     async def test_connection(self) -> bool:
         """Test if connection to FYTA API works."""
 
         return await self.client.test_connection()
 
     async def login(self) -> dict[str, str | datetime]:
@@ -117,17 +117,16 @@
                 "light": safe_get(plant_data, "measurements.light.values.current", float)}
             current_plant |= {
                 "moisture": safe_get(plant_data, "measurements.moisture.values.current", float)}
             current_plant |= {
                 "salinity": safe_get(plant_data, "measurements.salinity.values.current", float)}
             current_plant |= {"battery_level": safe_get(plant_data, "measurements.battery", float)}
             current_plant |= {
-                "last_updated": datetime.fromisoformat(
-                    plant_data["sensor"]["received_data_at"]
-                ).astimezone(self.timezone)
+                "last_updated": safe_get(
+                    plant_data, "sensor.received_data_at", datetime, self.timezone)
             }
 
         return current_plant
 
     @property
     def fyta_id(self) -> str:
         """ID for FYTA object."""
```

### Comparing `fyta_cli-0.3.4/src/fyta_cli/utils.py` & `fyta_cli-0.3.5/src/fyta_cli/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Utility functions for the FYTA integration."""
+from datetime import datetime
+from zoneinfo import ZoneInfo
 
-
-def safe_get(plant_data, key_path, expected_type):
+def safe_get(plant_data: dict, key_path: str, expected_type, tz: ZoneInfo | None = None):
     """Get a value from a nested dictionary and cast it to the expected type.
 
     Args:
         plant_data: The dictionary to get the value from.
         key_path: The path to the value in the dictionary. Seüarated by dots.
         expected_type: The expected type of the value (int, float, bool and str supported).
+        tz: Timezone needed to localize datetime (only required, if expected_type is datetime). 
 
     Returns: The value from the dictionary or None if the value is not found or the type is not
     as expected.
     """
     keys = key_path.split(".")
     value = plant_data
     try:
@@ -26,14 +28,21 @@
         return_value = __get_int(value)
     if expected_type == float:
         return_value =  __get_float(value)
     if expected_type == bool:
         return_value = __get_bool(value)
     if expected_type == str:
         return_value = str(value)
+    if expected_type == datetime:
+        return_value = __get_datetime(value, tz)
+
+    if "status" in keys and (return_value < 1 or return_value > 5):
+        #FYTA status has a scale from 1 to 5; return None, if no correct status is set
+        return_value = None
+
     return return_value
 
 
 def __get_bool(value):
     if isinstance(value, bool):
         return value
     if isinstance(value, str):
@@ -52,7 +61,15 @@
 
 
 def __get_int(value):
     try:
         return int(value)
     except (ValueError, TypeError):
         return None
+
+
+def __get_datetime(value: str, tz: str):
+    try:
+        return datetime.fromisoformat(value).astimezone(tz)
+    except (ValueError, TypeError):
+        return None
+
```

### Comparing `fyta_cli-0.3.4/LICENSE` & `fyta_cli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fyta_cli-0.3.4/pyproject.toml` & `fyta_cli-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fyta_cli"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the FYTA API"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `fyta_cli-0.3.4/PKG-INFO` & `fyta_cli-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fyta_cli
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python library to access the FYTA API
 Project-URL: Repository, https://github.com/dontinelli/fyta_cli.git
 Project-URL: Issues, https://github.com/dontinelli/fyta_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/fyta_cli/blob/master/CHANGELOG.md
 Project-URL: FYTA homepage, https://fyta.de/
 Project-URL: API Documentation, https://fyta-io.notion.site/FYTA-Public-API-d2f4c30306f74504924c9a40402a3afd
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

