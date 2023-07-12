# Comparing `tmp/wg_utilities-3.7.0.tar.gz` & `tmp/wg_utilities-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.7.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.8.0.tar", max compression
```

## Comparing `wg_utilities-3.7.0.tar` & `wg_utilities-3.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/README.md
--rw-r--r--   0        0        0     4825 2023-05-07 21:13:54.736314 wg_utilities-3.7.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      685 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4207 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    23741 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56658 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7580 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13265 2023-05-07 21:13:54.804312 wg_utilities-3.7.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15915 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    27248 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    51568 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22398 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-05-07 21:13:54.808312 wg_utilities-3.7.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 21:26:00.176983 wg_utilities-3.8.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-07-12 21:26:00.176983 wg_utilities-3.8.0/README.md
+-rw-r--r--   0        0        0     4798 2023-07-12 21:26:00.180983 wg_utilities-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      685 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4207 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    23741 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56658 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7580 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13265 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15915 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    27248 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    51568 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22398 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-07-12 21:26:00.248983 wg_utilities-3.8.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7006 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5786 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-07-12 21:26:00.252983 wg_utilities-3.8.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 wg_utilities-3.8.0/PKG-INFO
```

### Comparing `wg_utilities-3.7.0/LICENSE` & `wg_utilities-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/README.md` & `wg_utilities-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/pyproject.toml` & `wg_utilities-3.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.7.0"
+version = "3.8.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
@@ -18,28 +18,29 @@
 # Dependencies
 
 [tool.poetry.dependencies]
 python = "^3.10"
 async-upnp-client = { version = "*", optional = true }
 botocore = { version = "*", optional = true }
 flask = { version = ">=2.0.2", optional = true }
-"jetson.gpio" = { version = "*", markers = "sys_platform == 'linux'", optional = true  }
+"jetson.gpio" = { version = "*", platform = "linux", optional = true }
 lxml = { version = "==4.9.2", optional = true }
 pigpio = { version = "*", optional = true }
 pillow = { version = "*", optional = true }
-pydantic = { version = "*", optional = true }
-pyjwt = { version = "~=2.6.0", optional = true }
+pyjwt = { version = ">=2.6,<2.8", optional = true }
 python-dotenv = { version = "*", optional = true }
 pytz = ">=2022.1"
 requests = { version = ">=2.26.0", optional = true }
-"rpi.gpio" = { version = "*", markers = "sys_platform == 'linux'",  optional = true }
-spidev = { version = "*", markers = "sys_platform == 'linux'", optional = true  }
+"rpi.gpio" = { version = "*", platform = "linux", optional = true }
+spidev = { version = "*", platform = "linux", optional = true }
 strenum = { version = "*", optional = true }
 tzlocal = { version = "*", optional = true }
 xmltodict = { version = "*", optional = true }
+pydantic = "<2.0.0"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pylint = "*"
 pre-commit = "*"
 mypy = "*"
 types-requests = "*"
@@ -181,19 +182,20 @@
     "F",   # Pyflakes
     "N",   # PEP8 Naming
     "RUF", # Ruff-specific rules
     "UP",  # PyUpgrade
     "W",   # Pycodestyle warnings
 ]
 ignore = [
-    "D107",  # public-init
-    "D202",  # no-blank-line-after-function
-    "D203",  # one-blank-line-before-class
-    "D213",  # multi-line-summary-second-line
-    "D400",  # first-line-end-with-period
-    "D406",  # new-line-after-section-name
-    "D407",  # dashed-underline-after-section
-    "UP037", # quoted-annotation
+    "D107",   # public-init
+    "D202",   # no-blank-line-after-function
+    "D203",   # one-blank-line-before-class
+    "D213",   # multi-line-summary-second-line
+    "D400",   # first-line-end-with-period
+    "D406",   # new-line-after-section-name
+    "D407",   # dashed-underline-after-section
+    "UP037",  # quoted-annotation
+    "RUF012", # mutable-default-argument
 ]
 
 [tool.ruff.mccabe]
 max-complexity = 20
```

### Comparing `wg_utilities-3.7.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.8.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.8.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/_google.py` & `wg_utilities-3.8.0/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.8.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.8.0/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.8.0/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.8.0/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.8.0/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.8.0/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.8.0/wg_utilities/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.8.0/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.8.0/wg_utilities/clients/truelayer.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.8.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.8.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.8.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # EPD hardware init end
         return 0
 
     def getbuffer(self, image: Image) -> list[int]:  # noqa: D102
         buf = [0xFF] * (int(self.width / 8) * self.height)
         image_monocolor = image.convert("1")
         imwidth, imheight = image_monocolor.size
-        pixels = image_monocolor.load()  # type: ignore[func-returns-value]
+        pixels = image_monocolor.load()
         if imwidth == self.width and imheight == self.height:
             debug("Vertical")
             for y in range(imheight):
                 for x in range(imwidth):
                     # Set the bits for the column of pixels at the current position.
                     if pixels[x, y] == 0:
                         buf[int((x + y * self.width) / 8)] &= ~(0x80 >> (x % 8))
```

### Comparing `wg_utilities-3.7.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.8.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.8.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.8.0/wg_utilities/exceptions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Raises:
         ValueError: if the HA_LOG_ENDPOINT isn't set
         Exception: if posting the exception to HA fails, then an exception is raised
     """
     payload = {
         "client": gethostname(),
-        "message": f"{type(exc).__name__} in `{stack()[2].filename}`: {repr(exc)}",
+        "message": f"{type(exc).__name__} in `{stack()[2].filename}`: {exc!r}",
         "traceback": format_exc(),
     }
 
     try:
         try:
             # If the host is on the same network as HA, then an HTTP local URL can be
             # used
@@ -66,32 +66,41 @@
 
 def on_exception(
     exception_callback: Callable[[Exception], Any] = send_exception_to_home_assistant,
     *,
     raise_after_callback: bool = True,
     logger: Logger | None = None,
     ignore_exception_types: Iterable[type[Exception]] | None = None,
+    default_return_value: Any | None = None,
     _suppress_ignorant_warnings: bool | None = None,
 ) -> Callable[[Any], Any]:
     # pylint: disable=useless-type-doc,useless-param-doc
     """Parameterize the inner decorator with a decorator factory.
 
     Args:
         exception_callback (Callable): callback function to process the exception
         raise_after_callback (bool): raise the exception after the callback has run
         logger (Logger): optional logger for logging the exception
         ignore_exception_types (Iterable[type[Exception]]): optional iterable of
             exception types to ignore
+        default_return_value (Any): optional default return value for the decorated
+            function
         _suppress_ignorant_warnings (bool): optional flag to suppress warnings about
             ignoring exception types
 
     Returns:
         Callable: the actual decorator
     """
 
+    if default_return_value is not None and raise_after_callback:
+        raise ValueError(
+            "The `default_return_value` parameter can only be set when"
+            " `raise_after_callback` is False."
+        )
+
     def _decorator(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
         """Allow simple cover-all exception handler callback behaviour.
 
         Args:
             func (Callable): the function being wrapped
 
         Returns:
@@ -140,15 +149,15 @@
                         )
                 else:
                     exception_callback(exc)
 
                     if raise_after_callback:
                         raise
 
-                return None
+                return default_return_value
 
         return worker
 
     return _decorator
 
 
 __all__ = ["on_exception", "send_exception_to_home_assistant", "ResourceNotFoundError"]
```

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.8.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.8.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.8.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.8.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/json.py` & `wg_utilities-3.8.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/processes.py` & `wg_utilities-3.8.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.8.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/functions/xml.py` & `wg_utilities-3.8.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.8.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.8.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.7.0/PKG-INFO` & `wg_utilities-3.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.7.0
+Version: 3.8.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
@@ -22,16 +22,16 @@
 Requires-Dist: async-upnp-client ; extra == "devices-yamaha-yas-209"
 Requires-Dist: botocore
 Requires-Dist: flask (>=2.0.2) ; extra == "clients"
 Requires-Dist: jetson.gpio ; sys_platform == "linux"
 Requires-Dist: lxml (==4.9.2) ; extra == "functions"
 Requires-Dist: pigpio ; extra == "devices-dht22"
 Requires-Dist: pillow ; extra == "devices-epd"
-Requires-Dist: pydantic ; extra == "clients" or extra == "devices-yamaha-yas-209"
-Requires-Dist: pyjwt (>=2.6.0,<2.7.0) ; extra == "clients"
+Requires-Dist: pydantic (<2.0.0) ; extra == "clients" or extra == "devices-yamaha-yas-209"
+Requires-Dist: pyjwt (>=2.6,<2.8) ; extra == "clients"
 Requires-Dist: python-dotenv ; extra == "clients" or extra == "exceptions"
 Requires-Dist: pytz (>=2022.1) ; extra == "clients"
 Requires-Dist: requests (>=2.26.0) ; extra == "clients" or extra == "exceptions"
 Requires-Dist: rpi.gpio ; (sys_platform == "linux") and (extra == "devices-epd")
 Requires-Dist: spidev ; (sys_platform == "linux") and (extra == "devices-epd")
 Requires-Dist: strenum ; extra == "clients"
 Requires-Dist: tzlocal ; extra == "clients"
```

