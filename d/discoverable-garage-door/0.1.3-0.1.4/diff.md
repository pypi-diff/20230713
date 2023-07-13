# Comparing `tmp/discoverable_garage_door-0.1.3.tar.gz` & `tmp/discoverable_garage_door-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoverable_garage_door-0.1.3.tar", max compression
+gzip compressed data, was "discoverable_garage_door-0.1.4.tar", max compression
```

## Comparing `discoverable_garage_door-0.1.3.tar` & `discoverable_garage_door-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.3/LICENSE
--rw-r--r--   0        0        0     4359 2023-07-10 16:03:23.211414 discoverable_garage_door-0.1.3/README.md
--rw-r--r--   0        0        0      455 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.3/discoverable_garage_door/.config.yaml
--rw-r--r--   0        0        0      157 2023-07-07 01:12:50.933164 discoverable_garage_door-0.1.3/discoverable_garage_door/__init__.py
--rw-r--r--   0        0        0      801 2023-07-07 01:13:37.469035 discoverable_garage_door-0.1.3/discoverable_garage_door/__main__.py
--rw-r--r--   0        0        0     2857 2023-07-05 15:08:13.229050 discoverable_garage_door-0.1.3/discoverable_garage_door/config.py
--rw-r--r--   0        0        0     3013 2023-07-05 15:08:13.161050 discoverable_garage_door-0.1.3/discoverable_garage_door/cover.py
--rw-r--r--   0        0        0      439 2023-07-05 15:01:59.975398 discoverable_garage_door-0.1.3/discoverable_garage_door/logging.conf
--rw-r--r--   0        0        0      333 2023-07-05 15:08:12.673053 discoverable_garage_door-0.1.3/discoverable_garage_door/util.py
--rw-r--r--   0        0        0      410 2023-07-10 16:02:55.827602 discoverable_garage_door-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 discoverable_garage_door-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 15:01:59.971398 discoverable_garage_door-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4562 2023-07-11 16:56:08.832906 discoverable_garage_door-0.1.4/README.md
+-rw-r--r--   0        0        0      455 2023-07-13 00:40:17.470098 discoverable_garage_door-0.1.4/discoverable_garage_door/.config.yaml
+-rw-r--r--   0        0        0      157 2023-07-11 15:49:02.578942 discoverable_garage_door-0.1.4/discoverable_garage_door/__init__.py
+-rw-r--r--   0        0        0      863 2023-07-13 00:40:17.474098 discoverable_garage_door-0.1.4/discoverable_garage_door/__main__.py
+-rw-r--r--   0        0        0     2859 2023-07-13 00:40:17.474098 discoverable_garage_door-0.1.4/discoverable_garage_door/config.py
+-rw-r--r--   0        0        0      349 2023-07-13 00:41:36.617642 discoverable_garage_door-0.1.4/discoverable_garage_door/contacts.py
+-rw-r--r--   0        0        0     6123 2023-07-13 00:41:37.741636 discoverable_garage_door-0.1.4/discoverable_garage_door/cover.py
+-rw-r--r--   0        0        0      889 2023-07-13 00:41:36.825641 discoverable_garage_door-0.1.4/discoverable_garage_door/door.py
+-rw-r--r--   0        0        0     1669 2023-07-13 00:41:37.089639 discoverable_garage_door-0.1.4/discoverable_garage_door/gpio.py
+-rw-r--r--   0        0        0      439 2023-07-11 15:27:20.093083 discoverable_garage_door-0.1.4/discoverable_garage_door/logging.conf
+-rw-r--r--   0        0        0      333 2023-07-11 15:49:02.586942 discoverable_garage_door-0.1.4/discoverable_garage_door/util.py
+-rw-r--r--   0        0        0      410 2023-07-11 15:49:19.211037 discoverable_garage_door-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 discoverable_garage_door-0.1.4/PKG-INFO
```

### Comparing `discoverable_garage_door-0.1.3/LICENSE` & `discoverable_garage_door-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discoverable_garage_door-0.1.3/README.md` & `discoverable_garage_door-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
   - [installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
   - [Format](#format)
 - [Version History](#version-history)
   - [Version 0.1.1 - Complete build config](#version-011---complete-build-config)
   - [Version 0.1.2 - Add Lovelace UI exampe](#version-012---add-lovelace-ui-exampe)
+  - [Version 0.1.3 - Rename logger.conf](#version-013---rename-loggerconf)
+  - [Version 0.1.4 - Get test bed operating](#version-014---get-test-bed-operating)
 - [Uses ha-mqtt-discoverable](#uses-ha-mqtt-discoverable)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Requirements
 
 ### Raspberry PI
 
@@ -94,10 +96,12 @@
 
 ### Version 0.1.1 - Complete build config
 
 ### Version 0.1.2 - Add Lovelace UI exampe
 
 ### Version 0.1.3 - Rename logger.conf
 
+### Version 0.1.4 - Get test bed operating
+
 ## Uses ha-mqtt-discoverable
 
 - [ha-mqtt-discoverable-cli](https://github.com/unixorn/ha-mqtt-discoverable-cli)
```

### Comparing `discoverable_garage_door-0.1.3/discoverable_garage_door/__main__.py` & `discoverable_garage_door-0.1.4/discoverable_garage_door/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import signal
 from .util import logger
 
 from ha_mqtt_discoverable import Settings, __version__
 
 from discoverable_garage_door.config import Config, config
 from discoverable_garage_door.cover import CoverInfo, Cover, Settings
+from discoverable_garage_door.gpio import Gpio
 
-print(__version__)
-sys.exit(0)
 mqtt_settings = Settings.MQTT(
     host=config.mqtt_broker.host,
     username=config.mqtt_broker.username,
     password=config.mqtt_broker.password,
     discovery_prefix=config.mqtt_broker.discovery_prefix,
     state_prefix=config.mqtt_broker.state_prefix,
 )
@@ -24,7 +23,9 @@
         Cover.cover(mqtt=mqtt_settings, gpio_config=config.gpio, door_config=door)
     )
 
 try:
     signal.pause()
 except KeyboardInterrupt:
     print("\nStopping ...")
+    for door in doors:
+        door.cleanup()
```

### Comparing `discoverable_garage_door-0.1.3/discoverable_garage_door/config.py` & `discoverable_garage_door-0.1.4/discoverable_garage_door/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
     host: str = "hastings.attlocal.net"
     username: str = "homeassistant"
     password: str = ""
     discovery_prefix: str = "homeassistant"
     state_prefix: str = "hmd"
 
 
-class Door(BaseModel):
+class DoorInfo(BaseModel):
     name: str = "My Door"
     button_pin: int = 18
     opened_contact_pin: int = 27
     closed_contact_pin: int = 17
 
 
-class GPIO(BaseModel):
+class GpioInfo(BaseModel):
     button_push_duration_ms: int = 500
     contact_bounce_time_ms: int = 200
     contact_pullup: bool = True
-    doors: list["Door"] = []
+    doors: list["DoorInfo"] = []
 
 
 class Config(YamlModel):
     mqtt_broker: MQTT = MQTT()
-    gpio: GPIO = GPIO()
+    gpio: GpioInfo = GpioInfo()
 
     @staticmethod
     def _readfile(filepath) -> Config:
         config_file = abspath(filepath)
         logger.debug(f"importing logfile from file: {config_file}")
         with open(config_file, "r", encoding="utf-8") as f:
             return Config.parse_raw(f.read(), proto="yaml")
@@ -60,17 +60,16 @@
                 config = Config._readfile(config_file)
             else:
                 config_file = abspath(dirname(__file__) + "/.config.yaml")
                 if isfile(config_file) and exists(config_file):
                     config = Config._readfile(config_file)
                 else:
                     config = Config()
-        print(config)
         if len(config.gpio.doors) == 0:
-            config.gpio.doors.append(Door())
+            config.gpio.doors.append(DoorInfo())
         return config
 
     @staticmethod
     def config() -> Config:
         config_filepath: str = None
         if "config" in environ:
             config_filepath = environ["config"]
```

### Comparing `discoverable_garage_door-0.1.3/PKG-INFO` & `discoverable_garage_door-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discoverable-garage-door
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Tim Daley
 Author-email: timdaley@earthling.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ha-mqtt-discoverable (>=0.9.0,<0.10.0)
@@ -32,14 +32,16 @@
   - [installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
   - [Format](#format)
 - [Version History](#version-history)
   - [Version 0.1.1 - Complete build config](#version-011---complete-build-config)
   - [Version 0.1.2 - Add Lovelace UI exampe](#version-012---add-lovelace-ui-exampe)
+  - [Version 0.1.3 - Rename logger.conf](#version-013---rename-loggerconf)
+  - [Version 0.1.4 - Get test bed operating](#version-014---get-test-bed-operating)
 - [Uses ha-mqtt-discoverable](#uses-ha-mqtt-discoverable)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Requirements
 
 ### Raspberry PI
 
@@ -108,11 +110,13 @@
 
 ### Version 0.1.1 - Complete build config
 
 ### Version 0.1.2 - Add Lovelace UI exampe
 
 ### Version 0.1.3 - Rename logger.conf
 
+### Version 0.1.4 - Get test bed operating
+
 ## Uses ha-mqtt-discoverable
 
 - [ha-mqtt-discoverable-cli](https://github.com/unixorn/ha-mqtt-discoverable-cli)
```

