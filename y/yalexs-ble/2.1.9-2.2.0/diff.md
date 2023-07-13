# Comparing `tmp/yalexs_ble-2.1.9.tar.gz` & `tmp/yalexs_ble-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs_ble-2.1.9.tar", max compression
+gzip compressed data, was "yalexs_ble-2.2.0.tar", max compression
```

## Comparing `yalexs_ble-2.1.9.tar` & `yalexs_ble-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-03-26 21:19:09.562610 yalexs_ble-2.1.9/LICENSE
--rw-r--r--   0        0        0     3663 2023-03-26 21:19:09.562610 yalexs_ble-2.1.9/README.md
--rw-r--r--   0        0        0     2398 2023-03-26 21:19:10.358600 yalexs_ble-2.1.9/pyproject.toml
--rw-r--r--   0        0        0      871 2023-03-26 21:19:10.310600 yalexs_ble-2.1.9/src/yalexs_ble/__init__.py
--rw-r--r--   0        0        0     2225 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/const.py
--rw-r--r--   0        0        0    15275 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/lock.py
--rw-r--r--   0        0        0    32249 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/push.py
--rw-r--r--   0        0        0        0 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/py.typed
--rw-r--r--   0        0        0     2308 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/secure_session.py
--rw-r--r--   0        0        0     9539 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/session.py
--rw-r--r--   0        0        0     2642 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/util.py
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 yalexs_ble-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3663 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/README.md
+-rw-r--r--   0        0        0     2419 2023-07-13 04:55:24.387369 yalexs_ble-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      871 2023-07-13 04:55:24.359368 yalexs_ble-2.2.0/src/yalexs_ble/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/const.py
+-rw-r--r--   0        0        0    16785 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/lock.py
+-rw-r--r--   0        0        0    39986 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/push.py
+-rw-r--r--   0        0        0        0 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/py.typed
+-rw-r--r--   0        0        0     2324 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/secure_session.py
+-rw-r--r--   0        0        0    10542 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/session.py
+-rw-r--r--   0        0        0     2642 2023-07-13 04:55:23.411349 yalexs_ble-2.2.0/src/yalexs_ble/util.py
+-rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 yalexs_ble-2.2.0/PKG-INFO
```

### Comparing `yalexs_ble-2.1.9/LICENSE` & `yalexs_ble-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.9/README.md` & `yalexs_ble-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.9/pyproject.toml` & `yalexs_ble-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yalexs-ble"
-version = "2.1.9"
+version = "2.2.0"
 description = "Bluetooth control of Yale and August locks"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/yalexs-ble"
 documentation = "https://yalexs-ble.readthedocs.io"
 classifiers = [
@@ -29,14 +29,15 @@
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 bleak = ">=0.19.0"
 bleak-retry-connector = ">=2.9.0"
 async-timeout = ">=3.0.1"
 cryptography = ">=38.0.0"
+lru-dict = ">=1.1.4"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/__init__.py` & `yalexs_ble-2.2.0/src/yalexs_ble/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     local_name_is_unique,
     local_name_to_serial,
     serial_to_local_name,
     unique_id_from_device_adv,
     unique_id_from_local_name_address,
 )
 
-__version__ = "2.1.9"
+__version__ = "2.2.0"
 
 __all__ = [
     "AuthError",
     "ConnectionInfo",
     "DisconnectedError",
     "DoorStatus",
     "Lock",
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/const.py` & `yalexs_ble-2.2.0/src/yalexs_ble/const.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/lock.py` & `yalexs_ble-2.2.0/src/yalexs_ble/lock.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     SERIAL_NUMBER_CHARACTERISTIC,
     VALUE_TO_DOOR_STATUS,
     VALUE_TO_LOCK_STATUS,
     BatteryState,
     Commands,
     DoorStatus,
     LockInfo,
-    LockState,
     LockStatus,
 )
 from .secure_session import SecureSession
 from .session import AuthError, DisconnectedError, Session
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -100,43 +99,50 @@
         keyString: str,
         keyIndex: int,
         name: str,
         state_callback: Callable[
             [Iterable[LockStatus | DoorStatus | BatteryState]], None
         ],
         info: LockInfo | None = None,
+        disconnect_callback: Callable[[], None] | None = None,
     ) -> None:
         self.ble_device_callback = ble_device_callback
         self.key = bytes.fromhex(keyString)
         self.key_index = keyIndex
         self.name = name
         self.session: Session | None = None
         self.secure_session: SecureSession | None = None
         self.is_secure = False
         self._lock = asyncio.Lock()
         self._lock_info = info
         self.client: BleakClientWithServiceCache | None = None
-        self._disconnected_event: asyncio.Event | None = None
         self._state_callback = state_callback
+        self._disconnected = False
+        self._disconnect_callback = disconnect_callback
+        self._disconnected_futures: set[asyncio.Future[None]] = set()
 
     def set_name(self, name: str) -> None:
         self.name = name
 
     def disconnected(self, *args: Any, **kwargs: Any) -> None:
         _LOGGER.debug("%s: Disconnected from lock callback", self.name)
-        assert self._disconnected_event is not None  # nosec
-        self._disconnected_event.set()
+        self._disconnected = True
+        for future in self._disconnected_futures:
+            if not future.done():
+                future.set_result(None)
+        self._disconnected_futures.clear()
+        if self._disconnect_callback:
+            self._disconnect_callback()
 
     async def connect(self) -> None:
         """Connect to the lock."""
         _LOGGER.debug(
             "%s: Connecting to the lock",
             self.name,
         )
-        self._disconnected_event = asyncio.Event()
         try:
             self.client = await establish_connection(
                 BleakClientWithServiceCache,
                 self.ble_device_callback(),
                 self.name,
                 self.disconnected,
                 use_services_cache=True,
@@ -147,19 +153,23 @@
             raise err
         _LOGGER.debug("%s: Connected", self.name)
 
         self.session = Session(
             self.client,
             self.name,
             self._lock,
-            self._disconnected_event,
+            self._disconnected_futures,
             self._internal_state_callback,
         )
         self.secure_session = SecureSession(
-            self.client, self.name, self._lock, self._disconnected_event, self.key_index
+            self.client,
+            self.name,
+            self._lock,
+            self._disconnected_futures,
+            self.key_index,
         )
         session = self.session
         secure_session = self.secure_session
         _char_map = {
             session._read_characteristic: session.read_characteristic,
             session._write_characteristic: session.write_characteristic,
             secure_session._read_characteristic: secure_session.read_characteristic,
@@ -168,22 +178,22 @@
         for char_uuid, char in _char_map.items():
             if not char:
                 await self._handle_missing_characteristic(char_uuid)
 
         # Order matters here, we must start notify for the secure session before
         # the non-secure session
         await self.secure_session.start_notify()
-        await self.session.start_notify()
         try:
             await self._setup_session()
         except BleakError as err:
             error_desc = str(err).lower()
             if "invalid handle" in error_desc:
                 await self._handle_missing_characteristic(error_desc)
             raise err
+        await self.session.start_notify()
 
     async def _handle_missing_characteristic(self, char_uuid: str) -> None:
         """Handle missing characteristic."""
         self.secure_session = None
         self.session = None
         client = cast(BleakClientWithServiceCache, self.client)
         _LOGGER.warning(
@@ -211,24 +221,23 @@
             elif state[4] == 0x0F:
                 self._state_callback([self._parse_battery_state(state)])
             else:
                 _LOGGER.debug("%s: Unknown state: %s", self.name, state.hex())
         elif state[0] == 0xAA:
             if state[1] == Commands.UNLOCK.value:
                 self._state_callback([LockStatus.UNLOCKED])
-            if state[1] == Commands.LOCK.value:
+            elif state[1] == Commands.LOCK.value:
                 self._state_callback([LockStatus.LOCKED])
             else:
                 _LOGGER.debug("%s: Unknown state: %s", self.name, state.hex())
 
     async def _setup_session(self) -> None:
         """Setup the session."""
         assert self.session is not None  # nosec
         assert self.secure_session is not None  # nosec
-        assert self._disconnected_event is not None  # nosec
         _LOGGER.debug("%s: Setting up the session", self.name)
         self.secure_session.set_key(self.key)
         handshake_keys = os.urandom(16)
 
         # Send SEC_LOCK_TO_MOBILE_KEY_EXCHANGE
         cmd = self.secure_session.build_command(0x01)
         util._copy(cmd, handshake_keys[0x00:0x08], destLocation=0x04)
@@ -254,14 +263,16 @@
         response = await self.secure_session.execute(cmd, "SEC_INITIALIZATION_COMMAND")
         if response[0] != 0x04:
             raise AuthError(
                 "Authentication error: key or slot (key index) is incorrect: unexpected response to SEC_INITIALIZATION_COMMAND: "
                 + response.hex()
             )
         self.session.set_key(session_key)
+        self.secure_session.enable_cooldown()
+        self.session.enable_cooldown()
 
     @raise_if_not_connected
     async def lock_info(self) -> LockInfo:
         """Probe the lock for information."""
         _LOGGER.debug("%s: Probing the lock", self.name)
         assert self.client is not None  # nosec
         lock_info = []
@@ -297,56 +308,72 @@
         assert self.session is not None  # nosec
         await self.session.execute(
             self.session.build_command(Commands.UNLOCK.value), "force_unlock"
         )
         _LOGGER.debug("%s: Finished unlocking", self.name)
 
     async def lock(self) -> None:
-        if (await self.status()).lock == LockStatus.UNLOCKED:
+        if (await self.lock_status()) == LockStatus.UNLOCKED:
             await self.force_lock()
 
     async def unlock(self) -> None:
-        if (await self.status()).lock == LockStatus.LOCKED:
+        if (await self.lock_status()) == LockStatus.LOCKED:
             await self.force_unlock()
 
     async def _execute_command(self, cmd_byte: int, command_name: str) -> bytes:
         assert self.session is not None  # nosec
-        response = await self.session.execute(
-            self.session.build_operation_command(cmd_byte), command_name
+        command = self.session.build_operation_command(cmd_byte)
+        _LOGGER.debug("%s: send: [%s] [%s]", self.name, command.hex(), hex(cmd_byte))
+        response = await self.session.execute(command, command_name)
+        _LOGGER.debug(
+            "%s: response: [%s] [%s]", self.name, response.hex(), hex(cmd_byte)
         )
-        _LOGGER.debug("%s: response: [%s]", self.name, response.hex())
         return response
 
     def _parse_lock_and_door_state(
         self, response: bytes
     ) -> tuple[LockStatus, DoorStatus]:
         """Parse the lock and door state from the response."""
-        lock_status = response[0x08]
-        door_status = response[0x09]
-        lock_status_enum = VALUE_TO_LOCK_STATUS.get(lock_status, LockStatus.UNKNOWN)
-        door_status_enum = VALUE_TO_DOOR_STATUS.get(door_status, DoorStatus.UNKNOWN)
+        return self._parse_lock_status(response[0x08]), self._parse_door_status(
+            response[0x09]
+        )
 
+    def _parse_lock_status(self, lock_status: int) -> LockStatus:
+        """Parse the lock state from the response."""
+        lock_status_enum = VALUE_TO_LOCK_STATUS.get(lock_status, LockStatus.UNKNOWN)
         if lock_status_enum == LockStatus.UNKNOWN:
             _LOGGER.debug(
                 "%s: Unrecognized lock_status_str code: %s", self.name, hex(lock_status)
             )
+        return lock_status_enum
+
+    def _parse_door_status(self, door_status: int) -> DoorStatus:
+        """Parse the door state from the response."""
+        door_status_enum = VALUE_TO_DOOR_STATUS.get(door_status, DoorStatus.UNKNOWN)
         if door_status_enum == DoorStatus.UNKNOWN:
             _LOGGER.debug(
                 "%s: Unrecognized door_status_str code: %s", self.name, hex(door_status)
             )
-        return lock_status_enum, door_status_enum
+        return door_status_enum
 
     @raise_if_not_connected
-    async def status(self) -> LockState:
-        _LOGGER.debug("%s: Executing status", self.name)
-        response = await self._execute_command(
-            0x2F if self._lock_info and self._lock_info.door_sense else 0x02, "status"
-        )
-        _LOGGER.debug("%s: Finished executing status", self.name)
-        return LockState(*self._parse_lock_and_door_state(response), None, None)
+    async def lock_status(self) -> LockStatus:
+        _LOGGER.debug("%s: Executing lock_status", self.name)
+        # We used to use 0x2F here but it seems to be broken on some locks
+        response = await self._execute_command(0x02, "lock_status")
+        _LOGGER.debug("%s: Finished executing lock_status", self.name)
+        return self._parse_lock_status(response[0x08])
+
+    @raise_if_not_connected
+    async def door_status(self) -> DoorStatus:
+        _LOGGER.debug("%s: Executing door_status", self.name)
+        # We used to use 0x2F here but it seems to be broken on some locks
+        response = await self._execute_command(0x2E, "door_status")
+        _LOGGER.debug("%s: Finished executing door_status", self.name)
+        return self._parse_door_status(response[0x08])
 
     def _parse_battery_state(self, response: bytes) -> BatteryState:
         """Parse the battery state from the response."""
         voltage = (response[0x09] * 256 + response[0x08]) / 1000
         # The voltage is divided by 4 in the lock
         # since it uses 4 AA batteries. For the Li-ion
         # battery, this is likely wrong, but since we don't
@@ -366,31 +393,39 @@
         """Disconnect from the lock."""
         _LOGGER.debug("%s: Disconnecting from the lock", self.name)
         if not self.client or not self.client.is_connected:
             return
 
         try:
             await self._shutdown_connection()
+        except BleakError:
+            _LOGGER.debug(
+                "%s: Failed to shutdown connection to lock", self.name, exc_info=True
+            )
         finally:
-            await self.client.disconnect()
+            try:
+                await self.client.disconnect()
+            except BleakError:
+                _LOGGER.debug(
+                    "%s: Failed to disconnect from lock", self.name, exc_info=True
+                )
 
     async def _shutdown_connection(self) -> None:
         """Shutdown the connection."""
         _LOGGER.debug("%s: Shutting down the connection", self.name)
-        if (
-            not self.is_secure
-            or not self.secure_session
-            or self._disconnected_event is None
-        ):
+        if self.session:
+            await self.session.stop_notify()
+        if not self.is_secure or not self.secure_session or self._disconnected:
             return
         cmd = self.secure_session.build_command(0x05)
         cmd[0x11] = 0x00
         response = None
         try:
             response = await self.secure_session.execute(cmd, "shutdown")
+            await self.secure_session.stop_notify()
         except (AuthError, DisconnectedError):
             # Lock already disconnected us
             return
         except (BleakError, asyncio.TimeoutError, EOFError) as err:
             if not util.is_disconnected_error(err):
                 _LOGGER.debug(
                     "%s: Failed to cleanly disconnect from lock: %s", self.name, err
@@ -403,10 +438,9 @@
     def is_connected(self) -> bool:
         """Return True if the lock is connected."""
         return bool(
             self.client
             and self.client.is_connected
             and self.session
             and self.secure_session
-            and self._disconnected_event is not None
-            and not self._disconnected_event.is_set()
+            and not self._disconnected
         )
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/push.py` & `yalexs_ble-2.2.0/src/yalexs_ble/push.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, TypeVar, cast
 
 import async_timeout
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 from bleak.exc import BleakDBusError, BleakError
 from bleak_retry_connector import BLEAK_RETRY_EXCEPTIONS, BleakNotFoundError, get_device
+from lru import LRU  # pylint: disable=no-name-in-module
 
 from .const import (
     APPLE_MFR_ID,
     HAP_ENCRYPTED_FIRST_BYTE,
     HAP_FIRST_BYTE,
     YALE_MFR_ID,
     AuthState,
@@ -46,18 +47,24 @@
 
 WrapFuncType = TypeVar("WrapFuncType", bound=Callable[..., Any])
 
 NEVER_TIME = -86400.0
 
 DEFAULT_ATTEMPTS = 4
 
+# How long to wait to disconnect after an operation
 DISCONNECT_DELAY = 5.1
 
+# How long to wait to disconnect after an operation if there is a pending update
+DISCONNECT_DELAY_PENDING_UPDATE = 12.5
+
 RESYNC_DELAY = 0.01
 
+KEEP_ALIVE_TIME = 25.0  # Lock will disconnect after 30 seconds of inactivity
+
 # Number of seconds to wait after the first connection
 # to disconnect to free up the bluetooth adapter.
 FIRST_CONNECTION_DISCONNECT_TIME = 2.1
 
 # After a lock operation we need to wait for the lock to
 # update its state or it will return a stale state.
 LOCK_STALE_STATE_DEBOUNCE_DELAY = 6.1
@@ -74,15 +81,15 @@
 # How long to wait before processing a manual update request
 MANUAL_UPDATE_COALESCE_SECONDS = 0.05
 
 # How long to wait to query the lock after an operation to make sure its not jammed
 POST_OPERATION_SYNC_TIME = 10.00
 
 # How long to wait if we get an update storm from the lock
-UPDATE_IN_PROGRESS_DEFER_SECONDS = 1.0
+UPDATE_IN_PROGRESS_DEFER_SECONDS = DISCONNECT_DELAY - 1
 
 RETRY_BACKOFF_EXCEPTIONS = (BleakDBusError, DisconnectedError)
 
 RETRY_EXCEPTIONS = (ResponseError, *BLEAK_RETRY_EXCEPTIONS)
 
 # 255 seems to be broadcast randomly when
 # there is no update from the lock.
@@ -100,14 +107,37 @@
         _LOGGER.debug("%s: Acquiring lock", self.name)
         async with self._operation_lock:
             return await func(self, *args, **kwargs)
 
     return cast(WrapFuncType, _async_wrap_operation_lock)
 
 
+class AuthFailureHistory:
+    """Track the number of auth failures."""
+
+    def __init__(self) -> None:
+        """Init the history."""
+        self._failures_by_mac: dict[str, int] = LRU(1024)
+
+    def auth_failed(self, mac: str) -> None:
+        """Increment the number of auth failures."""
+        self._failures_by_mac[mac] = self._failures_by_mac.get(mac, 0) + 1
+
+    def auth_success(self, mac: str) -> None:
+        """Reset the number of auth failures."""
+        self._failures_by_mac[mac] = 0
+
+    def should_raise(self, mac: str) -> bool:
+        """Return if we should raise an error."""
+        return self._failures_by_mac.get(mac, 0) >= AUTH_FAILURE_TO_START_REAUTH
+
+
+_AUTH_FAILURE_HISTORY = AuthFailureHistory()
+
+
 def retry_bluetooth_connection_error(func: WrapFuncType) -> WrapFuncType:
     """Define a wrapper to retry on bleak error.
 
     The accessory is allowed to disconnect us any time so
     we need to retry the operation.
     """
 
@@ -118,27 +148,37 @@
         attempts = DEFAULT_ATTEMPTS
         max_attempts = attempts - 1
 
         for attempt in range(attempts):
             try:
                 return await func(self, *args, **kwargs)
             except AuthError:
-                self._auth_failures += 1
-                if self._auth_failures >= AUTH_FAILURE_TO_START_REAUTH:
+                _AUTH_FAILURE_HISTORY.auth_failed(self.address)
+                if _AUTH_FAILURE_HISTORY.should_raise(self.address):
                     # If the bluetooth connection drops in the middle of authentication
                     # we may see it as a failed authentication. If we see 5 failed
                     # authentications in a row we can reasonably assume that the key has
                     # changed and we should re-authenticate.
                     self._update_any_state([AuthState(successful=False)])
-                raise
+                    raise
+                _LOGGER.debug(
+                    "%s: Auth error calling %s, retrying (%s/%s)...",
+                    self.name,
+                    func,
+                    attempt,
+                    max_attempts,
+                    exc_info=True,
+                )
+                await asyncio.sleep(0.25)
             except BleakNotFoundError:
                 # The lock cannot be found so there is no
                 # point in retrying.
                 raise
             except RETRY_BACKOFF_EXCEPTIONS as err:
+                await self._async_handle_disconnected(err)
                 if attempt >= max_attempts:
                     _LOGGER.debug(
                         "%s: %s error calling %s, reach max attempts (%s/%s)",
                         self.name,
                         type(err),
                         func,
                         attempt,
@@ -156,14 +196,15 @@
                     0.25,
                     attempt,
                     max_attempts,
                     exc_info=True,
                 )
                 await asyncio.sleep(0.25)
             except RETRY_EXCEPTIONS as err:
+                await self._async_handle_disconnected(err)
                 if attempt >= max_attempts:
                     _LOGGER.debug(
                         "%s: %s error calling %s, reach max attempts (%s/%s)",
                         self.name,
                         type(err),
                         func,
                         attempt,
@@ -194,14 +235,16 @@
         local_name: str | None = None,
         address: str | None = None,
         ble_device: BLEDevice | None = None,
         key: str | None = None,
         key_index: int | None = None,
         advertisement_data: AdvertisementData | None = None,
         idle_disconnect_delay: float = DISCONNECT_DELAY,
+        always_connected: bool = False,
+        idle_disconnect_delay_pending_update: float = DISCONNECT_DELAY_PENDING_UPDATE,
     ) -> None:
         """Init the lock watcher."""
         if local_name is None and address is None:
             raise ValueError("Must specify either local_name or address")
         if not address and not local_name_is_unique(local_name):
             raise ValueError("local_name must be unique when address is not provided")
 
@@ -223,21 +266,29 @@
             Callable[[LockState, LockInfo, ConnectionInfo], None]
         ] = []
         self._update_task: asyncio.Task[None] | None = None
         self.loop = asyncio._get_running_loop()
         self._cancel_deferred_update: asyncio.TimerHandle | None = None
         self._client: Lock | None = None
         self._connect_lock = asyncio.Lock()
+        self._seen_this_session: set[
+            type[LockStatus] | type[DoorStatus] | type[BatteryState] | type[AuthState]
+        ] = set()
         self._disconnect_timer: asyncio.TimerHandle | None = None
+        self._keep_alive_timer: asyncio.TimerHandle | None = None
+        self._idle_disconnect_delay_pending_update = (
+            idle_disconnect_delay_pending_update
+        )
         self._idle_disconnect_delay = idle_disconnect_delay
         self._next_disconnect_delay = idle_disconnect_delay
         self._first_update_future: asyncio.Future[None] | None = None
         self._background_tasks: set[asyncio.Task[None]] = set()
-        self._auth_failures: int = 0
         self._last_lock_operation_complete_time = NEVER_TIME
+        self._last_operation_complete_time = NEVER_TIME
+        self._always_connected = always_connected
 
     @property
     def local_name(self) -> str | None:
         """Get the local name."""
         return self._local_name
 
     @property
@@ -292,14 +343,19 @@
         return None
 
     @property
     def ble_device(self) -> BLEDevice | None:
         """Return the current BLEDevice."""
         return self._ble_device
 
+    @property
+    def is_connected(self) -> bool:
+        """Return if the lock is connected."""
+        return bool(self._client and self._client.is_connected)
+
     def set_name(self, name: str) -> None:
         """Set the name of the lock."""
         self._name = name
 
     def reset_advertisement_state(self) -> None:
         """Reset the advertisement state."""
         self._last_adv_value = -1
@@ -338,18 +394,66 @@
         return Lock(
             lambda: self._ble_device,
             self._lock_key,
             self._lock_key_index,
             self.name,
             self._state_callback,
             self._lock_info,
+            self._disconnected_callback,
+        )
+
+    def _disconnected_callback(self) -> None:
+        """Handle a disconnect from the lock."""
+        _LOGGER.debug("%s: Disconnected from lock callback", self.name)
+        if self._always_connected and not _AUTH_FAILURE_HISTORY.should_raise(
+            self.address
+        ):
+            _LOGGER.debug(
+                "%s: Scheduling reconnect from disconnected callback", self.name
+            )
+            self._keep_alive()
+
+    def _keep_alive(self) -> None:
+        """Keep the lock connection alive."""
+        if not self._always_connected:
+            return
+        _LOGGER.debug("%s: Executing keep alive", self.name)
+        self._schedule_future_update(0)
+        self._schedule_next_keep_alive(KEEP_ALIVE_TIME)
+
+    def _time_since_last_operation(self) -> float:
+        """Return the time since the last operation."""
+        return time.monotonic() - self._last_operation_complete_time
+
+    def _reschedule_next_keep_alive(self) -> None:
+        """Reschedule the next keep alive."""
+        next_keep_alive_time = max(
+            0, KEEP_ALIVE_TIME - self._time_since_last_operation()
+        )
+        self._schedule_next_keep_alive(next_keep_alive_time)
+
+    def _schedule_next_keep_alive(self, delay: float) -> None:
+        """Schedule the next keep alive."""
+        self._cancel_keepalive_timer()
+        if not self._always_connected:
+            return
+        _LOGGER.debug(
+            "%s: Scheduling next keep alive in %s seconds",
+            self.name,
+            delay,
+        )
+        self._keep_alive_timer = self.loop.call_later(
+            delay,
+            self._keep_alive,
         )
 
     def _reset_disconnect_timer(self) -> None:
         """Reset disconnect timer."""
+        if self._always_connected:
+            return
         self._cancel_disconnect_timer()
         self._expected_disconnect = False
         timeout = self._next_disconnect_delay
         _LOGGER.debug(
             "%s: Resetting disconnect timer to %s seconds", self.name, timeout
         )
         self._disconnect_timer = self.loop.call_later(
@@ -364,15 +468,18 @@
             self._update_task = None
             update_task.cancel()
             with contextlib.suppress(Exception, asyncio.CancelledError):
                 await update_task
         await self._execute_disconnect()
 
     def _disconnect_with_timer(self, timeout: float) -> None:
-        """Disconnect from device."""
+        """Disconnect from device.
+
+        This should only ever be called from _reset_disconnect_timer
+        """
         if self._operation_lock.locked():
             _LOGGER.debug("%s: Disconnect timer reset due to operation lock", self.name)
             self._reset_disconnect_timer()
             return
         if self._cancel_deferred_update:
             _LOGGER.debug(
                 "%s: Disconnect timer fired while we were waiting to update", self.name
@@ -386,23 +493,41 @@
 
     def _cancel_disconnect_timer(self) -> None:
         """Cancel disconnect timer."""
         if self._disconnect_timer:
             self._disconnect_timer.cancel()
             self._disconnect_timer = None
 
+    def _cancel_keepalive_timer(self) -> None:
+        """Cancel keep alive timer."""
+        if self._keep_alive_timer:
+            self._keep_alive_timer.cancel()
+            self._keep_alive_timer = None
+
     async def _execute_timed_disconnect(self, timeout: float) -> None:
         """Execute timed disconnection."""
         _LOGGER.debug(
             "%s: Executing timed disconnect after timeout of %s",
             self.name,
             timeout,
         )
         await self._execute_disconnect()
 
+    async def _async_handle_disconnected(self, exc: Exception) -> None:
+        """Clean up after a disconnect."""
+        _LOGGER.debug("%s: Disconnected due to %s, cleaning up", self.name, exc)
+        if self._connect_lock.locked():
+            _LOGGER.error(
+                "%s: Disconnected while connection was in progress, ignoring",
+                self.name,
+            )
+            return
+        self._cancel_disconnect_timer()
+        await self._execute_disconnect()
+
     async def _execute_disconnect(self) -> None:
         """Execute disconnection."""
         async with self._connect_lock:
             if self._disconnect_timer:  # If the timer was reset, don't disconnect
                 return
             client = self._client
             self._client = None
@@ -415,33 +540,36 @@
         """Ensure connection to device is established."""
         if self._connect_lock.locked():
             self._reset_disconnect_timer()
             _LOGGER.debug(
                 "%s: Connection already in progress, waiting for it to complete",
                 self.name,
             )
-        if self._client and self._client.is_connected:
+        if self.is_connected:
+            assert self._client is not None  # nosec
             self._reset_disconnect_timer()
             return self._client
         async with self._connect_lock:
             # Check again while holding the lock
-            if self._client and self._client.is_connected:
+            if self.is_connected:
+                assert self._client is not None  # type: ignore[unreachable] # nosec
                 self._reset_disconnect_timer()
                 return self._client
             self._client = self._get_lock_instance()
             try:
                 await self._client.connect()
             except Exception as ex:
                 _LOGGER.debug(
                     "%s: Failed to connect due to %s, forcing disconnect", self.name, ex
                 )
                 await self._client.disconnect()
                 raise
             self._next_disconnect_delay = self._idle_disconnect_delay
             self._reset_disconnect_timer()
+            self._seen_this_session.clear()
             return self._client
 
     async def lock(self) -> None:
         """Lock the lock."""
         self._update_any_state([LockStatus.LOCKING])
         self._cancel_future_update()
         await self._execute_lock_operation(
@@ -458,45 +586,58 @@
 
     @operation_lock
     @retry_bluetooth_connection_error
     async def _execute_lock_operation(
         self, op_attr: str, pending_state: LockStatus, complete_state: LockStatus
     ) -> None:
         """Execute a lock operation."""
+        if not self._running:
+            raise RuntimeError(
+                f"{self.name}: Lock operation not possible because not running"
+            )
         _LOGGER.debug("%s: Starting %s", self.name, pending_state)
         self._update_any_state([pending_state])
         self._cancel_future_update()
         try:
             lock = await self._ensure_connected()
             self._cancel_future_update()
             await getattr(lock, op_attr)()
         except Exception:
             self._update_any_state([LockStatus.UNKNOWN])
             raise
         self._update_any_state([complete_state])
         _LOGGER.debug("%s: Finished %s", self.name, complete_state)
-        self._last_lock_operation_complete_time = time.monotonic()
+        now = time.monotonic()
+        self._last_lock_operation_complete_time = now
+        self._last_operation_complete_time = now
         self._reset_disconnect_timer()
+        self._reschedule_next_keep_alive()
 
     def _state_callback(
         self, states: Iterable[LockStatus | DoorStatus | BatteryState]
     ) -> None:
         """Handle state change."""
         self._reset_disconnect_timer()
         self._update_any_state(states)
 
+    def _get_current_state(self) -> LockState:
+        """Get the current state of the lock."""
+        return self._lock_state or LockState(
+            self.lock_status, self.door_status, self.battery, self.auth
+        )
+
     def _update_any_state(
         self, states: Iterable[LockStatus | DoorStatus | BatteryState | AuthState]
     ) -> None:
         _LOGGER.debug("%s: State changed: %s", self.name, states)
-        lock_state = self._lock_state or LockState(
-            self.lock_status, self.door_status, self.battery, self.auth
-        )
+        lock_state = self._get_current_state()
         original_lock_status = lock_state.lock
         for state in states:
+            state_type = type(state)
+            self._seen_this_session.add(state_type)
             if isinstance(state, AuthState):
                 lock_state = replace(lock_state, auth=state)
             elif isinstance(state, LockStatus):
                 lock_state = replace(lock_state, lock=state)
             elif isinstance(state, DoorStatus):
                 lock_state = replace(lock_state, door=state)
             elif isinstance(state, BatteryState):
@@ -518,18 +659,17 @@
         ):
             self._schedule_future_update(RESYNC_DELAY)
 
         self._callback_state(lock_state)
 
     async def update(self) -> None:
         """Request that status be updated."""
+        _LOGGER.debug("%s: Starting manual update", self.name)
         self._schedule_future_update_with_debounce(
-            0
-            if self._client and self._client.is_connected
-            else MANUAL_UPDATE_COALESCE_SECONDS
+            0 if self.is_connected else MANUAL_UPDATE_COALESCE_SECONDS
         )
 
     async def validate(self) -> None:
         """Validate lock credentials."""
         _LOGGER.debug("%s: Starting validate", self.name)
         await self._update()
         _LOGGER.debug("%s: Finished validate", self.name)
@@ -539,32 +679,55 @@
     async def _update(self) -> LockState:
         """Update the lock state."""
         has_lock_info = self._lock_info is not None
 
         _LOGGER.debug(
             "%s: Starting update (has_lock_info: %s)", self.name, has_lock_info
         )
-        try:
-            lock = await self._ensure_connected()
-            if not self._lock_info:
-                self._lock_info = await lock.lock_info()
-            state = await lock.status()
+        lock = await self._ensure_connected()
+        if not self._lock_info:
+            self._lock_info = await lock.lock_info()
+        # Asking for battery first seems to be reduce the chance of the lock
+        # getting into a bad state.
+        state = self._get_current_state()
+        made_request = False
+
+        if BatteryState not in self._seen_this_session:
+            made_request = True
             battery_state = await lock.battery()
-        except asyncio.CancelledError:
-            _LOGGER.debug(
-                "%s: In-progress update canceled due "
-                "to lock operation or setup timeout",
-                self.name,
-            )
-            raise
-        else:
-            self._auth_failures = 0
+            _AUTH_FAILURE_HISTORY.auth_success(self.address)
             state = replace(
                 state, battery=battery_state, auth=AuthState(successful=True)
             )
+
+        if (
+            DoorStatus not in self._seen_this_session
+            and self._lock_info
+            and self._lock_info.door_sense
+        ):
+            made_request = True
+            door_status = await lock.door_status()
+            _AUTH_FAILURE_HISTORY.auth_success(self.address)
+            state = replace(state, door=door_status, auth=AuthState(successful=True))
+
+        # Only ask for the lock status if we haven't seen
+        # it this session since notify callbacks will happen
+        # if it changes and the extra polling can cause the lock
+        # to get into a bad state.
+        #
+        # However, we always want to poll lock
+        # state to keep the connection alive if we are always connected.
+        if LockStatus not in self._seen_this_session or (
+            not made_request and self._always_connected
+        ):
+            made_request = True
+            lock_status = await lock.lock_status()
+            _AUTH_FAILURE_HISTORY.auth_success(self.address)
+            state = replace(state, lock=lock_status, auth=AuthState(successful=True))
+
         _LOGGER.debug("%s: Finished update", self.name)
         self._callback_state(state)
 
         if state.battery and state.battery.voltage <= 3.0:
             _LOGGER.debug(
                 "%s: Battery voltage is impossible: %s",
                 self.name,
@@ -586,14 +749,17 @@
             # the bluetooth adapter is out of connections
             # slots. We reset the timer to a low number
             # so that if another update request is pending
             # we do not disconnect until it completes.
             self._next_disconnect_delay = FIRST_CONNECTION_DISCONNECT_TIME
             self._reset_disconnect_timer()
 
+        if made_request:
+            self._last_operation_complete_time = time.monotonic()
+            self._reschedule_next_keep_alive()
         return state
 
     def _callback_state(self, lock_state: LockState) -> None:
         """Call the callbacks."""
         self._lock_state = lock_state
         _LOGGER.debug(
             "%s: New state: %s %s %s",
@@ -683,16 +849,34 @@
                 self.name,
                 self._lock_state,
                 self._last_hk_state,
                 self._last_adv_value,
                 next_update,
                 scheduled_update,
             )
-        if next_update:
-            self._schedule_future_update_with_debounce(next_update)
+        if not next_update:
+            return
+        if (
+            self.is_connected
+            and self._next_disconnect_delay != FIRST_CONNECTION_DISCONNECT_TIME
+            and (
+                self._time_since_last_operation()
+                + self._idle_disconnect_delay_pending_update
+            )
+            < KEEP_ALIVE_TIME
+        ):
+            # Already connected, state will be pushed, but stay
+            # connected a bit longer to make sure we get it unless
+            # this is the first connection or deferring the update
+            # would keep the connection idle for too long and
+            # get us disconnected anyways.
+            self._next_disconnect_delay = self._idle_disconnect_delay_pending_update
+            self._reset_disconnect_timer()
+            return
+        self._schedule_future_update_with_debounce(next_update)
 
     async def start(self) -> Callable[[], None]:
         """Start watching for updates."""
         _LOGGER.debug("Waiting for advertisement callbacks for %s", self.name)
         if self._running:
             raise RuntimeError("Already running")
         self._running = True
@@ -719,34 +903,35 @@
         if not self._running:
             raise RuntimeError("Not running")
         if not self._first_update_future:
             raise RuntimeError("Already waited for first update")
         try:
             async with async_timeout.timeout(timeout):
                 await self._first_update_future
-        except asyncio.TimeoutError:
+        except (asyncio.TimeoutError, asyncio.CancelledError) as ex:
             self._first_update_future.cancel()
             with contextlib.suppress(asyncio.CancelledError):
                 await self._first_update_future
-            raise NoAdvertisementError("No advertisement received")
+            raise NoAdvertisementError(
+                "No advertisement received before timeout"
+            ) from ex
         finally:
             self._first_update_future = None
 
     def _cancel_future_update(self) -> None:
         """Cancel an update."""
         if self._cancel_deferred_update:
             self._cancel_deferred_update.cancel()
             self._cancel_deferred_update = None
 
     def _schedule_future_update_with_debounce(self, seconds: float) -> None:
         """Schedule an update with a potential debounce."""
-        now = self.loop.time()
         future_update_time = seconds
         if self._cancel_deferred_update:
-            time_till_update = self._cancel_deferred_update.when() - now
+            time_till_update = self._cancel_deferred_update.when() - self.loop.time()
             if time_till_update < HK_UPDATE_COALESCE_SECONDS:
                 future_update_time = HK_UPDATE_COALESCE_SECONDS
                 _LOGGER.debug(
                     "%s: Existing update too soon %s, "
                     "rescheduling update for in %s seconds",
                     self.name,
                     time_till_update,
@@ -755,15 +940,17 @@
             elif time_till_update < seconds:
                 _LOGGER.debug(
                     "%s: Existing update in %s seconds will happen sooner than now",
                     self.name,
                     time_till_update,
                 )
                 return
-            _LOGGER.debug("%s: Rescheduling update", self.name)
+            _LOGGER.debug(
+                "%s: Rescheduling update for %s", self.name, future_update_time
+            )
         self._schedule_future_update(future_update_time)
 
     def _schedule_future_update(self, future_update_time: float) -> None:
         """Schedule an update in future seconds."""
         _LOGGER.debug(
             "%s: Scheduling update to happen in %s seconds",
             self.name,
@@ -818,22 +1005,28 @@
                 self.name,
                 ex,
                 exc_info=True,
             )
         except asyncio.CancelledError:
             self._set_update_state(RuntimeError("Update was canceled"))
             _LOGGER.debug("%s: In-progress update canceled", self.name)
+            raise
         except asyncio.TimeoutError as ex:
             self._set_update_state(ex)
             _LOGGER.exception("%s: Timed out updating", self.name)
         except BleakError as ex:
             wrapped_bleak_exc = BluetoothError(str(ex))
             wrapped_bleak_exc.__cause__ = ex
             self._set_update_state(wrapped_bleak_exc)
             _LOGGER.exception("%s: Bluetooth error updating", self.name)
+        except DisconnectedError as ex:
+            wrapped_bleak_exc = BluetoothError(str(ex))
+            wrapped_bleak_exc.__cause__ = ex
+            self._set_update_state(wrapped_bleak_exc)
+            _LOGGER.exception("%s: Disconnected while updating", self.name)
         except Exception as ex:  # pylint: disable=broad-except
             wrapped_exc = YaleXSBLEError(str(ex))
             wrapped_exc.__cause__ = ex
             self._set_update_state(wrapped_exc)
             _LOGGER.exception("%s: Unknown error updating", self.name)
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/secure_session.py` & `yalexs_ble-2.2.0/src/yalexs_ble/secure_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     _read_characteristic = SECURE_READ_CHARACTERISTIC
 
     def __init__(
         self,
         client: BleakClient,
         name: str,
         lock: asyncio.Lock,
-        disconnected_event: asyncio.Event,
+        disconnected_futures: set[asyncio.Future[None]],
         key_index: int,
     ) -> None:
-        super().__init__(client, name, lock, disconnected_event)
+        super().__init__(client, name, lock, disconnected_futures)
         self.key_index = key_index
         self.write_characteristic = client.services.get_characteristic(
             self._write_characteristic
         )
         self.read_characteristic = client.services.get_characteristic(
             self._read_characteristic
         )
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/session.py` & `yalexs_ble-2.2.0/src/yalexs_ble/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import asyncio
-import contextlib
 import logging
+import time
 from typing import Callable
 
 import async_timeout
 from bleak import BleakClient
 from bleak_retry_connector import BleakError
 from cryptography.hazmat.primitives.ciphers import (
     Cipher,
@@ -16,14 +16,16 @@
 )
 
 from . import util
 from .const import READ_CHARACTERISTIC, WRITE_CHARACTERISTIC
 
 _LOGGER = logging.getLogger(__name__)
 
+COOLDOWN_TIME = 0.25
+
 
 class YaleXSBLEError(Exception):
     """Base class for YaleXSBLE errors."""
 
 
 class AuthError(YaleXSBLEError):
     """Error during authentication."""
@@ -50,15 +52,15 @@
     _read_characteristic = READ_CHARACTERISTIC
 
     def __init__(
         self,
         client: BleakClient,
         name: str,
         lock: asyncio.Lock,
-        disconnected_event: asyncio.Event,
+        disconnected_futures: set[asyncio.Future[None]],
         state_callback: Callable[[bytes], None] | None = None,
     ) -> None:
         """Init the session."""
         self.name = name
         self._lock = lock
         self.cipher_decrypt: CipherContext | None = None
         self.cipher_encrypt: CipherContext | None = None
@@ -68,25 +70,31 @@
         )
         self.read_characteristic = client.services.get_characteristic(
             self._read_characteristic
         )
         self._notifications_started = False
         self._notify_future: asyncio.Future[bytes] | None = None
         self._state_callback = state_callback
-        self._disconnected_event = disconnected_event
+        self._disconnected_futures = disconnected_futures
         self._first_request = True
+        self._last_callback_time = -86400.0
+        self._enable_cooldown = False
 
     def set_key(self, key: bytes) -> None:
         self.cipher_encrypt = Cipher(
             algorithms.AES(key), modes.CBC(bytes(0x10))  # nosec
         ).encryptor()
         self.cipher_decrypt = Cipher(
             algorithms.AES(key), modes.CBC(bytes(0x10))  # nosec
         ).decryptor()
 
+    def enable_cooldown(self) -> None:
+        """Enable cooldown after each request."""
+        self._enable_cooldown = True
+
     def decrypt(self, data: bytes | bytearray) -> bytes:
         if self.cipher_decrypt is not None:
             cipherText = data[0x00:0x10]
             plainText = self.cipher_decrypt.update(cipherText)
             if type(data) is not bytearray:
                 data = bytearray(data)
             util._copy(data, plainText)
@@ -124,14 +132,15 @@
 
     async def _write(self, command: bytearray, command_name: str) -> bytes:
         """Write under the lock."""
         async with self._lock:
             return await self._locked_write(command, command_name)
 
     def _notify(self, char: int, data: bytes) -> None:
+        self._last_callback_time = time.monotonic()
         _LOGGER.debug(
             "%s: Receiving response via notify: %s (waiting=%s)",
             self.name,
             data.hex(),
             bool(self._notify_future),
         )
         decrypted_data = self.decrypt(data)
@@ -153,15 +162,15 @@
         self._notify_future = None
 
     async def _locked_write(self, command: bytearray, command_name: str) -> bytes:
         # NOTE: The last two bytes are not encrypted
         # General idea seems to be that if the last byte
         # of the command indicates an offline key offset (is non-zero),
         # the command is "secure" and encrypted with the offline key
-        if not self.client.is_connected or self._disconnected_event.is_set():
+        if not self.client.is_connected:
             raise BleakError("disconnected")
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         plainText = command[0x00:0x10]
         cipherText = self.cipher_encrypt.update(plainText)
         util._copy(command, cipherText)
         _LOGGER.debug(
             "%s: Encrypted command %s: %s", self.name, command_name, command.hex()
@@ -231,34 +240,51 @@
             pass
         except BleakError as err:
             _LOGGER.debug("%s: Bleak error stopping notify: %s", self.name, err)
             pass
 
     async def execute(self, command: bytearray, command_name: str) -> bytes:
         """Execute command."""
+        while (
+            self._enable_cooldown
+            and (cooldown_remain := time.monotonic() - self._last_callback_time)
+            < COOLDOWN_TIME
+        ):
+            _LOGGER.debug(
+                "%s: Waiting %s for lock to settle", self.name, cooldown_remain
+            )
+            # If we send commands to fast the lock may crash and stop
+            # advertising. This is a workaround to avoid that since
+            # it means a battery pull is required to recover.
+            await asyncio.sleep(COOLDOWN_TIME - cooldown_remain)
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         self._write_checksum(command)
-        write_task = asyncio.create_task(self._write(command, command_name))
-        disconnect_task = asyncio.create_task(self._disconnected_event.wait())
-        await asyncio.wait(
-            (write_task, disconnect_task),
-            return_when=asyncio.FIRST_COMPLETED,
-        )
-        if disconnect_task.done():
-            write_task.cancel()
-        if write_task.done():
-            try:
-                return await write_task
-            except BleakError as err:
-                if self._first_request and util.is_key_error(err):
-                    raise AuthError(
-                        f"Authentication error: key or slot (key index) is incorrect: {err}"
-                    ) from err
-                if util.is_disconnected_error(err):
-                    raise DisconnectedError(f"{self.name}: {err}") from err
-                raise
-            finally:
-                self._first_request = False
-        write_task.cancel()
-        with contextlib.suppress(asyncio.CancelledError, Exception):
-            await write_task
-        raise DisconnectedError(f"{self.name}: Disconnected")
+        task = asyncio.current_task()
+        disconnected_future = asyncio.get_running_loop().create_future()
+        self._disconnected_futures.add(disconnected_future)
+
+        def _on_disconnected(fut: asyncio.Future[None]) -> None:
+            if task and not task.done():
+                task.cancel()
+
+        disconnected_future.add_done_callback(_on_disconnected)
+        try:
+            return await self._write(command, command_name)
+        except BleakError as err:
+            if self._first_request and util.is_key_error(err):
+                raise AuthError(
+                    f"Authentication error: key or slot (key index) is incorrect: {err}"
+                ) from err
+            if util.is_disconnected_error(err):
+                raise DisconnectedError(f"{self.name}: {err}") from err
+            raise
+        except asyncio.CancelledError:
+            _LOGGER.debug(
+                "%s: `%s` cancelled due to disconnect during write",
+                self.name,
+                command_name,
+            )
+            raise DisconnectedError(f"{self.name}: Disconnected")
+        finally:
+            self._disconnected_futures.discard(disconnected_future)
+            disconnected_future.remove_done_callback(_on_disconnected)
+            self._first_request = False
```

### Comparing `yalexs_ble-2.1.9/src/yalexs_ble/util.py` & `yalexs_ble-2.2.0/src/yalexs_ble/util.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.9/PKG-INFO` & `yalexs_ble-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs-ble
-Version: 2.1.9
+Version: 2.2.0
 Summary: Bluetooth control of Yale and August locks
 Home-page: https://github.com/bdraco/yalexs-ble
 License: GNU General Public License v3.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: async-timeout (>=3.0.1)
 Requires-Dist: bleak (>=0.19.0)
 Requires-Dist: bleak-retry-connector (>=2.9.0)
 Requires-Dist: cryptography (>=38.0.0)
+Requires-Dist: lru-dict (>=1.1.4)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bdraco/yalexs-ble/issues
 Project-URL: Changelog, https://github.com/bdraco/yalexs-ble/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://yalexs-ble.readthedocs.io
 Project-URL: Repository, https://github.com/bdraco/yalexs-ble
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: yalexs-ble Version: 2.1.9 Summary: Bluetooth
+Metadata-Version: 2.1 Name: yalexs-ble Version: 2.2.0 Summary: Bluetooth
 control of Yale and August locks Home-page: https://github.com/bdraco/yalexs-
 ble License: GNU General Public License v3.0 Author: J. Nick Koston Author-
 email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Provides-
 Extra: docs Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist:
 async-timeout (>=3.0.1) Requires-Dist: bleak (>=0.19.0) Requires-Dist: bleak-
 retry-connector (>=2.9.0) Requires-Dist: cryptography (>=38.0.0) Requires-Dist:
-myst-parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: sphinx-rtd-theme
-(>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://github.com/
-bdraco/yalexs-ble/issues Project-URL: Changelog, https://github.com/bdraco/
-yalexs-ble/blob/main/CHANGELOG.md Project-URL: Documentation, https://yalexs-
-ble.readthedocs.io Project-URL: Repository, https://github.com/bdraco/yalexs-
-ble Description-Content-Type: text/markdown # Yale Access BLE
+lru-dict (>=1.1.4) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug
+Tracker, https://github.com/bdraco/yalexs-ble/issues Project-URL: Changelog,
+https://github.com/bdraco/yalexs-ble/blob/main/CHANGELOG.md Project-URL:
+Documentation, https://yalexs-ble.readthedocs.io Project-URL: Repository,
+https://github.com/bdraco/yalexs-ble Description-Content-Type: text/markdown #
+Yale Access BLE
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Bluetooth control of Yale and August locks ## Installation Install this via pip
 (or your favourite package manager): `pip install yalexs-ble` ## Fork history
 Thanks to: https://github.com/Friendly0Fire/augustpy https://github.com/
 terrcin/augustctl https://github.com/ethitter/augustctl https://github.com/
```

