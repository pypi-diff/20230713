# Comparing `tmp/terminal_manager-0.4.0.tar.gz` & `tmp/terminal_manager-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.4.0.tar", last modified: Thu Jul 13 06:57:09 2023, max compression
+gzip compressed data, was "terminal_manager-0.5.0.tar", last modified: Thu Jul 13 09:55:54 2023, max compression
```

## Comparing `terminal_manager-0.4.0.tar` & `terminal_manager-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.4.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.4.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      704 2023-07-13 06:55:47.000000 terminal_manager-0.4.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.699058 terminal_manager-0.4.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.703058 terminal_manager-0.4.0/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6526 2023-07-12 10:16:27.000000 terminal_manager-0.4.0/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5085 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1052 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4082 2023-07-13 06:40:49.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5192 2023-07-13 06:40:27.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5392 2023-07-13 06:40:07.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8339 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.703058 terminal_manager-0.4.0/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.545664 terminal_manager-0.5.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.5.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.5.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-13 09:45:59.000000 terminal_manager-0.5.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 09:55:54.545664 terminal_manager-0.5.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.537665 terminal_manager-0.5.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6542 2023-07-13 07:25:37.000000 terminal_manager-0.5.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5082 2023-07-13 09:29:31.000000 terminal_manager-0.5.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-13 07:25:10.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4114 2023-07-13 07:26:17.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5208 2023-07-13 07:28:16.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5418 2023-07-13 08:58:44.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8336 2023-07-13 09:29:54.000000 terminal_manager-0.5.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.4.0/LICENSE` & `terminal_manager-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.4.0/PKG-INFO` & `terminal_manager-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.4.0
-Summary: Control and monitor devices with terminal commands
+Version: 0.5.0
+Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `terminal_manager-0.4.0/pyproject.toml` & `terminal_manager-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
-description = "Control and monitor devices with terminal commands"
+description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/__init__.py` & `terminal_manager-0.5.0/src/terminal_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 
     @property
     def machine_type(self) -> str | None:
         if sensor := self.sensors_by_key.get(SensorKey.MACHINE_TYPE):
             return sensor.last_known_value
 
     @property
-    def interface(self) -> str | None:
-        if sensor := self.sensors_by_key.get(SensorKey.INTERFACE):
+    def network_interface(self) -> str | None:
+        if sensor := self.sensors_by_key.get(SensorKey.NETWORK_INTERFACE):
             return sensor.last_known_value
 
     @property
     def mac_address(self) -> str | None:
         if sensor := self.sensors_by_key.get(SensorKey.MAC_ADDRESS):
             return sensor.last_known_value
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/collection.py` & `terminal_manager-0.5.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.4.0/src/terminal_manager/command.py` & `terminal_manager-0.5.0/src/terminal_manager/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,24 +80,24 @@
 
         Raises:
             CommandError
         """
         try:
             string = await self.async_format(manager, variables)
         except CommandError as exc:
-            manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
+            manager.logger.info("%s: %s => %s", manager.name, self.string, exc)
             raise
 
         try:
             output = await manager.async_execute_command_string(string, self.timeout)
         except CommandError as exc:
-            manager.logger.debug("%s: %s => %s", manager.name, string, exc)
+            manager.logger.info("%s: %s => %s", manager.name, string, exc)
             raise
 
-        manager.logger.debug(
+        manager.logger.info(
             "%s: %s => %s, %s, %s",
             manager.name,
             string,
             output.stdout,
             output.stderr,
             output.code,
         )
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.5.0/src/terminal_manager/default_collections/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class ActionName:
     TURN_OFF = "Turn off"
     RESTART = "Restart"
 
 
 class SensorKey:
-    INTERFACE = "interface"
+    NETWORK_INTERFACE = "network_interface"
     MAC_ADDRESS = "mac_address"
     WAKE_ON_LAN = "wake_on_lan"
     MACHINE_TYPE = "machine_type"
     HOSTNAME = "hostname"
     OS_NAME = "os_name"
     OS_VERSION = "os_version"
     OS_ARCHITECTURE = "os_architecture"
@@ -22,15 +22,15 @@
     CPU_LOAD = "cpu_load"
     FREE_DISK_SPACE = "free_disk_space"
     TEMPERATURE = "temperature"
     PROCESSES = "processes"
 
 
 class SensorName:
-    INTERFACE = "Interface"
+    NETWORK_INTERFACE = "Network Interface"
     MAC_ADDRESS = "MAC Address"
     WAKE_ON_LAN = "Wake on LAN"
     MACHINE_TYPE = "Machine Type"
     HOSTNAME = "Hostname"
     OS_NAME = "OS Name"
     OS_VERSION = "OS Version"
     OS_ARCHITECTURE = "OS Architecture"
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.5.0/src/terminal_manager/default_collections/linux.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,39 +15,39 @@
             "/sbin/shutdown -r now",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         SensorCommand(
-            "cat /sys/class/net/{interface}/address",
+            "cat /sys/class/net/{network_interface}/address",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 )
             ],
         ),
         SensorCommand(
-            "file=/sys/class/net/{interface}/device/power/wakeup; "
+            "file=/sys/class/net/{network_interface}/device/power/wakeup; "
             + "[[ ! -f $file ]] || cat $file",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
                     payload_on="enabled",
                 )
             ],
         ),
         SensorCommand(
             "/sbin/route -n | awk '/^0.0.0.0/ {{print $NF}}'",
             sensors=[
                 TextSensor(
-                    SensorName.INTERFACE,
-                    SensorKey.INTERFACE,
+                    SensorName.NETWORK_INTERFACE,
+                    SensorKey.NETWORK_INTERFACE,
                 )
             ],
         ),
         SensorCommand(
             "uname -a | awk '{{print $1; print $2; print $3; print $(NF-1)}}'",
             sensors=[
                 TextSensor(
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
             + "@echo %j & @echo %k",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 ),
                 TextSensor(
-                    SensorName.INTERFACE,
-                    SensorKey.INTERFACE,
+                    SensorName.NETWORK_INTERFACE,
+                    SensorKey.NETWORK_INTERFACE,
                 ),
             ],
         ),
         SensorCommand(
             'for /f "skip=1 tokens=*" %i in (\'wmic ComputerSystem '
             + "get SystemType') do "
             + "@echo %i",
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         SensorCommand(
             "$x = Get-NetAdapterPowerManagement "
-            + '-Name "{interface}" | '
+            + '-Name "{network_interface}" | '
             + "Select WakeOnMagicPacket; "
             + "$x.WakeOnMagicPacket",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
-                    payload_on="enabled",
+                    payload_on="Enabled",
                 )
             ],
         ),
         SensorCommand(
             "$y = Get-CimInstance Win32_IP4RouteTable "
             + "-Filter \"Destination='0.0.0.0'\" | "
             + "Select InterfaceIndex; "
@@ -43,16 +43,16 @@
             + "$x.NetConnectionID",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 ),
                 TextSensor(
-                    SensorName.INTERFACE,
-                    SensorKey.INTERFACE,
+                    SensorName.NETWORK_INTERFACE,
+                    SensorKey.NETWORK_INTERFACE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
             + "Select Name, SystemType; "
             + "$x.Name; "
@@ -153,15 +153,15 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                 )
             ],
         ),
         SensorCommand(
-            "Get-Process | Measure | ForEach-Object {$_.Count}",
+            "Get-Process | Measure | ForEach-Object {{$_.Count}}",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.PROCESSES,
                     SensorKey.PROCESSES,
                 )
             ],
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/event.py` & `terminal_manager-0.5.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.4.0/src/terminal_manager/sensor.py` & `terminal_manager-0.5.0/src/terminal_manager/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,29 +68,29 @@
         return value_string
 
     def _validate(self, value: Any) -> None:
         ...
 
     def _update_value(self, manager: Manager, data: str | None) -> None:
         if data is None:
-            manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
+            manager.logger.info("%s: %s => %s", manager.name, self.key, self.value)
             self.value = None
             return
 
         try:
             value_string = self._render(data)
             value = self._convert(value_string)
             self._validate(value)
         except Exception as exc:  # pylint: disable=broad-except
-            manager.logger.debug("%s: %s => %s", manager.name, self.key, exc)
+            manager.logger.info("%s: %s => %s", manager.name, self.key, exc)
             self.value = None
             return
 
         self.value = self.last_known_value = value
-        manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
+        manager.logger.info("%s: %s => %s", manager.name, self.key, self.value)
 
     def _update_child_sensors(self, manager: Manager, data: list[str] | None) -> None:
         if data is None:
             for child in self.child_sensors:
                 child.update(manager, None)
             return
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager/synchronizer.py` & `terminal_manager-0.5.0/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.4.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.5.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.4.0
-Summary: Control and monitor devices with terminal commands
+Version: 0.5.0
+Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `terminal_manager-0.4.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.5.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

