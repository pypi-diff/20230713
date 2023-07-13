# Comparing `tmp/bluecurrent-api-1.0.3.tar.gz` & `tmp/bluecurrent-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecurrent-api-1.0.3.tar", last modified: Fri Apr 21 09:43:28 2023, max compression
+gzip compressed data, was "bluecurrent-api-1.0.4.tar", last modified: Thu Jul 13 10:44:40 2023, max compression
```

## Comparing `bluecurrent-api-1.0.3.tar` & `bluecurrent-api-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.551419 bluecurrent-api-1.0.3/
--rw-rw-rw-   0        0        0     1073 2022-09-09 13:33:12.000000 bluecurrent-api-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3805 2023-04-21 09:43:28.550406 bluecurrent-api-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3230 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/README.md
--rw-rw-rw-   0        0        0      762 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 09:43:28.551419 bluecurrent-api-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.502407 bluecurrent-api-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.511405 bluecurrent-api-1.0.3/src/bluecurrent_api/
--rw-rw-rw-   0        0        0       56 2022-10-03 11:18:14.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/__init__.py
--rw-rw-rw-   0        0        0     4436 2023-02-03 15:06:22.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/client.py
--rw-rw-rw-   0        0        0      670 2022-11-18 12:50:41.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/exceptions.py
--rw-rw-rw-   0        0        0     6328 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/utils.py
--rw-rw-rw-   0        0        0     8507 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/src/bluecurrent_api/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.542409 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/
--rw-rw-rw-   0        0        0     3805 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 09:43:28.000000 bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 09:43:28.548405 bluecurrent-api-1.0.3/tests/
--rw-rw-rw-   0        0        0     2873 2022-11-18 12:50:41.000000 bluecurrent-api-1.0.3/tests/test_client.py
--rw-rw-rw-   0        0        0     9452 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/tests/test_utils.py
--rw-rw-rw-   0        0        0    15803 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.3/tests/test_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:44:40.597250 bluecurrent-api-1.0.4/
+-rw-rw-rw-   0        0        0     1073 2022-09-09 13:33:12.000000 bluecurrent-api-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3805 2023-07-13 10:44:40.596725 bluecurrent-api-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3230 2023-04-21 09:42:55.000000 bluecurrent-api-1.0.4/README.md
+-rw-rw-rw-   0        0        0      762 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:44:40.597250 bluecurrent-api-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-13 10:44:40.553826 bluecurrent-api-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 10:44:40.564108 bluecurrent-api-1.0.4/src/bluecurrent_api/
+-rw-rw-rw-   0        0        0       56 2022-10-03 11:18:14.000000 bluecurrent-api-1.0.4/src/bluecurrent_api/__init__.py
+-rw-rw-rw-   0        0        0     4823 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/src/bluecurrent_api/client.py
+-rw-rw-rw-   0        0        0      666 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/src/bluecurrent_api/exceptions.py
+-rw-rw-rw-   0        0        0     6896 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/src/bluecurrent_api/utils.py
+-rw-rw-rw-   0        0        0     9329 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/src/bluecurrent_api/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:44:40.590473 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/
+-rw-rw-rw-   0        0        0     3805 2023-07-13 10:44:40.000000 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-13 10:44:40.000000 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:44:40.000000 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 10:44:40.000000 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 10:44:40.000000 bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 10:44:40.595124 bluecurrent-api-1.0.4/tests/
+-rw-rw-rw-   0        0        0     2867 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/tests/test_client.py
+-rw-rw-rw-   0        0        0     9453 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/tests/test_utils.py
+-rw-rw-rw-   0        0        0    15722 2023-07-13 10:44:12.000000 bluecurrent-api-1.0.4/tests/test_websocket.py
```

### Comparing `bluecurrent-api-1.0.3/LICENSE` & `bluecurrent-api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.3/PKG-INFO` & `bluecurrent-api-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bluecurrent-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wrapper for the Blue Current websocket api
 Author-email: Floris272 <florispuijk@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bluecurrent/HomeAssistantAPI
 Project-URL: Bug Tracker, https://github.com/bluecurrent/HomeAssistantAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Blue Current Api
 
 [![Documentation Status](https://readthedocs.com/projects/blue-current-homeassistantapi/badge/?version=latest&token=00ce4a850aedc0993b7075a8b2d5f8de98251adcdb4eada1f1fb3c02fee80039)](https://blue-current-homeassistantapi.readthedocs-hosted.com/en/latest/?badge=latest)
```

### Comparing `bluecurrent-api-1.0.3/README.md` & `bluecurrent-api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bluecurrent-api-1.0.3/pyproject.toml` & `bluecurrent-api-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bluecurrent-api"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Floris272", email="florispuijk@outlook.com" },
 ]
 description = "A wrapper for the Blue Current websocket api"
 readme = "README.md"
 license = {text = "MIT"}
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "websockets >= 10.0",
```

### Comparing `bluecurrent-api-1.0.3/src/bluecurrent_api/client.py` & `bluecurrent-api-1.0.4/src/bluecurrent_api/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,121 @@
 """Define an object to interact with the BlueCurrent websocket api."""
-from typing import Callable
+from datetime import timedelta
+from typing import Any, Callable, Optional
+
 from .utils import get_next_reset_delta
 from .websocket import Websocket
 
 
 class Client:
     """Api Client for the BlueCurrent Websocket Api."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the Client."""
         self.websocket = Websocket()
 
-    def get_next_reset_delta(self):
+    def get_next_reset_delta(self) -> timedelta:
         """Returns the next reset delta"""
         return get_next_reset_delta()
 
-    async def wait_for_response(self):
+    async def wait_for_response(self) -> None:
         """Wait for next response."""
         await self.websocket.get_receiver_event().wait()
 
-    async def validate_api_token(self, api_token: str):
+    async def validate_api_token(self, api_token: str) -> bool:
         """Validate an api_token."""
         return await self.websocket.validate_api_token(api_token)
 
-    async def get_email(self):
+    async def get_email(self) -> str:
         """Get user email."""
         return await self.websocket.get_email()
 
-    async def get_charge_cards(self):
+    async def get_charge_cards(self) -> list[dict[str, Any]]:
         """Get the charge cards."""
         return await self.websocket.get_charge_cards()
 
-    async def connect(self, api_token: str):
+    async def connect(self, api_token: str) -> None:
         """Connect to the websocket."""
         await self.websocket.connect(api_token)
 
-    async def start_loop(self, receiver: Callable):
+    async def start_loop(self, receiver: Callable[[dict[str, Any]], None]) -> None:
         """Start the receive loop."""
         await self.websocket.loop(receiver)
 
-    async def disconnect(self):
+    async def disconnect(self) -> None:
         """Disconnect the websocket."""
         await self.websocket.disconnect()
 
-    async def get_charge_points(self):
+    async def get_charge_points(self) -> None:
         """Get the charge points."""
         request = self._create_request("GET_CHARGE_POINTS")
         await self.websocket.send_request(request)
 
-    async def get_status(self, evse_id: str):
+    async def get_status(self, evse_id: str) -> None:
         """Get the status of a charge point."""
         request = self._create_request("GET_CH_STATUS", evse_id)
         await self.websocket.send_request(request)
 
-    async def get_settings(self, evse_id: str):
+    async def get_settings(self, evse_id: str) -> None:
         """Get the settings of a charge point."""
         request = self._create_request("GET_CH_SETTINGS", evse_id)
         await self.websocket.send_request(request)
 
-    async def get_grid_status(self, evse_id: str):
+    async def get_grid_status(self, evse_id: str) -> None:
         """Get the grid status of a charge point."""
         request = self._create_request("GET_GRID_STATUS", evse_id)
         await self.websocket.send_request(request)
 
-    async def set_public_charging(self, evse_id: str, value: bool):
+    async def set_linked_charge_cards_only(self, evse_id: str, value: bool) -> None:
         """Set public_charging of a charge point to a value."""
-        request = self._create_request("SET_PUBLIC_CHARGING", evse_id, value)
+        request = self._create_request("SET_PUBLIC_CHARGING", evse_id, not value)
         await self.websocket.send_request(request)
 
-    async def set_plug_and_charge(self, evse_id: str, value: bool):
+    async def set_plug_and_charge(self, evse_id: str, value: bool) -> None:
         """Set plug_and_charge of a charge point to a value."""
         request = self._create_request("SET_PLUG_AND_CHARGE", evse_id, value)
         await self.websocket.send_request(request)
 
-    async def set_operative(self, evse_id: str, value: bool):
+    async def block(self, evse_id: str, value: bool) -> None:
         """Set available of a charge point to a value."""
         command = "SET_OPERATIVE"
-        if value is False:
+        if value is True:
             command = "SET_INOPERATIVE"
         request = self._create_request(command, evse_id)
         await self.websocket.send_request(request)
 
-    async def reset(self, evse_id: str):
+    async def reset(self, evse_id: str) -> None:
         """Reset a charge point."""
         request = self._create_request("SOFT_RESET", evse_id)
         await self.websocket.send_request(request)
 
-    async def reboot(self, evse_id: str):
+    async def reboot(self, evse_id: str) -> None:
         """Reboot a charge point."""
         request = self._create_request("REBOOT", evse_id)
         await self.websocket.send_request(request)
 
-    async def start_session(self, evse_id: str, card_uid: str):
+    async def start_session(self, evse_id: str, card_uid: str) -> None:
         """Start a charge session at a charge point."""
-        request = self._create_request(
-            "START_SESSION", evse_id, card_uid=card_uid)
+        request = self._create_request("START_SESSION", evse_id, card_uid=card_uid)
         await self.websocket.send_request(request)
 
-    async def stop_session(self, evse_id: str):
+    async def stop_session(self, evse_id: str) -> None:
         """Stop a charge session at a charge point."""
         request = self._create_request("STOP_SESSION", evse_id)
         await self.websocket.send_request(request)
 
-    def _create_request(self, command, evse_id=None, value=None, card_uid=None):
+    def _create_request(
+        self,
+        command: str,
+        evse_id: Optional[str] = None,
+        value: Optional[bool] = None,
+        card_uid: Optional[str] = None,
+    ) -> dict[str, Any]:
         """Create a request."""
-        request = {"command": command}
+        request: dict[str, Any] = {"command": command}
 
         if evse_id:
             request["evse_id"] = evse_id
 
         if value is not None:
             request["value"] = value
```

### Comparing `bluecurrent-api-1.0.3/src/bluecurrent_api/exceptions.py` & `bluecurrent-api-1.0.4/src/bluecurrent_api/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Define package errors."""
 
 
 class BlueCurrentException(Exception):
     """Define a base error."""
 
 
-class WebsocketException(BlueCurrentException):
+class WebsocketError(BlueCurrentException):
     """Define an error related to the websocket connection."""
 
 
 class RequestLimitReached(BlueCurrentException):
     """Define an error for when the request limit is reached."""
```

### Comparing `bluecurrent-api-1.0.3/src/bluecurrent_api/utils.py` & `bluecurrent-api-1.0.4/src/bluecurrent_api/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,125 +1,123 @@
 """Define a functions for modifying incoming data."""
 from datetime import datetime, timedelta
+from typing import Any, Optional, Union
+
 import pytz
-from .exceptions import RequestLimitReached, WebsocketException
 
-TZ = pytz.timezone('Europe/Amsterdam')
+from .exceptions import BlueCurrentException, RequestLimitReached, WebsocketError
 
-ERRORS = {
-    0: WebsocketException("Unknown command"),
-    1: WebsocketException("Invalid Auth Token"),
-    2: WebsocketException("Not authorized"),
-    9: WebsocketException("Unknown error"),
-    42: RequestLimitReached("Request limit reached")
-}
+TZ = pytz.timezone("Europe/Amsterdam")
 
-SETTINGS = ['plug_and_charge', 'public_charging']
+ERRORS: dict[int, BlueCurrentException] = {
+    0: WebsocketError("Unknown command"),
+    1: WebsocketError("Invalid Auth Token"),
+    2: WebsocketError("Not authorized"),
+    9: WebsocketError("Unknown error"),
+    42: RequestLimitReached("Request limit reached"),
+}
 
-SMART_CHARGING = set()
+SMART_CHARGING: set[str] = set()
 
 
-def calculate_average_usage_from_phases(phases: tuple):
+def calculate_average_usage_from_phases(phases: list[float]) -> float:
     """Get the average of the phases that are not 0."""
     used_phases = [p for p in phases if p]
     if len(used_phases):
         return round(sum(used_phases) / len(used_phases), 1)
     return 0
 
 
-def calculate_total_kw(current: tuple, v_avg):
+def calculate_total_kw(c_avg: float, v_avg: float) -> float:
     """Calculate the total kW."""
-    return round((sum(current) * v_avg / 1000), 2)
+    return round((c_avg * v_avg * 1.732 / 1000), 2)
 
 
-def create_datetime(timestamp: str):
+def create_datetime(timestamp: str) -> Optional[datetime]:
     """Get a datetime object from an timestamp."""
 
     if timestamp == "":
         return None
 
-    if '+' in timestamp:
+    if "+" in timestamp:
         return datetime.strptime(timestamp, "%Y%m%d %H:%M:%S%z")
 
     time = datetime.strptime(timestamp, "%Y%m%d %H:%M:%S")
     time = TZ.localize(time)
     return time
 
 
-def get_vehicle_status(vehicle_status_key: str):
+def get_vehicle_status(vehicle_status_key: str) -> str:
     """Get the vehicle status."""
     statuses = {
         "A": "standby",
         "B": "vehicle_detected",
         "C": "ready",
         "D": "ready",
         "E": "no_power",
         "F": "vehicle_error",
     }
 
     return statuses[vehicle_status_key]
 
 
-def get_exception(message: dict):
+def get_exception(message: dict[str, Any]) -> BlueCurrentException:
     """Return a defined error message or one from the server"""
     error = message["error"]
     message = message["message"]
 
     if error in ERRORS:
         return ERRORS[error]
-    return WebsocketException(message)
+    return WebsocketError(message)
 
 
-def set_smart_charging(evse_id, smart_charging):
+def set_smart_charging(evse_id: str, smart_charging: bool) -> None:
     """Add or discard evse_id in SMART_CHARGING"""
     if smart_charging:
         SMART_CHARGING.add(evse_id)
     else:
         SMART_CHARGING.discard(evse_id)
 
 
-def handle_charge_points(message: dict):
+def handle_charge_points(message: dict[str, Any]) -> None:
     """Store the evse_id if it has smart charging enabled"""
     for charge_point in message["data"]:
-        set_smart_charging(
-            charge_point["evse_id"], charge_point["smart_charging"])
+        set_smart_charging(charge_point["evse_id"], charge_point["smart_charging"])
 
 
-def set_current_left(message: dict, c_avg):
+def set_current_left(message: dict[str, Any], c_avg: float) -> None:
     """Set current_left"""
     max_usage = message["data"]["max_usage"]
     smart_charging_max_usage = message["data"]["smartcharging_max_usage"]
 
     if message["evse_id"] in SMART_CHARGING:
         message["data"]["current_left"] = smart_charging_max_usage - c_avg
     else:
         message["data"]["current_left"] = max_usage - c_avg
 
 
-def handle_status(message: dict):
+def handle_status(message: dict[str, Any]) -> None:
     """Transform status values and add others."""
-    voltage1 = message["data"]["actual_v1"]
-    voltage2 = message["data"]["actual_v2"]
-    voltage3 = message["data"]["actual_v3"]
+    voltage1: float = message["data"]["actual_v1"]
+    voltage2: float = message["data"]["actual_v2"]
+    voltage3: float = message["data"]["actual_v3"]
 
-    v_avg = calculate_average_usage_from_phases((voltage1, voltage2, voltage3))
+    v_avg = calculate_average_usage_from_phases([voltage1, voltage2, voltage3])
     message["data"]["avg_voltage"] = v_avg
 
-    current1 = message["data"]["actual_p1"]
-    current2 = message["data"]["actual_p2"]
-    current3 = message["data"]["actual_p3"]
+    current1: float = message["data"]["actual_p1"]
+    current2: float = message["data"]["actual_p2"]
+    current3: float = message["data"]["actual_p3"]
 
-    c_avg = calculate_average_usage_from_phases(
-        (current1, current2, current3))
+    c_avg = calculate_average_usage_from_phases([current1, current2, current3])
     message["data"]["avg_current"] = c_avg
 
     set_current_left(message, c_avg)
 
-    message["data"]["total_kw"] = calculate_total_kw((
-        current1, current2, current3), v_avg)
+    message["data"]["total_kw"] = calculate_total_kw(c_avg, v_avg)
 
     vehicle_status_key = message["data"]["vehicle_status"]
     message["data"]["vehicle_status"] = get_vehicle_status(vehicle_status_key)
 
     start_datetime = message["data"]["start_datetime"]
     new_start_datetime = create_datetime(start_datetime)
 
@@ -129,70 +127,74 @@
     message["data"]["start_datetime"] = new_start_datetime
     message["data"]["stop_datetime"] = new_stop_datetime
 
     offline_since = message["data"]["offline_since"]
     message["data"]["offline_since"] = create_datetime(offline_since)
 
 
-def handle_settings(message: dict):
+def handle_settings(message: dict[str, Any]) -> None:
     """Transform settings object"""
-    for key in SETTINGS:
-        message["data"][key] = message["data"][key]["value"]
 
-    set_smart_charging(
-        message['data']['evse_id'], message["data"]["smart_charging"])
+    message["data"]["plug_and_charge"] = message["data"]["plug_and_charge"]["value"]
+    message["data"]["linked_charge_cards_only"] = not message["data"][
+        "public_charging"
+    ]["value"]
 
+    set_smart_charging(message["data"]["evse_id"], message["data"]["smart_charging"])
 
-def handle_grid(message: dict):
+
+def handle_grid(message: dict[str, Any]) -> None:
     """Add grid total and avg to a message."""
-    if "CURRENT" in message.get('object'):
+    if "CURRENT" in message["object"]:
         message["data"] = {}
-        message["data"]["grid_actual_p1"] = message.pop('grid_actual_p1')
-        message["data"]["grid_actual_p2"] = message.pop('grid_actual_p2')
-        message["data"]["grid_actual_p3"] = message.pop('grid_actual_p3')
-
-    current1 = message["data"]["grid_actual_p1"]
-    current2 = message["data"]["grid_actual_p2"]
-    current3 = message["data"]["grid_actual_p3"]
+        message["data"]["grid_actual_p1"] = message.pop("grid_actual_p1")
+        message["data"]["grid_actual_p2"] = message.pop("grid_actual_p2")
+        message["data"]["grid_actual_p3"] = message.pop("grid_actual_p3")
+
+    current1: float = message["data"]["grid_actual_p1"]
+    current2: float = message["data"]["grid_actual_p2"]
+    current3: float = message["data"]["grid_actual_p3"]
 
-    c_avg = calculate_average_usage_from_phases((current1, current2, current3))
+    c_avg = calculate_average_usage_from_phases([current1, current2, current3])
     message["data"]["grid_avg_current"] = c_avg
     c_max = max(current1, current2, current3)
     message["data"]["grid_max_current"] = c_max
 
 
-def handle_setting_change(message: dict):
+def handle_setting_change(message: dict[str, Any]) -> None:
     """Change result to a boolean."""
     message["result"] = "true" in message["result"]["setting"]
-    message["object"] = message["object"].replace("STATUS_SET_", "")
+
+    if message["object"] == "STATUS_SET_PUBLIC_CHARGING":
+        message["object"] = "LINKED_CHARGE_CARDS_ONLY"
+    else:
+        message["object"] = message["object"].replace("STATUS_SET_", "")
 
 
-def handle_session_messages(message: dict):
+def handle_session_messages(message: dict[str, Any]) -> None:
     """handle session messages."""
 
-    object_name = message["object"].replace(
-        "STATUS_", "").replace("RECEIVED_", "")
+    object_name = message["object"].replace("STATUS_", "").replace("RECEIVED_", "")
 
     if "STATUS" in message["object"] and message["error"]:
         name = object_name.lower()
-        error = message['error'].lower()
-        evse_id = message['evse_id']
+        error = message["error"].lower()
+        evse_id = message["evse_id"]
         message["error"] = f"{name} {error} for chargepoint: {evse_id}"
     message["object"] = object_name
 
 
-def get_dummy_message(evse_id):
+def get_dummy_message(evse_id: str) -> dict[str, Union[str, dict[str, Any]]]:
     """Return a CH_STATUS message with the current time as start_datetime"""
     return {
-        'object': 'CH_STATUS',
-        'data': {'start_datetime': datetime.now(TZ), 'evse_id': evse_id, }
+        "object": "CH_STATUS",
+        "data": {
+            "start_datetime": datetime.now(TZ),
+            "evse_id": evse_id,
+        },
     }
 
 
-def get_next_reset_delta():
+def get_next_reset_delta() -> timedelta:
     """Returns the timedelta to the next midnight"""
     now = datetime.now(TZ)
-    return now.replace(
-        hour=0,
-        minute=0,
-        second=30
-    ) + timedelta(days=1) - now
+    return now.replace(hour=0, minute=0, second=30) + timedelta(days=1) - now
```

### Comparing `bluecurrent-api-1.0.3/src/bluecurrent_api/websocket.py` & `bluecurrent-api-1.0.4/src/bluecurrent_api/websocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,241 +1,275 @@
 """Define an object that handles the connection to the Websocket"""
 import asyncio
 import json
-from typing import Callable
-from websockets.client import connect
-from websockets.exceptions import ConnectionClosed, InvalidStatusCode, ConnectionClosedError
+from asyncio import Event
+from typing import Any, Callable, Optional, cast
+
+from websockets.client import WebSocketClientProtocol, connect
+from websockets.exceptions import (
+    ConnectionClosed,
+    ConnectionClosedError,
+    InvalidStatusCode,
+    WebSocketException,
+)
+
 from .exceptions import (
-    InvalidApiToken, WebsocketException, NoCardsFound, RequestLimitReached, AlreadyConnected
+    AlreadyConnected,
+    InvalidApiToken,
+    NoCardsFound,
+    RequestLimitReached,
+    WebsocketError,
 )
 from .utils import (
-    handle_settings,
+    get_dummy_message,
+    get_exception,
     handle_charge_points,
-    handle_status,
     handle_grid,
-    handle_setting_change,
     handle_session_messages,
-    get_dummy_message,
-    get_exception
+    handle_setting_change,
+    handle_settings,
+    handle_status,
 )
 
 URL = "wss://motown.bluecurrent.nl/haserver"
 BUTTONS = ("START_SESSION", "STOP_SESSION", "SOFT_RESET", "REBOOT")
 
+
 class Websocket:
     """Class for handling requests and responses for the BlueCurrent Websocket Api."""
-    _connection = None
-    _has_connection = False
-    auth_token = None
-    receiver = None
-    receive_event = None
-    receiver_is_coroutine = None
 
-    def __init__(self):
+    _connection: Optional[WebSocketClientProtocol] = None
+    _has_connection: bool = False
+    auth_token: Optional[str] = None
+    receiver: Callable
+    receive_event: Optional[Event] = None
+    receiver_is_coroutine: bool
+
+    def __init__(self) -> None:
         pass
 
-    def get_receiver_event(self):
+    def get_receiver_event(self) -> Event:
         """Return cleared receive_event when connected."""
 
         self._check_connection()
         if self.receive_event is None:
-            self.receive_event = asyncio.Event()
+            self.receive_event = Event()
 
         self.receive_event.clear()
         return self.receive_event
 
-    async def validate_api_token(self, api_token: str):
+    async def validate_api_token(self, api_token: str) -> bool:
         """Validate an api token."""
         await self._connect()
         await self._send({"command": "VALIDATE_API_TOKEN", "token": api_token})
         res = await self._recv()
         await self.disconnect()
 
-        if res['object'] == 'ERROR':
+        if res["object"] == "ERROR":
             raise get_exception(res)
 
         if not res.get("success"):
             raise InvalidApiToken
         self.auth_token = "Token " + res["token"]
         return True
 
-    async def get_email(self):
+    async def get_email(self) -> str:
         """Return the user email"""
         if not self.auth_token:
-            raise WebsocketException("token not set")
+            raise WebsocketError("token not set")
         await self._connect()
         await self.send_request({"command": "GET_ACCOUNT"})
         res = await self._recv()
         await self.disconnect()
 
-        if res['object'] == 'ERROR':
+        if res["object"] == "ERROR":
             raise get_exception(res)
 
         if not res.get("login"):
-            raise WebsocketException('No email found')
-        return res['login']
+            raise WebsocketError("No email found")
+        return cast(str, res["login"])
 
-    async def get_charge_cards(self):
+    async def get_charge_cards(self) -> list[dict[str, Any]]:
         """Get the charge cards."""
         if not self.auth_token:
-            raise WebsocketException("token not set")
+            raise WebsocketError("token not set")
         await self._connect()
         await self.send_request({"command": "GET_CHARGE_CARDS"})
-        res = await self._recv()
+        res: dict[str, Any] = await self._recv()
         await self.disconnect()
-        cards = res.get("cards")
+        cards = cast(list[dict[str, Any]], res.get("cards"))
 
-        if res['object'] == 'ERROR':
+        if res["object"] == "ERROR":
             raise get_exception(res)
 
         if len(cards) == 0:
             raise NoCardsFound
         return cards
 
-    async def connect(self, api_token: str):
+    async def connect(self, api_token: str) -> None:
         """Validate api_token and connect to the websocket."""
         if self._has_connection:
-            raise WebsocketException("Connection already started.")
+            raise WebsocketError("Connection already started.")
         await self.validate_api_token(api_token)
         await self._connect()
 
-    async def _connect(self):
+    async def _connect(self) -> None:
         """Connect to the websocket."""
         try:
             self._connection = await connect(URL)
             self._has_connection = True
         except Exception as err:
             self.check_for_server_reject(err)
-            raise WebsocketException(
-                "Cannot connect to the websocket.") from err
+            raise WebsocketError("Cannot connect to the websocket.") from err
 
-    async def send_request(self, request: dict):
+    async def send_request(self, request: dict[str, Any]) -> None:
         """Add authorization and send request."""
         if not self.auth_token:
-            raise WebsocketException("Token not set")
+            raise WebsocketError("Token not set")
 
         request["Authorization"] = self.auth_token
         await self._send(request)
 
-    async def loop(self, receiver: Callable):
+    async def loop(self, receiver: Callable) -> None:
         """Loop the message_handler."""
 
         self.receiver = receiver
         self.receiver_is_coroutine = asyncio.iscoroutinefunction(receiver)
 
         # Needed for receiving updates
-        await self._send({"command": "HELLO", "Authorization": self.auth_token})
+        await self._send(
+            {
+                "command": "HELLO",
+                "Authorization": self.auth_token,
+                "header": "homeassistant",
+            }
+        )
 
         while True:
             stop = await self._message_handler()
             if stop:
                 break
 
-    async def _message_handler(self):
+    async def _message_handler(self) -> bool:
         """Wait for a message and give it to the receiver."""
 
-        message: dict = await self._recv()
+        message: dict[str, Any] = await self._recv()
 
         # websocket has disconnected
         if not message:
             return True
 
         object_name = message.get("object")
 
         if not object_name:
-            raise WebsocketException("Received message has no object.")
+            raise WebsocketError("Received message has no object.")
 
         # handle ERROR object
         if object_name == "ERROR":
             raise get_exception(message)
 
         # if object other than ERROR has an error key it will be send to the receiver.
         error = message.get("error")
 
         # ignored objects
-        if (("RECEIVED" in object_name and not error)
-                or object_name == "HELLO" or "OPERATIVE" in object_name):
+        if (
+            ("RECEIVED" in object_name and not error)
+            or object_name == "HELLO"
+            or "OPERATIVE" in object_name
+        ):
             return False
         if object_name == "CHARGE_POINTS":
             handle_charge_points(message)
         elif object_name == "CH_STATUS":
             handle_status(message)
         elif object_name == "CH_SETTINGS":
             handle_settings(message)
         elif "GRID" in object_name:
             handle_grid(message)
-        elif object_name in ('STATUS_SET_PUBLIC_CHARGING', 'STATUS_SET_PLUG_AND_CHARGE'):
+        elif object_name in (
+            "STATUS_SET_PUBLIC_CHARGING",
+            "STATUS_SET_PLUG_AND_CHARGE",
+        ):
             handle_setting_change(message)
         elif any(button in object_name for button in BUTTONS):
             handle_session_messages(message)
         else:
             return False
 
         self.handle_receive_event()
 
         await self.send_to_receiver(message)
 
         # Fix for api sending old start_datetime
-        if object_name == 'STATUS_START_SESSION' and not error:
-            await self.send_to_receiver(get_dummy_message(message['evse_id']))
+        if object_name == "STATUS_START_SESSION" and not error:
+            await self.send_to_receiver(get_dummy_message(message["evse_id"]))
 
-    async def send_to_receiver(self, message):
+        return False
+
+    async def send_to_receiver(self, message: dict[str, Any]) -> None:
         """Send data to the given receiver."""
         if self.receiver_is_coroutine:
             await self.receiver(message)
         else:
             self.receiver(message)
 
-    async def _send(self, data: dict):
+    async def _send(self, data: dict[str, Any]) -> None:
         """Send data to the websocket."""
         self._check_connection()
         try:
             data_str = json.dumps(data)
+            assert self._connection is not None
             await self._connection.send(data_str)
         except (ConnectionClosed, InvalidStatusCode) as err:
             self.handle_connection_errors(err)
 
-    async def _recv(self):
+    async def _recv(self) -> Any:
         """Receive data from de websocket."""
         self._check_connection()
+        assert self._connection is not None
         try:
             data = await self._connection.recv()
             return json.loads(data)
         except (ConnectionClosed, InvalidStatusCode) as err:
             self.handle_connection_errors(err)
+            return None
 
-    def handle_connection_errors(self, err):
+    def handle_connection_errors(self, err: WebSocketException) -> None:
         """Handle connection errors."""
         if self._has_connection:
             self._has_connection = False
             self.handle_receive_event()
             self.check_for_server_reject(err)
-            raise WebsocketException("Connection was closed.")
+            raise WebsocketError("Connection was closed.")
 
-    async def disconnect(self):
+    async def disconnect(self) -> None:
         """Disconnect from de websocket."""
         self._check_connection()
+        assert self._connection is not None
         if not self._has_connection:
-            raise WebsocketException("Connection is already closed.")
+            raise WebsocketError("Connection is already closed.")
         self._has_connection = False
         self.handle_receive_event()
         await self._connection.close()
 
-    def _check_connection(self):
+    def _check_connection(self) -> None:
         """Throw error if there is no connection."""
-        if not self._connection:
-            raise WebsocketException("No connection with the api.")
+        if self._connection is None:
+            raise WebsocketError("No connection with the api.")
 
-    def handle_receive_event(self):
+    def handle_receive_event(self) -> None:
         "Set receive_event if it exists"
         if self.receive_event is not None:
             self.receive_event.set()
 
-    def check_for_server_reject(self, err):
+    def check_for_server_reject(self, err: Exception) -> None:
         """Check if the client was rejected by the server"""
-        if isinstance(err, InvalidStatusCode) and err.headers.get('x-websocket-reject-reason'):
-            if 'Request limit reached' in err.headers.get('x-websocket-reject-reason'):
-                raise RequestLimitReached("Request limit reached") from err
-            if 'Already connected' in err.headers.get('x-websocket-reject-reason'):
-                raise AlreadyConnected("Already connected")
+
+        if isinstance(err, InvalidStatusCode):
+            reason = err.headers.get("x-websocket-reject-reason")
+            if reason is not None:
+                if "Request limit reached" in reason:
+                    raise RequestLimitReached("Request limit reached") from err
+                if "Already connected" in reason:
+                    raise AlreadyConnected("Already connected")
         if isinstance(err, ConnectionClosedError) and err.code == 4001:
             raise RequestLimitReached("Request limit reached") from err
```

### Comparing `bluecurrent-api-1.0.3/src/bluecurrent_api.egg-info/PKG-INFO` & `bluecurrent-api-1.0.4/src/bluecurrent_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bluecurrent-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A wrapper for the Blue Current websocket api
 Author-email: Floris272 <florispuijk@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bluecurrent/HomeAssistantAPI
 Project-URL: Bug Tracker, https://github.com/bluecurrent/HomeAssistantAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Blue Current Api
 
 [![Documentation Status](https://readthedocs.com/projects/blue-current-homeassistantapi/badge/?version=latest&token=00ce4a850aedc0993b7075a8b2d5f8de98251adcdb4eada1f1fb3c02fee80039)](https://blue-current-homeassistantapi.readthedocs-hosted.com/en/latest/?badge=latest)
```

### Comparing `bluecurrent-api-1.0.3/tests/test_client.py` & `bluecurrent-api-1.0.4/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,27 +45,27 @@
     test_send_request.assert_called_with(
         {'command': 'GET_CH_SETTINGS', 'evse_id': '101'})
 
     await client.get_grid_status('101')
     test_send_request.assert_called_with(
         {'command': 'GET_GRID_STATUS', 'evse_id': '101'})
 
-    await client.set_public_charging('101', True)
+    await client.set_linked_charge_cards_only('101', True)
     test_send_request.assert_called_with(
-        {'command': 'SET_PUBLIC_CHARGING', 'evse_id': '101', 'value': True})
+        {'command': 'SET_PUBLIC_CHARGING', 'evse_id': '101', 'value': False})
 
     await client.set_plug_and_charge('101', True)
     test_send_request.assert_called_with(
         {'command': 'SET_PLUG_AND_CHARGE', 'evse_id': '101', 'value': True})
 
-    await client.set_operative('101', True)
+    await client.block('101', False)
     test_send_request.assert_called_with(
         {'command': 'SET_OPERATIVE', 'evse_id': '101'})
 
-    await client.set_operative('101', False)
+    await client.block('101', True)
     test_send_request.assert_called_with(
         {'command': 'SET_INOPERATIVE', 'evse_id': '101'})
 
     await client.reset('101')
     test_send_request.assert_called_with(
         {'command': 'SOFT_RESET', 'evse_id': '101'})
```

### Comparing `bluecurrent-api-1.0.3/tests/test_utils.py` & `bluecurrent-api-1.0.4/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     assert total == 6
 
     total = calculate_average_usage_from_phases((None, None, None))
     assert total == 0
 
 
 def test_calculate_total_kW():
-    total = calculate_total_kw((14, 12, 15), 230)
-    assert total == 9.43
+    total = calculate_total_kw(14, 230)
+    assert total == 5.58
 
 
 def test_set_to_smart_charging():
     set_smart_charging('bcu101', True)
     assert SMART_CHARGING == {'bcu101'}
     set_smart_charging('bcu101', False)
     assert SMART_CHARGING == set()
@@ -132,15 +132,15 @@
 
     TZ = pytz.timezone('Europe/Amsterdam')
 
     handle_status(message)
 
     assert message["data"]["avg_voltage"] == 220.0
     assert message["data"]["avg_current"] == 8.0
-    assert message["data"]["total_kw"] == 5.28
+    assert message["data"]["total_kw"] == 3.05
     assert message["data"]["start_datetime"] == TZ.localize(datetime(
         2021, 11, 18, 14, 12, 23))
     assert message["data"]["stop_datetime"] == TZ.localize(datetime(
         2021, 11, 18, 14, 32, 23))
     assert message["data"]["offline_since"] == TZ.localize(datetime(
         2021, 11, 18, 14, 32, 23))
     assert message["data"]["vehicle_status"] == "standby"
@@ -160,15 +160,15 @@
                 'value': True,
             },
             'smart_charging': False
         }
     }
     handle_settings(message)
     assert message['data']['plug_and_charge'] == False
-    assert message['data']['public_charging'] == True
+    assert message['data']['linked_charge_cards_only'] == False
     assert SMART_CHARGING == set()
 
     message = {
         'data': {
             'evse_id': 'BCU102',
             'plug_and_charge': {
                 'value': False,
@@ -187,24 +187,24 @@
     message = {
         "object": "ERROR",
         "error": 0,
         "message": "Test error"
     }
 
     error = get_exception(message)
-    assert isinstance(error, WebsocketException)
+    assert isinstance(error, WebsocketError)
     assert str(error) == "Unknown command"
 
     message = {
         "object": "ERROR",
         "error": 99,
         "message": "Test error"
     }
     error = get_exception(message)
-    assert isinstance(error, WebsocketException)
+    assert isinstance(error, WebsocketError)
     assert str(error) == "Test error"
 
     message = {
         "object": "ERROR",
         "error": 42,
         "message": "Test error"
     }
@@ -238,26 +238,26 @@
     assert message["data"]["grid_avg_current"] == 13.7
     assert message["data"]["grid_max_current"] == 15
 
     assert len(message["data"]) == 5
 
 
 def test_handle_setting_change():
-    message = {'object': 'STATUS_SET_PUBLIC_CHARGING',
+    message = {'object': 'STATUS_SET_PLUG_AND_CHARGE',
                'result': {'setting': 'set true'}}
 
     handle_setting_change(message)
-    assert message == {'object': 'PUBLIC_CHARGING',
+    assert message == {'object': 'PLUG_AND_CHARGE',
                        'result': True}
 
     message = {'object': 'STATUS_SET_PUBLIC_CHARGING',
                'result': {'setting': 'set false'}}
 
     handle_setting_change(message)
-    assert message == {'object': 'PUBLIC_CHARGING',
+    assert message == {'object': 'LINKED_CHARGE_CARDS_ONLY',
                        'result': False}
 
 
 def test_handle_session_messages():
 
     message = {'object': 'RECEIVED_STOP_SESSION', 'success': False,
                'error': 'no active session for chargepoint: BCU101'}
```

### Comparing `bluecurrent-api-1.0.3/tests/test_websocket.py` & `bluecurrent-api-1.0.4/tests/test_websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from unittest.mock import AsyncMock
 from websockets.exceptions import InvalidStatusCode, ConnectionClosedError
 from websockets.frames import Close
 
 from src.bluecurrent_api.websocket import Websocket
-from src.bluecurrent_api.exceptions import WebsocketException, InvalidApiToken, NoCardsFound, RequestLimitReached, AlreadyConnected
+from src.bluecurrent_api.exceptions import WebsocketError, InvalidApiToken, NoCardsFound, RequestLimitReached, AlreadyConnected
 from asyncio.exceptions import TimeoutError
 import pytest
 from pytest_mock import MockerFixture
 import asyncio
 
 
 @pytest.mark.asyncio
 async def test_get_receiver_event(mocker: MockerFixture):
     websocket = Websocket()
 
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         websocket.get_receiver_event()
 
     mocker.patch.object(Websocket, '_connection')
 
     websocket.get_receiver_event()
     assert websocket.receive_event is not None
     assert websocket.receive_event.is_set() == False
@@ -65,32 +65,32 @@
     mocker.patch('src.bluecurrent_api.websocket.Websocket._send')
     mocker.patch('src.bluecurrent_api.websocket.Websocket.disconnect')
     mocker.patch(
         'src.bluecurrent_api.websocket.Websocket._recv',
         return_value={"object": "ACCOUNT", "login": 'test'}
     )
 
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.get_email()
     websocket.auth_token = 'abc'
     assert await websocket.get_email() == 'test'
 
     mocker.patch(
         'src.bluecurrent_api.websocket.Websocket._recv',
         return_value={"object": "ACCOUNT"}
     )
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.get_email()
 
     mocker.patch(
         'src.bluecurrent_api.websocket.Websocket._recv',
         return_value={"object": "ERROR",
                       "error": 42, 'message': "Request limit reached"}
     )
-    with pytest.raises(RequestLimitReached) as err:
+    with pytest.raises(RequestLimitReached):
         await websocket.get_email()
 
 
 @pytest.mark.asyncio
 async def test_get_charge_cards(mocker: MockerFixture):
     websocket = Websocket()
     mocker.patch('src.bluecurrent_api.websocket.Websocket._connect')
@@ -98,15 +98,15 @@
     mocker.patch('src.bluecurrent_api.websocket.Websocket.disconnect')
 
     mocker.patch(
         'src.bluecurrent_api.websocket.Websocket._recv',
         return_value={"object": "CHARGE_CARDS", "cards": []}
     )
 
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.get_charge_cards()
     websocket.auth_token = '123'
     with pytest.raises(NoCardsFound):
         await websocket.get_charge_cards()
 
     cards = [{"name": "card_1", "uid": "1234", "id": "abc"}]
     mocker.patch(
@@ -128,37 +128,36 @@
 @pytest.mark.asyncio
 async def test_connect(mocker: MockerFixture):
     mocker.patch('src.bluecurrent_api.websocket.Websocket._send')
     websocket = Websocket()
     api_token = '123'
 
     websocket._has_connection = True
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.connect(api_token)
 
 
 @pytest.mark.asyncio
 async def test__connect(mocker: MockerFixture):
     websocket = Websocket()
-
     mocker.patch.object(Websocket, '_connection')
     mocker.patch(
         'src.bluecurrent_api.websocket.connect',
         create=True,
         side_effect=ConnectionRefusedError
     )
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._connect()
 
     mocker.patch(
         'src.bluecurrent_api.websocket.connect',
         create=True,
         side_effect=TimeoutError
     )
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._connect()
 
     mocker.patch(
         'src.bluecurrent_api.websocket.connect',
         create=True,
         side_effect=InvalidStatusCode(
             403, {'x-websocket-reject-reason': 'Request limit reached'})
@@ -178,21 +177,21 @@
 
 @pytest.mark.asyncio
 async def test_send_request(mocker: MockerFixture):
     websocket = Websocket()
     mock_send = mocker.patch.object(Websocket, '_send')
 
     # without receiver
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.send_request({"command": "GET_CHARGE_POINTS"})
 
     websocket.receiver = mocker.Mock()
 
     # without token
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.send_request({"command": "GET_CHARGE_POINTS"})
 
     websocket.auth_token = '123'
 
     await websocket.send_request({"command": "GET_CHARGE_POINTS"})
 
     mock_send.assert_called_with(
@@ -307,52 +306,52 @@
     await websocket._message_handler()
     mock_handle_handle_session_messages.assert_called_with(message)
     mock_get_dummy_message.assert_called_with('BCU101')
 
     # no object
     message = {"value": True}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # unknown command
     message = {"error": 0, "object": "ERROR", "message": "Unknown command"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # unknown token
     message = {"error": 1, "object": "ERROR", "message": "Invalid Auth Token"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # token not autorized
     message = {"error": 2, "object": "ERROR", "message": "Not authorized"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # unknown error
     message = {"error": 9, "object": "ERROR", "message": "Unknown error"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # limit reached
     message = {"error": 42, "object": "ERROR",
                "message": "Request limit reached"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
     with pytest.raises(RequestLimitReached):
         await websocket._message_handler()
 
     # success false
     message = {"success": False, "error": "this is an error"}
     mocker.patch.object(Websocket, '_recv', return_value=message)
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket._message_handler()
 
     # None message
     message = None
     mocker.patch.object(Websocket, '_recv', return_value=message)
     assert await websocket._message_handler() == True
 
@@ -396,15 +395,15 @@
 
     test_close = mocker.patch(
         'src.bluecurrent_api.websocket.Websocket._connection.close',
         create=True,
         side_effect=AsyncMock()
     )
 
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         await websocket.disconnect()
 
     websocket._has_connection = True
     await websocket.disconnect()
     assert websocket._has_connection == False
     test_close.assert_called_once()
 
@@ -418,15 +417,15 @@
         Websocket, 'check_for_server_reject')
 
     websocket = Websocket()
 
     websocket._has_connection = True
     websocket.receive_event = asyncio.Event()
 
-    with pytest.raises(WebsocketException):
+    with pytest.raises(WebsocketError):
         websocket.handle_connection_errors(None)
 
     assert websocket._has_connection == False
     test_handle_receive_event.assert_called_once()
 
 
 @pytest.mark.asyncio
```

