# Comparing `tmp/ssh_terminal_manager-0.3.0.tar.gz` & `tmp/ssh_terminal_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.3.0.tar", last modified: Wed Jul 12 07:53:03 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.4.0.tar", last modified: Thu Jul 13 07:01:07 2023, max compression
```

## Comparing `ssh_terminal_manager-0.3.0.tar` & `ssh_terminal_manager-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.3.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.3.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      797 2023-07-12 07:27:33.000000 ssh_terminal_manager-0.3.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-12 07:53:03.344616 ssh_terminal_manager-0.3.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     9137 2023-07-12 06:56:45.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-12 03:59:09.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-12 07:53:03.340616 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-12 07:53:03.000000 ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.4.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.4.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      797 2023-07-13 07:00:04.000000 ssh_terminal_manager-0.4.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.459457 ssh_terminal_manager-0.4.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.459457 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8400 2023-07-12 10:33:18.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-12 08:15:06.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 07:01:07.463457 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      815 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-13 07:01:07.000000 ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.3.0/LICENSE` & `ssh_terminal_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.3.0/PKG-INFO` & `ssh_terminal_manager-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.3.0/pyproject.toml` & `ssh_terminal_manager-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with SSH terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,14 +20,14 @@
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.3.0",
+  "terminal-manager >= 0.4.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.3.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.4.0/src/ssh_terminal_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 from time import time
 
 import icmplib
 import paramiko
 import wakeonlan
 from terminal_manager import (
+    DEFAULT_ALLOW_TURN_OFF,
     DEFAULT_COMMAND_TIMEOUT,
     ActionCommand,
     BinarySensor,
     Collection,
     Command,
     CommandError,
     CommandOutput,
@@ -27,22 +28,21 @@
 from terminal_manager.default_collections import ActionKey, SensorKey
 
 from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("echo ''")
 
+ONLINE = "online"
+CONNECTED = "connected"
+
 DEFAULT_PORT = 22
 DEFAULT_PING_TIMEOUT = 4
 DEFAULT_SSH_TIMEOUT = 4
 DEFAULT_ADD_HOST_KEYS = False
-DEFAULT_ALLOW_TURN_OFF = False
-
-ONLINE = "online"
-CONNECTED = "connected"
 
 
 class CustomRejectPolicy(paramiko.MissingHostKeyPolicy):
     def missing_host_key(
         self, client: paramiko.SSHClient, hostname: str, key: paramiko.PKey
     ) -> None:
         raise SSHHostKeyUnknownError("Host key is unknown")
@@ -67,15 +67,14 @@
 
 class SSHManager(Manager):
     def __init__(
         self,
         host: str,
         *,
         name: str | None = None,
-        mac_address: str | None = None,
         port: int = DEFAULT_PORT,
         username: str | None = None,
         password: str | None = None,
         key_filename: str | None = None,
         host_keys_filename: str | None = None,
         add_host_keys: bool = DEFAULT_ADD_HOST_KEYS,
         allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
@@ -84,43 +83,41 @@
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
         collection: Collection | None = None,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         super().__init__(
             name=name or host,
             command_timeout=command_timeout,
+            allow_turn_off=allow_turn_off,
             collection=collection,
             logger=logger,
         )
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.key_filename = key_filename
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
-        self.allow_turn_off = allow_turn_off
-        self._mac_address = mac_address
+        self._mac_address = None
         self.state = State(self)
         self.client = paramiko.SSHClient()
         self.client.load_system_host_keys()
         self.client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
 
         if host_keys_filename:
             with open(host_keys_filename, "a", encoding="utf-8"):
                 pass
             self.client.load_host_keys(host_keys_filename)
 
     @property
     def mac_address(self) -> str | None:
-        if self._mac_address:
-            return self._mac_address
-        return super().mac_address
+        return self._mac_address or super().mac_address
 
     def _execute_command_string(self, string: str, timeout: int) -> CommandOutput:
         if not self.state.connected:
             raise CommandError("Not connected")
 
         try:
             stdin, stdout, stderr = self.client.exec_command(
@@ -257,39 +254,15 @@
             await self.async_connect()
         except SSHConnectError:
             if raise_errors:
                 raise
 
     async def async_turn_on(self) -> None:
         """Turn on by Wake on LAN."""
-        if self.state.online or self.mac_address is None:
+        if self.mac_address is None:
             return
 
         wakeonlan.send_magic_packet(self.mac_address)
 
-    async def async_turn_off(self) -> None:
-        """Turn off by running the `TURN_OFF` action.
-
-        Raises:
-            CommandError
-        """
-        if not (
-            self.state.connected
-            and self.allow_turn_off
-            and ActionKey.TURN_OFF in self.action_commands_by_key
-        ):
-            return
-
-        await self.async_run_action(ActionKey.TURN_OFF)
-
-    async def async_restart(self) -> None:
-        """Restart by running the `RESTART` action.
-
-        Raises:
-            CommandError
-        """
-        if not (
-            self.state.connected and ActionKey.RESTART in self.action_commands_by_key
-        ):
-            return
-
-        await self.async_run_action(ActionKey.RESTART)
+    def set_mac_address(self, mac_address: str | None) -> None:
+        """Set the MAC address."""
+        self._mac_address = mac_address
```

### Comparing `ssh_terminal_manager-0.3.0/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.4.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.3.0
+Version: 0.4.0
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

