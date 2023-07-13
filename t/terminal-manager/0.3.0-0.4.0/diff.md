# Comparing `tmp/terminal_manager-0.3.0.tar.gz` & `tmp/terminal_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.3.0.tar", last modified: Wed Jul 12 07:26:08 2023, max compression
+gzip compressed data, was "terminal_manager-0.4.0.tar", last modified: Thu Jul 13 06:57:09 2023, max compression
```

## Comparing `terminal_manager-0.3.0.tar` & `terminal_manager-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.3.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.3.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      704 2023-07-12 07:19:59.000000 terminal_manager-0.3.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.242628 terminal_manager-0.3.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.246628 terminal_manager-0.3.0/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5762 2023-07-12 06:44:51.000000 terminal_manager-0.3.0/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-12 03:52:34.000000 terminal_manager-0.3.0/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5085 2023-07-12 03:55:26.000000 terminal_manager-0.3.0/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-11 09:02:39.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1052 2023-07-12 06:44:13.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4115 2023-07-12 06:45:08.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4390 2023-07-12 06:45:18.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4272 2023-07-12 06:45:28.000000 terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-12 03:59:37.000000 terminal_manager-0.3.0/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-12 04:01:05.000000 terminal_manager-0.3.0/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-11 09:02:39.000000 terminal_manager-0.3.0/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8339 2023-07-12 04:08:12.000000 terminal_manager-0.3.0/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-12 04:05:10.000000 terminal_manager-0.3.0/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:26:08.250628 terminal_manager-0.3.0/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-12 07:26:08.000000 terminal_manager-0.3.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.4.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.4.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      704 2023-07-13 06:55:47.000000 terminal_manager-0.4.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.699058 terminal_manager-0.4.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.703058 terminal_manager-0.4.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     6526 2023-07-12 10:16:27.000000 terminal_manager-0.4.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5085 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.707058 terminal_manager-0.4.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1052 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4082 2023-07-13 06:40:49.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5192 2023-07-13 06:40:27.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5392 2023-07-13 06:40:07.000000 terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8339 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-12 08:15:06.000000 terminal_manager-0.4.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 06:57:09.703058 terminal_manager-0.4.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      679 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-13 06:57:09.000000 terminal_manager-0.4.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.3.0/LICENSE` & `terminal_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/PKG-INFO` & `terminal_manager-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: Control and monitor devices with terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.3.0/pyproject.toml` & `terminal_manager-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager/__init__.py` & `terminal_manager-0.4.0/src/terminal_manager/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .sensor import BinarySensor, NumberSensor, Sensor, TextSensor
 from .synchronizer import Synchronizer
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_NAME = "Manager"
 DEFAULT_COMMAND_TIMEOUT = 15
+DEFAULT_ALLOW_TURN_OFF = False
 
 
 @dataclass(frozen=True)
 class CommandOutput:
     timestamp: float
     stdout: list[str]
     stderr: list[str]
@@ -30,25 +31,27 @@
 
 class Manager(Collection, Synchronizer):
     def __init__(
         self,
         *,
         name: str = DEFAULT_NAME,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
+        allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
         collection: Collection | None = None,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         Synchronizer.__init__(self)
         Collection.__init__(
             self,
             name,
             collection.action_commands if collection else None,
             collection.sensor_commands if collection else None,
         )
         self.command_timeout = command_timeout
+        self.allow_turn_off = allow_turn_off
         self.logger = logger
 
     @property
     def hostname(self) -> str | None:
         if sensor := self.sensors_by_key.get(SensorKey.HOSTNAME):
             return sensor.last_known_value
 
@@ -182,7 +185,31 @@
             try:
                 await sensor.async_set(self, values[i])
             except (TypeError, ValueError, CommandError):
                 if raise_errors:
                     raise
 
         return await self.async_poll_sensors(keys, raise_errors=raise_errors)
+
+    async def async_turn_off(self) -> None:
+        """Turn off by running the `TURN_OFF` action.
+
+        Raises:
+            CommandError
+        """
+        if not (
+            ActionKey.TURN_OFF in self.action_commands_by_key and self.allow_turn_off
+        ):
+            return
+
+        await self.async_run_action(ActionKey.TURN_OFF)
+
+    async def async_restart(self) -> None:
+        """Restart by running the `RESTART` action.
+
+        Raises:
+            CommandError
+        """
+        if not ActionKey.RESTART in self.action_commands_by_key:
+            return
+
+        await self.async_run_action(ActionKey.RESTART)
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager/collection.py` & `terminal_manager-0.4.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager/command.py` & `terminal_manager-0.4.0/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.4.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.4.0/src/terminal_manager/default_collections/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     SensorKey.FREE_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
             "df -k | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
-            interval=300,
+            interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
                     unit="KiB",
@@ -118,15 +118,14 @@
             "echo $(($(cat /sys/class/thermal/thermal_zone0/temp) / 1000))",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
-                    float=True,
                 )
             ],
         ),
         SensorCommand(
             "ps -e --no-headers | wc -l",
             interval=60,
             sensors=[
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,39 @@
         ActionCommand(
             "shutdown -r -t 0",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
-        # TODO: MAC_ADDRESS
         # TODO: WAKE_ON_LAN
-        # TODO: INTERFACE
         SensorCommand(
-            "for /f \"skip=1 tokens=*\" %i in ('wmic ComputerSystem get SystemType') "
-            + "do @echo %i",
+            "for /f %i in ('wmic path win32_ip4routetable "
+            + "where \"Destination='0.0.0.0'\" "
+            + "get InterfaceIndex ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') do '
+            + '@for /f "skip=2 tokens=2,3 delims=," %j in (\'wmic nic '
+            + 'where "InterfaceIndex=%i" '
+            + "get MACAddress^, NetConnectionID /format:csv') do "
+            + "@echo %j & @echo %k",
+            sensors=[
+                TextSensor(
+                    SensorName.MAC_ADDRESS,
+                    SensorKey.MAC_ADDRESS,
+                ),
+                TextSensor(
+                    SensorName.INTERFACE,
+                    SensorKey.INTERFACE,
+                ),
+            ],
+        ),
+        SensorCommand(
+            'for /f "skip=1 tokens=*" %i in (\'wmic ComputerSystem '
+            + "get SystemType') do "
+            + "@echo %i",
             sensors=[
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
@@ -64,40 +83,44 @@
                 TextSensor(
                     SensorName.OS_ARCHITECTURE,
                     SensorKey.OS_ARCHITECTURE,
                 ),
             ],
         ),
         SensorCommand(
-            "for /f \"skip=1\" %i in ('wmic ComputerSystem get TotalPhysicalMemory') "
-            + "do @echo %i",
+            'for /f "skip=1" %i in (\'wmic ComputerSystem '
+            + "get TotalPhysicalMemory') do "
+            + "@echo %i",
             sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
                     unit="B",
                 ),
             ],
         ),
         SensorCommand(
-            "for /f \"skip=1\" %i in ('wmic OS get FreePhysicalMemory') do @echo %i",
+            'for /f "skip=1" %i in (\'wmic OS '
+            + "get FreePhysicalMemory') do "
+            + "@echo %i",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
                     unit="kB",
                 ),
             ],
         ),
         SensorCommand(
-            'for /f "tokens=1,2" %i in (\'wmic LogicalDisk get DeviceID^, FreeSpace ^| '
-            + 'findstr ":"\') '
-            + "do @echo %i^|%j",
-            interval=300,
+            'for /f "tokens=1,2" %i in (\'wmic LogicalDisk '
+            + "get DeviceID^, FreeSpace ^| "
+            + 'findstr ":"\') do '
+            + "@echo %i^|%j",
+            interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
                     unit="B",
@@ -113,29 +136,31 @@
                     SensorKey.CPU_LOAD,
                     unit="%",
                 ),
             ],
         ),
         SensorCommand(
             "for /f %i in ('wmic /namespace:\\\\root\\wmi "
-            + "PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature ^| "
-            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-            + "do @set /a x=(%i - 2732) / 10",
+            + "path MSAcpi_ThermalZoneTemperature "
+            + "get CurrentTemperature ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') do '
+            + "@set /a x=(%i - 2732) / 10",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
-                    float=True,
                 )
             ],
         ),
         SensorCommand(
-            'wmic process get processId | findstr /r "\\<[0-9][0-9]*\\>" | find /c /v ""',
+            "wmic process get processId | "
+            + 'findstr /r "\\<[0-9][0-9]*\\>" | '
+            + 'find /c /v ""',
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.PROCESSES,
                     SensorKey.PROCESSES,
                 )
             ],
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.4.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..collection import Collection
 from ..command import ActionCommand, SensorCommand
-from ..sensor import NumberSensor, TextSensor
+from ..sensor import BinarySensor, NumberSensor, TextSensor
 from .const import ActionKey, ActionName, SensorKey, SensorName
 
 windows_ps = Collection(
     "Windows (Power Shell)",
     [
         ActionCommand(
             "Stop-Computer -Force",
@@ -14,39 +14,70 @@
         ActionCommand(
             "Restart-Computer -Force",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
-        # TODO: MAC_ADDRESS
-        # TODO: WAKE_ON_LAN
-        # TODO: INTERFACE
+        SensorCommand(
+            "$x = Get-NetAdapterPowerManagement "
+            + '-Name "{interface}" | '
+            + "Select WakeOnMagicPacket; "
+            + "$x.WakeOnMagicPacket",
+            sensors=[
+                BinarySensor(
+                    SensorName.WAKE_ON_LAN,
+                    SensorKey.WAKE_ON_LAN,
+                    payload_on="enabled",
+                )
+            ],
+        ),
+        SensorCommand(
+            "$y = Get-CimInstance Win32_IP4RouteTable "
+            + "-Filter \"Destination='0.0.0.0'\" | "
+            + "Select InterfaceIndex; "
+            + "$x = Get-CimInstance Win32_NetworkAdapter "
+            + "-Property NetConnectionID, InterfaceIndex, MACAddress "
+            + '-Filter "InterfaceIndex=$($y.InterfaceIndex)" | '
+            + "Select MACAddress, NetConnectionID; "
+            + "$x.MACAddress; "
+            + "$x.NetConnectionID",
+            sensors=[
+                TextSensor(
+                    SensorName.MAC_ADDRESS,
+                    SensorKey.MAC_ADDRESS,
+                ),
+                TextSensor(
+                    SensorName.INTERFACE,
+                    SensorKey.INTERFACE,
+                ),
+            ],
+        ),
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
-            + "Select Name, SystemType;"
-            + "$x.Name;"
-            + "$x.SystemType;",
+            + "Select Name, SystemType; "
+            + "$x.Name; "
+            + "$x.SystemType",
             sensors=[
                 TextSensor(
                     SensorName.HOSTNAME,
                     SensorKey.HOSTNAME,
                 ),
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_OperatingSystem | "
-            + "Select Caption, Version, OSArchitecture;"
-            + "$x.Caption;"
-            + "$x.Version;"
-            + "$x.OSArchitecture;",
+            + "Select Caption, Version, OSArchitecture; "
+            + "$x.Caption; "
+            + "$x.Version; "
+            + "$x.OSArchitecture",
             sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
                 ),
                 TextSensor(
                     SensorName.OS_VERSION,
@@ -56,77 +87,76 @@
                     SensorName.OS_ARCHITECTURE,
                     SensorKey.OS_ARCHITECTURE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
-            + "Select TotalPhysicalMemory;"
-            + "$x.TotalPhysicalMemory;",
+            + "Select TotalPhysicalMemory; "
+            + "$x.TotalPhysicalMemory",
             sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
                     unit="B",
                 )
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_OperatingSystem | "
-            + "Select FreePhysicalMemory;"
-            + "$x.FreePhysicalMemory;",
+            + "Select FreePhysicalMemory; "
+            + "$x.FreePhysicalMemory",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
                     unit="kB",
                 )
             ],
         ),
         SensorCommand(
             "Get-CimInstance Win32_LogicalDisk | "
             + "Select DeviceID, FreeSpace | ForEach-Object "
             + '{{$_.DeviceID + "|" + $_.FreeSpace}}',
-            interval=300,
+            interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
                     unit="B",
                 )
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_Processor | "
-            + "Select LoadPercentage;"
-            + "$x.LoadPercentage;",
+            + "Select LoadPercentage; "
+            + "$x.LoadPercentage",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
                 )
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance msacpi_thermalzonetemperature "
             + '-namespace "root/wmi" | '
-            + "Select CurrentTemperature;"
-            + "($x.CurrentTemperature - 2732) / 10;",
+            + "Select CurrentTemperature; "
+            + "($x.CurrentTemperature - 2732) / 10",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
-                    float=True,
                 )
             ],
         ),
         SensorCommand(
             "Get-Process | Measure | ForEach-Object {$_.Count}",
             interval=60,
             sensors=[
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager/event.py` & `terminal_manager-0.4.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager/sensor.py` & `terminal_manager-0.4.0/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager/synchronizer.py` & `terminal_manager-0.4.0/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.3.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.4.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: Control and monitor devices with terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.3.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.4.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

