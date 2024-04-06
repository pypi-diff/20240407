# Comparing `tmp/vivintpy-2023.3.8.tar.gz` & `tmp/vivintpy-2023.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivintpy-2023.3.8.tar", max compression
+gzip compressed data, was "vivintpy-2023.3.9.tar", max compression
```

## Comparing `vivintpy-2023.3.8.tar` & `vivintpy-2023.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1076 2024-03-04 19:32:00.688794 vivintpy-2023.3.8/LICENSE
--rw-r--r--   0        0        0     2658 2024-03-04 19:32:00.688794 vivintpy-2023.3.8/README.md
--rw-r--r--   0        0        0     1046 2024-03-04 19:32:15.356963 vivintpy-2023.3.8/pyproject.toml
--rw-r--r--   0        0        0       63 2024-03-04 19:32:15.356963 vivintpy-2023.3.8/vivintpy/__init__.py
--rw-r--r--   0        0        0     7673 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/account.py
--rw-r--r--   0        0        0     4371 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/const.py
--rw-r--r--   0        0        0     8197 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/__init__.py
--rw-r--r--   0        0        0    12024 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/alarm_panel.py
--rw-r--r--   0        0        0     9317 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/camera.py
--rw-r--r--   0        0        0     1279 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/door_lock.py
--rw-r--r--   0        0        0     2068 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/garage_door.py
--rw-r--r--   0        0        0     1798 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/switch.py
--rw-r--r--   0        0        0     3325 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/thermostat.py
--rw-r--r--   0        0        0     3274 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/devices/wireless_sensor.py
--rw-r--r--   0        0        0     1657 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/entity.py
--rw-r--r--   0        0        0    12803 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/enums.py
--rw-r--r--   0        0        0      705 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/exceptions.py
--rw-r--r--   0        0        0    81878 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/proto/beam_pb2.py
--rw-r--r--   0        0        0   102437 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/proto/beam_pb2.pyi
--rw-r--r--   0        0        0   168580 2024-03-04 19:32:00.692794 vivintpy-2023.3.8/vivintpy/proto/beam_pb2_grpc.py
--rw-r--r--   0        0        0     1958 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/pubnub.py
--rw-r--r--   0        0        0        0 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/py.typed
--rw-r--r--   0        0        0     3664 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/system.py
--rw-r--r--   0        0        0     1288 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/utils.py
--rw-r--r--   0        0        0    19651 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/vivintskyapi.py
--rw-r--r--   0        0        0   411296 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/zjs_device_config_db.json
--rw-r--r--   0        0        0     1036 2024-03-04 19:32:00.696794 vivintpy-2023.3.8/vivintpy/zjs_device_config_db.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 vivintpy-2023.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/LICENSE
+-rw-r--r--   0        0        0     2658 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/README.md
+-rw-r--r--   0        0        0     1049 2024-04-06 22:25:48.560179 vivintpy-2023.3.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-06 22:25:48.560179 vivintpy-2023.3.9/vivintpy/__init__.py
+-rw-r--r--   0        0        0     7674 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/account.py
+-rw-r--r--   0        0        0     4371 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/const.py
+-rw-r--r--   0        0        0     8198 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/__init__.py
+-rw-r--r--   0        0        0    12193 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/alarm_panel.py
+-rw-r--r--   0        0        0    10352 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/camera.py
+-rw-r--r--   0        0        0     1280 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/door_lock.py
+-rw-r--r--   0        0        0     2069 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/garage_door.py
+-rw-r--r--   0        0        0     1799 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/switch.py
+-rw-r--r--   0        0        0     3326 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/thermostat.py
+-rw-r--r--   0        0        0     3275 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/devices/wireless_sensor.py
+-rw-r--r--   0        0        0     1658 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/entity.py
+-rw-r--r--   0        0        0    12804 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/enums.py
+-rw-r--r--   0        0        0      705 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/exceptions.py
+-rw-r--r--   0        0        0    81878 2024-04-06 22:25:33.244201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2.py
+-rw-r--r--   0        0        0   102437 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2.pyi
+-rw-r--r--   0        0        0   168580 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/proto/beam_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/pubnub.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/py.typed
+-rw-r--r--   0        0        0     3665 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/system.py
+-rw-r--r--   0        0        0     1289 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/utils.py
+-rw-r--r--   0        0        0    19652 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/vivintskyapi.py
+-rw-r--r--   0        0        0   429866 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/zjs_device_config_db.json
+-rw-r--r--   0        0        0     1037 2024-04-06 22:25:33.248201 vivintpy-2023.3.9/vivintpy/zjs_device_config_db.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 vivintpy-2023.3.9/PKG-INFO
```

### Comparing `vivintpy-2023.3.8/LICENSE` & `vivintpy-2023.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/README.md` & `vivintpy-2023.3.9/README.md`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/pyproject.toml` & `vivintpy-2023.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vivintpy"
-version = "2023.3.8"
+version = "2023.3.9"
 description = "Python library for interacting with a Vivint security and smart home system."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/vivintpy"
 repository = "https://github.com/natekspencer/vivintpy"
 keywords = ["Vivint", "alarm system", "security", "smart home", "home automation", "asynchronous"]
@@ -16,20 +16,20 @@
 pubnub = "^7.0"
 grpcio = "^1.51.1"
 protobuf = "^4.23.1"
 
 [tool.poetry.group.dev.dependencies]
 tox = ">=3.28,<5.0"
 pytest = "^7.2.2"
-pytest-asyncio = "^0.21.0"
+pytest-asyncio = ">=0.21,<0.24"
 pytest-cov = "^4.0.0"
 pytest-timeout = "^2.1.0"
 mypy = "^1.4"
 grpcio-tools = "1.60.1"
-ruff = "^0.2.0"
+ruff = "^0.3"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 pattern = "default-unprefixed"
```

### Comparing `vivintpy-2023.3.8/vivintpy/account.py` & `vivintpy-2023.3.9/vivintpy/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the Vivint class."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 
 import aiohttp
 from aiohttp.client_exceptions import ClientConnectionError
```

### Comparing `vivintpy-2023.3.8/vivintpy/const.py` & `vivintpy-2023.3.9/vivintpy/const.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/vivintpy/devices/__init__.py` & `vivintpy-2023.3.9/vivintpy/devices/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This package contains the various devices attached to a Vivint system."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Type, cast
 
 from ..const import VivintDeviceAttribute as Attribute
 from ..entity import Entity
 from ..enums import (
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/alarm_panel.py` & `vivintpy-2023.3.9/vivintpy/devices/alarm_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the AlarmPanel class."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Any, Type
 
 from ..const import AlarmPanelAttribute as Attribute
@@ -117,14 +118,19 @@
         return self.state == ArmedState.ARMED_STAY
 
     @property
     def state(self) -> ArmedState:
         """Return the panel's armed state."""
         return ArmedState(self.data.get(Attribute.STATE))  # type: ignore
 
+    @property
+    def credentials(self) -> dict:
+        """Return the panel credentials."""
+        return self.__panel_credentials
+
     def get_armed_state(self) -> Any:
         """Return the panel's arm state."""
         send_deprecation_warning("method get_armed_state", "property state")
         return self.data[Attribute.STATE]
 
     async def set_armed_state(self, state: int) -> None:
         """Set the armed state for a panel."""
@@ -144,17 +150,17 @@
         """Set the alarm to armed stay."""
         await self.set_armed_state(ArmedState.ARMED_STAY)
 
     async def arm_away(self) -> None:
         """Set the alarm to armed away."""
         await self.set_armed_state(ArmedState.ARMED_AWAY)
 
-    async def get_panel_credentials(self) -> dict:
+    async def get_panel_credentials(self, refresh: bool = False) -> dict:
         """Get the panel credentials."""
-        if not self.__panel_credentials:
+        if refresh or not self.__panel_credentials:
             self.__panel_credentials = await self.api.get_panel_credentials(self.id)
         return self.__panel_credentials
 
     async def get_software_update_details(self) -> dict[str, bool | str]:
         """Get the software update details."""
         if not self.system.is_admin:
             _LOGGER.warning(
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/camera.py` & `vivintpy-2023.3.9/vivintpy/devices/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Module that implements the Camera class."""
+
 from __future__ import annotations
 
 import logging
 from datetime import datetime
+from enum import IntEnum
 from typing import cast
 
 from ..const import CameraAttribute as Attribute
 from ..const import PanelCredentialAttribute
 from . import VivintDevice
 from .alarm_panel import AlarmPanel
 
@@ -53,14 +55,27 @@
     "vivotek_fd8134v_camera_device": ("Vivotek", "Dome Camera (FD8134V)"),
     "vivotek_fd8151v_camera_device": ("Vivotek", "Dome Camera (FD8151V)"),
     "vivotek_hd400w_camera_device": ("Vivotek", "Outdoor Camera v2 (HD400W)"),
     "vivotek_hdp450_camera_device": ("Vivotek", "Outdoor Camera (HDP450)"),
 }
 
 
+class RtspUrlType(IntEnum):
+    """Helper class for getting a specific RTSP URL.
+
+    DIRECT - Local access through your router
+    PANEL - Local access through your panel
+    EXTERNAL - External access through the Vivint cloud
+    """
+
+    LOCAL = 0
+    PANEL = 1
+    EXTERNAL = 2
+
+
 class Camera(VivintDevice):
     """Represents a Vivint camera."""
 
     alarm_panel: AlarmPanel
 
     def __init__(self, data: dict, alarm_panel: AlarmPanel):
         """Initialize a camera."""
@@ -142,35 +157,50 @@
         return await self.api.get_camera_thumbnail_url(
             self.alarm_panel.id,
             self.alarm_panel.partition_id,
             self.id,
             thumbnail_timestamp,
         )
 
+    def get_rtsp_access_url(
+        self, access_type: RtspUrlType = RtspUrlType.LOCAL, hd: bool = True
+    ) -> str | None:
+        """Return the rtsp URL for the camera."""
+        if access_type == RtspUrlType.LOCAL:
+            return (
+                f"rtsp://{self.data[Attribute.USERNAME]}:{self.data[Attribute.PASSWORD]}@{self.ip_address}:{self.data[Attribute.CAMERA_IP_PORT]}/{self.data[Attribute.CAMERA_DIRECT_STREAM_PATH if hd else Attribute.CAMERA_DIRECT_STREAM_PATH_STANDARD]}"
+                if self.data[Attribute.CAMERA_DIRECT_AVAILABLE]
+                and self.data.get(Attribute.ACTUAL_TYPE) not in SKIP_DIRECT
+                else None
+            )
+        if not (credentials := self.alarm_panel.credentials):
+            _LOGGER.error(
+                "You must call `get_panel_credentials` before getting the RTSP url via the panel or Vivint cloud."
+            )
+            return None
+        _type = "i" if access_type == RtspUrlType.PANEL else "e"
+        url = self.data[f"c{_type}u{'' if hd else 's'}"][0]
+        return f"{url[:7]}{credentials[PanelCredentialAttribute.NAME]}:{credentials[PanelCredentialAttribute.PASSWORD]}@{url[7:]}"
+
     async def get_rtsp_url(
         self,
         internal: bool = False,
         hd: bool = False,  # pylint: disable=invalid-name
-    ) -> str:
+    ) -> str | None:
         """Return the rtsp URL for the camera."""
-        credentials = await self.alarm_panel.get_panel_credentials()
-        url = self.data[f"c{'i' if internal else 'e'}u{'' if hd else 's'}"][0]
-        return f"{url[:7]}{credentials[PanelCredentialAttribute.NAME]}:{credentials[PanelCredentialAttribute.PASSWORD]}@{url[7:]}"
+        await self.alarm_panel.get_panel_credentials()
+        access_type = RtspUrlType.PANEL if internal else RtspUrlType.EXTERNAL
+        return self.get_rtsp_access_url(access_type, hd)
 
     async def get_direct_rtsp_url(
         self,
         hd: bool = False,  # pylint: disable=invalid-name
     ) -> str | None:
         """Return the direct rtsp url for this camera, in HD if requested, if any."""
-        return (
-            f"rtsp://{self.data[Attribute.USERNAME]}:{self.data[Attribute.PASSWORD]}@{self.ip_address}:{self.data[Attribute.CAMERA_IP_PORT]}/{self.data[Attribute.CAMERA_DIRECT_STREAM_PATH if hd else Attribute.CAMERA_DIRECT_STREAM_PATH_STANDARD]}"
-            if self.data[Attribute.CAMERA_DIRECT_AVAILABLE]
-            and self.data.get(Attribute.ACTUAL_TYPE) not in SKIP_DIRECT
-            else None
-        )
+        return self.get_rtsp_access_url(RtspUrlType.LOCAL, hd)
 
     async def set_as_doorbell_chime_extender(self, state: bool) -> None:
         """Set use as doorbell chime extender."""
         await self.api.set_camera_as_doorbell_chime_extender(
             self.alarm_panel.id, self.id, state
         )
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/door_lock.py` & `vivintpy-2023.3.9/vivintpy/devices/door_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the DoorLock class."""
+
 from __future__ import annotations
 
 from ..const import ZWaveDeviceAttribute as Attribute
 from ..utils import send_deprecation_warning
 from . import BypassTamperDevice, VivintDevice
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/garage_door.py` & `vivintpy-2023.3.9/vivintpy/devices/garage_door.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the GarageDoor class."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from ..const import ZWaveDeviceAttribute as Attribute
 from ..enums import GarageDoorState
 from ..utils import send_deprecation_warning
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/switch.py` & `vivintpy-2023.3.9/vivintpy/devices/switch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the Switch class."""
+
 from __future__ import annotations
 
 from ..const import SwitchAttribute as Attribute
 from ..utils import send_deprecation_warning
 from . import VivintDevice
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/thermostat.py` & `vivintpy-2023.3.9/vivintpy/devices/thermostat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the Thermostat class."""
+
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 from ..const import ThermostatAttribute as Attribute
 from ..enums import DeviceType, FanMode, HoldMode, OperatingMode, OperatingState
```

### Comparing `vivintpy-2023.3.8/vivintpy/devices/wireless_sensor.py` & `vivintpy-2023.3.9/vivintpy/devices/wireless_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the WirelessSensor class."""
+
 from __future__ import annotations
 
 import logging
 
 from ..const import WirelessSensorAttribute as Attributes
 from ..enums import EquipmentCode, EquipmentType, SensorType
 from ..utils import first_or_none
```

### Comparing `vivintpy-2023.3.8/vivintpy/entity.py` & `vivintpy-2023.3.9/vivintpy/entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the Entity class."""
+
 from __future__ import annotations
 
 from collections.abc import Callable
 
 UPDATE = "update"
```

### Comparing `vivintpy-2023.3.8/vivintpy/enums.py` & `vivintpy-2023.3.9/vivintpy/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that defines various enums."""
+
 from __future__ import annotations
 
 import logging
 from enum import Enum, IntEnum, unique
 from typing import Any
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `vivintpy-2023.3.8/vivintpy/exceptions.py` & `vivintpy-2023.3.9/vivintpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/vivintpy/proto/beam_pb2.py` & `vivintpy-2023.3.9/vivintpy/proto/beam_pb2.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/vivintpy/proto/beam_pb2.pyi` & `vivintpy-2023.3.9/vivintpy/proto/beam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/vivintpy/proto/beam_pb2_grpc.py` & `vivintpy-2023.3.9/vivintpy/proto/beam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vivintpy-2023.3.8/vivintpy/pubnub.py` & `vivintpy-2023.3.9/vivintpy/pubnub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the VivintPubNubSubscribeListener class."""
+
 from __future__ import annotations
 
 import logging
 from collections.abc import Callable
 from enum import Enum
 from typing import Any
```

### Comparing `vivintpy-2023.3.8/vivintpy/system.py` & `vivintpy-2023.3.9/vivintpy/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the System class."""
+
 from __future__ import annotations
 
 import logging
 
 from .const import PubNubMessageAttribute
 from .const import SystemAttribute as Attribute
 from .devices.alarm_panel import AlarmPanel
```

### Comparing `vivintpy-2023.3.8/vivintpy/utils.py` & `vivintpy-2023.3.9/vivintpy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities module."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections.abc import Callable, Iterable
 from typing import Any, TypeVar
 from warnings import warn
```

### Comparing `vivintpy-2023.3.8/vivintpy/vivintskyapi.py` & `vivintpy-2023.3.9/vivintpy/vivintskyapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module that implements the VivintSkyApi class."""
+
 from __future__ import annotations
 
 import json
 import logging
 import ssl
 from collections.abc import Callable
 from http.cookies import Morsel, SimpleCookie
```

### Comparing `vivintpy-2023.3.8/vivintpy/zjs_device_config_db.json` & `vivintpy-2023.3.9/vivintpy/zjs_device_config_db.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9427253540304981%*

 * *Differences: {"'0x0000:0x0003:0x0002'": "{'description': 'Z-Wave Power Plug'}",*

 * * "'0x0000:0x0003:0x000b'": "{'description': 'Z-Wave 9 Channel_module'}",*

 * * "'0x0000:0x0004:0x0004'": "{'description': 'USB Controller', 'label': '700 Series'}",*

 * * "'0x0001:0x524d:0x3330'": "{'description': 'Wall Switch/Transmitter (2-Gang)'}",*

 * * "'0x0002:0x0248:0xa020'": "{'description': 'Z-Wave Room Sensor'}",*

 * * "'0x0002:0x5fff:0xa010'": "{'description': 'Electronic Radiator Thermostat, Intended for Use with "*

 * *                           "Water  […]*

```diff
@@ -11,46 +11,46 @@
     },
     "0x0000:0x0003:0x0001": {
         "description": "Window/Door Sensor",
         "label": "SM-A702A",
         "manufacturer": "Sigma Designs (Former Zensys)"
     },
     "0x0000:0x0003:0x0002": {
-        "description": "Z-Wave power plug",
+        "description": "Z-Wave Power Plug",
         "label": "SM-PZ701U",
         "manufacturer": "Sigma Designs (Former Zensys)"
     },
     "0x0000:0x0003:0x0003": {
         "description": "Z-Wave Battery Wall Controller",
         "label": "K8",
         "manufacturer": "Sigma Designs (Former Zensys)"
     },
     "0x0000:0x0003:0x0008": {
         "description": "Z-Wave 500 Series Controller",
         "label": "ACC-UZB3",
         "manufacturer": "Silicon Labs"
     },
     "0x0000:0x0003:0x000b": {
-        "description": "Z-wave 9 channel_module",
+        "description": "Z-Wave 9 Channel_module",
         "label": "PS9EP",
         "manufacturer": "Sigma Designs (Former Zensys)"
     },
     "0x0000:0x0003:0xa10d": {
         "description": "Z-Wave Wall Controller",
         "label": "SR-ZV9001T4-DIM",
         "manufacturer": "Sunricher"
     },
     "0x0000:0x0003:0xa305": {
         "description": "Z-Wave Battery Wall Controller",
         "label": "K8",
         "manufacturer": "Sigma Designs (Former Zensys)"
     },
     "0x0000:0x0004:0x0004": {
-        "description": "700 Series-based Controller",
-        "label": "ZST10-700",
+        "description": "USB Controller",
+        "label": "700 Series",
         "manufacturer": "Silicon Labs"
     },
     "0x0001:0x4243:0x0000": {
         "description": "Anyplace Switch",
         "label": "Aspire RF9575",
         "manufacturer": "Eaton"
     },
@@ -101,15 +101,15 @@
     },
     "0x0001:0x5246:0x3133": {
         "description": "Isolated Contact Fixture Module",
         "label": "ZRF113",
         "manufacturer": "HomePro"
     },
     "0x0001:0x524d:0x3330": {
-        "description": "Wall Switch/Transmitter (2-gang)",
+        "description": "Wall Switch/Transmitter (2-Gang)",
         "label": "ZRM230",
         "manufacturer": "HomePro"
     },
     "0x0001:0x5250:0x3030": {
         "description": "Z-Wave Plug-In Appliance Module",
         "label": "ZRP100",
         "manufacturer": "HomePro"
@@ -186,15 +186,15 @@
     },
     "0x0002:0x0248:0xa010": {
         "description": "Living Connect Z Thermostat",
         "label": "DTHERMZ6",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x0248:0xa020": {
-        "description": "Z-Wave room sensor",
+        "description": "Z-Wave Room Sensor",
         "label": "DTHERMZ5",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x0248:0xa030": {
         "description": "HC-10",
         "label": "DFBH10Z1 / 088N7110",
         "manufacturer": "Danfoss"
@@ -211,20 +211,20 @@
     },
     "0x0002:0x0804:0x2002": {
         "description": "Danfoss RXZ2C",
         "label": "087N777200",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x5fff:0xa010": {
-        "description": "Electronic radiator thermostat, intended for use with water based room radiators.",
+        "description": "Electronic Radiator Thermostat, Intended for Use with Water Based Room Radiators.",
         "label": "Keemple smart radiator",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x6fff:0xa010": {
-        "description": "Electronic radiator thermostat, intended for use with water based room radiators.",
+        "description": "Electronic Radiator Thermostat, Intended for Use with Water Based Room Radiators.",
         "label": "Keemple smart radiator",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x7fff:0xa010": {
         "description": "Genius Valve",
         "label": "014G0804",
         "manufacturer": "Danfoss"
@@ -236,15 +236,15 @@
     },
     "0x0002:0x8004:0x0001": {
         "description": "Danfoss RET BZ",
         "label": "087N774500",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x8004:0x0400": {
-        "description": "RF Relay switching unit",
+        "description": "RF Relay Switching Unit",
         "label": "RXZ",
         "manufacturer": "Danfoss"
     },
     "0x0002:0x8004:0x2010": {
         "description": "Danfoss Randall - (Single Channel RF Relay Switching Unit)",
         "label": "RZ1",
         "manufacturer": "Danfoss"
@@ -311,15 +311,15 @@
     },
     "0x0005:0x0004:0x0003": {
         "description": "Outdoor Module",
         "label": "HA04",
         "manufacturer": "Intermatic"
     },
     "0x0005:0x0005:0x0003": {
-        "description": "Screw in lamp module",
+        "description": "Screw in Lamp Module",
         "label": "HA05",
         "manufacturer": "Intermatic"
     },
     "0x0005:0x4341:0x0600": {
         "description": "Dimmer Switch",
         "label": "CA600",
         "manufacturer": "Intermatic"
@@ -346,15 +346,15 @@
     },
     "0x0005:0x4841:0x0014": {
         "description": "Dimmer Switch",
         "label": "HA14WD",
         "manufacturer": "Intermatic"
     },
     "0x0005:0x4841:0x0018": {
-        "description": "15-amp Wall Switch",
+        "description": "15-Amp Wall Switch",
         "label": "HA18",
         "manufacturer": "Intermatic"
     },
     "0x0005:0x4841:0x0020": {
         "description": "Dimmer Switch",
         "label": "HA20",
         "manufacturer": "Intermatic"
@@ -486,15 +486,15 @@
     },
     "0x0010:0x0001:0x000b": {
         "description": "Thermostat",
         "label": "TZ45",
         "manufacturer": "Residential Control Systems, Inc. (RCS)"
     },
     "0x0010:0x0001:0x1001": {
-        "description": "FIBARO -2 Gateway",
+        "description": "Fibaro -2 Gateway",
         "label": "HC",
         "manufacturer": "Residential Control Systems, Inc. (RCS)"
     },
     "0x0010:0x0504:0x3431": {
         "description": "RCS C Load Controller",
         "label": "PMC40-L",
         "manufacturer": "Residential Control Systems, Inc. (RCS)"
@@ -586,15 +586,15 @@
     },
     "0x0015:0x0001:0x0001": {
         "description": "Mini Energy Dimmer",
         "label": "MH-P210",
         "manufacturer": "Lexel"
     },
     "0x0015:0x0002:0x0001": {
-        "description": "Mini Energy switch",
+        "description": "Mini Energy Switch",
         "label": "MH-S210",
         "manufacturer": "Lexel"
     },
     "0x0015:0x1007:0x0002": {
         "description": "Curtain Motor",
         "label": "JTB-1007-02",
         "manufacturer": "Lexel"
@@ -626,15 +626,15 @@
     },
     "0x0017:0x0001:0x0111": {
         "description": "Telguard",
         "label": "GDC1",
         "manufacturer": "HiTech Automation"
     },
     "0x0017:0x0006:0x0003": {
-        "description": "EbV floor heating regulator",
+        "description": "EbV Floor Heating Regulator",
         "label": "9600801000",
         "manufacturer": "HiTech Automation"
     },
     "0x0018:0x0001:0x0001": {
         "description": "LGUplus Gateway Dongle",
         "label": "GWG-01",
         "manufacturer": "Balboa Instruments"
@@ -666,15 +666,15 @@
     },
     "0x001a:0x4441:0x0000": {
         "description": "Dimmer Accessory Switch",
         "label": "RF9542-Z",
         "manufacturer": "Eaton"
     },
     "0x001a:0x4441:0x0502": {
-        "description": "Z-Wave Plus smart accessory dimmer",
+        "description": "Z-Wave Plus Smart Accessory Dimmer",
         "label": "RF9642",
         "manufacturer": "Eaton"
     },
     "0x001a:0x4441:0xaa00": {
         "description": "Dimmer Accessory Switch",
         "label": "RF9542-Z",
         "manufacturer": "Eaton"
@@ -716,15 +716,15 @@
     },
     "0x001a:0x4449:0xff00": {
         "description": "All Load Dimmer Light Switch",
         "label": "RF9540-N",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5244:0x0000": {
-        "description": "Duplex receptacle",
+        "description": "Duplex Receptacle",
         "label": "RFTR9505-T / RFTR9605",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5244:0x0505": {
         "description": "Eatons Z-Wave Plus Wireless Receptacle",
         "label": "RFTR9605-T",
         "manufacturer": "Eaton"
@@ -736,35 +736,35 @@
     },
     "0x001a:0x534c:0x0000": {
         "description": "15A Light Switch",
         "label": "RF9501",
         "manufacturer": "Eaton"
     },
     "0x001a:0x534c:0x0503": {
-        "description": "Z-Wave Plus wireless switch",
+        "description": "Z-Wave Plus Wireless Switch",
         "label": "RF9601",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5352:0x0000": {
         "description": "Accessory Switch",
         "label": "RF9517",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5352:0x0504": {
-        "description": "Z-Wave Plus smart accessory switch",
+        "description": "Z-Wave Plus Smart Accessory Switch",
         "label": "RF9617",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5354:0x0000": {
         "description": "Single-Pole Wireless Light Switch",
         "label": "RF9518",
         "manufacturer": "Eaton"
     },
     "0x001a:0x5354:0x0003": {
-        "description": "ASPIRE RF Appliance Control Plug-in Module",
+        "description": "ASPIRE RF Appliance Control Plug-In Module",
         "label": "RFAPM",
         "manufacturer": "Eaton"
     },
     "0x001a:0x574d:0x0000": {
         "description": "5-Scene Keypad",
         "label": "RFWC5",
         "manufacturer": "Eaton"
@@ -846,60 +846,65 @@
     },
     "0x001d:0x0301:0x0334": {
         "description": "Scene Capable Switch On/Off",
         "label": "VRS15",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0401:0x0206": {
-        "description": "Dimmer switch 600w incandescent",
+        "description": "Dimmer Switch 600W Incandescent",
         "label": "RZI06-1L",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0401:0x0209": {
         "description": "Incandescent Scene Capable Dimmer",
         "label": "VRI06",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0401:0x0334": {
         "description": "Incandescent Scene Capable Dimmer",
         "label": "VRI06",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0501:0x0206": {
-        "description": "Dimmer switch 1000w incandescent",
+        "description": "Dimmer Switch 1000 W Incandescent",
         "label": "RZI10-1L",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0501:0x0209": {
         "description": "Scene Capable Push On/Off Dimmer",
         "label": "VRI10",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0501:0x0334": {
         "description": "Scene Capable Push On/Off Dimmer",
         "label": "VRI10",
         "manufacturer": "Leviton"
     },
+    "0x001d:0x0601:0x0206": {
+        "description": "Dimmer Switch 1000 W Magnetic Low-Voltage",
+        "label": "RZM10-1L",
+        "manufacturer": "Leviton"
+    },
     "0x001d:0x0602:0x0334": {
         "description": "Scene Capable Push On/Off Dimmer",
         "label": "VRMX1",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0701:0x0206": {
-        "description": "4 zone controller",
+        "description": "4 Zone Controller",
         "label": "VRCZ4",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0702:0x0261": {
-        "description": "4 zone controller",
+        "description": "4 Zone Controller",
         "label": "VRCZ4",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0801:0x0206": {
-        "description": "4 zone controller",
+        "description": "4 Zone Controller",
         "label": "VRCZ4",
         "manufacturer": "Leviton"
     },
     "0x001d:0x0802:0x0209": {
         "description": "4-Scene Controller",
         "label": "VRCS4",
         "manufacturer": "Leviton"
@@ -961,55 +966,55 @@
     },
     "0x001d:0x1102:0x0243": {
         "description": "Vizia RF + 2-Button Scene Controller with Switches",
         "label": "VRCS2",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1202:0x0243": {
-        "description": "4-Zone Controller with local load control",
+        "description": "4-Zone Controller with Local Load Control",
         "label": "VRCZ4-MR",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1302:0x0243": {
-        "description": "4-Scene controller with load control",
+        "description": "4-Scene Controller with Load Control",
         "label": "VRCS4-M0",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1602:0x0209": {
         "description": "Receptacle",
         "label": "VRR15",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1603:0x0334": {
         "description": "Receptacle",
         "label": "VRR15",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1705:0x0334": {
-        "description": "Scene Capable Plug-in Dimmer",
+        "description": "Scene Capable Plug-In Dimmer",
         "label": "VRPD3",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1706:0x0334": {
-        "description": "Scene Capable Plug-in Dimmer",
+        "description": "Scene Capable Plug-In Dimmer",
         "label": "VRPD3",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1805:0x0334": {
-        "description": "Vizia RF + Scene Capable Plug-in Module",
+        "description": "Vizia RF + Scene Capable Plug-In Module",
         "label": "VRPA1",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1902:0x0334": {
-        "description": "Plug-in Lamp Dimming Module",
+        "description": "Plug-In Lamp Dimming Module",
         "label": "DZPD3",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1a02:0x0334": {
-        "description": "Plug-in Appliance Module",
+        "description": "Plug-In Appliance Module",
         "label": "DZPA1",
         "manufacturer": "Leviton"
     },
     "0x001d:0x1b03:0x0334": {
         "description": "Scene Capable Dimmer",
         "label": "DZMX1",
         "manufacturer": "Leviton"
@@ -1041,25 +1046,25 @@
     },
     "0x001d:0x3401:0x0001": {
         "description": "Scene Capable Switch On/Off",
         "label": "DZ15S",
         "manufacturer": "Leviton"
     },
     "0x001d:0x3501:0x0001": {
-        "description": "Plug-in Lamp Dimming Module",
+        "description": "Plug-In Lamp Dimming Module",
         "label": "DZPD3",
         "manufacturer": "Leviton"
     },
     "0x001d:0x3601:0x0001": {
-        "description": "Plug-in Appliance Module",
+        "description": "Plug-In Appliance Module",
         "label": "DZPA1",
         "manufacturer": "Leviton"
     },
     "0x001d:0x5893:0x0820": {
-        "description": "Scene Capable Plug-in Dimmer",
+        "description": "Scene Capable Plug-In Dimmer",
         "label": "VRPD3",
         "manufacturer": "Leviton"
     },
     "0x001e:0x0002:0x0001": {
         "description": "Wireless 3-in-1 Sensor",
         "label": "EZMotion Express",
         "manufacturer": "Express Controls"
@@ -1086,50 +1091,50 @@
     },
     "0x0020:0x8007:0x1391": {
         "description": "Advanced Remote Wireless Lighting Control",
         "label": "45601",
         "manufacturer": "Universal Electronics Inc."
     },
     "0x0020:0x8007:0x1398": {
-        "description": "Monster Revolution 200 remote",
+        "description": "Monster Revolution 200 Remote",
         "label": "8700BJ0-R",
         "manufacturer": "Universal Electronics Inc."
     },
     "0x0021:0x0101:0x0101": {
         "description": "Aoya Switch",
         "label": "SWITCH",
         "manufacturer": "Zykronix"
     },
     "0x002c:0x0002:0x0007": {
         "description": "FlexNET Dongle",
         "label": "Z-FLEXNET DONGL",
         "manufacturer": "Flex Automation"
     },
     "0x0030:0x0001:0x0001": {
-        "description": "Cytech UCM/ZWave",
+        "description": "Cytech UCM/Z-Wave",
         "label": "UCM/ZWAV",
         "manufacturer": "Cytech Technology Pre Ltd."
     },
     "0x0033:0x4647:0x0001": {
         "description": "US 115V",
         "label": "FG IMS",
         "manufacturer": "Electronic Solutions"
     },
     "0x0033:0x5250:0x3031": {
         "description": "AC Motor Controller - Window Coverings",
         "label": "ABMHZ",
         "manufacturer": "Electronic Solutions"
     },
     "0x0033:0x5250:0x3032": {
-        "description": "DC Motor Controller - Window coverings",
+        "description": "DC Motor Controller - Window Coverings",
         "label": "DBMZ",
         "manufacturer": "Electronic Solutions"
     },
     "0x0033:0x545a:0x0001": {
-        "description": "EU - Handheld remote control",
+        "description": "EU - Handheld Remote Control",
         "label": "TZ 3300",
         "manufacturer": "Electronic Solutions"
     },
     "0x0039:0x0001:0x0001": {
         "description": "Tuxedo Touch Keypad and Z-Wave Controller",
         "label": "TUXEDO TOUCH",
         "manufacturer": "Honeywell"
@@ -1226,40 +1231,40 @@
     },
     "0x0039:0x4952:0x3137": {
         "description": "In-Wall Toggle Switch, QFSW, 500S",
         "label": "39354 / 39461 / ZW4009",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x4f50:0x3032": {
-        "description": "Plug-in Outdoor Switch, 500S",
+        "description": "Plug-In Outdoor Switch, 500S",
         "label": "39346 / 39453 / ZW4201",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x4f50:0x3034": {
-        "description": "Plug-in Outdoor Switch V2, 500S",
+        "description": "Plug-In Outdoor Switch V2, 500S",
         "label": "39363 / 39470 / ZW4203",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x5044:0x3033": {
-        "description": "Plug-in 2-Outlet Dimmer, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, Simultaneous, 500S",
         "label": "39339 / 39346 / ZW3107",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x5044:0x3038": {
-        "description": "Plug-in 1-Outlet Dimmer, 500S",
+        "description": "Plug-In 1-Outlet Dimmer, 500S",
         "label": "39336 / 39443 / ZW3104",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x5052:0x3033": {
-        "description": "Plug-in 2-Outlet Switch, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Switch, Simultaneous, 500S",
         "label": "39342 / 39449 / ZW4106",
         "manufacturer": "Honeywell"
     },
     "0x0039:0x5052:0x3038": {
-        "description": "Plug-in 1-Outlet Switch, 500S",
+        "description": "Plug-In 1-Outlet Switch, 500S",
         "label": "39337 / 39444 / ZW4103",
         "manufacturer": "Honeywell"
     },
     "0x003b:0x0001:0x0468": {
         "description": "Schlage Connect Smart Deadbolt",
         "label": "BE468ZP",
         "manufacturer": "Allegion"
@@ -1516,15 +1521,15 @@
     },
     "0x0047:0x1e54:0x4841": {
         "description": "Somfy TaHomA Z-Wave Controller",
         "label": "TAHOM",
         "manufacturer": "Somfy"
     },
     "0x0047:0x2018:0x1805": {
-        "description": "Blind-curtain motor controller",
+        "description": "Blind-Curtain Motor Controller",
         "label": "SY-IOT101",
         "manufacturer": "Somfy"
     },
     "0x0047:0x3001:0x0b01": {
         "description": "Z-WAVE2RTS Interface",
         "label": "Z2RTSEU-5",
         "manufacturer": "Somfy"
@@ -1621,15 +1626,15 @@
     },
     "0x0047:0x5a52:0x5410": {
         "description": "Z-Wave to RTS Interface Virtual Node",
         "label": "ZRTSI-VNODE",
         "manufacturer": "Somfy"
     },
     "0x004f:0x0000:0x0000": {
-        "description": "Touch Panel- 4 Dimmers plus 4 ON-OFF- 5 Scenes",
+        "description": "Touch Panel- 4 Dimmers Plus 4 ON-OFF- 5 Scenes",
         "label": "FXA-0404",
         "manufacturer": "Flex Automation"
     },
     "0x004f:0x0001:0x0001": {
         "description": "Micro Dimmer",
         "label": "FX-D211",
         "manufacturer": "Flex Automation"
@@ -1641,15 +1646,15 @@
     },
     "0x004f:0x0002:0x0001": {
         "description": "Micro Relay",
         "label": "FX-R211",
         "manufacturer": "Flex Automation"
     },
     "0x004f:0x0003:0x0008": {
-        "description": "Smart dimmer",
+        "description": "Smart Dimmer",
         "label": "FX-D67",
         "manufacturer": "Flex Automation"
     },
     "0x004f:0x0004:0x0002": {
         "description": "Meter Switch",
         "label": "FX-S69",
         "manufacturer": "Flex Automation"
@@ -1706,35 +1711,35 @@
     },
     "0x0059:0x0004:0x0001": {
         "description": "7 Day Room Thermostat",
         "label": "C17-ZW",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x0005:0x0001": {
-        "description": "Z-Wave home energy meter",
+        "description": "Z-Wave Home Energy Meter",
         "label": "S123XXXR",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x0005:0x0005": {
         "description": "Generation Meter Series P",
         "label": "P123XXXR",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x000d:0x0001": {
         "description": "Secure Temperature Sensor",
         "label": "SES301",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x000d:0x0002": {
-        "description": "Temperature sensor",
+        "description": "Temperature Sensor",
         "label": "SES 302",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x000d:0x0003": {
-        "description": "Temperature and humidity sensor",
+        "description": "Temperature and Humidity Sensor",
         "label": "SES 303",
         "manufacturer": "Secure Meters (UK) Ltd."
     },
     "0x0059:0x000e:0x0001": {
         "description": "SSP",
         "label": "SSP 301",
         "manufacturer": "Secure Meters (UK) Ltd."
@@ -1886,25 +1891,25 @@
     },
     "0x0060:0x0004:0x0006": {
         "description": "Mini Plug Switch with Metering (Gen5)",
         "label": "AN181",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0004:0x0007": {
-        "description": "Switch without metering",
+        "description": "Switch without Metering",
         "label": "AN180",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0004:0x0008": {
         "description": "In-Wall Switch Module",
         "label": "HAN02",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0004:0x000b": {
-        "description": "Mini plug with metering",
+        "description": "Mini Plug with Metering",
         "label": "AN184",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0004:0x000c": {
         "description": "ON/OFF PLUG",
         "label": "AN186",
         "manufacturer": "Everspring"
@@ -1966,15 +1971,15 @@
     },
     "0x0060:0x000d:0x0001": {
         "description": "Smoke Sensor",
         "label": "SF812",
         "manufacturer": "Everspring"
     },
     "0x0060:0x000e:0x0001": {
-        "description": "Z-Wave Gateway w/ Casiva Server Solution",
+        "description": "Z-Wave Gateway W/ Casiva Server Solution",
         "label": "SC102",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0010:0x0001": {
         "description": "In-Wall Remote Insert",
         "label": "HAC01",
         "manufacturer": "Everspring"
@@ -1995,14 +2000,19 @@
         "manufacturer": "Everspring"
     },
     "0x0060:0x0015:0x0001": {
         "description": "Thermostatic Radiator Valve",
         "label": "AC301",
         "manufacturer": "Everspring"
     },
+    "0x0060:0x0034:0x0001": {
+        "description": "UK Socket Plug",
+        "label": "VES-ZW-SOC-28",
+        "manufacturer": "Vesternet"
+    },
     "0x0060:0x0101:0x0001": {
         "description": "Motion Detector",
         "label": "HSP02 / SP103",
         "manufacturer": "Everspring"
     },
     "0x0060:0x0104:0x0001": {
         "description": "Everspring Lamp Holder / Lamp Module",
@@ -2016,30 +2026,30 @@
     },
     "0x0060:0x0400:0x0001": {
         "description": "Everspring Lamp Holder / Lamp Module",
         "label": "AN142/ AN145 / AN148 / AN157",
         "manufacturer": "Everspring"
     },
     "0x0063:0x0004:0x3031": {
-        "description": "Plug-in Outdoor Switch, 300S",
+        "description": "Plug-In Outdoor Switch, 300S",
         "label": "12720 / ZW4201",
         "manufacturer": "GE"
     },
     "0x0063:0x0507:0x0403": {
         "description": "In-Wall Fan Speed Control, 300S",
         "label": "10974 / ZW4002",
         "manufacturer": "GE"
     },
     "0x0063:0x4450:0x3030": {
-        "description": "Plug-in 2-Outlet Dimmer, 1 Controlled, 300S",
+        "description": "Plug-In 2-Outlet Dimmer, 1 Controlled, 300S",
         "label": "45602 / ZW3101",
         "manufacturer": "GE"
     },
     "0x0063:0x4450:0x3031": {
-        "description": "Plug-in 1-Outlet Dimmer With Energy, 300S",
+        "description": "Plug-In 1-Outlet Dimmer with Energy, 300S",
         "label": "45652WB / ZW3102",
         "manufacturer": "Jasco"
     },
     "0x0063:0x4457:0x0003": {
         "description": "In-Wall Paddle Dimmer, 300S",
         "label": "45607 / ZW3002",
         "manufacturer": "GE"
@@ -2380,14 +2390,19 @@
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x4952:0x3235": {
         "description": "In-Wall Outlet, TR, 500S",
         "label": "55257 / ZW1002",
         "manufacturer": "Jasco"
     },
+    "0x0063:0x4952:0x3236": {
+        "description": "In-Wall Outlet, TR, Lt Almd, 500S",
+        "label": "14297 / ZW1002",
+        "manufacturer": "Enbrighten"
+    },
     "0x0063:0x4952:0x3237": {
         "description": "In-Wall Paddle Switch, QFSW, 500S",
         "label": "39348 / 54890 / 54891 / ZW4008",
         "manufacturer": "UltraPro"
     },
     "0x0063:0x4952:0x3238": {
         "description": "In-Wall Toggle Switch, QFSW, 500S",
@@ -2416,20 +2431,20 @@
     },
     "0x0063:0x4952:0x3339": {
         "description": "In-Wall Outlet, TR, 700S",
         "label": "58449 / ZWA1003",
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x4953:0x3031": {
-        "description": "Hinge Pin Door Sensor, 500S",
+        "description": "Hinge PIN Door Sensor, 500S",
         "label": "32562 / ZW6301",
         "manufacturer": "Jasco"
     },
     "0x0063:0x4953:0x3032": {
-        "description": "Hinge Pin Door Sensor, 500S",
+        "description": "Hinge PIN Door Sensor, 500S",
         "label": "32563 / ZW6301",
         "manufacturer": "GE"
     },
     "0x0063:0x4953:0x3033": {
         "description": "Portable Motion+Temp+Light Sensor, 500S",
         "label": "35211 / ZW6302B",
         "manufacturer": "GE"
@@ -2506,195 +2521,195 @@
     },
     "0x0063:0x4f44:0x3032": {
         "description": "Direct Wire 40A Outdoor Switch, 500S",
         "label": "14285 / ZW4007",
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x4f50:0x3031": {
-        "description": "Plug-in Outdoor Switch, 300S",
+        "description": "Plug-In Outdoor Switch, 300S",
         "label": "12720 / ZW4201",
         "manufacturer": "GE"
     },
     "0x0063:0x4f50:0x3032": {
-        "description": "Plug-in Outdoor Switch, 500S",
+        "description": "Plug-In Outdoor Switch, 500S",
         "label": "14284 / ZW4201",
         "manufacturer": "GE"
     },
     "0x0063:0x4f50:0x3033": {
-        "description": "Plug-in Outdoor Switch, 500S",
+        "description": "Plug-In Outdoor Switch, 500S",
         "label": "14311 / ZW4201",
         "manufacturer": "Jasco"
     },
     "0x0063:0x4f50:0x3034": {
-        "description": "Plug-in Outdoor Switch V2, 500S",
+        "description": "Plug-In Outdoor Switch V2, 500S",
         "label": "14298 / ZW4203",
         "manufacturer": "GE/Enbrighten"
     },
     "0x0063:0x4f50:0x3035": {
-        "description": "Plug-in Outdoor Switch V2, 500S",
+        "description": "Plug-In Outdoor Switch V2, 500S",
         "label": "14325 / ZW4203",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5042:0x4004": {
         "description": "Direct Wire 40A Outdoor Switch, 500S",
         "label": "14285 / ZW4007",
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x5044:0x3031": {
-        "description": "Plug-in 2-Outlet Dimmer, 1 Controlled, 300S",
+        "description": "Plug-In 2-Outlet Dimmer, 1 Controlled, 300S",
         "label": "12718 / ZW3103",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3032": {
-        "description": "Plug-in 1-Outlet Dimmer With Energy, 300S",
+        "description": "Plug-In 1-Outlet Dimmer with Energy, 300S",
         "label": "45652 / ZW3102",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3033": {
-        "description": "Plug-in 2-Outlet Dimmer, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, Simultaneous, 500S",
         "label": "14280 / ZW3107",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3035": {
-        "description": "Plug-in 2-Outlet Dimmer, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, Simultaneous, 500S",
         "label": "14307 / ZW3107",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5044:0x3037": {
-        "description": "Plug-in 1-Outlet Dimmer, 500S",
+        "description": "Plug-In 1-Outlet Dimmer, 500S",
         "label": "28166 / ZW3104",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5044:0x3038": {
-        "description": "Plug-in 1-Outlet Dimmer, 500S",
+        "description": "Plug-In 1-Outlet Dimmer, 500S",
         "label": "28167 / ZW3104",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3039": {
-        "description": "Plug-in 2-Outlet Dimmer, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, 1 Controlled, 500S",
         "label": "28170 / ZW3105",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5044:0x3130": {
-        "description": "Plug-in 2-Outlet Dimmer, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, 1 Controlled, 500S",
         "label": "28171 / ZW3105",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3131": {
-        "description": "Plug-in 2-Outlet Dimmer with USB, 500S",
+        "description": "Plug-In 2-Outlet Dimmer with USB, 500S",
         "label": "28174 / ZW3106",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5044:0x3132": {
-        "description": "Plug-in 2-Outlet Dimmer with USB, 500S",
+        "description": "Plug-In 2-Outlet Dimmer with USB, 500S",
         "label": "28175 / ZW3106",
         "manufacturer": "GE"
     },
     "0x0063:0x5044:0x3133": {
-        "description": "Plug-in 2-Outlet Dimmer, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, Simultaneous, 500S",
         "label": "55251 / ZW3107",
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x5044:0x3134": {
-        "description": "Plug-in 2-Outlet Dimmer, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, 1 Controlled, 500S",
         "label": "55252 / ZW3105",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5052:0x3031": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 300S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 300S",
         "label": "12719 / ZW4101",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3032": {
-        "description": "Plug-in 1-Outlet Switch With Energy, 300S",
+        "description": "Plug-In 1-Outlet Switch with Energy, 300S",
         "label": "45653 / ZW4102",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3033": {
-        "description": "Plug-in 2-Outlet Switch, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Switch, Simultaneous, 500S",
         "label": "14282 / ZW4106",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3035": {
-        "description": "Plug-in 2-Outlet Switch, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Switch, Simultaneous, 500S",
         "label": "14309 / ZW4106",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5052:0x3037": {
-        "description": "Plug-in 1-Outlet Switch, 500S",
+        "description": "Plug-In 1-Outlet Switch, 500S",
         "label": "28168 / ZW4103",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5052:0x3038": {
-        "description": "Plug-in 1-Outlet Switch, 500S",
+        "description": "Plug-In 1-Outlet Switch, 500S",
         "label": "28169 / ZW4103",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3039": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 500S",
         "label": "28172 / ZW4104",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5052:0x3130": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 500S",
         "label": "28713 / ZW4104",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3131": {
-        "description": "Plug-in 2-Outlet Switch with USB, 500S",
+        "description": "Plug-In 2-Outlet Switch with USB, 500S",
         "label": "28176 / ZW4105",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5052:0x3132": {
-        "description": "Plug-in 2-Outlet Switch with USB, 500S",
+        "description": "Plug-In 2-Outlet Switch with USB, 500S",
         "label": "28177 / ZW4105",
         "manufacturer": "GE"
     },
     "0x0063:0x5052:0x3133": {
-        "description": "Plug-in 2-Outlet Switch, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Switch, Simultaneous, 500S",
         "label": "55249 / ZW4106",
         "manufacturer": "Enbrighten"
     },
     "0x0063:0x5052:0x3134": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 500S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 500S",
         "label": "55250 / ZW4104",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5250:0x3030": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 300S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 300S",
         "label": "45603 / ZW4101",
         "manufacturer": "GE"
     },
     "0x0063:0x5250:0x3031": {
-        "description": "Plug-in 1-Outlet Switch With Energy, 300S",
+        "description": "Plug-In 1-Outlet Switch with Energy, 300S",
         "label": "45653WB / ZW4102",
         "manufacturer": "Jasco"
     },
     "0x0063:0x5250:0x3130": {
-        "description": "Plug-in Outdoor Switch, 300S",
+        "description": "Plug-In Outdoor Switch, 300S",
         "label": "45604 / ZW4201",
         "manufacturer": "GE"
     },
     "0x0063:0x5252:0x3530": {
         "description": "In-Wall Outlet, 300S",
         "label": "45605 / ZW1001",
         "manufacturer": "GE"
     },
     "0x0063:0x5257:0x3533": {
         "description": "In-Wall Paddle Switch, 300S",
         "label": "45609 / ZW4001",
         "manufacturer": "GE"
     },
     "0x0063:0x6363:0x3030": {
-        "description": "Plug-in 2-Outlet Switch, 1 Controlled, 300S",
+        "description": "Plug-In 2-Outlet Switch, 1 Controlled, 300S",
         "label": "45657 / ZW4101",
         "manufacturer": "AT&T"
     },
     "0x0063:0x6363:0x3130": {
-        "description": "Plug-in Outdoor Switch, 300S",
+        "description": "Plug-In Outdoor Switch, 300S",
         "label": "45658 / ZW4201",
         "manufacturer": "AT&T"
     },
     "0x0063:0x6363:0x3533": {
         "description": "In-Wall Paddle Switch, 300S",
         "label": "45655 / ZW4001",
         "manufacturer": "AT&T"
@@ -2711,70 +2726,70 @@
     },
     "0x0064:0x0001:0x0000": {
         "description": "One Paddle Wall Dimmer Insert",
         "label": "05433",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x1000:0x0003": {
-        "description": "Insert blind control",
+        "description": "Insert Blind Control",
         "label": "06436",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x1000:0x0009": {
         "description": "Switch",
         "label": "ZME_05431",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x1001:0x0000": {
         "description": "Plug Dimmer",
         "label": "064394",
         "manufacturer": "Schuko"
     },
     "0x0064:0x2001:0x0000": {
-        "description": "Duewi ZW BJ ES 1000 / Reitz 05431 / ZWave.me 05457 Single button wall switch",
+        "description": "Duewi ZW BJ ES 1000 / Reitz 05431 / Z-Wave.Me 05457 Single Button Wall Switch",
         "label": "ZW-ES-1000 / Reitz 05431",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x3001:0x0000": {
         "description": "Schuko Plug Switch",
         "label": "Duewi ZW-ZS-3500",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x3002:0x0000": {
         "description": "Indoor/Outdoor Wall Plug Switch",
         "label": "Duwi Z-Wave Plugin Switch",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x4001:0x0000": {
-        "description": "Duwi ZW ESJ 300 Blind Control",
+        "description": "Duwi Blind Control",
         "label": "ZW ESJ 300",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x5001:0x0000": {
         "description": "D\u00fcwi Remote Control",
         "label": "064459",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x5002:0x0000": {
-        "description": "Battery powered One paddle wall controller",
+        "description": "Battery Powered One Paddle Wall Controller",
         "label": "ZWWS",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0064:0x5003:0x0000": {
         "description": "D\u00fcwi Repeater",
         "label": "DUW_RPT",
         "manufacturer": "Reitz-Group.de"
     },
     "0x0068:0x0000:0x000d": {
         "description": "Door/Window Sensor with Magnet",
         "label": "78008",
         "manufacturer": "Good Way Technology Co., Ltd."
     },
     "0x0068:0x0000:0x0010": {
-        "description": "In wall Power Monitor Switch",
+        "description": "In Wall Power Monitor Switch",
         "label": "TD1311",
         "manufacturer": "Good Way Technology Co., Ltd."
     },
     "0x0068:0x0002:0x0001": {
         "description": "FG3200 Z-Wave\u00ae Home Gateway",
         "label": "GATEWAY / FG3200",
         "manufacturer": "Good Way Technology Co., Ltd."
@@ -2801,15 +2816,15 @@
     },
     "0x0068:0x0003:0x000b": {
         "description": "RGBW Dimmer Module",
         "label": "36511",
         "manufacturer": "Good Way Technology Co., Ltd."
     },
     "0x0068:0x0003:0x0015": {
-        "description": "In-wall switch",
+        "description": "In-Wall Switch",
         "label": "TD13010",
         "manufacturer": "Good Way Technology Co., Ltd."
     },
     "0x0068:0x0003:0x0016": {
         "description": "Panic Button",
         "label": "TR1B120Z1",
         "manufacturer": "Good Way Technology Co., Ltd."
@@ -2841,15 +2856,15 @@
     },
     "0x0071:0x0004:0x035d": {
         "description": "C Humidity Sensor",
         "label": "ES861",
         "manufacturer": "LS Control"
     },
     "0x0071:0x0005:0x035d": {
-        "description": "Setpoint sensor",
+        "description": "Setpoint Sensor",
         "label": "ES861C",
         "manufacturer": "LS Control"
     },
     "0x0077:0x0001:0x0001": {
         "description": "RAone SmartDimmer",
         "label": "SmartDimmer",
         "manufacturer": "INNOVUS"
@@ -2871,15 +2886,15 @@
     },
     "0x0077:0x0011:0x0001": {
         "description": "RAone SmartDimmer",
         "label": "SmartDimmer",
         "manufacturer": "INNOVUS"
     },
     "0x007a:0x0001:0x0002": {
-        "description": "Radio Push-button CONNECT, 1 button",
+        "description": "Radio Push-Button CONNECT, 1 Button",
         "label": "5071xx",
         "manufacturer": "Merten"
     },
     "0x007a:0x0001:0x0004": {
         "description": "Battery Powered Wall Controller",
         "label": "506219",
         "manufacturer": "Merten"
@@ -2896,30 +2911,30 @@
     },
     "0x007a:0x0003:0x0004": {
         "description": "Transmitter Flush-Mounted 4-Gang Switch",
         "label": "506004",
         "manufacturer": "Merten"
     },
     "0x007a:0x4002:0x0001": {
-        "description": "5044xx - Radio sensor cover for in-wall switch",
+        "description": "5044xx - Radio Sensor Cover for In-Wall Switch",
         "label": "5044XX",
         "manufacturer": "Merten"
     },
     "0x007a:0x4003:0x0001": {
-        "description": "5046xx - Radio sensor cover for in wall dimmer",
+        "description": "5046xx - Radio Sensor Cover for in Wall Dimmer",
         "label": "5046XX",
         "manufacturer": "Merten"
     },
     "0x007a:0x4003:0x0002": {
         "description": "Wall Dimmer Module - Flush Mounted",
         "label": "507900",
         "manufacturer": "Merten"
     },
     "0x007a:0x4004:0x0001": {
-        "description": "Roller shutter push-button",
+        "description": "Roller Shutter Push-Button",
         "label": "50x5xx",
         "manufacturer": "Merten"
     },
     "0x007a:0x4005:0x0001": {
         "description": "Argus 220 Connect Movement Detector",
         "label": "509519",
         "manufacturer": "Merten"
@@ -2931,75 +2946,75 @@
     },
     "0x007a:0x8001:0x8001": {
         "description": "Switch Wall Insert 1 Gang",
         "label": "507001",
         "manufacturer": "Merten"
     },
     "0x007a:0x8001:0x8002": {
-        "description": "Flush-mounted switch",
+        "description": "Flush-Mounted Switch",
         "label": "507501 / 507502",
         "manufacturer": "Merten"
     },
     "0x007a:0x8001:0x8003": {
         "description": "Dual Pole Wall Switch",
         "label": "507601",
         "manufacturer": "Merten"
     },
     "0x007a:0x8001:0x8004": {
-        "description": "Flush-mounted switch",
+        "description": "Flush-Mounted Switch",
         "label": "507501 / 507502",
         "manufacturer": "Merten"
     },
     "0x007a:0x8003:0x0001": {
         "description": "Connect Roller Shutter",
         "label": "507801",
         "manufacturer": "Merten"
     },
     "0x007e:0x0101:0x0206": {
         "description": "Plugin Appliance Module",
         "label": "ML LAS1000",
         "manufacturer": "Monster Cable"
     },
     "0x007e:0x0200:0x014e": {
-        "description": "Scene Capable Plug-in Dimmer",
+        "description": "Scene Capable Plug-In Dimmer",
         "label": "ML LD300",
         "manufacturer": "Monster Cable"
     },
     "0x007e:0x0400:0x014e": {
-        "description": "Dimmer switch 600w incandescent",
+        "description": "Dimmer Switch 600W Incandescent",
         "label": "IWD600S",
         "manufacturer": "Monster Cable"
     },
     "0x007e:0x0401:0x0206": {
-        "description": "Dimmer switch 600w incandescent",
+        "description": "Dimmer Switch 600W Incandescent",
         "label": "IWD600S",
         "manufacturer": "Monster Cable"
     },
     "0x007f:0x0001:0x0001": {
         "description": "Harmony Home Hub Extender",
         "label": "N-R0009",
         "manufacturer": "Logitech"
     },
     "0x0080:0x0001:0x0003": {
         "description": "MaxTronic - Grating Unit",
         "label": "Grating Unit",
         "manufacturer": "MaxTronic"
     },
     "0x0080:0x0004:0x0001": {
-        "description": "CO2 sensor",
+        "description": "CO2 Sensor",
         "label": "CO2 sensor",
         "manufacturer": "DucoTronic"
     },
     "0x0081:0x0014:0x0001": {
-        "description": "C - Wall mounted ventilation unit",
+        "description": "C - Wall Mounted Ventilation Unit",
         "label": "AEROPA",
         "manufacturer": "SIEGENIA-AUBI KG"
     },
     "0x0081:0x00a0:0x0001": {
-        "description": "Air quality sensor for indoor use",
+        "description": "Air Quality Sensor for Indoor Use",
         "label": "SENSOAIR",
         "manufacturer": "SIEGENIA-AUBI KG"
     },
     "0x0084:0x0013:0x0210": {
         "description": "Wireless Water and Temperature Alarm",
         "label": "WWA-02",
         "manufacturer": "FortrezZ LLC"
@@ -3046,15 +3061,15 @@
     },
     "0x0084:0x00a3:0x020e": {
         "description": "FTS05P Flood and Temperature Sensor",
         "label": "FTS05P",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0213:0x020c": {
-        "description": "Wireless, Z-Wave Emergency Water Shut-off Valve",
+        "description": "Wireless, Z-Wave Emergency Water Shut-Off Valve",
         "label": "WV-01_1002",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0213:0x0214": {
         "description": "Wireless Z-Wave Water Valve",
         "label": "WV-01",
         "manufacturer": "FortrezZ LLC"
@@ -3116,50 +3131,50 @@
     },
     "0x0084:0x0343:0x0205": {
         "description": "Siren & Strobe Alarm",
         "label": "SSA3-P4",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0451:0x010e": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0451:0x0110": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0453:0x010e": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0453:0x010f": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0453:0x0110": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0453:0x0111": {
-        "description": "Digital or Analog Voltage input and/or Dry Contact Relay",
+        "description": "Digital or Analog Voltage Input And/or Dry Contact Relay",
         "label": "MIMOlite",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0463:0x0207": {
-        "description": "Dual Digital or Analog Voltage input and Dual Contact Relay",
+        "description": "Dual Digital or Analog Voltage Input and Dual Contact Relay",
         "label": "MIMO2+",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0463:0x0208": {
-        "description": "Dual Digital or Analog Voltage input and Dual Contact Relay",
+        "description": "Dual Digital or Analog Voltage Input and Dual Contact Relay",
         "label": "MIMO2+",
         "manufacturer": "FortrezZ LLC"
     },
     "0x0084:0x0473:0x0110": {
         "description": "Flow Meter",
         "label": "FMI",
         "manufacturer": "FortrezZ LLC"
@@ -3175,46 +3190,51 @@
         "manufacturer": "Fakro"
     },
     "0x0085:0x0001:0x0004": {
         "description": "Remote",
         "label": "ZRH12",
         "manufacturer": "Fakro"
     },
-    "0x0085:0x0002:0x0001": {
-        "description": "Chain Actuator",
-        "label": "ZWS12",
-        "manufacturer": "Fakro"
-    },
     "0x0085:0x0002:0x0002": {
         "description": "Roller Shutter Module",
         "label": "ARZ",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0002:0x0003": {
-        "description": "Chain actuator 230VAC",
+        "description": "Chain Actuator 230VAC",
         "label": "ZWS230",
         "manufacturer": "Fakro"
     },
+    "0x0085:0x0002:0x0010": {
+        "description": "Chain Actuator",
+        "label": "ZWS12",
+        "manufacturer": "Fakro"
+    },
     "0x0085:0x0002:0x0011": {
-        "description": "Chain actuator - window opener",
+        "description": "Chain Actuator - Window Opener",
         "label": "ZWS12",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0002:0x0014": {
         "description": "Solar Powered Skylight",
         "label": "FVS",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0002:0x0111": {
-        "description": "Chain actuator - window opener",
+        "description": "Chain Actuator - Window Opener",
+        "label": "ZWS12",
+        "manufacturer": "Fakro"
+    },
+    "0x0085:0x0002:0x0116": {
+        "description": "Chain Actuator - Window Opener",
         "label": "ZWS12",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0003:0x0001": {
-        "description": "Chain actuator 230VAC",
+        "description": "Chain Actuator 230VAC",
         "label": "ZWS230",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0003:0x0011": {
         "description": "Roller Shutter",
         "label": "ARZ Z-Wave",
         "manufacturer": "Fakro"
@@ -3231,15 +3251,15 @@
     },
     "0x0085:0x0003:0x0112": {
         "description": "Roller Shutter",
         "label": "ARZ Z-Wave Solar",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0004:0x0011": {
-        "description": "Roller blind module",
+        "description": "Roller Blind Module",
         "label": "ARF",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0004:0x0012": {
         "description": "Roller Blind",
         "label": "ARF Z-Wave Solar",
         "manufacturer": "Fakro"
@@ -3266,30 +3286,30 @@
     },
     "0x0085:0x0006:0x0002": {
         "description": "Awning Blind",
         "label": "VMZ Solar",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0006:0x0112": {
-        "description": "Awning Blind z-wave plus version",
+        "description": "Awning Blind Z-Wave Plus Version",
         "label": "VMZ Solar z-wave plus",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0007:0x0001": {
         "description": "Weather Module",
         "label": "ZWMP",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0011:0x0001": {
         "description": "Chain Actuator",
         "label": "ZWS12",
         "manufacturer": "Fakro"
     },
     "0x0085:0x0022:0x0001": {
-        "description": "Roller Shutter FLiRS module",
+        "description": "Roller Shutter FLiRS Module",
         "label": "ZWRS MODULE",
         "manufacturer": "Fakro"
     },
     "0x0086:0x0000:0x0004": {
         "description": "Goodway (Lamp Dimmer-USA) 2/5",
         "label": "TD1010Z2",
         "manufacturer": "AEON Labs"
@@ -3301,30 +3321,30 @@
     },
     "0x0086:0x0000:0x0006": {
         "description": "GoodWay Z-Wave Power Monitor",
         "label": "TD1030Z1",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0001:0x0003": {
-        "description": "Minimote 4 button remote control",
+        "description": "Minimote 4 Button Remote Control",
         "label": "DSA03XXX-ZW",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0001:0x0016": {
-        "description": "4 button keyfob",
+        "description": "4 Button Keyfob",
         "label": "DSA22",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0001:0x0026": {
         "description": "Panic Button Key Fob",
         "label": "DSA38-ZW",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0001:0x0058": {
-        "description": "4 button keyfob - Gen 5",
+        "description": "4 Button Keyfob - Gen 5",
         "label": "ZW088",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0001:0x005a": {
         "description": "Z\u2010Stick Gen5 USB Controller",
         "label": "ZW090",
         "manufacturer": "AEON Labs"
@@ -3336,15 +3356,15 @@
     },
     "0x0086:0x0002:0x0002": {
         "description": "Water Sensor",
         "label": "DSB45",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0002:0x0004": {
-        "description": "Door/Window sensor Gen2",
+        "description": "Door/Window Sensor Gen2",
         "label": "DSB29",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0002:0x0005": {
         "description": "4 in 1 MultiSensor",
         "label": "DSB05",
         "manufacturer": "AEON Labs"
@@ -3356,15 +3376,15 @@
     },
     "0x0086:0x0002:0x001c": {
         "description": "Home Energy Meter G2",
         "label": "DSB28",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0002:0x001d": {
-        "description": "Door/Window sensor Gen2",
+        "description": "Door/Window Sensor Gen2",
         "label": "DSB29",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0002:0x002d": {
         "description": "Water Sensor",
         "label": "DSB45",
         "manufacturer": "AEON Labs"
@@ -3551,15 +3571,15 @@
     },
     "0x0086:0x0003:0x0084": {
         "description": "Dual Nano Switch with Energy Metering",
         "label": "ZW132",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0003:0x008b": {
-        "description": "Nano Switch Gen5 (without meter)",
+        "description": "Nano Switch Gen5 (Without Meter)",
         "label": "ZW139",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0003:0x008c": {
         "description": "Dual Nano Switch",
         "label": "ZW140",
         "manufacturer": "AEON Labs"
@@ -3591,30 +3611,30 @@
     },
     "0x0086:0x0004:0x0075": {
         "description": "Range Extender 6",
         "label": "ZW117",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0006:0x0002": {
-        "description": "Minimote 4 button remote control",
+        "description": "Minimote 4 Button Remote Control",
         "label": "DSA03XXX-ZW",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0019:0x0004": {
         "description": "Range Extender",
         "label": "DSD37",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x001b:0x0048": {
         "description": "Smart Switch Gen5",
         "label": "ZW075",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0101:0x0058": {
-        "description": "4 button keyfob - Gen 5",
+        "description": "4 Button Keyfob - Gen 5",
         "label": "ZW088",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0101:0x005a": {
         "description": "Z\u2010Stick Gen5 USB Controller",
         "label": "ZW090",
         "manufacturer": "AEON Labs"
@@ -3716,15 +3736,15 @@
     },
     "0x0086:0x0103:0x0084": {
         "description": "Dual Nano Switch with Energy Metering",
         "label": "ZW132",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0103:0x008b": {
-        "description": "Nano Switch Gen5 (without meter)",
+        "description": "Nano Switch Gen5 (Without Meter)",
         "label": "ZW139",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0103:0x008c": {
         "description": "Dual Nano Switch",
         "label": "ZW140",
         "manufacturer": "AEON Labs"
@@ -3756,15 +3776,15 @@
     },
     "0x0086:0x01f3:0x006f": {
         "description": "Nano Dimmer",
         "label": "ZW111",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0201:0x0058": {
-        "description": "4 button keyfob - Gen 5",
+        "description": "4 Button Keyfob - Gen 5",
         "label": "ZW088",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0201:0x005a": {
         "description": "Z\u2010Stick Gen5 USB Controller",
         "label": "ZW090",
         "manufacturer": "AEON Labs"
@@ -3866,15 +3886,15 @@
     },
     "0x0086:0x0203:0x0084": {
         "description": "Dual Nano Switch with Energy Metering",
         "label": "ZW132",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0203:0x008b": {
-        "description": "Nano Switch Gen5 (without meter)",
+        "description": "Nano Switch Gen5 (Without Meter)",
         "label": "ZW139",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0203:0x008c": {
         "description": "Dual Nano Switch",
         "label": "ZW140",
         "manufacturer": "AEON Labs"
@@ -3941,15 +3961,15 @@
     },
     "0x0086:0x0303:0x0079": {
         "description": "Aeotec LED Strip",
         "label": "ZW121",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0303:0x008b": {
-        "description": "Nano Switch Gen5 (without meter)",
+        "description": "Nano Switch Gen5 (Without Meter)",
         "label": "ZW139",
         "manufacturer": "AEON Labs"
     },
     "0x0086:0x0303:0x008c": {
         "description": "Dual Nano Switch",
         "label": "ZW140",
         "manufacturer": "AEON Labs"
@@ -4051,15 +4071,15 @@
     },
     "0x0086:0x6015:0x020d": {
         "description": "Door/Window Sensor 6",
         "label": "ZW112",
         "manufacturer": "AEON Labs"
     },
     "0x0089:0x0001:0x0101": {
-        "description": "Single relay switch",
+        "description": "Single Relay Switch",
         "label": "ZSL301EU",
         "manufacturer": "Team Precision PCL"
     },
     "0x0089:0x0002:0x0101": {
         "description": "Easy Light Dimmer Link",
         "label": "ZDL301",
         "manufacturer": "Team Precision PCL"
@@ -4081,20 +4101,20 @@
     },
     "0x008a:0x0002:0x0100": {
         "description": "Remote Display",
         "label": "BENEXT MYDISPLAY",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0003:0x0100": {
-        "description": "Movement sensor with temperature and light sensor",
+        "description": "Movement Sensor with Temperature and Light Sensor",
         "label": "Molite",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0003:0x0101": {
-        "description": "Movement sensor with temperature and light sensor",
+        "description": "Movement Sensor with Temperature and Light Sensor",
         "label": "Molite",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0004:0x0100": {
         "description": "Door Sensor",
         "label": "DOOR SENSOR",
         "manufacturer": "BeNext"
@@ -4106,23 +4126,28 @@
     },
     "0x008a:0x0005:0x0100": {
         "description": "Alarm Sound",
         "label": "BENEXT / ALARM SOUN",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0005:0x0101": {
-        "description": "Alarm sound",
+        "description": "Alarm Sound",
         "label": "Alarm Sound",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0006:0x0100": {
         "description": "Energy Switch +",
         "label": "ENERGY SWITCH",
         "manufacturer": "BeNext"
     },
+    "0x008a:0x0006:0x0101": {
+        "description": "Energy Switch +",
+        "label": "ENERGY SWITCH",
+        "manufacturer": "BeNext"
+    },
     "0x008a:0x0006:0x0200": {
         "description": "Energy Switch +",
         "label": "ENERGY SWITCH",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0007:0x0100": {
         "description": "Tag Reader",
@@ -4146,35 +4171,35 @@
     },
     "0x008a:0x0008:0x0101": {
         "description": "Power Switch EU",
         "label": "PowerSwitch",
         "manufacturer": "BeNext"
     },
     "0x008a:0x000d:0x0100": {
-        "description": "Built-in Dimmer",
+        "description": "Built-In Dimmer",
         "label": "builtInDimmer",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0018:0x0100": {
-        "description": "Plug-in Dimmer",
+        "description": "Plug-In Dimmer",
         "label": "plugInDimmer",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0020:0x0001": {
         "description": "Energy Switch +",
         "label": "ENERGY SWITCH",
         "manufacturer": "BeNext"
     },
     "0x008a:0x0021:0x0102": {
-        "description": "Thermostat for controlling the opentherm protocol",
+        "description": "Thermostat for Controlling the Opentherm Protocol",
         "label": "Heating Control",
         "manufacturer": "BeNext"
     },
     "0x008a:0x002f:0x0100": {
-        "description": "P1-dongle",
+        "description": "P1-Dongle",
         "label": "P1-dongle",
         "manufacturer": "BeNext"
     },
     "0x008b:0x0003:0x006f": {
         "description": "Nano Dimmer",
         "label": "ZW111",
         "manufacturer": "Trane Corporation"
@@ -4216,15 +4241,15 @@
     },
     "0x008b:0x4d53:0x4331": {
         "description": "LE130",
         "label": "LE130",
         "manufacturer": "Schlage"
     },
     "0x008b:0x4d53:0x4332": {
-        "description": "Trane Z WAVE Mini Split Remote control - ANZ",
+        "description": "Trane Z WAVE Mini Split Remote Control - ANZ",
         "label": "TRNZWR2",
         "manufacturer": "Trane Corporation"
     },
     "0x008b:0x5438:0x3234": {
         "description": "Ingersoll Rand XL824 Controller",
         "label": "XL824",
         "manufacturer": "Trane Corporation"
@@ -4395,14 +4420,19 @@
         "manufacturer": "Kwikset"
     },
     "0x0090:0x0003:0x0000": {
         "description": "Smart Code with Home Connect Technology",
         "label": "910",
         "manufacturer": "Kwikset"
     },
+    "0x0090:0x0003:0x0042": {
+        "description": "Convert Smart Lock",
+        "label": "914C",
+        "manufacturer": "Kwikset"
+    },
     "0x0090:0x0003:0x0236": {
         "description": "Door Lock",
         "label": "912",
         "manufacturer": "Kwikset"
     },
     "0x0090:0x0003:0x0238": {
         "description": "Smart Code with Home Connect Technology",
@@ -4496,55 +4526,55 @@
     },
     "0x0090:0x0811:0x23a8": {
         "description": "Home Connect 620 Connected Smart Lock",
         "label": "HC620",
         "manufacturer": "Kwikset"
     },
     "0x0091:0x0001:0x0091": {
-        "description": "Electricity meters",
+        "description": "Electricity Meters",
         "label": "electricity_meter",
         "manufacturer": "Kamstrup A/S"
     },
     "0x0092:0x0102:0x0002": {
         "description": "Martin Renz GmbH - UPz- Empf\u0084nger",
         "label": "UPz- Empfnger",
         "manufacturer": "Martin Renz GmbH"
     },
     "0x0094:0x0001:0x0001": {
-        "description": "Alarm.com Z-Wave Snap Device D v1",
+        "description": "Z-Wave Snap Device D v1",
         "label": "ADC-ZW-EV",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x0001:0x0101": {
-        "description": "Alarm.com Interlogix Simon XT/i Radio Module",
+        "description": "Interlogix Simon XT/i Radio Module",
         "label": "ADC-200H-EV",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x0001:0x0102": {
-        "description": "Alarm.com Hub",
+        "description": "Hub",
         "label": "ADC-NK-100T",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x0004:0x0104": {
         "description": "Wireless Alarm System with Integrated Home Automation",
         "label": "WS900-29",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x000a:0x010a": {
-        "description": "Alarm.com Module for DSC Panels",
+        "description": "Module for DSC Panels",
         "label": "ADC-620T",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x000b:0x010b": {
         "description": "ADTZWM - Wi-Fi\u00ae and Z-Wave\u00ae Module for Command",
         "label": "ADTZWM FOR COMMAN",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x000e:0x010e": {
-        "description": "Alarm.com Rev4.7 Radio Module",
+        "description": "Rev4.7 Radio Module",
         "label": "ADC-470L",
         "manufacturer": "Alarm.com"
     },
     "0x0094:0x0011:0x0111": {
         "description": "Smart Gateway",
         "label": "ADC-SG130Z",
         "manufacturer": "Alarm.com"
@@ -4571,30 +4601,30 @@
     },
     "0x0095:0x0001:0x0001": {
         "description": "QEES Ring EU",
         "label": "QEES MYKEY",
         "manufacturer": "Qees"
     },
     "0x0095:0x0002:0x0001": {
-        "description": "Wall mountable mini 4 button remote",
+        "description": "Wall Mountable Mini 4 Button Remote",
         "label": "Wall",
         "manufacturer": "Qees"
     },
     "0x0095:0x0003:0x0000": {
         "description": "QEES Power EU",
         "label": "QEES RETO",
         "manufacturer": "Qees"
     },
     "0x0095:0x3101:0x0001": {
         "description": "QEES Dimmer US",
         "label": "UNI",
         "manufacturer": "Qees"
     },
     "0x0095:0x3103:0x0001": {
-        "description": "Plug-in Socket Dimmer",
+        "description": "Plug-In Socket Dimmer",
         "label": "P313A",
         "manufacturer": "Qees"
     },
     "0x0095:0x3201:0x0001": {
         "description": "QEES P321I MyKey Remote EU",
         "label": "321-IQ(WB)-A1",
         "manufacturer": "Qees"
@@ -4636,35 +4666,35 @@
     },
     "0x0097:0x0024:0x0051": {
         "description": "iShutter",
         "label": "ISHUTTER",
         "manufacturer": "Wintop"
     },
     "0x0097:0x0024:0x0055": {
-        "description": "Blind controller",
+        "description": "Blind Controller",
         "label": "DHS-WIN-BLW-DHS",
         "manufacturer": "Wintop"
     },
     "0x0097:0x1121:0x5501": {
         "description": "In Wall Switch",
         "label": "Digital Home Systems",
         "manufacturer": "Wintop"
     },
     "0x0097:0x1122:0x5501": {
-        "description": "Dual In-wall Switch",
+        "description": "Dual In-Wall Switch",
         "label": "iModuleDouble",
         "manufacturer": "Wintop"
     },
     "0x0097:0x1180:0x4500": {
         "description": "Wintop iSensor",
         "label": "80",
         "manufacturer": "Wintop"
     },
     "0x0097:0x1180:0x5501": {
-        "description": "Multi-sensor",
+        "description": "Multisensor",
         "label": "Multisensor",
         "manufacturer": "Wintop"
     },
     "0x0097:0x1182:0x4500": {
         "description": "iDoorSensor",
         "label": "82",
         "manufacturer": "Wintop"
@@ -4681,35 +4711,35 @@
     },
     "0x0097:0x6123:0x4500": {
         "description": "Wintop iGate",
         "label": "IGAT",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6131:0x4101": {
-        "description": "Keypad with alarm activation rfid tag",
+        "description": "Keypad with Alarm Activation RFID Tag",
         "label": "MINI KEYPAD RFID",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6131:0x4501": {
-        "description": "Keypad with alarm activation rfid tag",
+        "description": "Keypad with Alarm Activation RFID Tag",
         "label": "MINI KEYPAD RFID",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6131:0x5501": {
-        "description": "Keypad with alarm activation rfid tag",
+        "description": "Keypad with Alarm Activation RFID Tag",
         "label": "MINI KEYPAD RFID",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6941:0x5501": {
         "description": "Appliance Module",
         "label": "LE120",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6942:0x4503": {
-        "description": "Wall Plug with dimming function",
+        "description": "Wall Plug with Dimming Function",
         "label": "iPlugDim",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6942:0x5503": {
         "description": "DHS Z-Wave Plug-In Dimmer",
         "label": "DHSZWDMPL01",
         "manufacturer": "Wintop"
@@ -4721,15 +4751,15 @@
     },
     "0x0097:0x6943:0x4501": {
         "description": "Wall Plug",
         "label": "EasyPlug",
         "manufacturer": "Wintop"
     },
     "0x0097:0x6943:0x5501": {
-        "description": "PlugIn Switch with power monitoring",
+        "description": "PlugIn Switch with Power Monitoring",
         "label": "PlugInSwitch",
         "manufacturer": "Wintop"
     },
     "0x0098:0x0000:0x0000": {
         "description": "Z-Wave Thermostat",
         "label": "CT30",
         "manufacturer": "Radio Thermostat Company of America (RTC)"
@@ -4886,75 +4916,75 @@
     },
     "0x0098:0x6e02:0x0101": {
         "description": "Thermostat",
         "label": "CT110",
         "manufacturer": "Radio Thermostat Company of America (RTC)"
     },
     "0x0098:0xc801:0x000c": {
-        "description": "Vivint Element Thermostat w/ other sensors",
+        "description": "Vivint Element Thermostat W/ Other Sensors",
         "label": "CT200",
         "manufacturer": "Radio Thermostat Company of America (RTC)"
     },
     "0x0098:0xc801:0x001d": {
-        "description": "Vivint Element Thermostat w/ other sensors",
+        "description": "Vivint Element Thermostat W/ Other Sensors",
         "label": "CT200",
         "manufacturer": "Radio Thermostat Company of America (RTC)"
     },
     "0x0098:0xc801:0x0022": {
-        "description": "Vivint Element Thermostat w/ other sensors",
+        "description": "Vivint Element Thermostat W/ Other Sensors",
         "label": "CT200X",
         "manufacturer": "Radio Thermostat Company of America (RTC)"
     },
     "0x0099:0x0001:0x0002": {
         "description": "OneGateway",
         "label": "GS1110-1-GR",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0001:0xa001": {
         "description": "AXON\u2122 Home Router",
         "label": "GWS-HR-001",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0002:0x0002": {
-        "description": "Single-socket PowerNode",
+        "description": "Single-Socket PowerNode",
         "label": "GWPN1",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0003:0x0003": {
-        "description": "Multi-socket PowerNode (5-plug)",
+        "description": "Multi-Socket PowerNode (5-Plug)",
         "label": "NP210",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0003:0x0004": {
-        "description": "Multi-socket PowerNode (6-plug)",
+        "description": "Multi-Socket PowerNode (6-Plug)",
         "label": "NP240 / NP242",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0003:0x0006": {
-        "description": "Multi-socket PowerNode (6-plug)",
+        "description": "Multi-Socket PowerNode (6-Plug)",
         "label": "NP240 / NP242",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x0099:0x0006:0x0001": {
-        "description": "GreenWave Reality In Home Display",
+        "description": "GreenWave Reality in Home Display",
         "label": "DE220",
         "manufacturer": "GreenWave Reality Inc."
     },
     "0x009b:0x1000:0x1001": {
         "description": "Go!Control Wireless Security System",
         "label": "2GIG CONTROL 1 345 / CONTROL 2 345",
         "manufacturer": "2gig Technologies Inc."
     },
     "0x009b:0x4350:0x3330": {
         "description": "2GIG GC3",
         "label": "2GIG-GC3-345",
         "manufacturer": "2gig Technologies Inc."
     },
     "0x009b:0x5354:0x5a31": {
-        "description": "2GIG Z-Wave Plus 700-series Programmable Thermostat",
+        "description": "2GIG Z-Wave Plus 700-Series Programmable Thermostat",
         "label": "2GIG-STZ",
         "manufacturer": "2gig Technologies Inc."
     },
     "0x009e:0x0001:0x0001": {
         "description": "AI Ring US (QEES)",
         "label": "0201002 V1.13",
         "manufacturer": "Adventure Interactive"
@@ -4966,15 +4996,15 @@
     },
     "0x0100:0x0001:0x0020": {
         "description": "Insignia LED TV 42",
         "label": "NS-42E859A11",
         "manufacturer": "Insignia"
     },
     "0x0102:0x0001:0x0001": {
-        "description": "Teleprtall Remote (SMK remote)",
+        "description": "Teleprtall Remote (SMK Remote)",
         "label": "REMOT",
         "manufacturer": "SMK Manufacturing Inc."
     },
     "0x0103:0x0001:0x0002": {
         "description": "Plug Actuator",
         "label": "SES FS-ZW",
         "manufacturer": "Diehl AKO"
@@ -4991,25 +5021,25 @@
     },
     "0x0106:0x0002:0x0001": {
         "description": "iControl MiFi Secure",
         "label": "649496 02012 5",
         "manufacturer": "iControl"
     },
     "0x0106:0x0003:0x0002": {
-        "description": "Piper NV Security camera / sensor",
+        "description": "Piper NV Security Camera / Sensor",
         "label": "PIPER NV",
         "manufacturer": "iControl"
     },
     "0x0106:0x0004:0x0001": {
-        "description": "iControl One Link controller",
+        "description": "iControl One Link Controller",
         "label": "CH-1000",
         "manufacturer": "iControl"
     },
     "0x0107:0x0403:0x1000": {
-        "description": "FIBARO Single Relais Switch",
+        "description": "Fibaro Single Relais Switch",
         "label": "FIBEFGS-213",
         "manufacturer": "MegaChips"
     },
     "0x0108:0x0002:0x000d": {
         "description": "Battery Motion Sensor",
         "label": "DCH-Z120",
         "manufacturer": "D-Link"
@@ -5021,35 +5051,35 @@
     },
     "0x0108:0x0002:0x001e": {
         "description": "Smoke Detector",
         "label": "DCH-Z310",
         "manufacturer": "D-Link"
     },
     "0x0108:0x0002:0x0034": {
-        "description": "mydlink\u2122 Door/Window Sensor",
+        "description": "mydlink Door/Window Sensor",
         "label": "DCH-Z112",
         "manufacturer": "D-Link"
     },
     "0x0108:0x0004:0x000a": {
         "description": "Siren",
         "label": "DCH-Z510",
         "manufacturer": "D-Link"
     },
     "0x0108:0x0020:0x0001": {
-        "description": "mydlink\u00ae Connected Home Hub",
+        "description": "mydlink Connected Home Hub",
         "label": "DCH-G020",
         "manufacturer": "D-Link"
     },
     "0x0108:0x0022:0x0003": {
         "description": "D-Link mydlink Connected Home Hub",
         "label": "DCH-G022",
         "manufacturer": "D-Link"
     },
     "0x0108:0x2801:0x0001": {
-        "description": "Staples Connect Hub powered by D-Link",
+        "description": "Staples Connect Hub Powered by D-Link",
         "label": "DCH-G021",
         "manufacturer": "D-Link"
     },
     "0x0109:0x0000:0x0000": {
         "description": "USB Dongle",
         "label": "ZU1401",
         "manufacturer": "Vision Security"
@@ -5221,20 +5251,20 @@
     },
     "0x0109:0x2005:0x0503": {
         "description": "AC/DC Siren",
         "label": "ZM1602",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2005:0x0505": {
-        "description": "Siren with LED strobe light",
+        "description": "Siren with LED Strobe Light",
         "label": "ZM1601-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2005:0x0508": {
-        "description": "Siren with LED strobe light",
+        "description": "Siren with LED Strobe Light",
         "label": "ZM1601-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2005:0x0518": {
         "description": "Battery Operated Siren",
         "label": "ZM1621",
         "manufacturer": "Vision Security"
@@ -5246,40 +5276,40 @@
     },
     "0x0109:0x2006:0x0620": {
         "description": "Door Lock with Handle",
         "label": "ZM1702",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2006:0x0621": {
-        "description": "Monoprice keypad door lock",
+        "description": "Monoprice Keypad Door Lock",
         "label": "ZM1701",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2006:0x0622": {
-        "description": "Monoprice keypad door lock",
+        "description": "Monoprice Keypad Door Lock",
         "label": "ZM1701",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2007:0x0703": {
-        "description": "Monoprice ZWave On/Off Plugin",
+        "description": "Monoprice Z-Wave On/Off Plugin",
         "label": "ZL7201",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2007:0x0706": {
-        "description": "Plug-in On/Off Module",
+        "description": "Plug-In On/Off Module",
         "label": "ZL7201DE-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2008:0x0801": {
         "description": "Lamp Dimmer Module",
         "label": "ZL7101",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2008:0x0803": {
-        "description": "Monoprice ZWave Dimmer Plugin",
+        "description": "Monoprice Z-Wave Dimmer Plugin",
         "label": "ZL7101",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2009:0x0901": {
         "description": "AC/DC Siren",
         "label": "ZM1602",
         "manufacturer": "Vision Security"
@@ -5311,30 +5341,30 @@
     },
     "0x0109:0x200c:0x0c02": {
         "description": "In Wall Relay Switch",
         "label": "ZL7431",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x200c:0x0c06": {
-        "description": "In-wall Switch",
+        "description": "In-Wall Switch",
         "label": "ZL7434-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x200d:0x0d03": {
-        "description": "Drapery controller (up/stop/down)",
+        "description": "Drapery Controller (Up/stop/down)",
         "label": "ZW4101",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x200f:0x0f03": {
         "description": "CO Detector",
         "label": "ZS6301",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x200f:0x0f04": {
-        "description": "Carbon monoxide detector",
+        "description": "Carbon Monoxide Detector",
         "label": "ZS6301-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2012:0x1203": {
         "description": "Z-Wave Repeater",
         "label": "ZR1202EU-5",
         "manufacturer": "Vision Security"
@@ -5346,15 +5376,15 @@
     },
     "0x0109:0x2012:0x1207": {
         "description": "Z-Wave Repeater",
         "label": "ZR1202EU-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2014:0x1401": {
-        "description": "Plug in Z-Wave to 433Mhz bridge plus lamp dimmer",
+        "description": "Plug in Z-Wave to 433Mhz Bridge Plus Lamp Dimmer",
         "label": "Z-BRDG-433",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2016:0x1616": {
         "description": "In Wall Relay Switch",
         "label": "ZL7431",
         "manufacturer": "Vision Security"
@@ -5366,25 +5396,25 @@
     },
     "0x0109:0x2017:0x1717": {
         "description": "In Wall Dual Relay Switch",
         "label": "ZL7432",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2017:0x1719": {
-        "description": "In-wall Two Relay",
+        "description": "In-Wall Two Relay",
         "label": "ZL7435-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x2018:0x1805": {
         "description": "Curtain Module",
         "label": "ZW4111EU-5",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x201a:0x1aa4": {
-        "description": "Plug In Power Monitor",
+        "description": "Plug in Power Monitor",
         "label": "PID15903",
         "manufacturer": "Vision Security"
     },
     "0x0109:0x201b:0x1b02": {
         "description": "Keyfob",
         "label": "ZT1101",
         "manufacturer": "Vision Security"
@@ -5546,65 +5576,60 @@
     },
     "0x010c:0x0001:0x0001": {
         "description": "ThereGate Gateway Controller",
         "label": "Gateway Controller",
         "manufacturer": "There Corporation"
     },
     "0x010e:0x0003:0x0002": {
-        "description": "Danalock v2 circle",
+        "description": "Danalock v2 Circle",
         "label": "BTZW125",
         "manufacturer": "Poly-control"
     },
     "0x010e:0x0008:0x0002": {
-        "description": "Danalock v2 circle",
+        "description": "Danalock v2 Circle",
         "label": "BTZW125",
         "manufacturer": "Poly-control"
     },
     "0x010e:0x0008:0x0004": {
         "description": "Danalock Universal Module V1",
         "label": "BTZEUMV1",
         "manufacturer": "Poly-control"
     },
     "0x010e:0x0009:0x0001": {
-        "description": "Z-Wave controlled door lock with Bluetooth Smart",
+        "description": "Z-Wave Controlled Door Lock with Bluetooth Smart",
         "label": "Danalock V3-BTZE",
         "manufacturer": "Poly-control"
     },
     "0x010e:0x0009:0x0002": {
         "description": "Danalock Universal Module V3",
         "label": "UMV3-BTZ",
         "manufacturer": "Poly-control"
     },
-    "0x010f:0x0000:0x1000": {
-        "description": "FIBARO Smoke Sensor",
-        "label": "Smoke Sensor",
-        "manufacturer": "Fibargroup"
-    },
     "0x010f:0x0000:0x1001": {
-        "description": "FIBARO Flood Sensor",
-        "label": "FGFS-101 ()",
+        "description": "Fibaro Flood Sensor",
+        "label": "FGFS-101",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0000:0x2001": {
-        "description": "FIBARO Flood Sensor",
-        "label": "FGFS-101 ()",
+        "description": "Fibaro Flood Sensor",
+        "label": "FGFS-101",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0001:0x1001": {
-        "description": "FIBARO",
+        "description": "Fibaro",
         "label": "HC2",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0002:0x1000": {
-        "description": "FIBARO Home Center Lite",
+        "description": "Fibaro Home Center Lite",
         "label": "HCL",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0002:0x1001": {
-        "description": "FIBARO Home Center Lite",
+        "description": "Fibaro Home Center Lite",
         "label": "HCL",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0003:0x1000": {
         "description": "Home Center 3",
         "label": "FGHC3-001",
         "manufacturer": "Fibargroup"
@@ -5945,14 +5970,19 @@
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0403:0x3000": {
         "description": "Single Switch 2",
         "label": "FGS213",
         "manufacturer": "Fibargroup"
     },
+    "0x010f:0x0403:0x4000": {
+        "description": "Single Switch 2",
+        "label": "FGS213",
+        "manufacturer": "Fibargroup"
+    },
     "0x010f:0x0403:0x6000": {
         "description": "Single Switch 2",
         "label": "FGS213",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0404:0x1000": {
         "description": "Smart Module",
@@ -6290,14 +6320,19 @@
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0c00:0x3000": {
         "description": "Smoke Sensor",
         "label": "FGSS001",
         "manufacturer": "Fibargroup"
     },
+    "0x010f:0x0c00:0x4000": {
+        "description": "Smoke Sensor",
+        "label": "FGSS001",
+        "manufacturer": "Fibargroup"
+    },
     "0x010f:0x0c02:0x1002": {
         "description": "Smoke Detector",
         "label": "FGSD002",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x0c02:0x1003": {
         "description": "Smoke Detector",
@@ -6431,20 +6466,20 @@
     },
     "0x010f:0x1501:0x1000": {
         "description": "Fibaro Wall Plug",
         "label": "FGWPG-121",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x1701:0x2000": {
-        "description": "FIBARO Wall Plug",
+        "description": "Fibaro Wall Plug",
         "label": "FGWPB-111",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x1801:0x1000": {
-        "description": "FIBARO Wall Plug UK",
+        "description": "Fibaro Wall Plug UK",
         "label": "FGWPG-111",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x1a01:0x1000": {
         "description": "Walli Double Switch",
         "label": "FGWDSEU-221",
         "manufacturer": "Fibargroup"
@@ -6461,15 +6496,15 @@
     },
     "0x010f:0x1d01:0x1000": {
         "description": "Fibaro Walli Roller Shutter",
         "label": "FGWREU-111",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x1f01:0x1000": {
-        "description": "Fibaro Walli Outlet type E/F",
+        "description": "Fibaro Walli Outlet Type E/F",
         "label": "FGWOE-011",
         "manufacturer": "Fibargroup"
     },
     "0x010f:0x2301:0x1000": {
         "description": "Walli Controller",
         "label": "FGWCEU-201",
         "manufacturer": "Fibargroup"
@@ -6486,15 +6521,15 @@
     },
     "0x0110:0x2411:0x0001": {
         "description": "nanogrid\u2122 Wireless Light Switch",
         "label": "FDN2311",
         "manufacturer": "Frostdale"
     },
     "0x0110:0x7333:0x0031": {
-        "description": "3way switch with temp sensor",
+        "description": "3way Switch with Temp Sensor",
         "label": "FDN2300",
         "manufacturer": "Frostdale"
     },
     "0x0111:0x1000:0x0010": {
         "description": "Tronico SmartPlug",
         "label": "SPZ7113",
         "manufacturer": "Tronico Technology Co. Ltd."
@@ -6561,15 +6596,15 @@
     },
     "0x0113:0x5246:0x3133": {
         "description": "20A Relay Fixture Module",
         "label": "LFM-20",
         "manufacturer": "Evolve"
     },
     "0x0113:0x5250:0x3030": {
-        "description": "Appliance module",
+        "description": "Appliance Module",
         "label": "LPM-15",
         "manufacturer": "Evolve"
     },
     "0x0113:0x5252:0x3530": {
         "description": "Duplex Receptacle",
         "label": "LOM15",
         "manufacturer": "Evolve"
@@ -6611,20 +6646,20 @@
     },
     "0x0115:0x0024:0x0001": {
         "description": "Floor Thermostat",
         "label": "ZME_FT",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x0100:0x0001": {
-        "description": "4 button keyfob",
+        "description": "4 Button Keyfob",
         "label": "KFOB",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x0100:0x0002": {
-        "description": "4 button keyfob",
+        "description": "4 Button Keyfob",
         "label": "KFOB",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x0100:0x0004": {
         "description": "Double Paddle Wall Controller",
         "label": "WCD2",
         "manufacturer": "Z-Wave.Me"
@@ -6641,15 +6676,15 @@
     },
     "0x0115:0x0100:0x0103": {
         "description": "Secure 4 Button Key Chain Controller",
         "label": "ZME_KFOB-S",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x0100:0x0400": {
-        "description": "Z-Wave weather interface",
+        "description": "Z-Wave Weather Interface",
         "label": "Z-Weather",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x0110:0x0001": {
         "description": "Z-Uno",
         "label": "V3",
         "manufacturer": "Z-Wave.Me"
@@ -6676,15 +6711,15 @@
     },
     "0x0115:0x0400:0x0004": {
         "description": "Single Paddle Wall Controller",
         "label": "ZME_06443",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x1000:0x0001": {
-        "description": "Flush mountable switch",
+        "description": "Flush Mountable Switch",
         "label": "ZME_06431",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x1000:0x0002": {
         "description": "Zwave.Me Dimmer Set Everlux",
         "label": "ZME_06433",
         "manufacturer": "Z-Wave.Me"
@@ -6696,15 +6731,15 @@
     },
     "0x0115:0x1000:0x0004": {
         "description": "Single Paddle Wall Controller",
         "label": "ZME_06443",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x1000:0x0100": {
-        "description": "Double switch",
+        "description": "Double Switch",
         "label": "ZME_05461",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0115:0x1000:0x0200": {
         "description": "Wall Plug Switch",
         "label": "ZME_06437",
         "manufacturer": "Z-Wave.Me"
@@ -6716,20 +6751,20 @@
     },
     "0x0115:0xf111:0x1111": {
         "description": "MultiRelay",
         "label": "RS-10PM2",
         "manufacturer": "Haseman"
     },
     "0x0115:0xf222:0x2111": {
-        "description": "4x Relay and 4x Universal Dimmer",
+        "description": "4X Relay and 4X Universal Dimmer",
         "label": "R4D4",
         "manufacturer": "Haseman"
     },
     "0x0115:0xffff:0xffff": {
-        "description": "Blinds controller",
+        "description": "Blinds Controller",
         "label": "ZME_05459",
         "manufacturer": "Z-Wave.Me"
     },
     "0x0116:0x0001:0x0001": {
         "description": "Motion Detector",
         "label": "HSP02",
         "manufacturer": "Chromagic Technologies Corporation"
@@ -6741,30 +6776,30 @@
     },
     "0x0116:0x0010:0x0001": {
         "description": "Chromagic Z-Wave Remote Button (EU)",
         "label": "HAC01",
         "manufacturer": "Chromagic Technologies Corporation"
     },
     "0x0116:0x0011:0x0001": {
-        "description": "In wall single switch",
+        "description": "In Wall Single Switch",
         "label": "HAN01",
         "manufacturer": "Chromagic Technologies Corporation"
     },
     "0x0116:0x0011:0x0002": {
-        "description": "-1 - Z-Wave In Wall Switch",
+        "description": "-1 - Z-Wave in Wall Switch",
         "label": "HAN02",
         "manufacturer": "Chromagic Technologies Corporation"
     },
     "0x0116:0x1182:0x4501": {
-        "description": "Contact and temperature sensor",
+        "description": "Contact and Temperature Sensor",
         "label": "ITEMP",
         "manufacturer": "Chromagic Technologies Corporation"
     },
     "0x0116:0x1188:0x4501": {
-        "description": "Contact and temperature sensor",
+        "description": "Contact and Temperature Sensor",
         "label": "ITEMP",
         "manufacturer": "Chromagic Technologies Corporation"
     },
     "0x0117:0x0001:0x0080": {
         "description": "Gewa Andromeda Socket",
         "label": "419880",
         "manufacturer": "Abilia"
@@ -6821,15 +6856,15 @@
     },
     "0x0118:0x0003:0x0008": {
         "description": "Wall Plug Dimmer",
         "label": "TZ67",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0004:0x0002": {
-        "description": "Smart meter switch",
+        "description": "Smart Meter Switch",
         "label": "TZ69",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0004:0x0003": {
         "description": "Dual Paddle Wall Dimmer",
         "label": "TZ65D",
         "manufacturer": "TKB Home"
@@ -6861,15 +6896,15 @@
     },
     "0x0118:0x0102:0x2056": {
         "description": "TKB Switch D",
         "label": "TZ56",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0116:0x3119": {
-        "description": "Smart meter switch",
+        "description": "Smart Meter Switch",
         "label": "TZ69",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0121:0x0133": {
         "description": "In Wall Micro Switch",
         "label": "TZ78",
         "manufacturer": "TKB Home"
@@ -6886,15 +6921,15 @@
     },
     "0x0118:0x0202:0x0611": {
         "description": "Wall Plug Dimmer",
         "label": "TZ67",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0103": {
-        "description": "Smart meter switch",
+        "description": "Smart Meter Switch",
         "label": "TZ69",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0201": {
         "description": "Dual Paddle Wall Dimmer",
         "label": "TZ55D",
         "manufacturer": "TKB Home"
@@ -6906,46 +6941,46 @@
     },
     "0x0118:0x0311:0x0203": {
         "description": "Double Relay Wall Switch",
         "label": "TZ37",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0302": {
-        "description": "RGB dimmer switch",
+        "description": "RGB Dimmer Switch",
         "label": "TZ77",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0303": {
         "description": "Rollershutter Controller",
         "label": "TZ75",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0304": {
-        "description": "Insert two channel switch module",
+        "description": "Insert Two Channel Switch Module",
         "label": "TZ74",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0305": {
-        "description": "Insert switch module",
+        "description": "Insert Switch Module",
         "label": "TZ79",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0505": {
         "description": "Weekly Programming Thermostat with LCD Touch Screen",
         "label": "TZE93",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0311:0x0506": {
         "description": "Color Touch Heating Thermostat",
         "label": "TZE96",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0808:0x0808": {
-        "description": "Single Paddle Wall Dimmer",
-        "label": "TZ55S",
+        "description": "Single/Dual Paddle Wall Dimmer",
+        "label": "TZ35S / TZ35D / TZ55S / TZ55D",
         "manufacturer": "TKB Home"
     },
     "0x0118:0x0b00:0x0002": {
         "description": "Lifting Controller (Blinds Controller)",
         "label": "GR308",
         "manufacturer": "TKB Home"
     },
@@ -6956,20 +6991,20 @@
     },
     "0x011a:0x0101:0x0102": {
         "description": "Binary Switch",
         "label": "ZW15S",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0101:0x0103": {
-        "description": "Duplex receptacle",
+        "description": "Duplex Receptacle",
         "label": "ZW15R",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0101:0x0104": {
-        "description": "Plug-in Appliance Module",
+        "description": "Plug-In Appliance Module",
         "label": "ZWN-333",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0101:0x0603": {
         "description": "20A Tamper Resistant Duplex Receptacle",
         "label": "ZW20R",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
@@ -6991,30 +7026,30 @@
     },
     "0x011a:0x0102:0x0202": {
         "description": "Dimmer",
         "label": "ZW500D",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0111:0x0101": {
-        "description": "In-wall Smart Meter Duplex Receptacle",
+        "description": "In-Wall Smart Meter Duplex Receptacle",
         "label": "ZW20RM",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0111:0x0102": {
         "description": "Binary Switch + Meter",
         "label": "ZW15SM",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0111:0x0105": {
         "description": "In-Wall Smart Meter Duplex Receptacle (15A)",
         "label": "ZW15RM-PLUS",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0111:0x0201": {
-        "description": "In-wall Smart Meter Dimmer Switch",
+        "description": "In-Wall Smart Meter Dimmer Switch",
         "label": "ZW500DM",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x0111:0x0202": {
         "description": "ZWN323M",
         "label": "Plug-In Smart Meter Dimmer Switch",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
@@ -7041,15 +7076,15 @@
     },
     "0x011a:0x0801:0x0b03": {
         "description": "Scene Controller",
         "label": "ZWN-SC7",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x1112:0x3040": {
-        "description": "ENERWAVE Z-WAVE Dimmer Switch",
+        "description": "ENERWAVE Z-Wave Dimmer Switch",
         "label": "ZW500",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
     },
     "0x011a:0x1415:0x3343": {
         "description": "Binary Switch",
         "label": "ZW15S",
         "manufacturer": "Wenzhou MTLC Electric Appliances Co., Ltd."
@@ -7081,15 +7116,15 @@
     },
     "0x0122:0x0000:0x0000": {
         "description": "Prodrive - ED2.0 Meter Adapter",
         "label": "ED2.0 METER ADAPTER",
         "manufacturer": "MSK - Miyakawa Seisakusho"
     },
     "0x0122:0x0001:0x0001": {
-        "description": "MSK CT type electric power measuring instrument",
+        "description": "MSK CT Type Electric Power Measuring Instrument",
         "label": "ME-D101",
         "manufacturer": "MSK - Miyakawa Seisakusho"
     },
     "0x0123:0x0001:0x0063": {
         "description": "Iwatsu LED Dimmer",
         "label": "LED Dimmer",
         "manufacturer": "IWATSU"
@@ -7286,15 +7321,15 @@
     },
     "0x0129:0x6600:0x0002": {
         "description": "Conexis L1",
         "label": "SD-L1000-CH",
         "manufacturer": "Yale"
     },
     "0x0129:0x6f01:0x0001": {
-        "description": "External siren",
+        "description": "External Siren",
         "label": "SR-BX-ZW",
         "manufacturer": "Yale"
     },
     "0x0129:0x8001:0x0b00": {
         "description": "NexTouch Wireless Push Button with Z-Wave",
         "label": "NTB610",
         "manufacturer": "Yale"
@@ -7305,41 +7340,46 @@
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0x1000": {
         "description": "Real Living Assure Lock with Z-Wave and Bluetooth",
         "label": "YRD426-ZW2",
         "manufacturer": "Yale"
     },
+    "0x0129:0x8002:0x1600": {
+        "description": "Assure Touchscreen Deadbolt",
+        "label": "YRD226 / YRC226 / YRC246 / YRD256 / YRC256 / YRD446",
+        "manufacturer": "Yale"
+    },
     "0x0129:0x8002:0x4600": {
         "description": "Assure Touchscreen Deadbolt",
         "label": "YRD226 / YRC226 / YRC246 / YRD256 / YRC256 / YRD446",
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0x46c2": {
-        "description": "Assure Interconnected Z-Wave Enabled Touch Screen Deadbolt",
+        "description": "Assure Interconnected Keyed Touch Screen Deadbolt",
         "label": "YRC226-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0x46c5": {
-        "description": "Assure Interconnected Z-Wave Enabled SL Touch Screen Deadbolt",
+        "description": "Assure Interconnected Keyless Touch Screen Deadbolt",
         "label": "YRC256-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0x46d2": {
-        "description": "Assure Z-Wave Enabled Touch Screen Deadbolt",
+        "description": "Assure Keyed Touch Screen Deadbolt",
         "label": "YRD226-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0x46d5": {
-        "description": "Assure SL Lock",
+        "description": "Assure Keyless Touch Screen Deadbolt",
         "label": "YRD256-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8002:0xa570": {
-        "description": "Assure SL Lock",
+        "description": "Assure Keyless Touch Screen Deadbolt",
         "label": "YRD256-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8003:0x0b00": {
         "description": "NexTouch Wireless Touchscreen with Z-Wave",
         "label": "NTB620",
         "manufacturer": "Yale"
@@ -7351,25 +7391,25 @@
     },
     "0x0129:0x8004:0x1000": {
         "description": "Assure Lock with Bluetooth Z-Wave Enabled Push Button Deadbolt",
         "label": "YRD416",
         "manufacturer": "Yale"
     },
     "0x0129:0x8004:0x46c1": {
-        "description": "Interconnected Z-Wave Enabled Keypad Deadbolt",
+        "description": "Interconnected Push Button Deadbolt",
         "label": "YRC216-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8004:0x46d1": {
-        "description": "Assure Z-Wave Enabled Keypad Deadbolt",
+        "description": "Assure Keyed Push Button Deadbolt",
         "label": "YRD216-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8007:0x0a00": {
-        "description": "NexTouch Sectional Mortise Push Button Keypad Lock with cylinder with deadbolt",
+        "description": "NexTouch Sectional Mortise Push Button Keypad Lock with Cylinder with Deadbolt",
         "label": "NTM610 / NTM615 / NTM630 / NTM625",
         "manufacturer": "Yale"
     },
     "0x0129:0x8008:0x0a00": {
         "description": "NexTouch Sectional Mortise Touch Screen Keypad Lock",
         "label": "NTM620 / NTM625 / NTM640 / NTM645",
         "manufacturer": "Yale"
@@ -7411,15 +7451,15 @@
     },
     "0x0129:0x8014:0x1604": {
         "description": "Assure Lock for Andersen Patio Doors",
         "label": "YRM476",
         "manufacturer": "Yale"
     },
     "0x0129:0x803a:0x0508": {
-        "description": "Touchscreen Deadbolt with Integrated ZWave Plus",
+        "description": "Touchscreen Deadbolt with Integrated Z-Wave Plus",
         "label": "YRD156",
         "manufacturer": "Yale"
     },
     "0x0129:0x803b:0x0508": {
         "description": "ProSL Key Free Keypad Deadbolt with Z-Wave Plus",
         "label": "YRD136",
         "manufacturer": "Yale"
@@ -7481,20 +7521,20 @@
     },
     "0x0129:0x8101:0x0b2a": {
         "description": "NexTouch Touch Screen Lever Lock",
         "label": "NTB642-ZW2",
         "manufacturer": "Yale"
     },
     "0x0129:0x8101:0x8109": {
-        "description": "Yale Real Living\u00ae Assure Lock\u00ae SL Key Free Touchscreen Deadbolt",
+        "description": "Assure 2nd Generation Keyless Touch Screen Deadbolt",
         "label": "YRD652-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8101:0x810a": {
-        "description": "Real Living\u00ae Assure Lock\u2122 Z-Wave Enabled Push Button Deadbolt",
+        "description": "Assure 2nd Generation Keyed Push Button Deadbolt",
         "label": "NF-YRD612-ZW3",
         "manufacturer": "Yale"
     },
     "0x0129:0x8102:0x0c0c": {
         "description": "NexTouch Keypad Exit Rim Trim",
         "label": "NTT612-ZW2",
         "manufacturer": "Yale"
@@ -7510,14 +7550,34 @@
         "manufacturer": "Yale"
     },
     "0x0129:0x8103:0x12d4": {
         "description": "Z-Wave Enabled Keyless Deadbolt",
         "label": "YRD642-ZW2",
         "manufacturer": "Yale"
     },
+    "0x0129:0x8103:0x52c2": {
+        "description": "Assure 2nd Generation Fire Rated Keyed Interconnected Touch Screen Deadbolt",
+        "label": "YRC622-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8103:0x52c4": {
+        "description": "Assure 2nd Generation Fire Rated Keyless Interconnected Touch Screen Deadbolt",
+        "label": "YRC642-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8103:0x52d2": {
+        "description": "Assure 2nd Generation Fire Rated Keyed Touch Screen Deadbolt",
+        "label": "YRD622-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8103:0x52d4": {
+        "description": "Assure 2nd Generation Fire Rated Keyless Touch Screen Deadbolt",
+        "label": "YRD642-ZW3",
+        "manufacturer": "Yale"
+    },
     "0x0129:0x8104:0x05d1": {
         "description": "Yale Assure 2 Lock SL Keyed Keypad",
         "label": "YRD410-ZW2",
         "manufacturer": "Yale"
     },
     "0x0129:0x8104:0x05d2": {
         "description": "Yale Assure 2 Lock SL Keyed Touchscreen",
@@ -7530,29 +7590,79 @@
         "manufacturer": "Yale"
     },
     "0x0129:0x8104:0x05d5": {
         "description": "Yale Assure 2 Lock\u00ae SL Key Free Touchscreen Deadbolt",
         "label": "YRD450-ZW2",
         "manufacturer": "Yale"
     },
+    "0x0129:0x8104:0x45d1": {
+        "description": "Assure 2 Keyed Push Button Deadbolt",
+        "label": "YRD410-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8104:0x45d2": {
+        "description": "Assure 2 Keyed Touch Screen Deadbolt",
+        "label": "YRD420-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8104:0x45d3": {
+        "description": "Assure 2 Keyless Push Button Deadbolt",
+        "label": "YRD430-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8104:0x45d5": {
+        "description": "Assure 2 Keyless Touch Screen Deadbolt",
+        "label": "YRD450-ZW3",
+        "manufacturer": "Yale"
+    },
     "0x0129:0x8109:0x0dd2": {
         "description": "Assure Lock Touchscreen Deadbolt",
         "label": "NF-YRD622-ZW2",
         "manufacturer": "Yale"
     },
     "0x0129:0x8109:0x0dd5": {
         "description": "Assure Lock\u00ae SL Key Free Touchscreen Deadbolt",
         "label": "YRD652-ZW2",
         "manufacturer": "Yale"
     },
+    "0x0129:0x8109:0x4dc2": {
+        "description": "Assure 2nd Generation Interconnected Keyed Touch Screen Deadbolt",
+        "label": "NF-YRC622-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8109:0x4dc5": {
+        "description": "Assure 2nd Generation Interconnected Keyless Touch Screen Deadbolt",
+        "label": "YRC652-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8109:0x4dd2": {
+        "description": "Assure 2nd Generation Keyed Touch Screen Deadbolt",
+        "label": "NF-YRD622-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x8109:0x4dd5": {
+        "description": "Assure 2nd Generation Keyless Touch Screen Deadbolt",
+        "label": "YRD652-ZW3",
+        "manufacturer": "Yale"
+    },
     "0x0129:0x810a:0x0dd1": {
         "description": "Assure Lock\u2122 Z-Wave Enabled Push Button Deadbolt",
         "label": "NF-YRD612-ZW2",
         "manufacturer": "Yale"
     },
+    "0x0129:0x810a:0x4dc1": {
+        "description": "Assure 2nd Generation Interconnected Keyed Push Button Deadbolt",
+        "label": "NF-YRC612-ZW3",
+        "manufacturer": "Yale"
+    },
+    "0x0129:0x810a:0x4dd1": {
+        "description": "Assure 2nd Generation Keyed Push Button Deadbolt",
+        "label": "NF-YRD612-ZW3",
+        "manufacturer": "Yale"
+    },
     "0x0129:0x842a:0x3cac": {
         "description": "Real Living Touchscreen Lever Lock",
         "label": "YRL210 / YRL220",
         "manufacturer": "Yale"
     },
     "0x0129:0xc600:0x0002": {
         "description": "Smart Door Lock Z-Wave Module 2",
@@ -7596,20 +7706,20 @@
     },
     "0x012a:0x4744:0x3032": {
         "description": "Z-Wave Plug-In Dimmer",
         "label": "QZ2140-840",
         "manufacturer": "Qolsys"
     },
     "0x012a:0x4744:0x3033": {
-        "description": "Smart Plug-in Switch",
+        "description": "Smart Plug-In Switch",
         "label": "IQ Outlet",
         "manufacturer": "Qolsys"
     },
     "0x012a:0x4744:0x3034": {
-        "description": "Smart Plug In Dimmer",
+        "description": "Smart Plug in Dimmer",
         "label": "IQ Dimmer",
         "manufacturer": "Qolsys"
     },
     "0x012a:0xff00:0xff0d": {
         "description": "IQ Smart Dimmer",
         "label": "QZ2142-840",
         "manufacturer": "Qolsys"
@@ -7651,40 +7761,40 @@
     },
     "0x0131:0x0001:0x0012": {
         "description": "In Wall Dual Relay",
         "label": "PAN04",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0001:0x0015": {
-        "description": "roller shutter",
+        "description": "Roller Shutter",
         "label": "PAN08",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0002:0x0002": {
-        "description": "RGBW bulb",
+        "description": "RGBW Bulb",
         "label": "RGBWE27ZW",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0002:0x0003": {
         "description": "RGBW Bulb V2",
         "label": "RGBWE2",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0002:0x000c": {
-        "description": "Door/temp/illumination/motion sensor",
+        "description": "Door/temp/illumination/motion Sensor",
         "label": "PSP02",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0002:0x001e": {
         "description": "Smoke Sensor",
         "label": "PH-PSG01",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0003:0x0082": {
-        "description": "Door sensor",
+        "description": "Door Sensor",
         "label": "NE-NAS-DS01Z",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0003:0x0512": {
         "description": "Auto Valve",
         "label": "GR-105",
         "manufacturer": "Zipato"
@@ -7696,45 +7806,55 @@
     },
     "0x0131:0x0003:0x1083": {
         "description": "Indoor Siren",
         "label": "NE-NAS-AB02Z",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0003:0x1089": {
-        "description": "PIR motion sensor and light measurement",
+        "description": "PIR Motion Sensor and Light Measurement",
         "label": "NE-NAS-PD01Z",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0004:0x000a": {
         "description": "Multisound Indoor Siren",
         "label": "PH-PSE02",
         "manufacturer": "Zipato"
     },
+    "0x0131:0x0004:0x1118": {
+        "description": "Contact Sensor 2",
+        "label": "AH-NEO-DS07Z",
+        "manufacturer": "Alloy"
+    },
+    "0x0131:0x0004:0x1123": {
+        "description": "5 in 1 PIR Motion Sensor",
+        "label": "AH-NAS-PD07U1",
+        "manufacturer": "Alloy"
+    },
     "0x0131:0x0006:0x001a": {
         "description": "Micro Module Energy Meter",
         "label": "ZIP-PAB01",
         "manufacturer": "Zipato"
     },
     "0x0131:0x0033:0x1082": {
-        "description": "Door sensor",
+        "description": "Door Sensor",
         "label": "NE-NAS-DS01Z",
         "manufacturer": "Zipato"
     },
     "0x0131:0x2001:0x0106": {
         "description": "Door Window Sensor",
         "label": "ZD2102-5",
         "manufacturer": "Zipato"
     },
     "0x0131:0x2002:0x0205": {
-        "description": "Multi Sensor Dual: motion and temperature sensor",
+        "description": "Multi Sensor Dual: Motion and Temperature Sensor",
         "label": "ZP3102",
         "manufacturer": "Zipato"
     },
     "0x0131:0x201f:0x1f20": {
-        "description": "Zipato 4 in 1 Door Sensor",
+        "description": "4 in 1 Door Sensor",
         "label": "VS-ZD2301",
         "manufacturer": "Zipato"
     },
     "0x0131:0x220a:0x1352": {
         "description": "MINI ENERGY DIMMER",
         "label": "MH-P220",
         "manufacturer": "Zipato"
@@ -7751,15 +7871,15 @@
     },
     "0x0131:0x8004:0x1000": {
         "description": "Smart Water Leakage Sensor",
         "label": "HM-HS1WL-Z",
         "manufacturer": "Zipato"
     },
     "0x0131:0x8005:0x1000": {
-        "description": "CO Sensor with acoustic alarm",
+        "description": "CO Sensor with Acoustic Alarm",
         "label": "HM-HS1CA",
         "manufacturer": "Zipato"
     },
     "0x0133:0x0001:0x0001": {
         "description": "Home Automation and Control Unit",
         "label": "PGZNG1-2ADNAS",
         "manufacturer": "Netgear"
@@ -7776,30 +7896,30 @@
     },
     "0x0135:0x0003:0x0001": {
         "description": "Dimmer Module",
         "label": "SHD2210",
         "manufacturer": "ZyXEL"
     },
     "0x0135:0x0004:0x0001": {
-        "description": "Plug-in On/Off Module",
+        "description": "Plug-In On/Off Module",
         "label": "SHD2110",
         "manufacturer": "ZyXEL"
     },
     "0x0135:0x0004:0x0002": {
         "description": "On/Off Plug with Metering",
         "label": "SHD3110",
         "manufacturer": "ZyXEL"
     },
     "0x0135:0x0006:0x0001": {
         "description": "Temperature/Humidity Sensor",
         "label": "SHD1110",
         "manufacturer": "ZyXEL"
     },
     "0x0135:0x000b:0x0001": {
-        "description": "Flood sensor",
+        "description": "Flood Sensor",
         "label": "ST812",
         "manufacturer": "ZyXEL"
     },
     "0x0135:0x0101:0x0001": {
         "description": "PIR Sensor",
         "label": "SHD 1112",
         "manufacturer": "ZyXEL"
@@ -7856,110 +7976,115 @@
     },
     "0x013b:0x1000:0x1828": {
         "description": "Astralink Android Home Station",
         "label": "HXS1000",
         "manufacturer": "AstraLink"
     },
     "0x013c:0x0001:0x0000": {
-        "description": "Smart Energy Plug In Switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN16",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0001": {
-        "description": "Smart Energy Plug In Switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN11",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0003": {
-        "description": "In Wall Dual Relay Switch Module 2x1.5kW with power meter",
+        "description": "In Wall Dual Relay Switch Module 2x1.5kW with Power Meter",
         "label": "PAN04",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0004": {
         "description": "In Wall Dual Relay (1 Way) Switch Module 2 x 1.5kW",
         "label": "PAN06",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0005": {
-        "description": "TWO SPDT Switch module with meter",
+        "description": "TWO SPDT Switch Module with Meter",
         "label": "Philio PAN07-1A",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0006": {
         "description": "Relay Insert for Blind Control",
         "label": "PAN08",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x000f": {
         "description": "In Wall Micromodule Single Switch",
         "label": "PAN03",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0010": {
-        "description": "Single relay in-wall switch module",
+        "description": "Single Relay In-Wall Switch Module",
         "label": "PAN05-1B",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0011": {
-        "description": "Smart Energy Plug In Switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN11",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0012": {
-        "description": "In Wall Dual Relay Switch Module 2x1.5kW with power meter",
+        "description": "In Wall Dual Relay Switch Module 2x1.5kW with Power Meter",
         "label": "PAN04",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0013": {
         "description": "In Wall Dual Relay (1 Way) Switch Module 2 x 1.5kW",
         "label": "PAN06",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0014": {
-        "description": "In Wall Dual Relay Switch Module 2x1.5kW with power meter",
+        "description": "In Wall Dual Relay Switch Module 2x1.5kW with Power Meter",
         "label": "PAN04",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0015": {
-        "description": "Roller shutter controller",
+        "description": "Roller Shutter Controller",
         "label": "PAN08-1a",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0029": {
-        "description": "Smart Energy Plug In Switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN16",
         "manufacturer": "Philio Technology Corp"
     },
+    "0x013c:0x0001:0x002f": {
+        "description": "Smart Outlet Plug",
+        "label": "NSG-AB-02",
+        "manufacturer": "Safe Grow"
+    },
     "0x013c:0x0001:0x0030": {
-        "description": "Smart Energy Plug In Switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN11",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0038": {
-        "description": "Smart Energy plug In switch",
+        "description": "Smart Energy Plug in Switch",
         "label": "PAN15-1-NES",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0061": {
-        "description": "In Wall Dual Relay Switch Module 2x1.5kW with power meter",
+        "description": "In Wall Dual Relay Switch Module 2x1.5kW with Power Meter",
         "label": "PAN04",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0073": {
         "description": "Smart Switch Box",
         "label": "PAN26",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0077": {
         "description": "In-Wall Dual Relay Switch Module",
         "label": "PAN30",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0001:0x0080": {
-        "description": "In Wall Roller shutter Controller",
+        "description": "In Wall Roller Shutter Controller",
         "label": "PAN34",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0002:0x0002": {
         "description": "Slim Multi-Sensor (Door/Motion/Temperature/Illumination)",
         "label": "PSM02",
         "manufacturer": "Philio Technology Corp"
@@ -7986,15 +8111,15 @@
     },
     "0x013c:0x0002:0x001f": {
         "description": "Flood Sensor",
         "label": "PAT02-A",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0002:0x0020": {
-        "description": "Z-Wave room sensor",
+        "description": "Z-Wave Room Sensor",
         "label": "PAT02-B",
         "manufacturer": "Philio Technology Corp"
     },
     "0x013c:0x0002:0x0021": {
         "description": "Flood Sensor",
         "label": "PAT02-C",
         "manufacturer": "Philio Technology Corp"
@@ -8142,35 +8267,40 @@
     "0x0147:0x0002:0x0003": {
         "description": "Z-Wave Daughtercard",
         "label": "RaZberry",
         "manufacturer": "Z-Wave.me"
     },
     "0x0147:0x0400:0x0001": {
         "description": "Z-Wave.Me Razberry Daughtercard",
-        "label": "RaZberry Controller 2016 ZWave+",
+        "label": "RaZberry Controller 2016 Z-Wave+",
         "manufacturer": "Z-Wave.me"
     },
     "0x0147:0x0400:0x0002": {
         "description": "Z-Wave.Me Razberry Daughtercard",
-        "label": "RaZberry Controller 2016 ZWave+",
+        "label": "RaZberry Controller 2016 Z-Wave+",
+        "manufacturer": "Z-Wave.me"
+    },
+    "0x0147:0x0401:0x0001": {
+        "description": "Z-Wave Shield",
+        "label": "RaZberry 7",
         "manufacturer": "Z-Wave.me"
     },
     "0x0147:0x0401:0x0101": {
-        "description": "Z-Wave Shield for Raspberry Pi",
+        "description": "Z-Wave Shield with External Antenna",
         "label": "RaZberry 7 Pro",
         "manufacturer": "Z-Wave.me"
     },
     "0x0148:0x0001:0x0001": {
         "description": "Thermostatic Valve",
         "label": "STELLA Z",
         "manufacturer": "Eurotronics"
     },
     "0x0148:0x0002:0x0001": {
         "description": "Thermostatic Valve",
-        "label": "COMET Z",
+        "label": "Comet Z",
         "manufacturer": "Eurotronics"
     },
     "0x0148:0x0003:0x0001": {
         "description": "Thermostatic Valve",
         "label": "Spirit",
         "manufacturer": "Eurotronics"
     },
@@ -8185,22 +8315,27 @@
         "manufacturer": "Eurotronics"
     },
     "0x0148:0x0004:0x0001": {
         "description": "Temperature & Humidity Sensor",
         "label": "TFS 700087",
         "manufacturer": "Eurotronic"
     },
+    "0x0148:0x0004:0x0003": {
+        "description": "Radiator Thermostat",
+        "label": "Comet Z",
+        "manufacturer": "Eurotronics"
+    },
     "0x0148:0x0005:0x0001": {
         "description": "Air Quality Sensor",
         "label": "EUR_AIRQUALITY",
         "manufacturer": "EUROtronic"
     },
     "0x0148:0x4672:0xbd41": {
         "description": "Thermostatic Valve",
-        "label": "COMET Z",
+        "label": "Comet Z",
         "manufacturer": "Eurotronics"
     },
     "0x0149:0x0004:0x0009": {
         "description": "Energy Driven Switch",
         "label": "C7",
         "manufacturer": "wiDom"
     },
@@ -8236,15 +8371,15 @@
     },
     "0x0149:0x1214:0x0800": {
         "description": "WiDom Smart Roller Shutter",
         "label": "UMS2",
         "manufacturer": "wiDom"
     },
     "0x0149:0x1214:0x0900": {
-        "description": "Widom Smart Dry contact",
+        "description": "Widom Smart Dry Contact",
         "label": "DRY",
         "manufacturer": "wiDom"
     },
     "0x0149:0x1214:0x0a00": {
         "description": "Widom Smart Dimmer",
         "label": "WTE",
         "manufacturer": "wiDom"
@@ -8281,15 +8416,15 @@
     },
     "0x014a:0x0004:0x0002": {
         "description": "Z-Wave Door/Window Sensor",
         "label": "DWZWAVE25",
         "manufacturer": "Ecolink"
     },
     "0x014a:0x0004:0x0003": {
-        "description": "Z-wave Plus Gold Plated Reliability Garage Door Tilt Sensor",
+        "description": "Z-Wave Plus Gold Plated Reliability Garage Door Tilt Sensor",
         "label": "TILT-ZWAVE2.5-ECO",
         "manufacturer": "Ecolink"
     },
     "0x014a:0x0005:0x000a": {
         "description": "Ecolink Z-Wave Plus Wireless Siren",
         "label": "SC-ZWAVE5",
         "manufacturer": "Ecolink"
@@ -8441,15 +8576,15 @@
     },
     "0x014f:0x4153:0x3031": {
         "description": "ADT Security Hub",
         "label": "Security Hub",
         "manufacturer": "ADT"
     },
     "0x014f:0x4450:0x3030": {
-        "description": "Plug-in Wall Dimmer",
+        "description": "Plug-In Wall Dimmer",
         "label": "PD300Z-2",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x4457:0x3034": {
         "description": "Wall Dimmer Switch",
         "label": "WD500Z-1",
         "manufacturer": "Nortek Security & Control LLC"
@@ -8496,15 +8631,15 @@
     },
     "0x014f:0x5044:0x3533": {
         "description": "300 Watt, Plug-In Dimmer Series 500",
         "label": "PD300EMZ5-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5053:0x3531": {
-        "description": "Plug-in Appliance Module",
+        "description": "Plug-In Appliance Module",
         "label": "PS15EMZ5-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5246:0x3133": {
         "description": "Isolated Contact Fixture Module",
         "label": "FS20Z",
         "manufacturer": "Nortek Security & Control LLC"
@@ -8516,15 +8651,15 @@
     },
     "0x014f:0x5252:0x3530": {
         "description": "In-Wall Single Outlet",
         "label": "WO15Z",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5257:0x3533": {
-        "description": "In-wall Switch",
+        "description": "In-Wall Switch",
         "label": "WS15Z-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5343:0x3132": {
         "description": "Wall Mounted Switch",
         "label": "WA00Z-1",
         "manufacturer": "Nortek Security & Control LLC"
@@ -8551,30 +8686,30 @@
     },
     "0x014f:0x5457:0x3033": {
         "description": "3-Way Wall Accessory Switch",
         "label": "WT00Z-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5744:0x3530": {
-        "description": "An in-wall lighting dimmer",
+        "description": "An In-Wall Lighting Dimmer",
         "label": "WD500Z5-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5749:0x3135": {
         "description": "Sprinkler Controller Supporting Flow Sensors, Rain Sensors and Moisture Sensors",
         "label": "GoControl Smart Irrigation Controller",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x574f:0x3535": {
         "description": "In-Wall Single Outlet",
         "label": "WO15EMZ5",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5753:0x3535": {
-        "description": "In-wall Switch",
+        "description": "In-Wall Switch",
         "label": "WS15Z-1",
         "manufacturer": "Nortek Security & Control LLC"
     },
     "0x014f:0x5754:0x3530": {
         "description": "3-Way Wall Accessory Switch",
         "label": "WT00Z5-1",
         "manufacturer": "Linear (Nortek Security Control LLC)"
@@ -8616,15 +8751,15 @@
     },
     "0x0150:0x000a:0x002b": {
         "description": "SmartThings Link",
         "label": "SmartThings Link",
         "manufacturer": "SmartThings, Inc."
     },
     "0x0151:0x0001:0x0001": {
-        "description": "Energy switch",
+        "description": "Energy Switch",
         "label": "SW-ESW02",
         "manufacturer": "Sercomm Corp"
     },
     "0x0151:0x0002:0x0001": {
         "description": "Clamp Power Meter",
         "label": "SW-CLP01",
         "manufacturer": "Sercomm Corp"
@@ -8666,60 +8801,60 @@
     },
     "0x0152:0x0500:0x0000": {
         "description": "Water Leak Sensor Alarm",
         "label": "Topvico TP-819ZW",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0500:0x0001": {
-        "description": "Door/Window detector",
+        "description": "Door/Window Detector",
         "label": "GR-309N",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0500:0x0002": {
         "description": "Smoke + Carbon Monoxide + Natural Liquefied Gas Leak Detector",
         "label": "TP-807ZG",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0500:0x0003": {
         "description": "Z\u2011Wave Plus Motion Sensor",
         "label": "ZSE02",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0500:0x0004": {
-        "description": "Inwall dual switch",
+        "description": "Inwall Dual Switch",
         "label": "GR-M-202N-2",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0500:0x0005": {
-        "description": "3 Gang In-wall Switch",
+        "description": "3 Gang In-Wall Switch",
         "label": "GR-B3-3",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0505:0x0001": {
         "description": "Water Leak Sensor Alarm",
         "label": "Topvico TP-819ZW",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0152:0x0a00:0x0004": {
-        "description": "3 Gang In-wall Switch",
+        "description": "3 Gang In-Wall Switch",
         "label": "GR-B3-3",
         "manufacturer": "UFairy G.R. Tech"
     },
     "0x0154:0x0001:0x0001": {
         "description": "Wall Plug Meter Switch",
         "label": "123665",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0003:0x0001": {
         "description": "Indoor/Outdoor Wall Plug Switch",
         "label": "05438",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0003:0x000a": {
-        "description": "Popp Smart Outdoor Plug - IP44 rated",
+        "description": "Popp Smart Outdoor Plug - IP44 Rated",
         "label": "POPE700397",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0003:0x0512": {
         "description": "Flow Stop",
         "label": "POPE009501",
         "manufacturer": "Popp & Co"
@@ -8751,40 +8886,40 @@
     },
     "0x0154:0x0004:0x0008": {
         "description": "Water Leakage Sensor",
         "label": "POPE700052",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0004:0x000d": {
-        "description": "10-Years Smoke Detector Without Siren",
+        "description": "10-Years Smoke Detector without Siren",
         "label": "POPE700342",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0004:0x0010": {
-        "description": "10-Years Smoke Detector Without Siren",
+        "description": "10-Years Smoke Detector without Siren",
         "label": "POPE700342",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0004:0x0011": {
         "description": "POPP Rain-Sensor",
         "label": "POPE700168",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0004:0x0014": {
-        "description": "Popp Mold detector",
+        "description": "Popp Mold Detector",
         "label": "POPE701202",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0005:0x0001": {
         "description": "Electric Strike Lock Control",
         "label": "012501",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0005:0x0002": {
-        "description": "Battery driven IP44 keypad for access control.",
+        "description": "Battery Driven IP44 Keypad for Access Control.",
         "label": "700045",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0005:0x0003": {
         "description": "Flow Stop 2",
         "label": "POPE701479",
         "manufacturer": "Popp & Co"
@@ -8806,15 +8941,15 @@
     },
     "0x0154:0x0100:0x0400": {
         "description": "Z-Weather",
         "label": "005206",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0202:0x0511": {
-        "description": "Plug-in Switch",
+        "description": "Plug-In Switch",
         "label": "123610 68G",
         "manufacturer": "Popp & Co"
     },
     "0x0154:0x0202:0x0611": {
         "description": "Dimmer",
         "label": "123580 67G",
         "manufacturer": "Popp & Co"
@@ -8846,35 +8981,35 @@
     },
     "0x0156:0x5448:0x0001": {
         "description": "Element Thermostat V2",
         "label": "EV2",
         "manufacturer": "Vivint"
     },
     "0x0157:0x0003:0x0002": {
-        "description": "Z-Wave Motor for water/gas ball valves",
+        "description": "Z-Wave Motor for Water/gas Ball Valves",
         "label": "EVC200",
         "manufacturer": "EcoNet Controls"
     },
     "0x0157:0x0003:0x0512": {
         "description": "Wireless Water Shutoff Valve",
         "label": "EBV105",
         "manufacturer": "EcoNet Controls"
     },
     "0x0157:0x0005:0x0003": {
         "description": "Water Shutoff Valve",
         "label": "GR-105",
         "manufacturer": "EcoNet Controls"
     },
     "0x0157:0x0100:0x0100": {
-        "description": "Z-Vent ZWave Controlled HVAC Air Register",
+        "description": "Z-Vent Z-Wave Controlled HVAC Air Register",
         "label": "EV100",
         "manufacturer": "EcoNet Controls"
     },
     "0x0159:0x0001:0x0001": {
-        "description": "Flush dimmer",
+        "description": "Flush Dimmer",
         "label": "ZMNHDA",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0001:0x0051": {
         "description": "Flush Dimmer Plus",
         "label": "ZMNHDD",
         "manufacturer": "Qubino"
@@ -8896,35 +9031,35 @@
     },
     "0x0159:0x0001:0x0055": {
         "description": "Mini Dimmer",
         "label": "ZMNHHD",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0001": {
-        "description": "Flush 2 relays",
+        "description": "Flush 2 Relays",
         "label": "ZMNHBA",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0002": {
-        "description": "Flush 1 relay",
+        "description": "Flush 1 Relay",
         "label": "ZMNHAA",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0051": {
         "description": "Flush 2 Relay",
         "label": "ZMNHBD",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0052": {
-        "description": "Flush 1 relay",
+        "description": "Flush 1 Relay",
         "label": "ZMNHAD",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0053": {
-        "description": "Flush 1D relay",
+        "description": "Flush 1D Relay",
         "label": "ZMNHND",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0002:0x0054": {
         "description": "Smart Plug",
         "label": "Smart Plug 16A",
         "manufacturer": "Qubino"
@@ -8951,30 +9086,30 @@
     },
     "0x0159:0x0004:0x0051": {
         "description": "Flush Pilot",
         "label": "ZMNHJD",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0004:0x0052": {
-        "description": "Flush pilot (DIN version)",
+        "description": "Flush Pilot (DIN Version)",
         "label": "ZMNHUD",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0005:0x0001": {
-        "description": "Flush on/off thermostat",
+        "description": "Flush On/off Thermostat",
         "label": "ZMNHIA",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0005:0x0003": {
-        "description": "Flush PWM thermostat",
+        "description": "Flush PWM Thermostat",
         "label": "ZMNHLA",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0005:0x0051": {
-        "description": "Flush on/off thermostat",
+        "description": "Flush On/off Thermostat",
         "label": "ZMNHID",
         "manufacturer": "Qubino"
     },
     "0x0159:0x0005:0x0052": {
         "description": "Flush Heat & Cool Thermostat",
         "label": "ZMNHKD",
         "manufacturer": "Qubino"
@@ -9016,18 +9151,23 @@
     },
     "0x0159:0x0008:0x0052": {
         "description": "Luxy Smart Switch",
         "label": "ZMNKAD1",
         "manufacturer": "Qubino"
     },
     "0x015a:0x1007:0x0002": {
-        "description": "Curtain motor",
+        "description": "Curtain Motor",
         "label": "Curtain Motor",
         "manufacturer": "Jin Tao Bao"
     },
+    "0x015a:0x2000:0x0003": {
+        "description": "Shades Remote Controller",
+        "label": "JTB-ZMNKGD1",
+        "manufacturer": "Jin Tao Bao"
+    },
     "0x015a:0x3005:0x0003": {
         "description": "Thermostat Control Panel",
         "label": "JTB-3005-03",
         "manufacturer": "Jin Tao Bao"
     },
     "0x015a:0x3011:0x0003": {
         "description": "3CH Touch Wall Switch",
@@ -9076,55 +9216,55 @@
     },
     "0x015d:0x0115:0x201c": {
         "description": "Smart Outlet",
         "label": "ZW32",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0115:0x4e1c": {
-        "description": "In-line, in-wall 110v Z-Wave power switch",
+        "description": "In-Line, In-Wall 110V Z-Wave Power Switch",
         "label": "ZW78S",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0211:0x241c": {
         "description": "Smart Plug(1 Channel)",
         "label": "ZW36",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0211:0x242c": {
         "description": "In-Wall Smart Switch",
         "label": "ZW661",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0211:0x601c": {
-        "description": "Outdoor Smart Plug - 1 channel",
+        "description": "Outdoor Smart Plug - 1 Channel",
         "label": "ZW96",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0212:0x271c": {
         "description": "Smart Plug Dimmer",
         "label": "ZW39",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0212:0x272c": {
         "description": "In-Wall Smart Dimmer",
         "label": "ZW671",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0221:0x251c": {
-        "description": "Inovelli 2 channel smart plug",
+        "description": "Inovelli 2 Channel Smart Plug",
         "label": "ZW37",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0221:0x611c": {
-        "description": "Outdoor Smart Plug - 2 channel",
+        "description": "Outdoor Smart Plug - 2 Channel",
         "label": "ZW97",
         "manufacturer": "show home"
     },
     "0x015d:0x0226:0x621c": {
-        "description": "Smart Plug(Built-in Energy Meter)",
+        "description": "Smart Plug with Built-In Energy Meter",
         "label": "ZW98",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x0621:0xf21c": {
         "description": "2 Outlet Power Strip",
         "label": "ZW1502",
         "manufacturer": "Willis Electric Co., Ltd."
@@ -9136,20 +9276,20 @@
     },
     "0x015d:0x0651:0xf51c": {
         "description": "Smart Energy Power Strip",
         "label": "ZEN20",
         "manufacturer": "Zooz"
     },
     "0x015d:0x1111:0x1e1c": {
-        "description": "Wall mounted switch",
+        "description": "Wall Mounted Switch",
         "label": "ZEN23",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x1215:0x261c": {
-        "description": "Smart Plug(built-in energy meter)",
+        "description": "Smart Plug with Built-In Energy Meter",
         "label": "ZW38",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x1215:0x262c": {
         "description": "Show Home, In-Wall-Smart-Outlet BSI",
         "label": "ZW691",
         "manufacturer": "Willis Electric Co., Ltd."
@@ -9166,23 +9306,28 @@
     },
     "0x015d:0x1e02:0x1e02": {
         "description": "Inovelli In-Wall Switch (On/Off) Scene Enabled",
         "label": "NZW30T",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x1f00:0x1f00": {
-        "description": "In-wall Dimming Switch",
+        "description": "In-Wall Dimming Switch",
         "label": "NZW31",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x1f01:0x1f01": {
-        "description": "In-wall Dimming Switch",
+        "description": "In-Wall Dimming Switch",
         "label": "NZW31",
         "manufacturer": "Willis Electric Co., Ltd."
     },
+    "0x015d:0x1f02:0x1f02": {
+        "description": "In-Wall Smart Dimmer",
+        "label": "NZW31T",
+        "manufacturer": "Inovelli"
+    },
     "0x015d:0x2003:0x701c": {
         "description": "Motion Sensor",
         "label": "ZW112",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x2003:0xb11c": {
         "description": "Door Window Sensor",
@@ -9226,15 +9371,15 @@
     },
     "0x015d:0x4000:0x0f1c": {
         "description": "Siren Box",
         "label": "ZW15",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x6000:0x6000": {
-        "description": "Outdoor Plug-in Module (1-Channel)",
+        "description": "Outdoor Plug-In Module (1-Channel)",
         "label": "NZW96",
         "manufacturer": "Willis Electric Co., Ltd."
     },
     "0x015d:0x6100:0x6100": {
         "description": "Inovelli Outdoor Smart Plug (2 Channel)",
         "label": "NZW97",
         "manufacturer": "Willis Electric Co., Ltd."
@@ -9302,35 +9447,40 @@
     "0x015f:0x0732:0x5102": {
         "description": "Water / Electrical Heating Thermostat",
         "label": "MH7H",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0801:0x3102": {
         "description": "Fan Coil Thermostat",
-        "label": "MH8-FC",
+        "label": "MH8-FC / MH8-FC4",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0801:0x5102": {
         "description": "Fan Coil Thermostat",
-        "label": "MH8-FC",
+        "label": "MH8-FC / MH8-FC4",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0802:0x3102": {
         "description": "Fan Coil Thermostat",
-        "label": "MH8-FC",
+        "label": "MH8-FC / MH8-FC4",
+        "manufacturer": "McoHome Technology Co., Ltd."
+    },
+    "0x015f:0x0802:0x5101": {
+        "description": "Fan Coil Thermostat",
+        "label": "MH8-FC / MH8-FC4",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0802:0x5102": {
         "description": "Fan Coil Thermostat",
-        "label": "MH8-FC",
+        "label": "MH8-FC / MH8-FC4",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0803:0x5102": {
         "description": "Fan Coil Thermostat",
-        "label": "MH8-FC",
+        "label": "MH8-FC / MH8-FC4",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x0901:0x3102": {
         "description": "CO2 Monitor Air Quality Detector",
         "label": "MH9-CO2",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
@@ -9371,20 +9521,20 @@
     },
     "0x015f:0x0a05:0x0201": {
         "description": "PM2.5 Monitor",
         "label": "MH10-PM2.5-WA",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x2121:0x1352": {
-        "description": "Mini Combo Switch Two-load",
+        "description": "Mini Combo Switch Two-Load",
         "label": "MH-S212",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x2121:0x1353": {
-        "description": "Mini Combo Switch Two-load",
+        "description": "Mini Combo Switch Two-Load",
         "label": "MH-S212",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x2201:0x1252": {
         "description": "Micro Switch",
         "label": "MH-S220",
         "manufacturer": "McoHome Technology Co., Ltd."
@@ -9421,23 +9571,28 @@
     },
     "0x015f:0x3102:0x0204": {
         "description": "Touch Panel Switch 4 Button",
         "label": "MH-S314",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x3111:0x1302": {
-        "description": "Touch Panel Switch (Single) High inrush current",
+        "description": "Touch Panel Switch (Single) High Inrush Current",
         "label": "MH-S311H",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x3111:0x5102": {
-        "description": "Touch Panel Switch (Single) High inrush current",
+        "description": "Touch Panel Switch (Single) High Inrush Current",
         "label": "MH-S311H",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
+    "0x015f:0x3112:0x7102": {
+        "description": "Touch Panel Switch 1 Button",
+        "label": "MH-S411",
+        "manufacturer": "McoHome Technology Co., Ltd."
+    },
     "0x015f:0x3121:0x1302": {
         "description": "Two Way Switch",
         "label": "MH-S312",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x3121:0x5102": {
         "description": "Two Way Switch",
@@ -9445,14 +9600,19 @@
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x3122:0x5102": {
         "description": "Two Way Switch",
         "label": "MH-S312",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
+    "0x015f:0x3122:0x7102": {
+        "description": "Touch Panel Switch 2 Button",
+        "label": "MH-S412",
+        "manufacturer": "McoHome Technology Co., Ltd."
+    },
     "0x015f:0x3141:0x1302": {
         "description": "Touch Panel Switch 4 Button",
         "label": "MH-S314",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x3141:0x5102": {
         "description": "Touch Panel Switch 4 Button",
@@ -9520,14 +9680,19 @@
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0x5131:0x5103": {
         "description": "Touch Panel Switch 3-Way",
         "label": "MH-S513",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
+    "0x015f:0xa803:0x1351": {
+        "description": "9 in 1 MULTI-SENSOR",
+        "label": "A8-9",
+        "manufacturer": "McoHome Technology Co., Ltd."
+    },
     "0x015f:0xa803:0x1352": {
         "description": "9 in 1 MULTI-SENSOR",
         "label": "A8-9",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0xa803:0x135a": {
         "description": "9 in 1 MULTI-SENSOR",
@@ -9537,26 +9702,31 @@
     "0x015f:0xc221:0x5102": {
         "description": "MCO HOME Micro Shutter",
         "label": "MH-C221",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0xc321:0x5102": {
         "description": "Shutter Panel",
-        "label": "MH-S521",
+        "label": "MH-C321",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0xc421:0x5102": {
-        "description": "MCO HOME Micro Shutter",
+        "description": "Shutter Panel",
         "label": "MH-C421",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
-    "0x015f:0xc521:0x5101": {
+    "0x015f:0xc521:0x5106": {
         "description": "Shutter Panel",
-        "label": "MH-S521",
-        "manufacturer": "McoHome Technology Co., Ltd."
+        "label": "MH-C521",
+        "manufacturer": "McoHome Co., Ltd."
+    },
+    "0x015f:0xc621:0x5106": {
+        "description": "Shutter Panel",
+        "label": "MH-C621",
+        "manufacturer": "McoHome Co., Ltd."
     },
     "0x015f:0xd221:0x7102": {
         "description": "Micro Switch",
         "label": "MH-DS221",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x015f:0xd311:0x5102": {
@@ -9576,20 +9746,20 @@
     },
     "0x015f:0xf501:0x7102": {
         "description": "Fan Coil Thermostat",
         "label": "MH5-2A",
         "manufacturer": "McoHome Technology Co., Ltd."
     },
     "0x0160:0x0001:0x0001": {
-        "description": "Z-Wave extender",
+        "description": "Z-Wave Extender",
         "label": "ES800ZWP_EU_MXX",
         "manufacturer": "Essence Security"
     },
     "0x0162:0x0001:0x03e9": {
-        "description": "AV Scenario Controller with universal IR",
+        "description": "AV Scenario Controller with Universal IR",
         "label": "HSK-100Z",
         "manufacturer": "HomeScenario"
     },
     "0x0163:0x3001:0x0301": {
         "description": "Queenlock Z-Wave Deadbolt Lock",
         "label": "ZW-702",
         "manufacturer": "Queenlock Ind. Co., Ltd."
@@ -9616,15 +9786,15 @@
     },
     "0x0165:0x0002:0x0003": {
         "description": "Wall Switch",
         "label": "CWS-3101",
         "manufacturer": "ID-RF"
     },
     "0x0166:0x0002:0x0001": {
-        "description": "RemSwiid Z-Wave remote controller",
+        "description": "RemSwiid Z-Wave Remote Controller",
         "label": "SW-ZRC",
         "manufacturer": "CBCC Domotique SAS"
     },
     "0x0166:0x0002:0x0004": {
         "description": "ZURC Remote Control",
         "label": "SW-ZRC2",
         "manufacturer": "CBCC Domotique SAS"
@@ -9676,20 +9846,20 @@
     },
     "0x016a:0x0002:0x0070": {
         "description": "Door/Window Sensor 6",
         "label": "FT112",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0002:0x0082": {
-        "description": "Wall-mount four Button",
+        "description": "Wall-Mount Four Button",
         "label": "FT130",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0003:0x0060": {
-        "description": "Plug-in Switch",
+        "description": "Plug-In Switch",
         "label": "FT096",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0003:0x0062": {
         "description": "9W Color Light Bulb",
         "label": "FT098",
         "manufacturer": "Fantem"
@@ -9731,15 +9901,15 @@
     },
     "0x016a:0x0102:0x0066": {
         "description": "Oomi Touch",
         "label": "FT102",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0103:0x0060": {
-        "description": "Plug-in Switch",
+        "description": "Plug-In Switch",
         "label": "FT096",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0103:0x0079": {
         "description": "LED RGBWW Strip",
         "label": "FT121",
         "manufacturer": "Fantem"
@@ -9761,15 +9931,15 @@
     },
     "0x016a:0x0202:0x0070": {
         "description": "Door/Window Sensor 6",
         "label": "FT112",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0203:0x0060": {
-        "description": "Plug-in Switch",
+        "description": "Plug-In Switch",
         "label": "FT096",
         "manufacturer": "Fantem"
     },
     "0x016a:0x0203:0x006f": {
         "description": "Nano Dimmer",
         "label": "FT111",
         "manufacturer": "Fantem"
@@ -9816,15 +9986,15 @@
     },
     "0x0170:0x0000:0x0000": {
         "description": "SiteSage",
         "label": "950-000012",
         "manufacturer": "Powerhouse Dynamics"
     },
     "0x0171:0x0001:0x0002": {
-        "description": "WeBeHome gateway",
+        "description": "WeBeHome Gateway",
         "label": "HG2",
         "manufacturer": "WeBeHome AB"
     },
     "0x0171:0x0001:0x0003": {
         "description": "Home Gateway 2 Plus",
         "label": "WBH-HG2+",
         "manufacturer": "WeBeHome AB"
@@ -9846,20 +10016,20 @@
     },
     "0x0173:0x4c47:0x4c44": {
         "description": "Leak Gopher Z-Wave Leak Detector",
         "label": "LGZWL",
         "manufacturer": "Leak Intelligence, LLC"
     },
     "0x0175:0x0000:0x0001": {
-        "description": "devolo Home Control Central Unit",
+        "description": "Devolo Home Control Central Unit",
         "label": "MT2600 / MT2601",
         "manufacturer": "Devolo"
     },
     "0x0175:0x0001:0x0001": {
-        "description": "Smart Energy Plug-in Switch",
+        "description": "Smart Energy Plug-In Switch",
         "label": "PAN11",
         "manufacturer": "Devolo"
     },
     "0x0175:0x0001:0x0011": {
         "description": "Home Control Metering Plug",
         "label": "MT02646",
         "manufacturer": "Devolo"
@@ -9951,20 +10121,20 @@
     },
     "0x0176:0x0003:0x0002": {
         "description": "Wall Plug Switch",
         "label": "TZWP-100",
         "manufacturer": "Telldus Technologies AB"
     },
     "0x0176:0x0003:0x0003": {
-        "description": "Telldus socket and energy meter",
+        "description": "Socket and Energy Meter",
         "label": "TZWP-102",
         "manufacturer": "Telldus Technologies AB"
     },
     "0x0176:0x0005:0x0001": {
-        "description": "Door/window sensor",
+        "description": "Door/window Sensor",
         "label": "TZDW-100",
         "manufacturer": "Telldus Technologies AB"
     },
     "0x0178:0x4252:0x3230": {
         "description": "Nexia Bridge",
         "label": "BR200NX",
         "manufacturer": "Nexia Home Intelligence"
@@ -9996,30 +10166,30 @@
     },
     "0x0179:0x0013:0x0021": {
         "description": "CH-201 Thermostat",
         "label": "CH-201",
         "manufacturer": "ConnectHome"
     },
     "0x0179:0x0021:0x0011": {
-        "description": "CH-601 THE ELECTRIC CRANE",
+        "description": "CH-601 the ELECTRIC CRANE",
         "label": "CH-601",
         "manufacturer": "ConnectHome"
     },
     "0x0179:0x0041:0x0014": {
         "description": "CH-103 Relay",
         "label": "CH-103",
         "manufacturer": "ConnectHome"
     },
     "0x017c:0x0001:0x000a": {
-        "description": "heatapp! repeater S2",
+        "description": "heatapp! Repeater S2",
         "label": "9601921000",
         "manufacturer": "EbV"
     },
     "0x017c:0x0006:0x0003": {
-        "description": "heatapp! floor is a controller for thermal actuators in underfloor heating installations and is part of the heatapp! system, providing individual circ",
+        "description": "8-Channel Underfloor Heating Controller",
         "label": "heatapp! floor",
         "manufacturer": "EbV"
     },
     "0x017e:0x0001:0x0002": {
         "description": "FlexHub",
         "label": "TGFX-HUB1",
         "manufacturer": "Telular"
@@ -10051,15 +10221,15 @@
     },
     "0x0183:0x0201:0x0701": {
         "description": "Universe Future Gateway",
         "label": "ZWG2000AG",
         "manufacturer": "Universe Future"
     },
     "0x0184:0x4447:0x3031": {
-        "description": "Plug-in On/Off Switch",
+        "description": "Plug-In On/Off Switch",
         "label": "PA-100",
         "manufacturer": "Dragon Tech Industrial, Ltd."
     },
     "0x0184:0x4447:0x3033": {
         "description": "Wall On/Off Switch",
         "label": "WS-100",
         "manufacturer": "Dragon Tech Industrial, Ltd."
@@ -10076,15 +10246,15 @@
     },
     "0x0184:0x4754:0x3038": {
         "description": "HomeSeer Smart Bulb",
         "label": "HS-DTA19+",
         "manufacturer": "Dragon Tech Industrial, Ltd."
     },
     "0x0185:0x0003:0x0009": {
-        "description": "PIR motion sensor",
+        "description": "PIR Motion Sensor",
         "label": "ZM-800",
         "manufacturer": "Ningbo Sentek Electronics Co., Ltd."
     },
     "0x0189:0x0104:0x0301": {
         "description": "Z-Wave LUX PIR Sensor",
         "label": "117001",
         "manufacturer": "Ness Corporation Pty Ltd."
@@ -10125,19 +10295,69 @@
         "manufacturer": "Grib"
     },
     "0x018b:0x0040:0x0100": {
         "description": "Smart Gas Controller",
         "label": "GCR-01S",
         "manufacturer": "Grib"
     },
+    "0x018c:0x0042:0x0005": {
+        "description": "Smart Plug with Power Meter",
+        "label": "PM-B400ZW-N",
+        "manufacturer": "Dawon DNS"
+    },
+    "0x018c:0x0042:0x0006": {
+        "description": "Smart Plug with Power Meter",
+        "label": "PM-B400ZW-N",
+        "manufacturer": "Dawon DNS"
+    },
+    "0x018c:0x0057:0x0001": {
+        "description": "1-Button Smart Switch",
+        "label": "SSD-105",
+        "manufacturer": "LG U+"
+    },
+    "0x018c:0x0058:0x0001": {
+        "description": "2-Button Smart Switch",
+        "label": "SSD-205",
+        "manufacturer": "LG U+"
+    },
+    "0x018c:0x0059:0x0001": {
+        "description": "3-Button Smart Switch",
+        "label": "SSD-305",
+        "manufacturer": "LG U+"
+    },
+    "0x018c:0x0061:0x0001": {
+        "description": "1-Channel Power Switch",
+        "label": "PM-140-ZW",
+        "manufacturer": "Dawon"
+    },
+    "0x018c:0x0062:0x0001": {
+        "description": "2-Channel Power Switch",
+        "label": "PM-S240-ZW",
+        "manufacturer": "Dawon"
+    },
+    "0x018c:0x0063:0x0001": {
+        "description": "3-Button Wall Switch",
+        "label": "PM-S340-ZW",
+        "manufacturer": "Dawon"
+    },
+    "0x018c:0x0064:0x0001": {
+        "description": "1-Channel Power Switch",
+        "label": "PM-140-ZW",
+        "manufacturer": "Dawon"
+    },
     "0x018c:0x0065:0x0001": {
         "description": "2-Channel Power Switch",
         "label": "PM-S240-ZW",
         "manufacturer": "Dawon"
     },
+    "0x018c:0x0066:0x0001": {
+        "description": "3-Button Wall Switch",
+        "label": "PM-S340-ZW",
+        "manufacturer": "Dawon"
+    },
     "0x018e:0x0001:0x0001": {
         "description": "Door Contact",
         "label": "DC-15ZW",
         "manufacturer": "Climax Technology, Ltd."
     },
     "0x018e:0x0001:0x0002": {
         "description": "Z-Wave Motion Sensor",
@@ -10280,14 +10500,19 @@
         "manufacturer": "Building 36 Technologies"
     },
     "0x0190:0x0006:0x0001": {
         "description": "Alarm.com Smart Thermostat",
         "label": "ADC-T 3000",
         "manufacturer": "Building 36 Technologies"
     },
+    "0x0190:0x0007:0x0001": {
+        "description": "Smart Water Valve & Meter",
+        "label": "ADC-SWM150",
+        "manufacturer": "Building 36 Technologies"
+    },
     "0x0193:0x0001:0x0001": {
         "description": "Universal Devices ISY-994i ZW",
         "label": "ISY-994ZW",
         "manufacturer": "Universal Devices, Inc"
     },
     "0x0193:0x0001:0x0002": {
         "description": "Universal Devices ISY-994i ZW",
@@ -10326,15 +10551,15 @@
     },
     "0x0195:0x0001:0x0001": {
         "description": "MyAlert",
         "label": "MYALERT001",
         "manufacturer": "M2M Solution"
     },
     "0x0196:0x00b7:0x0097": {
-        "description": "Touch screen wall switch",
+        "description": "Touch Screen Wall Switch",
         "label": "BrightSwitch",
         "manufacturer": "Bellatrix Systems, Inc."
     },
     "0x0198:0x0003:0x0001": {
         "description": "Voyager",
         "label": "T3700 / T3800 / T3900 / T4700 / T4800 / T4900",
         "manufacturer": "Venstar Inc."
@@ -10366,15 +10591,15 @@
     },
     "0x019a:0x0004:0x000c": {
         "description": "Strips Comfort 700",
         "label": "11 02 022",
         "manufacturer": "Sensative AB"
     },
     "0x019b:0x0001:0x0001": {
-        "description": "ZWave Thermostat",
+        "description": "Z-Wave Thermostat",
         "label": "TF016 / TF021",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0002:0x2201": {
         "description": "Heatit Z-Dim2",
         "label": "Z-DIM2",
         "manufacturer": "Heatit"
@@ -10391,35 +10616,35 @@
     },
     "0x019b:0x0003:0x0018": {
         "description": "Wireless Smoke Detector",
         "label": "Z-Smoke Battery",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x0201": {
-        "description": "ZWave Thermostat",
+        "description": "Z-Wave Thermostat",
         "label": "TF016 / TF021",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x0202": {
         "description": "Floor Thermostat",
         "label": "Z-TRM 2",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x0203": {
-        "description": "Floor thermostat",
+        "description": "Floor Thermostat",
         "label": "Z-TRM3",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x0208": {
-        "description": "Multipurpose relay",
+        "description": "Multipurpose Relay",
         "label": "Z-RELAY",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x020a": {
-        "description": "Relay control",
+        "description": "Relay Control",
         "label": "Z Water",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0003:0x2200": {
         "description": "Knob Smart Dimmer",
         "label": "Z-Dim",
         "manufacturer": "Heatit"
@@ -10436,38 +10661,63 @@
     },
     "0x019b:0x0003:0x3602": {
         "description": "Wireless Smoke Detector",
         "label": "Z-Smoke Battery",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0004:0x0204": {
-        "description": "Battery operated thermostat",
+        "description": "Battery Operated Thermostat",
         "label": "Z-Temp2",
         "manufacturer": "Heatit"
     },
+    "0x019b:0x0004:0x020b": {
+        "description": "Relay Controller",
+        "label": "Z-WATER2",
+        "manufacturer": "Heatit"
+    },
     "0x019b:0x0004:0x2201": {
         "description": "Heatit Z-Dim2",
         "label": "Z-DIM2",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0004:0x2403": {
         "description": "Z-Push Wall Controller",
         "label": "Z-PH WALL CONTROLLER",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0004:0x3500": {
-        "description": "High power relay",
+        "description": "High Power Relay",
         "label": "ZM Single Relay 16A",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0004:0x3502": {
         "description": "Floor Thermostat",
         "label": "ZM THERMOSTAT 16A",
         "manufacturer": "Heatit"
     },
+    "0x019b:0x0021:0x2101": {
+        "description": "Heatit ZM Dimmer",
+        "label": "ZM DIMMER",
+        "manufacturer": "Heatit"
+    },
+    "0x019b:0x0030:0x3001": {
+        "description": "Floor Thermostat",
+        "label": "Z-TRM6",
+        "manufacturer": "Heatit"
+    },
+    "0x019b:0x0062:0x6201": {
+        "description": "Heatit Z-HAN2",
+        "label": "Z-HAN2",
+        "manufacturer": "Heatit"
+    },
+    "0x019b:0x0101:0x000a": {
+        "description": "Leakage Stopper",
+        "label": "BVS-ZWU",
+        "manufacturer": "Heatit"
+    },
     "0x019b:0x0300:0xa305": {
         "description": "Wall Mounted Switch",
         "label": "Z Push Button 8",
         "manufacturer": "Heatit"
     },
     "0x019b:0x0300:0xa306": {
         "description": "Wall Mounted Switch",
@@ -10496,15 +10746,15 @@
     },
     "0x019d:0x0003:0x0010": {
         "description": "Mobilus Tubular Motor",
         "label": "EZRS",
         "manufacturer": "MOBILUS MOTOR Sp\u00f3\u0142ka z o.o."
     },
     "0x019e:0x0001:0x0001": {
-        "description": "Multiradio server for home automation with optional cloud connectivitiy",
+        "description": "Multiradio Server for Home Automation with Optional Cloud Connectivitiy",
         "label": "Wibutler Pro",
         "manufacturer": "iEXERGY GmbH"
     },
     "0x019f:0x0001:0x0001": {
         "description": "Smartee",
         "label": "SM2001",
         "manufacturer": "Webee Life"
@@ -10621,20 +10871,20 @@
     },
     "0x0202:0x2008:0x0803": {
         "description": "Monoprice, P/N , Plug-In Dimmer",
         "label": "11994",
         "manufacturer": "Monoprice"
     },
     "0x0207:0x0027:0x0100": {
-        "description": "Drapery hardware",
+        "description": "Drapery Hardware",
         "label": "Shuttle S/L",
         "manufacturer": "Forest Group Nederland B.V"
     },
     "0x0208:0x0003:0x0300": {
-        "description": "Siterwell eyesonsor",
+        "description": "Siterwell Eyesonsor",
         "label": "SW es01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0100:0x0004": {
         "description": "RGB Bulb",
         "label": "HKZW-RGB01",
         "manufacturer": "HANK Electronics Ltd."
@@ -10645,41 +10895,46 @@
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0100:0x000a": {
         "description": "Smart Plug",
         "label": "HKZW-SO05",
         "manufacturer": "HANK Electronics Ltd."
     },
+    "0x0208:0x0100:0x0019": {
+        "description": "Smart Plug",
+        "label": "HKZW-SO08",
+        "manufacturer": "Hank"
+    },
     "0x0208:0x0101:0x0004": {
         "description": "RGB Bulb",
         "label": "HKZW-RGB01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0101:0x0005": {
-        "description": "Smart Plug with two USB ports",
+        "description": "Smart Plug with Two USB Ports",
         "label": "HKZW-SO01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0101:0x000a": {
         "description": "Smart Plug",
         "label": "HKZW-SO03",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0200:0x0008": {
         "description": "Door and Window Sensor",
         "label": "HKZW-DWS01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0200:0x0009": {
-        "description": "One-key Scene Controller",
+        "description": "One-Key Scene Controller",
         "label": "HKZW-SCN01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0200:0x000b": {
-        "description": "Four-key Scene Controller",
+        "description": "Four-Key Scene Controller",
         "label": "SCN04",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0200:0x000f": {
         "description": "Flood Sensor",
         "label": "HKZW-FLD01",
         "manufacturer": "HANK Electronics Ltd."
@@ -10696,35 +10951,35 @@
     },
     "0x0208:0x0201:0x0008": {
         "description": "Door and Window Sensor",
         "label": "HKZW-DWS01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0201:0x0009": {
-        "description": "One-key Scene Controller",
+        "description": "One-Key Scene Controller",
         "label": "HKZW-SCN01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0201:0x000b": {
-        "description": "Four-key Scene Controller",
+        "description": "Four-Key Scene Controller",
         "label": "SCN04",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0201:0x000f": {
         "description": "Flood Sensor",
         "label": "HKZW-FLD01",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0201:0x0012": {
         "description": "Motion Sensor",
         "label": "HKZW-MS02",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0208:0x0101": {
-        "description": "Smart Plug with two USB ports",
+        "description": "Smart Plug with Two USB Ports",
         "label": "PID15654",
         "manufacturer": "HANK Electronics Ltd."
     },
     "0x0208:0x0300:0x0012": {
         "description": "Motion Sensor",
         "label": "HKZW-MS02",
         "manufacturer": "HANK Electronics Ltd."
@@ -10808,50 +11063,50 @@
         "description": "Westinghouse RTS-PZ-AU",
         "label": "9002",
         "manufacturer": "Strattec Advanced Logic, LLC"
     },
     "0x021c:0x1010:0x1008": {
         "description": "1 Gang Wall Switch",
         "label": "J1506",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x5000:0x1000": {
         "description": "Door Lock with Handle",
         "label": "DL9101V",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x5010:0x1001": {
-        "description": "Smart Door Lock",
-        "label": "ILOCK15",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "description": "Wall Reader",
+        "label": "J1825",
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd"
     },
     "0x021c:0x634b:0x504c": {
-        "description": "Smart lock",
-        "label": "iLock",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "description": "Smart Door Lock",
+        "label": "ILOCK15",
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x8000:0x1000": {
         "description": "Door Sensor",
         "label": "J1504",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x8002:0x1000": {
-        "description": "Carbon monoxide detector, smoke detector",
+        "description": "Carbon Monoxide Detector, Smoke Detector",
         "label": "Smoke Detector",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x8004:0x1000": {
         "description": "Domux Water Leakage Sensor",
         "label": "DX1WL-Z",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021c:0x8011:0x1000": {
         "description": "Motion Sensor",
         "label": "J1505",
-        "manufacturer": "Shenzhen iSurpass Technology Co. , Ltd."
+        "manufacturer": "Shenzhen iSurpass Technology Co., Ltd."
     },
     "0x021d:0x0003:0x0001": {
         "description": "Touchscreen Digital Deadbolt",
         "label": "DB2",
         "manufacturer": "Shenzhen Kaadas Intelligent Technology Co., Ltd."
     },
     "0x021d:0x0003:0x0002": {
@@ -10886,30 +11141,30 @@
     },
     "0x021f:0x0003:0x0085": {
         "description": "Dome Leak Sensor",
         "label": "DMWS1",
         "manufacturer": "Elexa Consumer Products Inc."
     },
     "0x021f:0x0003:0x0087": {
-        "description": "Dome On/Off zwave wall plug for controlling small appliances and lights.",
+        "description": "Dome On/Off Zwave Wall Plug for Controlling Small Appliances and Lights.",
         "label": "DMOF1",
         "manufacturer": "Elexa Consumer Products Inc."
     },
     "0x021f:0x0003:0x0088": {
         "description": "Dome Wireless Siren",
         "label": "DMS01",
         "manufacturer": "Elexa Consumer Products Inc."
     },
     "0x021f:0x0003:0x0101": {
-        "description": "Dome door & window sensor",
+        "description": "Dome Door & Window Sensor",
         "label": "DMWD1",
         "manufacturer": "Elexa Consumer Products Inc."
     },
     "0x021f:0x0003:0x0104": {
-        "description": "Dome Battery powered Z-Wave Plus enabled mousetrap",
+        "description": "Dome Battery Powered Z-Wave Plus Enabled Mousetrap",
         "label": "DMMZ1",
         "manufacturer": "Elexa Consumer Products Inc."
     },
     "0x021f:0x0003:0x0108": {
         "description": "Range Extender",
         "label": "DMEX1",
         "manufacturer": "Dome"
@@ -11001,15 +11256,15 @@
     },
     "0x022e:0x0004:0x0004": {
         "description": "Window/Door Sensor",
         "label": "SHP-SB100Z",
         "manufacturer": "Samsung SDS"
     },
     "0x022e:0x0005:0x0005": {
-        "description": "Motion sensor",
+        "description": "Motion Sensor",
         "label": "SHP-SR100Z",
         "manufacturer": "Samsung SDS"
     },
     "0x022e:0x0006:0x0006": {
         "description": "Gradient Sensor",
         "label": "SHP-SG100Z",
         "manufacturer": "Samsung SDS"
@@ -11036,35 +11291,40 @@
     },
     "0x0233:0x0049:0x0001": {
         "description": "U+ Switch",
         "label": "SSE-301",
         "manufacturer": "eZEX Corporation"
     },
     "0x0233:0x004c:0x0001": {
-        "description": "U+ Switch",
+        "description": "Smart Switch",
         "label": "SSE-302",
-        "manufacturer": "eZEX Corporation"
+        "manufacturer": "LG U+"
     },
     "0x0233:0x004c:0x0002": {
         "description": "U+ Switch",
         "label": "SSE-303",
-        "manufacturer": "eZEX Corporation"
+        "manufacturer": "LG U+"
+    },
+    "0x0233:0x0059:0x0001": {
+        "description": "IoT Switch",
+        "label": "SSE-304",
+        "manufacturer": "LG U+"
     },
     "0x0234:0x0002:0x010a": {
-        "description": "FUGA Wall 4-way Switch with LED + Relay",
+        "description": "FUGA Wall 4-Way Switch with LED + Relay",
         "label": "ZHC5010",
         "manufacturer": "Logic Group"
     },
     "0x0234:0x0003:0x010a": {
-        "description": "FUGA Wall 4-way Switch with LED + Relay",
+        "description": "FUGA Wall 4-Way Switch with LED + Relay",
         "label": "ZHC5010",
         "manufacturer": "Logic Group"
     },
     "0x0234:0x0003:0x010c": {
-        "description": "Push button 6-gang",
+        "description": "Push Button 6-Gang",
         "label": "Heatit Z-Scene Controller",
         "manufacturer": "Logic Group"
     },
     "0x0234:0x0003:0x010d": {
         "description": "DIN Rail Interface",
         "label": "ZIF5020",
         "manufacturer": "Logic Group"
@@ -11141,20 +11401,20 @@
     },
     "0x023b:0x0001:0x0001": {
         "description": "Multiple RF Home Gateway",
         "label": "F4-ZB-ZWE",
         "manufacturer": "ROC-Connect, Inc."
     },
     "0x023c:0x0001:0x0001": {
-        "description": "The Quickbox - Home Edition",
+        "description": "Quickbox - Home Edition",
         "label": "QBBIOZW",
         "manufacturer": "SafeTech Products"
     },
     "0x023c:0x0001:0x0002": {
-        "description": "The Doorlock",
+        "description": "Doorlock",
         "label": "QLDLZW",
         "manufacturer": "SafeTech Products"
     },
     "0x023d:0x0043:0x0001": {
         "description": "IoT DoorCam",
         "label": "DCH-01",
         "manufacturer": "Honest Technology Co., Ltd."
@@ -11201,25 +11461,25 @@
     },
     "0x0242:0x0003:0x0011": {
         "description": "WTR-1000-11",
         "label": "03110101",
         "manufacturer": "Winytechnology"
     },
     "0x0242:0x0a02:0x0061": {
-        "description": "Sensor Input device (KASAIHOUCHIKIADAPTOR01)",
+        "description": "Sensor Input Device (KASAIHOUCHIKIADAPTOR01)",
         "label": "UFA01",
         "manufacturer": "KDDI CORPORATION"
     },
     "0x0244:0xba5e:0x0001": {
         "description": "Homey",
         "label": "HOMEY",
         "manufacturer": "Athom BV"
     },
     "0x0245:0x0003:0x0001": {
-        "description": "Metering Plug switching 16A",
+        "description": "Metering Plug Switching 16A",
         "label": "PSC234ZW",
         "manufacturer": "permundo GmbH"
     },
     "0x0245:0x0003:0x0002": {
         "description": "Metering Relay Switch, 16A",
         "label": "PSC132ZW",
         "manufacturer": "permundo GmbH"
@@ -11231,20 +11491,20 @@
     },
     "0x0246:0x0001:0x0001": {
         "description": "Smart Plug",
         "label": "3210-L",
         "manufacturer": "CentraLite Systems, Inc"
     },
     "0x0248:0x0001:0x0001": {
-        "description": "coqon qbox",
+        "description": "Coqon Qbox",
         "label": "CQNGATEV1",
         "manufacturer": "neusta next GmbH & Co. KG"
     },
     "0x0248:0x0003:0x0001": {
-        "description": "Plug module",
+        "description": "Plug Module",
         "label": "PSMZ0001",
         "manufacturer": "neusta next GmbH & Co. KG"
     },
     "0x0249:0x0002:0x0001": {
         "description": "Smart Color Button",
         "label": "PSR07",
         "manufacturer": "WeBeHome"
@@ -11316,15 +11576,15 @@
     },
     "0x024f:0x0003:0x1011": {
         "description": "Standalone 1-10V Dimmer",
         "label": "AD1-10V",
         "manufacturer": "SE Devices"
     },
     "0x024f:0x0003:0x1012": {
-        "description": "Standalone Mosfet Dimmer",
+        "description": "Standalone MOSFET Dimmer",
         "label": "AM",
         "manufacturer": "SE Devices"
     },
     "0x024f:0x0003:0x1013": {
         "description": "Standalone Relay 1-Pole",
         "label": "AR1P",
         "manufacturer": "SE Devices"
@@ -11495,19 +11755,29 @@
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
     "0x0258:0x0010:0x0702": {
         "description": "Door/Window Sensor Plus",
         "label": "NEO-DS07Z",
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
+    "0x0258:0x0010:0x0716": {
+        "description": "Neo Coolcam Repeater",
+        "label": "NAS-RP01Z1",
+        "manufacturer": "Shenzhen Neo Electronics Co., Ltd"
+    },
     "0x0258:0x0010:0x0720": {
         "description": "5 in 1 PIR Motion Sensor",
         "label": "NAS-PD07Z",
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
+    "0x0258:0x0010:0x0722": {
+        "description": "Neo Coolcam Repeater",
+        "label": "NAS-WR02ZU",
+        "manufacturer": "Shenzhen Neo Electronics Co., Ltd"
+    },
     "0x0258:0x0020:0x0718": {
         "description": "5 in 1 PIR Motion Sensor",
         "label": "NAS-PD07ZU1",
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
     "0x0258:0x0020:0x0720": {
         "description": "5 in 1 PIR Motion Sensor",
@@ -11540,14 +11810,19 @@
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
     "0x0258:0x0200:0x1031": {
         "description": "PIR Motion Sensor 3",
         "label": "NAS-PD03Z",
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
+    "0x0258:0x0200:0x1036": {
+        "description": "PIR Motion, Temperature & Light Sensor",
+        "label": "NAS_PD02Z-2",
+        "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
+    },
     "0x0258:0x0300:0x1027": {
         "description": "Wall Plug Switch",
         "label": "NAS-WR01ZE",
         "manufacturer": "Shenzhen Neo Electronics Co., Ltd."
     },
     "0x0259:0x0003:0x0002": {
         "description": "P-M-O",
@@ -11651,30 +11926,30 @@
     },
     "0x0260:0x8012:0x1000": {
         "description": "Smart CO Alarm",
         "label": "HM-723ESY-Z",
         "manufacturer": "Shenzhen Heiman Technology Co., Ltd."
     },
     "0x0261:0x0101:0x0201": {
-        "description": "Wall plug smart switch",
+        "description": "Wall Plug Smart Switch",
         "label": "WP-US-2/U2/1",
         "manufacturer": "KOOL KONCEPTS"
     },
     "0x0262:0x0003:0x0001": {
         "description": "TPD Z-Wave",
         "label": "DBZF-3410",
         "manufacturer": "Taiwan Fu Hsing Industrial Co., Ltd."
     },
     "0x0262:0x0004:0x0001": {
         "description": "Electronic Z-Wave Deadbolt",
         "label": "GB05DBF",
         "manufacturer": "Taiwan Fu Hsing Industrial Co., Ltd."
     },
     "0x0265:0x0001:0x0001": {
-        "description": "Smart home camera gateway",
+        "description": "Smart Home Camera Gateway",
         "label": "IC731Z",
         "manufacturer": "StarVedia"
     },
     "0x0265:0x0001:0x0003": {
         "description": "Megapixel Z-Wave IP Camera",
         "label": "IC722Z",
         "manufacturer": "StarVedia"
@@ -11716,15 +11991,15 @@
     },
     "0x0266:0x0005:0x0001": {
         "description": "Smoke Alarm Sensor",
         "label": "GS559",
         "manufacturer": "Siterwell Technology HK Co., Ltd."
     },
     "0x0266:0x0006:0x0001": {
-        "description": "carbon monoxide alarm",
+        "description": "Carbon Monoxide Alarm",
         "label": "GS816",
         "manufacturer": "Siterwell Technology HK Co., Ltd."
     },
     "0x0266:0x0007:0x0001": {
         "description": "Heat Alarm",
         "label": "GS412",
         "manufacturer": "Siterwell Technology HK Co., Ltd."
@@ -11735,14 +12010,19 @@
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0001:0x00da": {
         "description": "Switch IO: On/Off Power Switch",
         "label": "10002034-13X",
         "manufacturer": "SimonTech S.L.U"
     },
+    "0x0267:0x0001:0x00f5": {
+        "description": "Switch IO: On/Off Power Switch",
+        "label": "10002034-13X",
+        "manufacturer": "SimonTech S.L.U"
+    },
     "0x0267:0x0001:0x0107": {
         "description": "Switch IO: On/Off Power Switch",
         "label": "10002034-13X",
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0001:0x0477": {
         "description": "Switch IO: On/Off Power Switch",
@@ -11790,39 +12070,49 @@
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0004:0x0177": {
         "description": "Simon IO: Roller Blind",
         "label": "10002080-13x",
         "manufacturer": "SimonTech S.L.U"
     },
+    "0x0267:0x0005:0x0000": {
+        "description": "Simon IO: Master Roller Blind",
+        "label": "10002081-13x",
+        "manufacturer": "SimonTech S.L.U"
+    },
     "0x0267:0x0005:0x00f4": {
         "description": "Simon IO: Master Roller Blind",
         "label": "10002081-13x",
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0005:0x01c3": {
         "description": "Simon IO: Master Roller Blind",
         "label": "10002081-13x",
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0009:0x0000": {
-        "description": "iO Cover for the Simon 100 schuko plug socket",
+        "description": "iO Cover for the Simon 100 Schuko Plug Socket",
         "label": "10002041-130",
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0009:0x0022": {
         "description": "iO Cover for the Simon 100 Schuko Plug Socket",
         "label": "10002041-13X",
         "manufacturer": "SimonTech S.L.U"
     },
     "0x0267:0x0011:0x0000": {
-        "description": "Sensor de humo iO",
+        "description": "Sensor De Humo iO",
         "label": "10002862-039",
         "manufacturer": "SimonTech S.L.U"
     },
+    "0x0267:0x0102:0x0000": {
+        "description": "Simon IO: Roller Blind (700 Series)",
+        "label": "1000X080-XXX",
+        "manufacturer": "SimonTech S.L.U"
+    },
     "0x0268:0x0001:0x0001": {
         "description": "Nexa Bridge",
         "label": "NEXA BRIDGE V1",
         "manufacturer": "Nexa Trading AB"
     },
     "0x0268:0x0002:0x1027": {
         "description": "Metered Wall Plug Switch",
@@ -11871,40 +12161,40 @@
     },
     "0x0270:0x0101:0x000a": {
         "description": "Water Ball Valve Servo",
         "label": "BVS-ZWU",
         "manufacturer": "Custos"
     },
     "0x0271:0x0001:0x1a73": {
-        "description": "PIR sensor with relay and light",
+        "description": "PIR Sensor with Relay and Light",
         "label": "XLED Home 2",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0271:0x0001:0x1a74": {
-        "description": "Indoor LED-light with motion sensor",
+        "description": "Indoor LED-Light with Motion Sensor",
         "label": "RS LED D2 Z-Wave",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0271:0x0001:0x1a75": {
-        "description": "Sensor-switched outdoor up and downlighting",
+        "description": "Sensor-Switched Outdoor Up and Downlighting",
         "label": "L 810 LED iHF",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0271:0x0002:0x19fb": {
-        "description": "Infrared motion detector with orientation light",
+        "description": "Infrared Motion Detector with Orientation Light",
         "label": "MotionSwitch LED",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0271:0x0002:0x1a72": {
-        "description": "PIR sensor with relay",
+        "description": "PIR Sensor with Relay",
         "label": "IS140-2",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0271:0x0002:0x6770": {
-        "description": "PIR sensor with relay",
+        "description": "PIR Sensor with Relay",
         "label": "IS140-2",
         "manufacturer": "STEINEL GmbH"
     },
     "0x0272:0x0001:0x0001": {
         "description": "Dune HD Solo 4K",
         "label": "SOLO4K",
         "manufacturer": "Dune-HD"
@@ -11925,14 +12215,19 @@
         "manufacturer": "Pixela Corporation"
     },
     "0x027a:0x0001:0x0005": {
         "description": "Outdoor Motion Sensor",
         "label": "ZSE29",
         "manufacturer": "Zooz"
     },
+    "0x027a:0x0001:0x000d": {
+        "description": "700 Series USB Controller",
+        "label": "ZST10-700",
+        "manufacturer": "Zooz"
+    },
     "0x027a:0x0003:0x0000": {
         "description": "Water Sensor",
         "label": "ZSE30",
         "manufacturer": "Zooz"
     },
     "0x027a:0x0003:0x0003": {
         "description": "Indoor Siren",
@@ -11965,14 +12260,24 @@
         "manufacturer": "Zooz"
     },
     "0x027a:0x0003:0x0512": {
         "description": "Valve Control",
         "label": "ZAC03",
         "manufacturer": "Zooz"
     },
+    "0x027a:0x0004:0x0110": {
+        "description": "DC Signal Sensor",
+        "label": "ZEN55 LR",
+        "manufacturer": "Zooz"
+    },
+    "0x027a:0x0004:0x0510": {
+        "description": "Range Extender",
+        "label": "ZAC38",
+        "manufacturer": "Zooz"
+    },
     "0x027a:0x0004:0x0610": {
         "description": "800 Series Long Range USB Controller",
         "label": "ZST39 LR",
         "manufacturer": "Zooz"
     },
     "0x027a:0x0004:0x0611": {
         "description": "800 Series Long Range GPIO Module",
@@ -11986,15 +12291,15 @@
     },
     "0x027a:0x000c:0x0003": {
         "description": "S2 Multisiren",
         "label": "ZSE19",
         "manufacturer": "Zooz"
     },
     "0x027a:0x0101:0x000a": {
-        "description": "Smart Plug with 2 USB ports",
+        "description": "Smart Plug with 2 USB Ports",
         "label": "ZEN06",
         "manufacturer": "Zooz"
     },
     "0x027a:0x0101:0x000d": {
         "description": "Power Switch",
         "label": "ZEN15",
         "manufacturer": "Zooz"
@@ -12069,83 +12374,129 @@
                 "$if": "productType === 0x0904",
                 "value": "ZEN52 LR"
             },
             "ZEN52"
         ],
         "manufacturer": "Zooz"
     },
+    "0x027a:0x0904:0x0218": {
+        "description": "0-10 V Dimmer",
+        "label": "ZEN54 LR",
+        "manufacturer": "Zooz"
+    },
+    "0x027a:0x0904:0x0219": {
+        "description": "DC Motor Controller",
+        "label": "ZEN53 LR",
+        "manufacturer": "Zooz"
+    },
     "0x027a:0x1111:0x1e1c": {
         "description": "Z-Wave Plus On/Off Toggle Switch",
         "label": "ZEN23",
         "manufacturer": "Zooz"
     },
     "0x027a:0x2021:0x2101": {
         "description": "4-in-1 Sensor",
         "label": [
             {
-                "$if": "firmwareVersion === 32.32 || firmwareVersion >= 1.10 && firmwareVersion < 16.9",
+                "$if": "firmwareVersion >= 32.32 || firmwareVersion >= 1.10 && firmwareVersion < 16.9",
                 "value": "ZSE40 700"
             },
             "ZSE40"
         ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x4953:0x3133": {
         "description": "Portable Smart Motion Sensor",
         "label": "ZW6302",
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa001": {
-        "description": "Z-Wave Plus 700 Series ON/OFF Switch",
-        "label": "ZEN71",
+        "description": "ON/OFF Switch",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 3.10 && firmwareVersion < 10.0",
+                "value": "ZEN71 800LR"
+            },
+            "ZEN71"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa002": {
-        "description": "Z-Wave Plus 700 Series Dimmer Switch",
-        "label": "ZEN72",
+        "description": "Dimmer Switch",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 3.10 && firmwareVersion < 10.0",
+                "value": "ZEN72 800LR"
+            },
+            "ZEN72"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa003": {
         "description": "700 Toggle Switch",
         "label": "ZEN73",
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa004": {
         "description": "700 Toggle Dimmer",
         "label": "ZEN74",
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa006": {
-        "description": "Z-Wave Plus 700 Series S2 ON/OFF Switch",
-        "label": "ZEN76",
+        "description": "S2 ON/OFF Switch",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 3.10 && firmwareVersion < 10.0",
+                "value": "ZEN76 800LR"
+            },
+            "ZEN76"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa007": {
-        "description": "Z-Wave Plus 700 Series S2 Dimmer Switch",
-        "label": "ZEN77",
+        "description": "S2 Dimmer Switch",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 4.10 && firmwareVersion < 10.0",
+                "value": "ZEN77 800LR"
+            },
+            "ZEN77"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa008": {
         "description": "Scene Controller",
-        "label": "ZEN32",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 2.10 && firmwareVersion < 10.0",
+                "value": "ZEN32 800LR"
+            },
+            "ZEN32"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xa00a": {
         "description": "Universal Relay",
         "label": "ZEN17",
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xb001": {
         "description": "Outdoor Smart Plug",
         "label": "ZEN05",
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xb002": {
         "description": "Indoor Smart Plug",
-        "label": "ZEN04",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 2.10",
+                "value": "ZEN04 800LR"
+            },
+            "ZEN04"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0x7000:0xb003": {
         "description": "700 Series Outdoor Double Plug",
         "label": "ZEN14",
         "manufacturer": "Zooz"
     },
@@ -12186,15 +12537,15 @@
     },
     "0x027a:0xa000:0xa003": {
         "description": "Double Plug",
         "label": "ZEN25",
         "manufacturer": "Zooz"
     },
     "0x027a:0xa000:0xa004": {
-        "description": "Z-Wave Plus Power Strip, VER. 2.0",
+        "description": "Z-Wave Plus Power Strip",
         "label": "ZEN20",
         "manufacturer": "Zooz"
     },
     "0x027a:0xa000:0xa008": {
         "description": "Dimmer & Dry Contact Relay",
         "label": "ZEN30",
         "manufacturer": "Zooz"
@@ -12227,15 +12578,21 @@
     "0x027a:0xb112:0x261c": {
         "description": "Z-Wave Plus Toggle Dimmer Light Switch Ver 2.0",
         "label": "ZEN24",
         "manufacturer": "Zooz"
     },
     "0x027a:0xbb00:0xbb08": {
         "description": "Scene Controller",
-        "label": "ZEN32",
+        "label": [
+            {
+                "$if": "firmwareVersion >= 2.10 && firmwareVersion < 10.0",
+                "value": "ZEN32 800LR"
+            },
+            "ZEN32"
+        ],
         "manufacturer": "Zooz"
     },
     "0x027a:0xbb00:0xbb0a": {
         "description": "Universal Relay",
         "label": "ZEN17",
         "manufacturer": "Zooz"
     },
@@ -12251,15 +12608,15 @@
     },
     "0x027e:0x0002:0x0001": {
         "description": "Nokia Smart Home GPON ONT",
         "label": "G-240WZ",
         "manufacturer": "Nokia"
     },
     "0x0280:0x0001:0x0001": {
-        "description": "smanos Smart Hub",
+        "description": "Smanos Smart Hub",
         "label": "K2",
         "manufacturer": "Chuango Security Technology Corporation"
     },
     "0x0283:0x0001:0x0001": {
         "description": "TP-LINK Smart Home Router",
         "label": "SMART HOME ROUTER",
         "manufacturer": "TP-Link Technologies Co., Ltd."
@@ -12301,15 +12658,15 @@
     },
     "0x0287:0x0004:0x0072": {
         "description": "Window Blind Controller",
         "label": "iblinds V3",
         "manufacturer": "HAB Home Intelligence LLC"
     },
     "0x028a:0x0001:0x0001": {
-        "description": "Qua station",
+        "description": "Qua Station",
         "label": "KTS31MW",
         "manufacturer": "Askey Computer Corp."
     },
     "0x028c:0x00eb:0xeb20": {
         "description": "Energy Bridge",
         "label": "PWLY-274343",
         "manufacturer": "Powerley"
@@ -12321,25 +12678,25 @@
     },
     "0x0293:0x0003:0x0014": {
         "description": "Four Touch Panel and Power Socket",
         "label": "HTP-4S1-FB",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x0018": {
-        "description": "8 way touch light switch",
+        "description": "8 Way Touch Light Switch",
         "label": "HTP-8S0-XX",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x001a": {
         "description": "Touch Panel Switch",
         "label": "HG-TS10",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x0024": {
-        "description": "Z-Wave Switch with 2 on/off light switches and 2 up/down blinds switches",
+        "description": "Z-Wave Switch with 2 On/off Light Switches and 2 Up/down Blinds Switches",
         "label": "Lumi LM-S4ZW (C-L)",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x0113": {
         "description": "Hogar Pebble",
         "label": "HC-TB-ZW",
         "manufacturer": "Home controls"
@@ -12361,15 +12718,15 @@
     },
     "0x0293:0x0003:0x4413": {
         "description": "3 Touch Panel Switch",
         "label": "HTP-3S0",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x4414": {
-        "description": "Z-Wave Switch with 4 on/off light switches",
+        "description": "Z-Wave Switch with 4 On/off Light Switches",
         "label": "Lumi LM-SxZW (C-L)",
         "manufacturer": "Home controls"
     },
     "0x0293:0x0003:0x441a": {
         "description": "10 Touch Panel Switch",
         "label": "HTP-10S0",
         "manufacturer": "Home controls"
@@ -12396,15 +12753,15 @@
     },
     "0x0299:0x0001:0x157c": {
         "description": "DIGIT ISIO STC+",
         "label": "4757",
         "manufacturer": "TechniSat Digital GmbH"
     },
     "0x0299:0x0001:0x15e0": {
-        "description": "TECHNIMEDIA UHD TV line software",
+        "description": "TECHNIMEDIA UHD TV Line Software",
         "label": "5600",
         "manufacturer": "TechniSat Digital GmbH"
     },
     "0x0299:0x0001:0x1644": {
         "description": "DigiPal SMART HOME",
         "label": "9530",
         "manufacturer": "TechniSat Digital GmbH"
@@ -12416,21 +12773,21 @@
     },
     "0x0299:0x0001:0x1838": {
         "description": "SONATA 1",
         "label": "4790",
         "manufacturer": "TechniSat Digital GmbH"
     },
     "0x0299:0x0001:0x189c": {
-        "description": "TECHNIVISTA TV line software",
+        "description": "TECHNIVISTA TV Line Software",
         "label": "6300",
         "manufacturer": "TechniSat Digital GmbH"
     },
     "0x0299:0x0002:0x1a90": {
-        "description": "Flush On/Off switch",
-        "label": "Single-Switch ",
+        "description": "Flush On/Off Switch",
+        "label": "Single-Switch",
         "manufacturer": "TechniSat"
     },
     "0x0299:0x0003:0x1a91": {
         "description": "Flush Series Switch",
         "label": "Double-Switch",
         "manufacturer": "TechniSat"
     },
@@ -12466,20 +12823,20 @@
     },
     "0x0300:0x0301:0x0041": {
         "description": "Bypass Door Window Sensor Z-Wave 700",
         "label": "7AA-SS-VE-A0",
         "manufacturer": "LEEDARSON LIGHTING CO., Ltd."
     },
     "0x0300:0x0301:0x0042": {
-        "description": "Z-WAVE 700 Motion Sensor Pet Immunity",
+        "description": "Z-Wave 700 Motion Sensor Pet Immunity",
         "label": "7CA-SS-VE-A0",
         "manufacturer": "LEEDARSON LIGHTING CO., Ltd."
     },
     "0x0300:0x0301:0x0044": {
-        "description": "Z-WAVE 700 Keypad",
+        "description": "Z-Wave 700 Keypad",
         "label": "7BA-KP-V-B-A0",
         "manufacturer": "LEEDARSON LIGHTING CO., Ltd."
     },
     "0x0301:0x0048:0x010f": {
         "description": "Clamp Energy Meter",
         "label": "Zwave Clamp",
         "manufacturer": "Seco"
@@ -12496,50 +12853,50 @@
     },
     "0x0307:0x4447:0x3033": {
         "description": "In-Wall On/Off Switch",
         "label": "86/102",
         "manufacturer": "SATCO Products, Inc."
     },
     "0x030a:0x0103:0x0090": {
-        "description": "Curtain motor",
+        "description": "Curtain Motor",
         "label": "DT82TV/F-1.2/14",
         "manufacturer": "Dooya"
     },
     "0x030c:0x0001:0xa101": {
         "description": "Fios Quantum Gateway",
         "label": "FIOS-G1100-V1",
         "manufacturer": "Verizon"
     },
     "0x030d:0x0101:0x0101": {
         "description": "Z-Wave Plus Wireless Receiving Controller",
         "label": "ERC307",
         "manufacturer": "Hampoo"
     },
     "0x030f:0x0001:0x0001": {
-        "description": "Double Switch in a dual relay in-wall module.",
+        "description": "Double Switch in A Dual Relay In-Wall Module.",
         "label": "DS100",
         "manufacturer": "Vemmio"
     },
     "0x030f:0x0003:0x0003": {
         "description": "Motion and Light Mini Sensor",
         "label": "MT-100",
         "manufacturer": "Vemmio"
     },
     "0x0312:0x0004:0xee02": {
         "description": "Smart Dimmer Switch",
         "label": "MS11ZS",
         "manufacturer": "Minoston"
     },
     "0x0312:0x0111:0x261c": {
-        "description": "In-wall Smart Dimmer",
+        "description": "In-Wall Smart Dimmer",
         "label": "NZW31T",
         "manufacturer": "Inovelli"
     },
     "0x0312:0x0221:0x251c": {
-        "description": "Show Home, 2 channel smart plug, ZWave Plus",
+        "description": "Show Home, 2 Channel Smart Plug, Z-Wave Plus",
         "label": "ZW37",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0x0713:0xd100": {
         "description": "Door/Window Temperature & Humidity Sensor",
         "label": "MSE30Z",
         "manufacturer": "Minoston"
@@ -12566,35 +12923,35 @@
     },
     "0x0312:0x1f00:0x1f00": {
         "description": "In-Wall Dimming Switch Scene Enabled",
         "label": "NZW31S",
         "manufacturer": "Inovelli"
     },
     "0x0312:0x1f01:0x1f01": {
-        "description": "In-wall Dimming Switch",
+        "description": "In-Wall Dimming Switch",
         "label": "NZW31",
         "manufacturer": "Inovelli"
     },
     "0x0312:0x1f02:0x1f02": {
-        "description": "In-wall Smart Dimmer",
+        "description": "In-Wall Smart Dimmer",
         "label": "NZW31T",
         "manufacturer": "Inovelli"
     },
     "0x0312:0x2003:0xb31c": {
         "description": "Smoke Sensor",
         "label": "ZW1103",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0x2003:0xb51c": {
         "description": "Shock Sensor",
         "label": "ZW1105",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0x2003:0xc41c": {
-        "description": "Flood leak sensor",
+        "description": "Flood Leak Sensor",
         "label": "EZW1204",
         "manufacturer": "NIE Technology Co., Ltd."
     },
     "0x0312:0x2400:0x2400": {
         "description": "On/Off Smart Plug + Signal Repeater (Z-Wave Plus)",
         "label": "NZW36",
         "manufacturer": "NIE Technology Co., Ltd."
@@ -12620,36 +12977,41 @@
         "manufacturer": "NIE Technology Co., Ltd."
     },
     "0x0312:0x6100:0x6100": {
         "description": "2-Channel Dual Smart Plug",
         "label": "NZW37",
         "manufacturer": "NIE Technology Co., Ltd."
     },
+    "0x0312:0x7000:0x7002": {
+        "description": "Z-Wave Knob Dimmer Switch",
+        "label": "ZKS31",
+        "manufacturer": "NIE Technology Co., Ltd."
+    },
     "0x0312:0x7000:0xf001": {
         "description": "S2 Remote Control Switch",
         "label": "ZW922",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xa000:0xa007": {
         "description": "Smart Outlet",
         "label": "ZW32",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xa000:0xaa02": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xaa00:0xaa01": {
-        "description": "S2 In-wall Smart ON/OFF Switch",
+        "description": "S2 In-Wall Smart ON/OFF Switch",
         "label": "ZW30",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xaa00:0xaa02": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xac01:0x4001": {
         "description": "Mini Smart Plug",
         "label": "N4001",
         "manufacturer": "New One"
@@ -12666,15 +13028,15 @@
     },
     "0x0312:0xb003:0xc11c": {
         "description": "Door/Window Sensor",
         "label": "ZW1201",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xb112:0x1f1c": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xb115:0x201c": {
         "description": "Smart Outlet",
         "label": "ZW32",
         "manufacturer": "EVA Logik"
@@ -12691,15 +13053,15 @@
     },
     "0x0312:0xb221:0x251c": {
         "description": "2-Channel Dual Smart Plug",
         "label": "NZW37",
         "manufacturer": "NIE Technology Co., Ltd."
     },
     "0x0312:0xbb00:0xbb01": {
-        "description": "S2 In-wall Smart ON/OFF Switch",
+        "description": "S2 In-Wall Smart ON/OFF Switch",
         "label": "ZW30",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xbb00:0xbb02": {
         "description": "S2 Smart Start Dimmer Switch",
         "label": "ZW31S",
         "manufacturer": "EVA Logik"
@@ -12731,15 +13093,15 @@
     },
     "0x0312:0xee00:0xee01": {
         "description": "Smart On/Off Switch",
         "label": "MS10ZS",
         "manufacturer": "Minoston"
     },
     "0x0312:0xee00:0xee02": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xee00:0xee03": {
         "description": "Smart On/Off Toggle Switch",
         "label": "MS12ZS",
         "manufacturer": "Minoston"
@@ -12761,46 +13123,46 @@
     },
     "0x0312:0xff00:0xff03": {
         "description": "Smart On/Off Switch",
         "label": "MS10ZS",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff04": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xff00:0xff05": {
-        "description": "Zwave Plug 2 channel plugin outlet",
+        "description": "Zwave Plug 2 Channel Plugin Outlet",
         "label": "MP20Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff06": {
-        "description": "Smart Plug - 1 channel",
+        "description": "Smart Plug - 1 Channel",
         "label": "MP21Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff07": {
         "description": "Z-Wave Outdoor Smart Plug",
         "label": "MP22Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff08": {
-        "description": "Outdoor Smart Plug - 1 channel",
+        "description": "Outdoor Smart Plug - 1 Channel",
         "label": "MP23Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff09": {
-        "description": "Outdoor Smart Plug - 2 channel",
+        "description": "Outdoor Smart Plug - 2 Channel",
         "label": "MP24Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff0c": {
-        "description": "Smart Plug - 1 channel",
-        "label": "MP21Z",
+        "description": "Mini Smart Plug",
+        "label": "MP21Z / MP31Z",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff00:0xff0d": {
         "description": "Smart Plug Dimmer",
         "label": "MP21ZD",
         "manufacturer": "Minoston"
     },
@@ -12826,28 +13188,33 @@
     },
     "0x0312:0xff01:0xff03": {
         "description": "Smart On/Off Switch",
         "label": "MS10ZS",
         "manufacturer": "Minoston"
     },
     "0x0312:0xff01:0xff04": {
-        "description": "S2 In-wall Smart Dimmer switch",
+        "description": "S2 In-Wall Smart Dimmer Switch",
         "label": "ZW31",
         "manufacturer": "EVA Logik"
     },
     "0x0312:0xff07:0xff03": {
         "description": "Z-Wave Outdoor Smart Plug",
         "label": "MP22ZD",
         "manufacturer": "Minoston"
     },
     "0x0313:0x0001:0x0001": {
-        "description": "wireless handle",
+        "description": "Wireless Handle",
         "label": "FG-FR404-ZW-HF",
         "manufacturer": "Hoppe"
     },
+    "0x0313:0x0701:0x0002": {
+        "description": "eHandle ConnectSense",
+        "label": "E0400Z-EF",
+        "manufacturer": "Hoppe"
+    },
     "0x0315:0x0001:0x0001": {
         "description": "Z-Wave ToolBox",
         "label": "ZWP-TBX",
         "manufacturer": "zwaveproducts.com"
     },
     "0x0315:0x0202:0x0001": {
         "description": "Water Leak Detector",
@@ -12935,14 +13302,19 @@
         "manufacturer": "Inovelli"
     },
     "0x031e:0x000e:0x0001": {
         "description": "Red Series Fan + Light Switch",
         "label": "LZW36",
         "manufacturer": "Inovelli"
     },
+    "0x031e:0x0015:0x0001": {
+        "description": "2-1 Dimmer",
+        "label": "VZW31-SN",
+        "manufacturer": "Inovelli"
+    },
     "0x0320:0x0001:0x0001": {
         "description": "Magnetic Contact",
         "label": "HO-09ZW",
         "manufacturer": "China Security & Fire IOT Sensing CO., Ltd."
     },
     "0x0320:0x0002:0x0001": {
         "description": "Wireless Passive Infrared Detector",
@@ -12966,60 +13338,75 @@
     },
     "0x032c:0x3003:0x0007": {
         "description": "PIR Detect Sensor",
         "label": "SK-3003-07",
         "manufacturer": "Shenzhen Saykey Technology Co., Ltd."
     },
     "0x032c:0x3007:0x0005": {
-        "description": "Curtain Motor Control external module",
+        "description": "Curtain Motor Control External Module",
         "label": "SK-3007-05",
         "manufacturer": "Shenzhen Saykey Technology Co., Ltd."
     },
     "0x032c:0x5005:0x0002": {
         "description": "Keyfob Remote Control",
         "label": "SK-5005-02",
         "manufacturer": "Shenzhen Saykey Technology Co., Ltd."
     },
     "0x032d:0x3002:0x0006": {
         "description": "",
         "label": "BSL01",
         "manufacturer": "Benetek"
     },
     "0x032e:0x0004:0x0042": {
-        "description": "DSI-101 binary switch",
+        "description": "DSI-101 Binary Switch",
         "label": "DSI-101 binary switch",
         "manufacturer": "DEFARO"
     },
     "0x032e:0x0013:0x0021": {
         "description": "Thermostat Actuator",
         "label": "DAT-101",
         "manufacturer": "Defaro"
     },
     "0x032e:0x0021:0x0013": {
-        "description": "Double relay Switch 2x1.7kW",
+        "description": "Double Relay Switch 2x1.7kW",
         "label": "DAS-102",
         "manufacturer": "DEFARO"
     },
     "0x032e:0x0060:0x0031": {
-        "description": "Dimmer with sensors support",
+        "description": "Dimmer with Sensors Support",
         "label": "DAD-101",
         "manufacturer": "DEFARO"
     },
     "0x0330:0x0003:0xa10d": {
         "description": "Wall Controller",
         "label": "SR-ZV9001T4-DIM",
         "manufacturer": "ShenZhen Sunricher Technology, Ltd."
     },
     "0x0330:0x0003:0xa305": {
-        "description": "4 group single color wall mounted remote",
+        "description": "4 Group Single Color Wall Mounted Remote",
         "label": "ZV9001K8-DIM",
         "manufacturer": "Sunricher"
     },
+    "0x0330:0x0004:0xd00d": {
+        "description": "Motor Controller",
+        "label": "VES-ZW-MOT-018",
+        "manufacturer": "Vesternet"
+    },
+    "0x0330:0x0004:0xd019": {
+        "description": "High Load Switch",
+        "label": "VES-ZW-HLD-016",
+        "manufacturer": "Vesternet"
+    },
+    "0x0330:0x0004:0xd109": {
+        "description": "2 Channel Switch",
+        "label": "VES-ZW-SWI-014",
+        "manufacturer": "Vesternet"
+    },
     "0x0330:0x0200:0xd002": {
-        "description": "Z-wave CCT LED controller",
+        "description": "Z-Wave CCT LED Controller",
         "label": "ZV9102FA-CCT",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0200:0xd004": {
         "description": "Z-Wave Smart Plug",
         "label": "SR-ZV9021A",
         "manufacturer": "ShenZhen Sunricher Technology, Ltd."
@@ -13071,15 +13458,15 @@
     },
     "0x0330:0x021a:0xd002": {
         "description": "RGBW LED Controller",
         "label": "ZV9101",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0300:0xa103": {
-        "description": "4 group CCT touch panel secondary controller",
+        "description": "4 Group CCT Touch Panel Secondary Controller",
         "label": "ZV9002T4-CCT",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0300:0xa104": {
         "description": "CCT Wall Controller",
         "label": "ZV9001T-CCT",
         "manufacturer": "Sunricher"
@@ -13106,18 +13493,23 @@
     },
     "0x0330:0x0300:0xa305": {
         "description": "Wall Mounted Switch",
         "label": "Heatit Z-Push Button 8",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0300:0xa306": {
-        "description": "2 group single color wall mounted remote",
+        "description": "2 Group Single Color Wall Mounted Remote",
         "label": "ZV9001K4-DIM-G2",
         "manufacturer": "Sunricher"
     },
+    "0x0330:0x0300:0xa307": {
+        "description": "Wall Controller - 2 Button",
+        "label": "VES-ZW-WAL-003",
+        "manufacturer": "Vesternet"
+    },
     "0x0330:0x0300:0xa30c": {
         "description": "Touch Panel RGBW Wall Controller",
         "label": "ZV9001K4-RGBW",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0300:0xa30f": {
         "description": "Z-Wave Dim Remote Control",
@@ -13131,17 +13523,17 @@
     },
     "0x0330:0x0300:0xb301": {
         "description": "5 Channel Dimmer Remote Control",
         "label": "ZV9001K12-DIM-Z5",
         "manufacturer": "Sunricher"
     },
     "0x0330:0x0300:0xb302": {
-        "description": "4 Channel Dimmer Remote Control",
-        "label": "ZV9001K12-DIM-Z4",
-        "manufacturer": "Sunricher"
+        "description": "Remote Control - 12 Button",
+        "label": "VES-ZW-REM-010",
+        "manufacturer": "Vesternet"
     },
     "0x0330:0x0301:0xa101": {
         "description": "Wall Controller",
         "label": "SR-ZV9002T3-CCT",
         "manufacturer": "ShenZhen Sunricher Technology, Ltd."
     },
     "0x0330:0x0301:0xa105": {
@@ -13180,14 +13572,24 @@
         "manufacturer": "Sunricher"
     },
     "0x0330:0x031a:0xa10d": {
         "description": "Wall Controller",
         "label": "SR-ZV9001T4-DIM",
         "manufacturer": "ShenZhen Sunricher Technology, Ltd."
     },
+    "0x0330:0x0400:0xd105": {
+        "description": "Push-Button Coupler",
+        "label": "SR-ZV2833PAC",
+        "manufacturer": "Sunricher"
+    },
+    "0x0330:0x0400:0xd10a": {
+        "description": "Multisensor",
+        "label": "SR-ZV9032A-EU",
+        "manufacturer": "ShenZhen Sunricher Technology, Ltd."
+    },
     "0x0331:0x0001:0x1001": {
         "description": "Gateway",
         "label": "WK-0001",
         "manufacturer": "Winka Electronic Co., Ltd."
     },
     "0x0333:0x0001:0x0001": {
         "description": "Home IoT",
@@ -13276,30 +13678,170 @@
     },
     "0x0344:0x0004:0x000a": {
         "description": "High Load Switch",
         "label": "HE-HLS01",
         "manufacturer": "HELTUN"
     },
     "0x0345:0x0001:0x0001": {
-        "description": "Swidget module with USB port",
+        "description": "Swidget Module with USB Port",
         "label": "ZW000RW",
         "manufacturer": "Swidget Corp"
     },
+    "0x0345:0x0100:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0101:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0105:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0108:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0200:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0201:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0205:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0208:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0300:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0301:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0305:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0308:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0400:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0401:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0405:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0408:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0500:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0501:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0505:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0508:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0600:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0601:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0605:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0608:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0700:0x0002": {
+        "description": "Universal Control Insert",
+        "label": "ZW000UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0701:0x0002": {
+        "description": "Universal Control Insert + USB",
+        "label": "ZW001UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0705:0x0002": {
+        "description": "Universal Control Insert + Air Quality",
+        "label": "ZW008UWA",
+        "manufacturer": "Swidget Corp"
+    },
+    "0x0345:0x0708:0x0002": {
+        "description": "Universal Control Insert + Temperature/Humidity/Motion",
+        "label": "ZW006UWA",
+        "manufacturer": "Swidget Corp"
+    },
     "0x0346:0x0001:0x0101": {
         "description": "Base Station v2",
         "label": "SVHSZWB1",
         "manufacturer": "Ring"
     },
     "0x0346:0x0101:0x0201": {
-        "description": "Alarm Keypad (1st generation)",
+        "description": "Alarm Keypad (1st Generation)",
         "label": "4AK1S7-0EN0 / 4AK1E9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0101:0x0202": {
-        "description": "Alarm Keypad (1st generation)",
+        "description": "Alarm Keypad (1st Generation)",
         "label": "4AK1S7-0EN0 / 4AK1E9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0101:0x0301": {
         "description": "Keypad v2",
         "label": "4AK1SZ",
         "manufacturer": "Ring"
@@ -13325,14 +13867,19 @@
         "manufacturer": "Ring"
     },
     "0x0346:0x0201:0x0401": {
         "description": "Contact Sensor Gen2",
         "label": "4SD2SZ-0EN0",
         "manufacturer": "Ring"
     },
+    "0x0346:0x0201:0x0601": {
+        "description": "Contact Sensor Gen2",
+        "label": "4SD2SZ-0EN0",
+        "manufacturer": "Ring"
+    },
     "0x0346:0x0301:0x0201": {
         "description": "Motion Sensor",
         "label": "4SP1S7-0EN0 / 4SPAE9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0301:0x0202": {
         "description": "Motion Sensor",
@@ -13346,75 +13893,100 @@
     },
     "0x0346:0x0301:0x0401": {
         "description": "Motion Sensor Gen2",
         "label": "4SP1SZ",
         "manufacturer": "Ring"
     },
     "0x0346:0x0401:0x0101": {
-        "description": "Range Extender (1st generation)",
+        "description": "Range Extender (1st Generation)",
         "label": "4AR1S7-0EN0 / 4AR1E9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0401:0x0102": {
-        "description": "Range Extender (1st generation)",
+        "description": "Range Extender (1st Generation)",
         "label": "4AR1S7-0EN0 / 4AR1E9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0401:0x0202": {
-        "description": "Range Extender (1st generation)",
+        "description": "Range Extender (1st Generation)",
         "label": "4AR1S7-0EN0 / 4AR1E9-0EU0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0401:0x0301": {
-        "description": "Range Extender (2nd generation)",
+        "description": "Range Extender (2nd Generation)",
         "label": "4AR1SZ-0EN0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0401:0x0401": {
-        "description": "Range Extender (2nd generation)",
+        "description": "Range Extender (2nd Generation)",
         "label": "4AR1SZ-0EN0",
         "manufacturer": "Ring"
     },
+    "0x0346:0x0601:0x0101": {
+        "description": "Ring Smoke/CO Listener",
+        "label": "4SS1S80EN0",
+        "manufacturer": "Ring"
+    },
     "0x0346:0x0701:0x0301": {
         "description": "Outdoor Siren",
         "label": "5D22E2 / 5AT3T4",
         "manufacturer": "Ring"
     },
     "0x0346:0x0701:0x0401": {
         "description": "Outdoor Siren",
         "label": "5D22E2 / 5AT3T4",
         "manufacturer": "Ring"
     },
+    "0x0346:0x0801:0x0301": {
+        "description": "Panic Button (2nd Gen)",
+        "label": "5F56E9",
+        "manufacturer": "Ring"
+    },
+    "0x0346:0x0801:0x0401": {
+        "description": "Panic Button (2nd Gen)",
+        "label": "5F56E9",
+        "manufacturer": "Ring"
+    },
     "0x0346:0x0a01:0x0301": {
         "description": "Glass Break Sensor",
         "label": "Glass Break Sensor",
         "manufacturer": "Ring"
     },
+    "0x0346:0x0a01:0x0401": {
+        "description": "Glass Break Sensor",
+        "label": "Glass Break Sensor",
+        "manufacturer": "Ring"
+    },
     "0x0346:0x0b01:0x0101": {
         "description": "Retrofit Alarm Kit",
         "label": "4AW1SZ-0EN0",
         "manufacturer": "Ring"
     },
     "0x0346:0x0c01:0x0301": {
         "description": "Outdoor Contact Sensor",
         "label": "B0923BK77S",
         "manufacturer": "Ring"
     },
+    "0x0346:0x0c01:0x0401": {
+        "description": "Outdoor Contact Sensor",
+        "label": "B0923BK77S",
+        "manufacturer": "Ring"
+    },
     "0x0348:0x0001:0x0001": {
         "description": "Central Home Unit",
         "label": "CHU00001-W",
         "manufacturer": "KUNDO xT GmbH"
     },
     "0x0349:0x0013:0x3700": {
-        "description": "homee Z-Wave Cube",
+        "description": "Homee Z-Wave Cube",
         "label": "HOMEE\u20130002",
         "manufacturer": "Codeatelier GmbH"
     },
     "0x0349:0x0013:0x3900": {
-        "description": "homee Z-Wave Cube Green",
+        "description": "Homee Z-Wave Cube Green",
         "label": "ESTMK-Z-WAV",
         "manufacturer": "Codeatelier GmbH"
     },
     "0x034b:0x0001:0x0001": {
         "description": "iRemocon Wi-Fi",
         "label": "IRM-03WL",
         "manufacturer": "Glamo Inc."
@@ -13441,37 +14013,37 @@
     },
     "0x034e:0x0001:0x0101": {
         "description": "Radio Base Module",
         "label": "MTBAS-100-WL",
         "manufacturer": "TEM AG"
     },
     "0x034f:0x0003:0x0001": {
-        "description": "electronic deadbolt lock",
+        "description": "Electronic Deadbolt Lock",
         "label": "PL2S0S10-ZW",
         "manufacturer": "TONG LUNG METAL INDUSTRY CO., Ltd."
     },
     "0x0353:0x0001:0x0001": {
         "description": "Connect+ Security Panel with Z-Wave Controller",
         "label": "RE6100",
         "manufacturer": "Alula"
     },
     "0x0357:0x0057:0x0002": {
-        "description": "",
+        "description": "1-Button Smart Switch",
         "label": "UPowerSwitch",
-        "manufacturer": "Shenzhen 3nod Acousticlink Co., Ltd."
+        "manufacturer": "LG U+"
     },
     "0x0357:0x0058:0x0002": {
-        "description": "",
+        "description": "2-Button Smart Switch",
         "label": "UPowerSwitch",
-        "manufacturer": "Shenzhen 3nod Acousticlink Co., Ltd."
+        "manufacturer": "LG U+"
     },
     "0x0357:0x0059:0x0002": {
-        "description": "",
+        "description": "3-Button Smart Switch",
         "label": "UPowerSwitch",
-        "manufacturer": "Shenzhen 3nod Acousticlink Co., Ltd."
+        "manufacturer": "LG U+"
     },
     "0x0358:0x0001:0x0001": {
         "description": "LodeStar",
         "label": "LSHAC-Z5B3K4-100",
         "manufacturer": "Star Automation"
     },
     "0x0361:0x0003:0x0008": {
@@ -13576,15 +14148,15 @@
     },
     "0x0371:0x0002:0x0007": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA008",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0002:0x0009": {
-        "description": "a\u00ebrQ Temperature and Humidity Sensor v1.0",
+        "description": "a\u00ebrQ Temperature and Humidity Sensor V1.0",
         "label": "ZWA009",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0002:0x000b": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA011",
         "manufacturer": "Aeotec Ltd."
@@ -13691,28 +14263,33 @@
     },
     "0x0371:0x0102:0x0007": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA008",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0102:0x0009": {
-        "description": "a\u00ebrQ Temperature and Humidity Sensor v1.0",
+        "description": "a\u00ebrQ Temperature and Humidity Sensor V1.0",
         "label": "ZWA009",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0102:0x000b": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA011",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0102:0x000c": {
         "description": "Door / Window Sensor 7 Pro",
         "label": "ZWA012",
         "manufacturer": "Aeotec Ltd."
     },
+    "0x0371:0x0102:0x0012": {
+        "description": "Water Sensor 7 Basic",
+        "label": "ZWA018",
+        "manufacturer": "Aeotec Ltd."
+    },
     "0x0371:0x0102:0x0013": {
         "description": "Water Sensor 7 Pro",
         "label": "ZWA019",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0102:0x0016": {
         "description": "illumino WallMote 7",
@@ -13801,15 +14378,15 @@
     },
     "0x0371:0x0202:0x0007": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA008",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0202:0x0009": {
-        "description": "a\u00ebrQ Temperature and Humidity Sensor v1.0",
+        "description": "a\u00ebrQ Temperature and Humidity Sensor V1.0",
         "label": "ZWA009",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0371:0x0202:0x000b": {
         "description": "Door/Window Sensor 7",
         "label": "ZWA011",
         "manufacturer": "Aeotec Ltd."
@@ -13861,20 +14438,20 @@
     },
     "0x0371:0x1c02:0x0005": {
         "description": "TriSensor",
         "label": "ZWA005",
         "manufacturer": "Aeotec Ltd."
     },
     "0x0373:0x0003:0x0001": {
-        "description": "Z wave module for ID Lock 150 and 101",
+        "description": "Z Wave Module for ID Lock 150 and 101",
         "label": "ID-150",
         "manufacturer": "ID Lock AS"
     },
     "0x0374:0x0001:0x0001": {
-        "description": "Z-Wave Gateway Controller and hub",
+        "description": "Z-Wave Gateway Controller and Hub",
         "label": "HCS-W1001",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0374:0x0001:0x0081": {
         "description": "DIGITAL DOOR LOCK",
         "label": "HDL-5200SK",
         "manufacturer": "Hyundai Telecom"
@@ -13886,30 +14463,30 @@
     },
     "0x0374:0x0001:0x0083": {
         "description": "DIGITAL DOOR LOCK",
         "label": "HDL-7390SK",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0374:0x0002:0x0001": {
-        "description": "Z-Wave Gateway Controller and hub",
+        "description": "Z-Wave Gateway Controller and Hub",
         "label": "HCS-W1001",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0374:0x0003:0x0001": {
-        "description": "Z-Wave Gateway Controller and hub",
+        "description": "Z-Wave Gateway Controller and Hub",
         "label": "HAS-R2071M",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0374:0x0004:0x0001": {
-        "description": "Z-Wave Gateway Controller and hub",
+        "description": "Z-Wave Gateway Controller and Hub",
         "label": "HCS-W1001",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0374:0x0005:0x0001": {
-        "description": "Z-Wave Gateway Controller and hub",
+        "description": "Z-Wave Gateway Controller and Hub",
         "label": "HCS-W1001",
         "manufacturer": "Hyundai Telecom"
     },
     "0x0377:0x0001:0x0001": {
         "description": "Smart Home Gateway",
         "label": "WSR 1706 V 1.0",
         "manufacturer": "HORNBACH Baumarkt AG"
@@ -14016,15 +14593,15 @@
     },
     "0x039b:0x0001:0x0013": {
         "description": "TIM_BOX",
         "label": "UZW4010TIM2",
         "manufacturer": "Reply S.p.A."
     },
     "0x0400:0x0001:0x0001": {
-        "description": "iota",
+        "description": "Iota",
         "label": "IOT",
         "manufacturer": "Abode"
     },
     "0x0402:0x0001:0x0001": {
         "description": "AI Home Gateway",
         "label": "NCP-HG100",
         "manufacturer": "Sony Mobile Communications Inc."
@@ -14056,15 +14633,15 @@
     },
     "0x0403:0x0002:0x0003": {
         "description": "Smart Smoke Sensor",
         "label": "SHRM10000",
         "manufacturer": "ABUS Security-Center GmbH Co. KG"
     },
     "0x0403:0x0003:0x0000": {
-        "description": "High-volume siren (95 dB) and LED strobe light",
+        "description": "High-Volume Siren (95 dB) and LED Strobe Light",
         "label": "SHSG10000",
         "manufacturer": "ABUS Security-Center GmbH & Co. KG"
     },
     "0x0403:0x0003:0x0001": {
         "description": "ABUS Security Center Bulb",
         "label": "SHLM10000",
         "manufacturer": "ABUS Security-Center GmbH & Co. KG"
@@ -14201,25 +14778,25 @@
     },
     "0x041b:0x4952:0x3133": {
         "description": "In-Wall Outlet, Tamper Resistant, 500S",
         "label": "39456 / ZW1002",
         "manufacturer": "Resideo"
     },
     "0x041b:0x4f50:0x3035": {
-        "description": "Plug-in Outdoor Switch V2, 500S",
+        "description": "Plug-In Outdoor Switch V2, 500S",
         "label": "39453 / ZW4203",
         "manufacturer": "Resideo"
     },
     "0x041b:0x5044:0x3033": {
-        "description": "Plug-in 2-Outlet Dimmer, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Dimmer, Simultaneous, 500S",
         "label": "39446 / ZW3107",
         "manufacturer": "Resideo"
     },
     "0x041b:0x5052:0x3033": {
-        "description": "Plug-in 2-Outlet Switch, Simultaneous, 500S",
+        "description": "Plug-In 2-Outlet Switch, Simultaneous, 500S",
         "label": "39449 / ZW4106",
         "manufacturer": "Resideo"
     },
     "0x041c:0x8001:0x1000": {
         "description": "Motion Sensor",
         "label": "51111",
         "manufacturer": "Kjell & Co Elektronik"
@@ -14231,15 +14808,15 @@
     },
     "0x041c:0x8006:0x1000": {
         "description": "Smart Metering Plug",
         "label": "51110",
         "manufacturer": "Kjell & Co Elektronik"
     },
     "0x041c:0x8007:0x1000": {
-        "description": "Smart Humidity And Temperature Sensor",
+        "description": "Smart Humidity and Temperature Sensor",
         "label": "51112",
         "manufacturer": "Kjell & Co Elektronik"
     },
     "0x041e:0x0001:0x0001": {
         "description": "SmartHome IoT Hub",
         "label": "EIH-100E",
         "manufacturer": "Enplug"
@@ -14271,20 +14848,20 @@
     },
     "0x042f:0x0001:0x0001": {
         "description": "IOTAS Hub",
         "label": "CONNECT2",
         "manufacturer": "IOTAS"
     },
     "0x0431:0x0202:0x0001": {
-        "description": "ECO-DIM Z-Wave Led dimmer",
+        "description": "ECO-DIM Z-Wave LED Dimmer",
         "label": "ECO-DIM",
         "manufacturer": "EcoDim"
     },
     "0x0431:0x0202:0x0002": {
-        "description": "ECO-DIM Z-Wave Led dimmer",
+        "description": "ECO-DIM Z-Wave LED Dimmer",
         "label": "ECO-DIM",
         "manufacturer": "EcoDim"
     },
     "0x0432:0x0001:0x0001": {
         "description": "ONE X5100",
         "label": "S30851-S2563-R101",
         "manufacturer": "Gigaset"
@@ -14305,14 +14882,19 @@
         "manufacturer": "Q-light"
     },
     "0x0436:0x0004:0x5001": {
         "description": "1 Gang Touch Panel Switch",
         "label": "LM-S1ZW",
         "manufacturer": "Lumi"
     },
+    "0x0438:0x0004:0x0108": {
+        "description": "16 A Thermostat - White",
+        "label": "4512757",
+        "manufacturer": "Namron"
+    },
     "0x0438:0x0004:0xd019": {
         "description": "Switch 16A",
         "label": "4512746",
         "manufacturer": "Namron"
     },
     "0x0438:0x0200:0xd004": {
         "description": "16A Thermostat Wall Plug",
@@ -14326,20 +14908,20 @@
     },
     "0x0438:0x0200:0xd00c": {
         "description": "In-Wall Dimmer Module",
         "label": "Z-Wave Dimmer 2 400W",
         "manufacturer": "Namron"
     },
     "0x0438:0x0200:0xd013": {
-        "description": "16A Touch thermostat - White",
+        "description": "16A Touch Thermostat - White",
         "label": "4512744",
         "manufacturer": "Namron"
     },
     "0x0438:0x0200:0xd025": {
-        "description": "16A Touch thermostat - Black",
+        "description": "16A Touch Thermostat - Black",
         "label": "4512745",
         "manufacturer": "Namron"
     },
     "0x0438:0x0202:0x0002": {
         "description": "LED Dimmer",
         "label": "1402756",
         "manufacturer": "Namron"
@@ -14356,25 +14938,25 @@
     },
     "0x0438:0x0300:0xa30f": {
         "description": "1-Channel Wireless Switch",
         "label": "K2",
         "manufacturer": "Namron"
     },
     "0x0438:0x0300:0xb302": {
-        "description": "4-channel Remote Control",
+        "description": "4-Channel Remote Control",
         "label": "4512711",
         "manufacturer": "Namron"
     },
     "0x0438:0x0400:0xd10a": {
         "description": "Multisensor",
         "label": "SR-ZV9032A-EU",
         "manufacturer": "Namron"
     },
     "0x0441:0x2400:0x1000": {
-        "description": "BusT4-Z-Wave interface",
+        "description": "BusT4-Z-Wave Interface",
         "label": "IBT4ZWAVE",
         "manufacturer": "NICE Spa"
     },
     "0x0445:0x0020:0x0001": {
         "description": "Z-Wave Gateway",
         "label": "TRF-ZW10",
         "manufacturer": "URC Automation"
@@ -14386,30 +14968,30 @@
     },
     "0x0447:0x000e:0x1107": {
         "description": "Z-Wave Plus Receptacle",
         "label": "SQR44102",
         "manufacturer": "Schneider Electric"
     },
     "0x0447:0x000e:0x1108": {
-        "description": "Z-Wave Plus Plug-in",
+        "description": "Z-Wave Plus Plug-In",
         "label": "SQR62102WHZ",
         "manufacturer": "Schneider Electric"
     },
     "0x0447:0x000e:0x1202": {
         "description": "Z-Wave Plus Dimmer",
         "label": "SQR22102",
         "manufacturer": "Schneider Electric"
     },
     "0x0447:0x000e:0x1301": {
         "description": "Z-Wave Plus Auxiliary Switch",
         "label": "SQR50101",
         "manufacturer": "Schneider Electric"
     },
     "0x0447:0x0111:0x1101": {
-        "description": "Z-Wave Plug-in",
+        "description": "Z-Wave Plug-In",
         "label": "SQR62101WHZ",
         "manufacturer": "Schneider Electric"
     },
     "0x0447:0x0111:0x1102": {
         "description": "Z-Wave Switch Single Pole",
         "label": "SQR14101",
         "manufacturer": "Schneider Electric"
@@ -14441,16 +15023,16 @@
     },
     "0x044c:0x0003:0x0004": {
         "description": "OpenTherm Actuator v4",
         "label": "MyOT v4",
         "manufacturer": "SmartDHOME"
     },
     "0x044e:0x0004:0x0001": {
-        "description": "Aidoo Control HVAC unit",
-        "label": "AZAI6WSPFU2",
+        "description": "Aidoo Control HVAC Unit",
+        "label": "AZAI6ZWEFU2",
         "manufacturer": "Airzone"
     },
     "0x044f:0x1100:0x0001": {
         "description": "Kitchen Hub",
         "label": "UVH1301",
         "manufacturer": "GE"
     },
@@ -14475,86 +15057,176 @@
         "manufacturer": "Cherubini S.p.A."
     },
     "0x0456:0x0013:0x3800": {
         "description": "700 Series Cube",
         "label": "HOMEE-005",
         "manufacturer": "Homee"
     },
+    "0x045a:0x0000:0x0400": {
+        "description": "Thermostatic Radiator Valve",
+        "label": "Z-TRV-V01",
+        "manufacturer": "ZVIDAR"
+    },
     "0x045a:0x0004:0x0111": {
         "description": "Door Window Sensor",
         "label": "Z-DWS-V01",
         "manufacturer": "ZVIDAR"
     },
     "0x045a:0x0004:0x0610": {
         "description": "800 Series USB Controller",
         "label": "Z-DG-V01",
         "manufacturer": "ZVIDAR"
     },
+    "0x045a:0x0904:0x0507": {
+        "description": "Smart Curtain Motor",
+        "label": "Z-CM-V01",
+        "manufacturer": "ZVIDAR"
+    },
+    "0x0460:0x0002:0x0081": {
+        "description": "Wave 2PM",
+        "label": "QNSW-002P16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x0083": {
+        "description": "Wave 1",
+        "label": "QNSW-001X16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x0084": {
+        "description": "Wave 1PM",
+        "label": "QNSW-001P16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x0088": {
+        "description": "Wave Plug US",
+        "label": "QNPL-001X16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x0089": {
+        "description": "Wave Plug UK",
+        "label": "QNPL-001X12",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008a": {
+        "description": "Wave Pro 1",
+        "label": "QPSW-0A1X16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008b": {
+        "description": "Wave Pro 1PM",
+        "label": "QPSW-0A1P16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008c": {
+        "description": "Wave Pro 2",
+        "label": "QPSW-0A2X16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008d": {
+        "description": "Wave Pro 2PM",
+        "label": "QPSW-0A2P16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008e": {
+        "description": "Wave 1 Mini",
+        "label": "QMSW-0A1X8",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0002:0x008f": {
+        "description": "Wave 1PM Mini",
+        "label": "QMSW-0A1P8",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0003:0x0082": {
+        "description": "Wave Shutter",
+        "label": "QNSH-001P10",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0007:0x0081": {
+        "description": "Wave PM Mini",
+        "label": "QMEM-0A1PC16",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0009:0x0081": {
+        "description": "Wave I4",
+        "label": "QNSN-0A24X",
+        "manufacturer": "Shelly Europe Ltd."
+    },
+    "0x0460:0x0009:0x0082": {
+        "description": "Wave I4 DC",
+        "label": "QNSN-0D24X",
+        "manufacturer": "Shelly Europe Ltd."
+    },
     "0x4118:0x0002:0x0002": {
         "description": "Slim Multi-Sensor",
         "label": "TSM02",
         "manufacturer": "TKB Home"
     },
     "0x5254:0x0000:0x531e": {
-        "description": "Z-Wave enabled universal remote control",
+        "description": "Z-Wave Enabled Universal Remote Control",
         "label": "Z-URC500",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0000:0x531f": {
-        "description": "Z-Wave enabled universal remote control",
+        "description": "Z-Wave Enabled Universal Remote Control",
         "label": "Z-URC500",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0000:0x5320": {
-        "description": "Z-Wave enabled universal remote control",
+        "description": "Z-Wave Enabled Universal Remote Control",
         "label": "Z-URC500",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0000:0x8380": {
         "description": "Remote Control",
         "label": "ZRC-100",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0000:0x8510": {
-        "description": "Scene master 8 button remote",
+        "description": "Scene Master 8 Button Remote",
         "label": "BW8510",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0001:0x8332": {
-        "description": "Z-Wave enabled universal remote control",
+        "description": "Z-Wave Enabled Universal Remote Control",
         "label": "Z-URC500",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0001:0x8380": {
         "description": "Remote Control",
         "label": "ZRC-100",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0001:0x8510": {
-        "description": "Scene master 8 button remote",
+        "description": "Scene Master 8 Button Remote",
         "label": "BW8510",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0002:0x0004": {
         "description": "",
         "label": "Z-URC 300",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0002:0x8380": {
         "description": "Remote Control",
         "label": "ZRC-100",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0002:0x8510": {
-        "description": "Scene master 8 button remote",
+        "description": "Scene Master 8 Button Remote",
         "label": "BW8510",
         "manufacturer": "Remotec"
     },
+    "0x5254:0x0004:0x8492": {
+        "description": "IR AC & AV Extender",
+        "label": "ZXT-800",
+        "manufacturer": "Remotec"
+    },
     "0x5254:0x000b:0x8510": {
-        "description": "Scene master 8 button remote",
+        "description": "Scene Master 8 Button Remote",
         "label": "BW8510",
         "manufacturer": "Remotec"
     },
     "0x5254:0x0100:0x8371": {
         "description": "AV IR Extender",
         "label": "ZXT-310",
         "manufacturer": "Remotec"
@@ -14651,33 +15323,33 @@
     },
     "0x5254:0x8001:0x0000": {
         "description": "Remotec Switch Module",
         "label": "ZRM-80S",
         "manufacturer": "Remotec"
     },
     "0x5254:0x8001:0x8020": {
-        "description": "Wall plug switch",
+        "description": "Wall Plug Switch",
         "label": "BW8020S",
         "manufacturer": "Remotec"
     },
     "0x5254:0x8200:0x8130": {
         "description": "Dimming Switch Module (Dual Mode)",
         "label": "ZDS-210NA",
         "manufacturer": "Remotec"
     },
     "0x5254:0x8201:0x0200": {
         "description": "Remotec Dimming Module",
         "label": "ZDM-80S",
         "manufacturer": "Remotec"
     },
     "0x5254:0x8201:0x8021": {
-        "description": "Wall plug dimmer switch",
+        "description": "Wall Plug Dimmer Switch",
         "label": "ZDM-80",
         "manufacturer": "Remotec"
     },
     "0x5254:0x8201:0x8120": {
         "description": "Dual Mode Switch-Dimmer",
         "label": "BW8120",
         "manufacturer": "Remotec"
     },
-    "updated_at": "2023-03-09T18:47:28.189185"
+    "updated_at": "2024-04-06T22:22:20.961929"
 }
```

### Comparing `vivintpy-2023.3.8/vivintpy/zjs_device_config_db.py` & `vivintpy-2023.3.9/vivintpy/zjs_device_config_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Script to generate Z-Wave device data."""
+
 from __future__ import annotations
 
 import json
 import os
 
 ZJS_DEVICE_CONFIG_DB_FILE = os.path.join(
     os.path.dirname(__file__), "zjs_device_config_db.json"
```

### Comparing `vivintpy-2023.3.8/PKG-INFO` & `vivintpy-2023.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivintpy
-Version: 2023.3.8
+Version: 2023.3.9
 Summary: Python library for interacting with a Vivint security and smart home system.
 Home-page: https://github.com/natekspencer/vivintpy
 License: MIT
 Keywords: Vivint,alarm system,security,smart home,home automation,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.8 Summary: Python library
+Metadata-Version: 2.1 Name: vivintpy Version: 2023.3.9 Summary: Python library
 for interacting with a Vivint security and smart home system. Home-page: https:
 //github.com/natekspencer/vivintpy License: MIT Keywords: Vivint,alarm
 system,security,smart home,home automation,asynchronous Author: Nathan Spencer
 Author-email: natekspencer@gmail.com Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

