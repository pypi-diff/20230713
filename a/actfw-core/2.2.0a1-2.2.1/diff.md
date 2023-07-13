# Comparing `tmp/actfw-core-2.2.0a1.tar.gz` & `tmp/actfw_core-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actfw-core-2.2.0a1.tar", max compression
+gzip compressed data, was "actfw_core-2.2.1.tar", max compression
```

## Comparing `actfw-core-2.2.0a1.tar` & `actfw_core-2.2.1.tar`

### file list

```diff
@@ -1,31 +1,40 @@
--rw-r--r--   0        0        0     1067 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/LICENSE.txt
--rw-r--r--   0        0        0     1955 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/README.md
--rw-r--r--   0        0        0     1678 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/__init__.py
--rw-r--r--   0        0        0      113 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/agent_app_protocol/__init__.py
--rw-r--r--   0        0        0     3297 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/agent_app_protocol/service_server.py
--rw-r--r--   0        0        0      152 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/compat/queue.py
--rw-r--r--   0        0        0     3676 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/schema/agent_app_protocol.py
--rw-r--r--   0        0        0      158 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/util/result.py
--rw-r--r--   0        0        0     1183 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/_private/util/thread.py
--rw-r--r--   0        0        0     2305 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/application.py
--rw-r--r--   0        0        0     5956 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/capture.py
--rw-r--r--   0        0        0     3158 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/command_server.py
--rw-r--r--   0        0        0        0 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/py.typed
--rw-r--r--   0        0        0      209 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/schema/agent_app_protocol.py
--rw-r--r--   0        0        0     2700 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/service_client.py
--rw-r--r--   0        0        0      281 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/__init__.py
--rw-r--r--   0        0        0     1381 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/consumer.py
--rw-r--r--   0        0        0      150 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/isolated.py
--rw-r--r--   0        0        0     1318 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/join.py
--rw-r--r--   0        0        0      841 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/pipe.py
--rw-r--r--   0        0        0     1816 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/producer.py
--rw-r--r--   0        0        0      604 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/task.py
--rw-r--r--   0        0        0      910 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/task/tee.py
--rw-r--r--   0        0        0     2714 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/util/pad.py
--rw-r--r--   0        0        0       41 2022-04-11 08:42:29.359499 actfw-core-2.2.0a1/actfw_core/v4l2/__init__.py
--rw-r--r--   0        0        0    25843 2022-04-11 08:42:29.363499 actfw-core-2.2.0a1/actfw_core/v4l2/control.py
--rw-r--r--   0        0        0     7862 2022-04-11 08:42:29.363499 actfw-core-2.2.0a1/actfw_core/v4l2/types.py
--rw-r--r--   0        0        0    33703 2022-04-11 08:42:29.363499 actfw-core-2.2.0a1/actfw_core/v4l2/video.py
--rw-r--r--   0        0        0     2661 2022-04-11 08:42:29.363499 actfw-core-2.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     3046 2022-04-11 08:42:49.173573 actfw-core-2.2.0a1/setup.py
--rw-r--r--   0        0        0     3084 2022-04-11 08:42:49.173990 actfw-core-2.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-13 07:17:02.764409 actfw_core-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     2161 2023-07-13 07:17:02.764409 actfw_core-2.2.1/README.md
+-rw-r--r--   0        0        0     1713 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/agent_app_protocol/__init__.py
+-rw-r--r--   0        0        0     3297 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/agent_app_protocol/service_server.py
+-rw-r--r--   0        0        0      152 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/compat/queue.py
+-rw-r--r--   0        0        0     3676 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/schema/agent_app_protocol.py
+-rw-r--r--   0        0        0      158 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/util/result.py
+-rw-r--r--   0        0        0     1183 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/_private/util/thread.py
+-rw-r--r--   0        0        0     2305 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/application.py
+-rw-r--r--   0        0        0     6932 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/capture.py
+-rw-r--r--   0        0        0     3277 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/command_server.py
+-rw-r--r--   0        0        0     1304 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/data/LICENSE.txt
+-rw-r--r--   0        0        0      100 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/data/README.md
+-rw-r--r--   0        0        0    19023 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/data/imx219.json
+-rw-r--r--   0        0        0    19003 2023-07-13 07:17:02.764409 actfw_core-2.2.1/actfw_core/data/ov5647.json
+-rw-r--r--   0        0        0       51 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/linux/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/linux/dma_heap.py
+-rw-r--r--   0        0        0      951 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/linux/ioctl.py
+-rw-r--r--   0        0        0      197 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/linux/types.py
+-rw-r--r--   0        0        0        0 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/py.typed
+-rw-r--r--   0        0        0      209 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/schema/agent_app_protocol.py
+-rw-r--r--   0        0        0     2700 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/service_client.py
+-rw-r--r--   0        0        0     6913 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/system.py
+-rw-r--r--   0        0        0      281 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/__init__.py
+-rw-r--r--   0        0        0     1381 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/consumer.py
+-rw-r--r--   0        0        0      150 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/isolated.py
+-rw-r--r--   0        0        0     1318 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/join.py
+-rw-r--r--   0        0        0      841 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/pipe.py
+-rw-r--r--   0        0        0     1816 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/producer.py
+-rw-r--r--   0        0        0      604 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/task.py
+-rw-r--r--   0        0        0      910 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/task/tee.py
+-rw-r--r--   0        0        0    38807 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/unicam_isp_capture.py
+-rw-r--r--   0        0        0     2714 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/util/pad.py
+-rw-r--r--   0        0        0       41 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/v4l2/__init__.py
+-rw-r--r--   0        0        0    26657 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/v4l2/control.py
+-rw-r--r--   0        0        0    12822 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/v4l2/types.py
+-rw-r--r--   0        0        0    49870 2023-07-13 07:17:02.768409 actfw_core-2.2.1/actfw_core/v4l2/video.py
+-rw-r--r--   0        0        0     2659 2023-07-13 07:17:02.768409 actfw_core-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 actfw_core-2.2.1/PKG-INFO
```

### Comparing `actfw-core-2.2.0a1/LICENSE.txt` & `actfw_core-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/README.md` & `actfw_core-2.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -86,9 +86,13 @@
 ### Releasing package & API doc
 
 CI will automatically do.
 Follow the following branch/tag rules.
 
 1. Make changes for next version in `master` branch (via pull-requests).
 2. Make a PR that updates version in `pyproject.toml` and merge it to `master` branch.
-3. Create Git tag from `master` branch's HEAD named `release-<New version>`. E.g. `release-1.4.0`.
+3. Create GitHub release from `master` branch's HEAD.
+    1. [Draft a new release](https://github.com/Idein/actfw-core/releases/new).
+    2. Create new tag named `release-<New version>` (e.g. `release-1.4.0`) from `Choose a tag` pull down menu.
+    3. Write title and description.
+    4. Publish release.
 4. Then CI will build/upload package to PyPI & API doc to GitHub Pages.
```

### Comparing `actfw-core-2.2.0a1/actfw_core/__init__.py` & `actfw_core-2.2.1/actfw_core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 from typing import Any, Callable, Dict, List
 
-from . import capture, task  # noqa: F401
+from . import capture, linux, system, task, unicam_isp_capture  # noqa: F401
 from .application import Application  # noqa: F401
 from .command_server import CommandServer  # noqa: F401
 from .service_client import ServiceClient  # noqa: F401
 
 
 def notify(
     notification: List[Dict[str, Any]],
```

### Comparing `actfw-core-2.2.0a1/actfw_core/_private/agent_app_protocol/service_server.py` & `actfw_core-2.2.1/actfw_core/_private/agent_app_protocol/service_server.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/_private/schema/agent_app_protocol.py` & `actfw_core-2.2.1/actfw_core/_private/schema/agent_app_protocol.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/_private/util/thread.py` & `actfw_core-2.2.1/actfw_core/_private/util/thread.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/application.py` & `actfw_core-2.2.1/actfw_core/application.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/capture.py` & `actfw_core-2.2.1/actfw_core/capture.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
-from typing import Callable, Generic, Iterable, Tuple, TypeVar
+from typing import Callable, Generic, Iterable, Tuple, TypeVar, Union
 
+from actfw_core.system import DeviceInfo, EnvironmentVariableNotSet, get_actcast_firmware_type
 from actfw_core.v4l2.video import V4L2_PIX_FMT, Video, VideoPort  # type: ignore
 
 from .task import Producer
 from .util.pad import _PadBase, _PadDiscardingOld
 
 T = TypeVar("T")
 
@@ -39,25 +40,25 @@
 
     FormatSelector = enum.Enum("FormatSelector", "DEFAULT PROPER MAXIMUM")
 
     """Captured Frame Producer for Video4Linux"""
 
     def __init__(
         self,
-        device: str = "/dev/video0",
+        device: Union[str, DeviceInfo] = "/dev/video0",
         size: Tuple[int, int] = (640, 480),
         framerate: int = 30,
         expected_format: V4L2_PIX_FMT = V4L2_PIX_FMT.RGB24,
         fallback_formats: Iterable[V4L2_PIX_FMT] = (V4L2_PIX_FMT.YUYV, V4L2_PIX_FMT.MJPEG),
         format_selector: FormatSelector = FormatSelector.DEFAULT,
     ) -> None:
         """
 
         Args:
-            device (str): v4l device path
+            device (str | DeviceInfo): v4l device path or info
             size (int, int): expected capture resolution
             framerate (int): expected capture framerate
             expected_format (:class:`~actfw_core.v4l2.video.V4L2_PIX_FMT`): expected capture format
             fallback_formats (list of :class:`~actfw_core.v4l2.video.V4L2_PIX_FMT`): fallback capture format
             format_selector (:class:`~actfw_core.capture.V4LCameraCapture.FormatSelector): how to select a format from listed formats supported by a camera. # noqa: B006 B950
                 DEFAULT selects the first format that meets the conditions.
                 PROPER selects the smallest format that meets the conditions.
@@ -68,19 +69,41 @@
 
         Notes:
             If a camera doesn't support the expected_format,
             try to capture one of the fallback_formats and convert it to expected_format.
 
         """
         super().__init__()
+        if isinstance(device, DeviceInfo):
+            device_path = None
+            for node in device.nodes:
+                if node.label == "image_source":
+                    device_path = node.path
+            if device_path is None:
+                raise RuntimeError("not found image_source.")
+            else:
+                device = str(device_path)
+        elif isinstance(device, str):
+            pass
+        else:
+            raise RuntimeError(f"the type of device={device} must be str or DeviceInfo.")
+
         self.video = Video(device)
 
         width, height = size
 
-        if self.video.query_capability() == VideoPort.CSI:
+        cap = self.video.query_capability()
+        try:
+            firmware_type = get_actcast_firmware_type()
+            if firmware_type == "raspberrypi-bullseye" and cap == VideoPort.CSI:
+                raise RuntimeError("CSI camera is not supported in bullseye yet.")
+        except EnvironmentVariableNotSet:
+            pass
+
+        if cap == VideoPort.CSI:
 
             # workaround for bcm2835-v4l2 format pixsize & bytesperline bug
             width = (width + 31) // 32 * 32
             height = (height + 15) // 16 * 16
 
             # workaround for bcm2835-v4l2 IMX219 32x32 -> 800x800 capture timeout bug
             candidates = self.video.lookup_config(64, 64, 5, V4L2_PIX_FMT.RGB24, V4L2_PIX_FMT.RGB24)
```

### Comparing `actfw-core-2.2.0a1/actfw_core/command_server.py` & `actfw_core-2.2.1/actfw_core/command_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,18 @@
             while self.running:
                 with self.img_lock:
                     if self.img is None:
                         continue
                     else:
                         break
             try:
-                assert self.img is not None
+                if self.img is None:
+                    # this server may be terminating
+                    # re-check self.running
+                    continue
 
                 conn, _ = s.accept()
                 request, err = CommandRequest.parse(conn)
                 if err:
                     response = CommandResponse(
                         copy.copy(request.id_),
                         Status.GENERAL_ERROR,
```

### Comparing `actfw-core-2.2.0a1/actfw_core/service_client.py` & `actfw_core-2.2.1/actfw_core/service_client.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/consumer.py` & `actfw_core-2.2.1/actfw_core/task/consumer.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/join.py` & `actfw_core-2.2.1/actfw_core/task/join.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/pipe.py` & `actfw_core-2.2.1/actfw_core/task/pipe.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/producer.py` & `actfw_core-2.2.1/actfw_core/task/producer.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/task.py` & `actfw_core-2.2.1/actfw_core/task/task.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/task/tee.py` & `actfw_core-2.2.1/actfw_core/task/tee.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/util/pad.py` & `actfw_core-2.2.1/actfw_core/util/pad.py`

 * *Files identical despite different names*

### Comparing `actfw-core-2.2.0a1/actfw_core/v4l2/control.py` & `actfw_core-2.2.1/actfw_core/v4l2/control.py`

 * *Files 6% similar despite different names*

```diff
@@ -398,14 +398,26 @@
     DETECT_CLASS = V4L2_CTRL_CLASS.DETECT | 1
 
     DETECT_MD_MODE = DETECT_CLASS_BASE + 1
     DETECT_MD_GLOBAL_THRESHOLD = DETECT_CLASS_BASE + 2
     DETECT_MD_THRESHOLD_GRID = DETECT_CLASS_BASE + 3
     DETECT_MD_REGION_GRID = DETECT_CLASS_BASE + 4
 
+    # For bcm2835-isp
+    USER_BCM2835_ISP_BASE = USER_BASE + 0x10E0
+    USER_BCM2835_ISP_CC_MATRIX = USER_BCM2835_ISP_BASE + 0x0001
+    USER_BCM2835_ISP_LENS_SHADING = USER_BCM2835_ISP_BASE + 0x0002
+    USER_BCM2835_ISP_BLACK_LEVEL = USER_BCM2835_ISP_BASE + 0x0003
+    USER_BCM2835_ISP_GEQ = USER_BCM2835_ISP_BASE + 0x0004
+    USER_BCM2835_ISP_GAMMA = USER_BCM2835_ISP_BASE + 0x0005
+    USER_BCM2835_ISP_DENOISE = USER_BCM2835_ISP_BASE + 0x0006
+    USER_BCM2835_ISP_SHARPEN = USER_BCM2835_ISP_BASE + 0x0007
+    USER_BCM2835_ISP_DPC = USER_BCM2835_ISP_BASE + 0x0008
+    USER_BCM2835_ISP_CDN = USER_BCM2835_ISP_BASE + 0x0009
+
 
 class V4L2_POWER_LINE(enum.IntEnum):
     FREQUENCY_DISABLED = 0
     FREQUENCY_50HZ = 1
     FREQUENCY_60HZ = 2
     FREQUENCY_AUTO = 3
 
@@ -909,14 +921,19 @@
 V4L2_JPEG_ACTIVE_MARKER_APP0 = 1 << 0
 V4L2_JPEG_ACTIVE_MARKER_APP1 = 1 << 1
 V4L2_JPEG_ACTIVE_MARKER_COM = 1 << 16
 V4L2_JPEG_ACTIVE_MARKER_DQT = 1 << 17
 V4L2_JPEG_ACTIVE_MARKER_DHT = 1 << 18
 
 
+V4L2_CTRL_WHICH_CUR_VAL = 0
+V4L2_CTRL_WHICH_DEF_VAL = 0x0F000000
+V4L2_CTRL_WHICH_REQUEST_VAL = 0x0F010000
+
+
 class V4L2_CTRL_TYPE(enum.IntEnum):
     INTEGER = 1
     BOOLEAN = 2
     MENU = 3
     BUTTON = 4
     INTEGER64 = 5
     CTRL_CLASS = 6
@@ -936,7 +953,10 @@
 V4L2_CTRL_FLAG_INACTIVE = 0x0010
 V4L2_CTRL_FLAG_SLIDER = 0x0020
 V4L2_CTRL_FLAG_WRITE_ONLY = 0x0040
 V4L2_CTRL_FLAG_VOLATILE = 0x0080
 V4L2_CTRL_FLAG_HAS_PAYLOAD = 0x0100
 V4L2_CTRL_FLAG_EXECUTE_ON_WRITE = 0x0200
 V4L2_CTRL_FLAG_MODIFY_LAYOUT = 0x0400
+
+V4L2_CTRL_FLAG_NEXT_CTRL = 0x80000000
+V4L2_CTRL_FLAG_NEXT_COMPOUND = 0x40000000
```

### Comparing `actfw-core-2.2.0a1/actfw_core/v4l2/video.py` & `actfw_core-2.2.1/actfw_core/v4l2/video.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # type: ignore
 # flake8: noqa
 
+import copy
 import enum
 import errno
 import io
 import itertools
 import mmap
 import os
 import select
+import time
+import warnings
 from ctypes import *
 from ctypes.util import find_library
+from typing import List
 
+from actfw_core.linux.ioctl import _IOR, _IOW, _IOWR
 from actfw_core.v4l2.control import *
 from actfw_core.v4l2.types import *
 
 
 class _libv4l2(object):
     def __init__(self):
         self.lib = None
@@ -99,71 +104,37 @@
             raise FileNotFoundError("Not found: 'libv4lconvert.so'")
         return self.lib.v4lconvert_try_format(*args, **kwargs)
 
 
 _v4l2 = _libv4l2()
 _v4lconvert = _libv4lconvert()
 
-_IOC_NRBITS = 8
-_IOC_TYPEBITS = 8
-
-_IOC_SIZEBITS = 14
-_IOC_DIRBITS = 2
-
-_IOC_NRMASK = (1 << _IOC_NRBITS) - 1
-_IOC_TYPEMASK = (1 << _IOC_TYPEBITS) - 1
-_IOC_SIZEMASK = (1 << _IOC_SIZEBITS) - 1
-_IOC_DIRMASK = (1 << _IOC_DIRBITS) - 1
-
-_IOC_NRSHIFT = 0
-_IOC_TYPESHIFT = _IOC_NRSHIFT + _IOC_NRBITS
-_IOC_SIZESHIFT = _IOC_TYPESHIFT + _IOC_TYPEBITS
-_IOC_DIRSHIFT = _IOC_SIZESHIFT + _IOC_SIZEBITS
-
-_IOC_NONE = 0
-_IOC_WRITE = 1
-_IOC_READ = 2
-
-
-def _IOC(dir, type, nr, size):
-    return (dir << _IOC_DIRSHIFT) | (ord(type) << _IOC_TYPESHIFT) | (nr << _IOC_NRSHIFT) | (size << _IOC_SIZESHIFT)
-
-
-def _IO(type, nr):
-    return _IOC(_IOC_NONE, type, nr, 0)
-
-
-def _IOR(type, nr, size):
-    return _IOC(_IOC_READ, type, nr, sizeof(size))
-
-
-def _IOW(type, nr, size):
-    return _IOC(_IOC_WRITE, type, nr, sizeof(size))
-
-
-def _IOWR(type, nr, size):
-    return _IOC(_IOC_READ | _IOC_WRITE, type, nr, sizeof(size))
-
 
 class _VIDIOC(enum.IntEnum):
     QUERYCAP = _IOR("V", 0, capability)
     ENUM_FMT = _IOWR("V", 2, fmtdesc)
     S_FMT = _IOWR("V", 5, format)
+    SUBDEV_S_FMT = _IOWR("V", 5, subdev_format)
+    S_SELECTION = _IOWR("V", 95, selection)
     REQBUFS = _IOWR("V", 8, requestbuffers)
     QUERYBUF = _IOWR("V", 9, buffer)
     QBUF = _IOWR("V", 15, buffer)
+    EXPBUF = _IOWR("V", 16, exportbuffer)
     DQBUF = _IOWR("V", 17, buffer)
     STREAMON = _IOW("V", 18, c_int)
     STREAMOFF = _IOW("V", 19, c_int)
     S_PARM = _IOWR("V", 22, streamparm)
     G_CTRL = _IOWR("V", 27, control)
     S_CTRL = _IOWR("V", 28, control)
     QUERYCTRL = _IOWR("V", 36, queryctrl)
+    G_EXT_CTRLS = _IOWR("V", 71, v4l2_ext_controls)
+    S_EXT_CTRLS = _IOWR("V", 72, v4l2_ext_controls)
     ENUM_FRAMESIZES = _IOWR("V", 74, frmsizeenum)
     ENUM_FRAMEINTERVALS = _IOWR("V", 75, frmivalenum)
+    QUERY_EXT_CTRL = _IOWR("V", 103, v4l2_query_ext_ctrl)
 
 
 _V4L2_CAP_VIDEO_CAPTURE = 0x00000001
 _V4L2_CAP_VIDEO_OUTPUT = 0x00000002
 _V4L2_CAP_VIDEO_OVERLAY = 0x00000004
 _V4L2_CAP_VBI_CAPTURE = 0x00000010
 _V4L2_CAP_VBI_OUTPUT = 0x00000020
@@ -335,27 +306,33 @@
     SE401 = _fourcc("S", "4", "0", "1")
     S5C_UYVY_JPG = _fourcc("S", "5", "C", "I")
     Y8I = _fourcc("Y", "8", "I", " ")
     Y12I = _fourcc("Y", "1", "2", "I")
     Z16 = _fourcc("Z", "1", "6", " ")
 
 
+class V4L2_META_FMT(enum.IntEnum):
+    BCM2835_ISP_STATS = _fourcc("B", "S", "T", "A")
+
+
 class V4L2_BUF_TYPE(enum.IntEnum):
     VIDEO_CAPTURE = 1
     VIDEO_OUTPUT = 2
     VIDEO_OVERLAY = 3
     VBI_CAPTURE = 4
     VBI_OUTPUT = 5
     SLICED_VBI_CAPTURE = 6
     SLICED_VBI_OUTPUT = 7
     VIDEO_OUTPUT_OVERLAY = 8
     VIDEO_CAPTURE_MPLANE = 9
     VIDEO_OUTPUT_MPLANE = 10
     SDR_CAPTURE = 11
     SDR_OUTPUT = 12
+    META_CAPTURE = 13
+    META_OUTPUT = 14
     PRIVATE = 0x80
 
 
 class V4L2_FRMSIZE_TYPE(enum.IntEnum):
     DISCRETE = 1
     CONTINUOUS = 2
     STEPWISE = 3
@@ -387,14 +364,459 @@
 class V4L2_MEMORY(enum.IntEnum):
     MMAP = 1
     USERPTR = 2
     OVERLAY = 3
     DMABUF = 4
 
 
+class V4L2_SUBDEV_FORMAT_WHENCE(enum.IntEnum):
+    TRY = 0
+    ACTIVE = 1
+
+
+class MEDIA_BUS_FMT(enum.IntEnum):
+    SBGGR8_1X8 = 0x3001
+    SBGGR10_1X10 = 0x3007
+    SGBRG10_1X10 = 0x300E
+
+
+class V4L2_SEL_TGT(enum.IntEnum):
+    CROP = 0x0000
+    CROP_DEFAULT = 0x0001
+    CROP_BOUNDS = 0x0002
+    NATIVE_SIZE = 0x0003
+    COMPOSE = 0x0100
+    COMPOSE_DEFAULT = 0x0101
+    COMPOSE_BOUNDS = 0x0102
+    COMPOSE_PADDED = 0x0103
+
+
+class V4L2_SEL_FLAG(enum.IntEnum):
+    GE = 1 << 0
+    LE = 1 << 1
+    KEEP_CONFIG = 1 << 2
+
+
+class RawVideo(object):
+    def __init__(self, device, blocking=False, init_controls=[], v4l2_buf_type=V4L2_BUF_TYPE.VIDEO_CAPTURE):
+        self.device = device
+        self.v4l2_buf_type = v4l2_buf_type
+        flags = os.O_RDWR
+        if not blocking:
+            flags |= os.O_NONBLOCK
+        self.device_fd = os.open(self.device, flags)
+        self.buffers: Optional[List[VideoBuffer]] = None  # set when enqueu
+
+        if len(init_controls) != 0:
+            self.init_controls(init_controls)
+
+    def close(self):
+        os.close(self.device_fd)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, ex_type, ex_value, trace):
+        self.close()
+
+    def _ioctl(self, request, arg):
+        while True:
+            result = _v4l2.ioctl(self.device_fd, request, arg)
+            e = get_errno()
+            if not (((-1 == result) and ((e == errno.EINTR)))):
+                break
+        return result
+
+    def set_pix_format(self, expected_width, expected_height, expected_format: V4L2_PIX_FMT):
+
+        fmt = format()
+        fmt.type = self.v4l2_buf_type
+        fmt.fmt.pix.width = expected_width
+        fmt.fmt.pix.height = expected_height
+        fmt.fmt.pix.pixelformat = expected_format
+        fmt.fmt.pix.field = V4L2_FIELD.INTERLACED  # TODO: check if this is appropriate
+        result = self._ioctl(_VIDIOC.S_FMT, byref(fmt))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_S_FMT){}".format(errno.errorcode[get_errno()]))
+
+        self.fmt = fmt
+        return (
+            fmt.fmt.pix.width,
+            fmt.fmt.pix.height,
+            fmt.fmt.pix.pixelformat,
+        )
+
+    def set_meta_format(self, dataformat: V4L2_META_FMT, buffersize):
+        fmt = format()
+        fmt.type = V4L2_BUF_TYPE.META_CAPTURE
+        fmt.fmt.meta.dataformat = dataformat
+        fmt.fmt.meta.buffersize = buffersize
+        result = self._ioctl(_VIDIOC.S_FMT, byref(fmt))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_S_FMT){}".format(errno.errorcode[get_errno()]))
+
+        self.fmt = fmt
+
+    def set_subdev_format(self, expected_width, expected_height, expected_format: MEDIA_BUS_FMT):
+        fmt = subdev_format()
+        fmt.pad = 0  # hard code
+        fmt.which = V4L2_SUBDEV_FORMAT_WHENCE.ACTIVE
+        fmt.format.width = expected_width
+        fmt.format.height = expected_height
+        fmt.format.code = expected_format
+
+        result = self._ioctl(_VIDIOC.SUBDEV_S_FMT, byref(fmt))
+        if -1 == result:
+            raise RuntimeError("ioctl(SUBDEV_S_FMT){}".format(errno.errorcode[get_errno()]))
+
+        self.subdev_fmt = fmt
+        return (fmt.format.width, fmt.format.height, fmt.format.code)
+
+    def set_selection(self, left, top, width, height):
+        sel = selection()
+        sel.type = self.v4l2_buf_type
+        sel.target = V4L2_SEL_TGT.CROP
+        sel.flags = 0
+        sel.r.left = left
+        sel.r.top = top
+        sel.r.width = width
+        sel.r.height = height
+
+        result = self._ioctl(_VIDIOC.S_SELECTION, byref(sel))
+        if result != 0:
+            raise RuntimeError(f"ioctl(S_SELECTION){errno.errorcode[get_errno()]}")
+
+    def init_controls(self, targets):
+        queries = self.query_ext_controls()
+        if len(queries) == 0:
+            return
+        else:
+            ctrls = []
+            for q in queries:
+                if targets == ["all"] or q.name.decode() in targets:
+                    i = self.make_initializer(q)
+                    if i is not None:
+                        print(f"init {q.name}")
+                        ctrls.append(i)
+            if len(ctrls) != 0:
+                self.set_ext_controls(ctrls)
+
+    def query_ext_controls(self) -> List[v4l2_query_ext_ctrl]:
+        res = []
+        query = v4l2_query_ext_ctrl()
+        query.id = V4L2_CTRL_FLAG_NEXT_CTRL | V4L2_CTRL_FLAG_NEXT_COMPOUND
+        while 0 == self._ioctl(_VIDIOC.QUERY_EXT_CTRL, byref(query)):
+            if query.type != V4L2_CTRL_TYPE.CTRL_CLASS:
+                q = copy.copy(query)
+                res.append(q)
+            query.id |= V4L2_CTRL_FLAG_NEXT_CTRL | V4L2_CTRL_FLAG_NEXT_COMPOUND
+
+        return res
+
+    def make_initializer(self, query):
+        if query.flags & V4L2_CTRL_FLAG_DISABLED:
+            return None
+        if query.flags & V4L2_CTRL_FLAG_READ_ONLY:
+            return None
+
+        if query.id == V4L2_CID.USER_BCM2835_ISP_LENS_SHADING:
+            return None
+
+        ctrl = v4l2_ext_control()
+        ctrl.id = query.id
+        ctrl.size = 0
+        ctrl.reserved2 = (c_uint32 * 1)()
+        ctrl.reserved2[0] = 0
+
+        if query.type in [V4L2_CTRL_TYPE.INTEGER, V4L2_CTRL_TYPE.BOOLEAN, V4L2_CTRL_TYPE.MENU]:
+            ctrl.value = query.default_value
+        elif query.type == V4L2_CTRL_TYPE.INTEGER64:
+            ctrl.value64 = query.default_value
+        elif query.type == V4L2_CTRL_TYPE.U8:
+            ctrl.size = query.elems * query.elem_size
+            val = (c_uint8 * query.elems)()
+            for i in range(query.elems):
+                val[i] = query.default_value
+            ctrl.ptr = cast(val, c_void_p)
+        else:
+            return None
+
+        return ctrl
+
+    def get_ext_controls(self, ids: List[V4L2_CID]) -> List[v4l2_ext_control]:
+        ctrls = v4l2_ext_controls()
+        ctr_arr = (v4l2_ext_control * len(ids))()
+        for (i, ctrl_id) in enumerate(ids):
+            ctr_arr[i].id = ctrl_id
+
+        ctrls.which = V4L2_CTRL_WHICH_CUR_VAL
+        ctrls.controls = ctr_arr
+        ctrls.count = len(ctr_arr)
+        ctrls.request_fd = 0
+        result = self._ioctl(_VIDIOC.G_EXT_CTRLS, byref(ctrls))
+
+        if -1 == result:
+            raise RuntimeError("ioctl(G_EXT_CTRLS){}".format(errno.errorcode[get_errno()]))
+
+        return ctr_arr
+
+    def set_ext_controls(self, ctr_list: List[v4l2_ext_controls]):
+        ctrls = v4l2_ext_controls()
+        ctr_arr = (v4l2_ext_control * len(ctr_list))()
+        for (i, ctrl) in enumerate(ctr_list):
+            ctr_arr[i] = ctrl
+
+        ctrls.which = V4L2_CTRL_WHICH_CUR_VAL
+        ctrls.controls = ctr_arr
+        ctrls.count = len(ctr_arr)
+        result = self._ioctl(_VIDIOC.S_EXT_CTRLS, byref(ctrls))
+
+        if -1 == result:
+            raise RuntimeError("ioctl(S_EXT_CTRLS){}".format(errno.errorcode[get_errno()]))
+
+        return ctr_arr
+
+    def set_framerate(self, conf):
+
+        parm = streamparm()
+        parm.type = self.v4l2_buf_type
+        parm.parm.capture.timeperframe = conf.interval
+        parm.parm.capture.capturemode = V4L2_MODE_HIGHQUALITY
+
+        result = self._ioctl(_VIDIOC.S_PARM, byref(parm))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_S_PARM)")
+
+        return True
+
+    def set_horizontal_flip(self, flip):
+        """
+        Flip video (horizontal) if it supported.
+
+        Args:
+            flip (boolean): enable flip
+
+        Returns:
+            boolean: result
+        """
+
+        qctrl = queryctrl()
+        qctrl.id = V4L2_CID.HFLIP
+        result = self._ioctl(_VIDIOC.QUERYCTRL, byref(qctrl))
+        if -1 == result:
+            return False
+        if qctrl.flags & V4L2_CTRL_FLAG_DISABLED:
+            return False
+
+        ctrl = control()
+        ctrl.id = V4L2_CID.HFLIP
+        ctrl.value = flip
+
+        result = self._ioctl(_VIDIOC.S_CTRL, byref(ctrl))
+        if -1 == result:
+            return False
+        expected = ctrl.value
+        result = self._ioctl(_VIDIOC.G_CTRL, byref(ctrl))
+        if -1 == result:
+            return False
+        if expected != ctrl.value:
+            return False
+
+        return True
+
+    def set_vertical_flip(self, flip):
+        """
+        Flip video (vertical) if it supported.
+
+        Args:
+            flip (boolean): enable flip
+
+        Returns:
+            boolean: result
+        """
+
+        qctrl = queryctrl()
+        qctrl.id = V4L2_CID.VFLIP
+        result = self._ioctl(_VIDIOC.QUERYCTRL, byref(qctrl))
+        if -1 == result:
+            return False
+        if qctrl.flags & V4L2_CTRL_FLAG_DISABLED:
+            return False
+
+        ctrl = control()
+        ctrl.id = V4L2_CID.VFLIP
+        ctrl.value = flip
+
+        result = self._ioctl(_VIDIOC.S_CTRL, byref(ctrl))
+        if -1 == result:
+            return False
+        expected = ctrl.value
+        result = self._ioctl(_VIDIOC.G_CTRL, byref(ctrl))
+        if -1 == result:
+            return False
+        if expected != ctrl.value:
+            return False
+
+        return True
+
+    def set_exposure_time(self, ms=None):
+        """
+        Set exposure time.
+
+        Args:
+            ms (int or None): exposure time [msec] (None means auto)
+
+        Returns:
+            boolean: result
+        """
+
+        if ms is None:
+            ctrl = control()
+            ctrl.id = V4L2_CID.EXPOSURE_AUTO
+            ctrl.value = V4L2_EXPOSURE.AUTO
+            result = self._ioctl(_VIDIOC.S_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            expected = ctrl.value
+            result = self._ioctl(_VIDIOC.G_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            if expected != ctrl.value:
+                return False
+        else:
+            ctrl = control()
+            ctrl.id = V4L2_CID.EXPOSURE_AUTO
+            ctrl.value = V4L2_EXPOSURE.MANUAL
+            result = self._ioctl(_VIDIOC.S_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            expected = ctrl.value
+            result = self._ioctl(_VIDIOC.G_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            if expected != ctrl.value:
+                return False
+
+            ctrl.id = V4L2_CID.EXPOSURE_ABSOLUTE
+            ctrl.value = int(10 * ms)  # [100us]
+            result = self._ioctl(_VIDIOC.S_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            expected = ctrl.value
+            result = self._ioctl(_VIDIOC.G_CTRL, byref(ctrl))
+            if -1 == result:
+                return False
+            if expected != ctrl.value:
+                return False
+
+        return True
+
+    def request_buffers(self, n, v4l2_memory: V4L2_MEMORY = V4L2_MEMORY.MMAP, dma_fds=[]) -> int:
+
+        req = requestbuffers()
+        req.count = n
+        req.type = self.v4l2_buf_type
+        req.memory = v4l2_memory
+
+        result = self._ioctl(_VIDIOC.REQBUFS, byref(req))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_REQBUFS): {}".format(errno.errorcode[get_errno()]))
+
+        if req.count <= 0:
+            raise RuntimeError("ioctl(VIDIOC_REQBUFS): insufficient buffer count")
+
+        if v4l2_memory == V4L2_MEMORY.MMAP:
+            self.buffers = [VideoBuffer(self, i, V4L2_MEMORY.MMAP, v4l2_buf_type=self.v4l2_buf_type) for i in range(req.count)]
+        elif v4l2_memory == V4L2_MEMORY.DMABUF:
+            if req.count != len(dma_fds):
+                raise RuntimeError("requested buffer count mismatch with number of given dma file descriptor")
+
+            self.buffers = [
+                VideoBuffer(self, i, V4L2_MEMORY.DMABUF, fd, v4l2_buf_type=self.v4l2_buf_type) for (i, fd) in enumerate(dma_fds)
+            ]
+
+        return req.count
+
+    def export_buffers(self):
+        export_fds = []
+        # all buffer in self.buffers is MMAP_BUFFER
+        for video_buf in self.buffers:
+            expbuf = exportbuffer()
+            expbuf.type = self.v4l2_buf_type
+            expbuf.index = video_buf.buf.index
+            result = self._ioctl(_VIDIOC.EXPBUF, byref(expbuf))
+            if -1 == result:
+                raise RuntimeError("ioctl(VIDIOC_EXPBUF): {}".format(errno.errorcode[get_errno()]))
+
+            export_fds.append(expbuf.fd)
+
+        return export_fds
+
+    def queue_all_buffers(self):
+        for video_buf in self.buffers:
+            result = self._ioctl(_VIDIOC.QBUF, byref(video_buf.buf))
+            if -1 == result:
+                raise RuntimeError("ioctl(VIDIOC_QBUF): {}".format(errno.errorcode[get_errno()]))
+
+    def queue_buffer(self, index):
+        video_buf = self.buffers[index]
+        result = self._ioctl(_VIDIOC.QBUF, byref(video_buf.buf))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_QBUF): {}".format(errno.errorcode[get_errno()]))
+
+    def start_streaming(self):
+
+        cap = c_int(self.v4l2_buf_type)
+        result = self._ioctl(_VIDIOC.STREAMON, byref(cap))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_STREAMON): {}".format(errno.errorcode[get_errno()]))
+
+    def stop_streaming(self):
+
+        cap = c_int(self.v4l2_buf_type)
+        result = self._ioctl(_VIDIOC.STREAMOFF, byref(cap))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_STREAMON): {}".format(errno.errorcode[get_errno()]))
+
+        return True
+
+    def dequeue_buffer_nonblocking(self, v4l2_memory: V4L2_MEMORY = V4L2_MEMORY.MMAP):
+        buf = buffer()
+        buf.type = self.v4l2_buf_type
+        buf.memory = v4l2_memory
+        result = self._ioctl(_VIDIOC.DQBUF, byref(buf))
+        if result != 0 and get_errno() == errno.EAGAIN:
+            return None
+        elif -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_DQBUF): {}".format(errno.errorcode[get_errno()]))
+
+        return self.buffers[buf.index]
+
+    # blocking
+    def dequeue_buffer(self, timeout=1, v4l2_memory: V4L2_MEMORY = V4L2_MEMORY.MMAP):
+        rlist, _, _ = select.select([self.device_fd], [], [], timeout)
+        if len(rlist) == 0:
+            raise RuntimeError("Capture timeout")
+
+        buf = buffer()
+        buf.type = self.v4l2_buf_type
+        buf.memory = v4l2_memory
+        result = self._ioctl(_VIDIOC.DQBUF, byref(buf))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_DQBUF): {}".format(errno.errorcode[get_errno()]))
+
+        return self.buffers[buf.index]
+
+    def requeue_buffer(self, video_buf):
+
+        result = self._ioctl(_VIDIOC.QBUF, byref(video_buf.buf))
+        if -1 == result:
+            raise RuntimeError("ioctl(VIDIOC_QBUF): {}".format(errno.errorcode[get_errno()]))
+
+
 VideoPort = enum.Enum("VideoPort", "CSI USB")
 
 
 class VideoConfig(object):
     def __init__(self, width=640, height=480, pixel_format=V4L2_PIX_FMT.RGB24, framerate=30):
         self.pixel_format = pixel_format
         self.width = width
@@ -406,15 +828,29 @@
 
 class Video(object):
     def __init__(self, device="/dev/video0", blocking=False):
         self.device = device
         flags = os.O_RDWR
         if not blocking:
             flags |= os.O_NONBLOCK
-        self.device_fd = os.open(self.device, flags)
+
+        for i in range(3):
+            try:
+                self.device_fd = os.open(self.device, flags)
+                break
+            except OSError as e:
+                # retry 3 times when device is busy
+                if e.errno != errno.EBUSY or i == 2:
+                    raise RuntimeError(f"open {self.device}: {errno.errorcode[e.errno]}")
+            warnings.warn(
+                f"Retrying to open {self.device} after 1 second.",
+                RuntimeWarning,
+            )
+            time.sleep(1)
+
         self.converter = _v4lconvert.create(self.device_fd)
         self.buffers: Optional[List[VideoBuffer]] = None  # set when enqueu
 
     def close(self):
         os.close(self.device_fd)
 
     def __enter__(self):
@@ -435,15 +871,15 @@
         cap = capability()
         result = self._ioctl(_VIDIOC.QUERYCAP, byref(cap))
         if not (cap.capabilities & _V4L2_CAP_VIDEO_CAPTURE):
             raise RuntimeError("The device doesn't support the single-planar API through the Video Capture interface.")
         if not (cap.capabilities & _V4L2_CAP_STREAMING):
             raise RuntimeError("The device doesn't support the streaming I/O method.")
         driver = "".join(map(chr, itertools.takewhile(lambda x: x > 0, cap.driver)))
-        if driver == "bm2835 mmal":
+        if driver == "bm2835 mmal" or driver == "unicam":
             return VideoPort.CSI
         elif driver[: len("uvcvideo")] == "uvcvideo":
             return VideoPort.USB
         else:
             raise RuntimeError("unknown driver '{}'".format(driver))
 
     def lookup_config(self, width, height, framerate, pixel_format, expected_format):
@@ -850,22 +1286,15 @@
         result = self._ioctl(_VIDIOC.STREAMOFF, byref(cap))
         if -1 == result:
             raise RuntimeError("ioctl(VIDIOC_STREAMON): {}".format(errno.errorcode[get_errno()]))
 
         return True
 
     def dequeue_buffer(self, timeout=1):
-        class FDWrapper:
-            def __init__(self, fd):
-                self.fd = fd
-
-            def fileno(self):
-                return self.fd
-
-        rlist, _, _ = select.select([FDWrapper(self.device_fd)], [], [], timeout)
+        rlist, _, _ = select.select([self.device_fd], [], [], timeout)
         if len(rlist) == 0:
             raise RuntimeError("Capture timeout")
 
         buf = buffer()
         buf.type = V4L2_BUF_TYPE.VIDEO_CAPTURE
         buf.memory = V4L2_MEMORY.MMAP
         result = self._ioctl(_VIDIOC.DQBUF, byref(buf))
@@ -913,50 +1342,94 @@
 
         self.video.requeue_buffer(buf)
 
         return dst
 
 
 class VideoBuffer(object):
-    def __init__(self, video, index):
+    def __init__(
+        self, video, index, v4l2_memory: V4L2_MEMORY = V4L2_MEMORY.MMAP, dma_fd=None, v4l2_buf_type=V4L2_BUF_TYPE.VIDEO_CAPTURE
+    ):
 
         buf = buffer()
-        buf.type = V4L2_BUF_TYPE.VIDEO_CAPTURE
-        buf.memory = V4L2_MEMORY.MMAP
+        buf.type = v4l2_buf_type
+        buf.memory = v4l2_memory
         buf.index = index
 
         set_errno(0)
         result = video._ioctl(_VIDIOC.QUERYBUF, byref(buf))
         if -1 == result:
-            raise RuntimeError("ioctl(VIDIOC_QYERYBUF): {}".format(errno.errorcode[get_errno()]))
+            raise RuntimeError("ioctl(VIDIOC_QUERYBUF): {}".format(errno.errorcode[get_errno()]))
 
-        result = _v4l2.mmap(
-            None,
-            buf.length,
-            mmap.PROT_READ | mmap.PROT_WRITE,
-            mmap.MAP_SHARED,
-            video.device_fd,
-            buf.m.offset,
-        )
-        if result == -1:
-            raise RuntimeError("mmap failed: {}".format(errno.errorcode[get_errno()]))
+        if v4l2_memory == V4L2_MEMORY.MMAP:
+            result = _v4l2.mmap(
+                None,
+                buf.length,
+                mmap.PROT_READ | mmap.PROT_WRITE,
+                mmap.MAP_SHARED,
+                video.device_fd,
+                buf.m.offset,
+            )
+            if result == -1:
+                raise RuntimeError("mmap failed: {}".format(errno.errorcode[get_errno()]))
 
-        self.video = video
-        self.buf = buf
-        self.mapped_buf = cast(result, POINTER(c_uint8))
+            self.video = video
+            self.buf = buf
+            self.mapped_buf = cast(result, POINTER(c_uint8))
+        elif v4l2_memory == V4L2_MEMORY.DMABUF:
+            self.video = video
+            self.buf = buf
+            self.buf.m.fd = dma_fd
+            self.dma_fd = dma_fd
 
     def unmap_buffer(self):
         if self.mapped_buf is None:
             return
         result = _v4l2.munmap(self.mapped_buf, self.buf.length)
         if result == -1:
             raise RuntimeError("munmap failed: {}".format(errno.errorcode[get_errno()]))
         self.mapped_buf = None
 
 
+class V4LConverter(object):
+    def __init__(self, device_fd) -> None:
+        self.converter = _v4lconvert.create(device_fd)
+
+    def convert(self, buffer: VideoBuffer, src_fmt, dst_fmt) -> bytes:
+        if buffer.buf.memory == V4L2_MEMORY.DMABUF:
+            raise RuntimeError("V4LConverter.convert: expected memory type MMAP")
+
+        dst = bytes(dst_fmt.fmt.pix.sizeimage)
+        _v4lconvert.convert(
+            self.converter,
+            byref(src_fmt),
+            byref(dst_fmt),
+            buffer.mapped_buf,
+            src_fmt.fmt.pix.sizeimage,
+            cast(dst, POINTER(c_ubyte)),
+            dst_fmt.fmt.pix.sizeimage,
+        )
+
+        return dst
+
+    def try_convert(self, src_fmt, expected_width, expected_height, expected_format) -> format:
+        dst_fmt = format()
+        dst_fmt.type = V4L2_BUF_TYPE.VIDEO_CAPTURE
+        dst_fmt.fmt.pix.width = expected_width
+        dst_fmt.fmt.pix.height = expected_height
+        dst_fmt.fmt.pix.pixelformat = expected_format
+        dst_fmt.fmt.pix.field = V4L2_FIELD.INTERLACED
+
+        result = _v4lconvert.try_format(self.converter, byref(src_fmt), byref(dst_fmt))
+        if -1 == result:
+            raise RuntimeError("incompatible format")
+
+        return dst_fmt
+
+
 # if __name__ == '__main__':
 
 #     from PIL import Image
 #     import traceback
 
 #     with Video('/dev/video1') as video:
 #         print("video.query_capability():",video.query_capability())
```

### Comparing `actfw-core-2.2.0a1/pyproject.toml` & `actfw_core-2.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ]
 description = "Core components of actfw, independent of specific devices"
 keywords = ['actcast']
 license = "MIT"
 name = "actfw-core"
 readme = "README.md"
 repository = "https://github.com/Idein/actfw-core"
-version = "2.2.0a1"
+version = "2.2.1"
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
 
 # This library is intended to be used to implement [Actcast application](https://actcast.io/docs/ForVendor/ApplicationDevelopment/).
 # Dependencies should be compatible with those provided by apt in Actcast application's base image
 # to prevent installing different versions.  Notice that, IIUC, there is a possibility that
```

### Comparing `actfw-core-2.2.0a1/setup.py` & `actfw_core-2.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,126 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: actfw-core
+Version: 2.2.1
+Summary: Core components of actfw, independent of specific devices
+Home-page: https://github.com/Idein/actfw-core
+License: MIT
+Keywords: actcast
+Author: Idein Inc.
+Requires-Python: >=3.6.2,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: Pillow (>=5,<6) ; python_version < "3.8"
+Requires-Dist: Pillow (>=8,<9) ; python_version >= "3.8"
+Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version < "3.7"
+Project-URL: Changelog, https://github.com/Idein/actfw-core/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://idein.github.io/actfw-core/latest/
+Project-URL: Repository, https://github.com/Idein/actfw-core
+Description-Content-Type: text/markdown
+
+# actfw-core
+
+Core components of actfw, a framework for Actcast Application written in Python.
+actfw-core is intended to be independent of any specific device.
+
+## Installation
+
+```console
+sudo apt-get update
+sudo apt-get install -y python3-pip python3-pil 
+sudo apt-get install -y libv4l-0 libv4lconvert0  # if using `V4LCameraCapture`
+pip3 install actfw-core
+```
+
+## Document
+
+* [API References](https://idein.github.io/actfw-core/latest/)
+
+## Usage
+
+Construct your application with a task parallel model
+
+* Application
+  * `actfw_core.Application` : Main application
+* Workers
+  * `actfw_core.task.Producer` : Task generator
+    * `actfw_core.capture.V4LCameraCapture` : Generate UVC camera capture image
+  * `actfw_core.task.Pipe` : Task to Task converter
+  * `actfw_core.task.Consumer` : Task terminator
+
+Each worker is executed in parallel.
+
+User should
+
+* Define subclass of `Producer/Pipe/Consumer`
+
+```python
+class MyPipe(actfw_core.task.Pipe):
+    def proc(self, i):
+        ...
+```
+
+* Connect defined worker objects
+
+```python
+p  = MyProducer()
+f1 = MyPipe()
+f2 = MyPipe()
+c  = MyConsumer()
+p.connect(f1)
+f1.connect(f2)
+f2.connect(c)
+```
+
+* Register to `Application`
+
+```python
+app = actfw_core.Application()
+app.register_task(p)
+app.register_task(f1)
+app.register_task(f2)
+app.register_task(c)
+```
+
+* Execute application
+
+```python
+app.run()
+```
+
+## Development Guide
+
+### Installation of dev requirements
+
+```console
+pip3 install poetry
+poetry install
+```
+
+### Running tests
+
+```console
+poetry run nose2 -v
+```
+
+### Releasing package & API doc
+
+CI will automatically do.
+Follow the following branch/tag rules.
+
+1. Make changes for next version in `master` branch (via pull-requests).
+2. Make a PR that updates version in `pyproject.toml` and merge it to `master` branch.
+3. Create GitHub release from `master` branch's HEAD.
+    1. [Draft a new release](https://github.com/Idein/actfw-core/releases/new).
+    2. Create new tag named `release-<New version>` (e.g. `release-1.4.0`) from `Choose a tag` pull down menu.
+    3. Write title and description.
+    4. Publish release.
+4. Then CI will build/upload package to PyPI & API doc to GitHub Pages.
 
-packages = \
-['actfw_core',
- 'actfw_core._private.agent_app_protocol',
- 'actfw_core._private.compat',
- 'actfw_core._private.schema',
- 'actfw_core._private.util',
- 'actfw_core.schema',
- 'actfw_core.task',
- 'actfw_core.util',
- 'actfw_core.v4l2']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':python_version < "3.7"': ['dataclasses>=0.8,<0.9'],
- ':python_version < "3.8"': ['Pillow>=5,<6'],
- ':python_version >= "3.8"': ['Pillow>=8,<9']}
-
-setup_kwargs = {
-    'name': 'actfw-core',
-    'version': '2.2.0a1',
-    'description': 'Core components of actfw, independent of specific devices',
-    'long_description': "# actfw-core\n\nCore components of actfw, a framework for Actcast Application written in Python.\nactfw-core is intended to be independent of any specific device.\n\n## Installation\n\n```console\nsudo apt-get update\nsudo apt-get install -y python3-pip python3-pil \nsudo apt-get install -y libv4l-0 libv4lconvert0  # if using `V4LCameraCapture`\npip3 install actfw-core\n```\n\n## Document\n\n* [API References](https://idein.github.io/actfw-core/latest/)\n\n## Usage\n\nConstruct your application with a task parallel model\n\n* Application\n  * `actfw_core.Application` : Main application\n* Workers\n  * `actfw_core.task.Producer` : Task generator\n    * `actfw_core.capture.V4LCameraCapture` : Generate UVC camera capture image\n  * `actfw_core.task.Pipe` : Task to Task converter\n  * `actfw_core.task.Consumer` : Task terminator\n\nEach worker is executed in parallel.\n\nUser should\n\n* Define subclass of `Producer/Pipe/Consumer`\n\n```python\nclass MyPipe(actfw_core.task.Pipe):\n    def proc(self, i):\n        ...\n```\n\n* Connect defined worker objects\n\n```python\np  = MyProducer()\nf1 = MyPipe()\nf2 = MyPipe()\nc  = MyConsumer()\np.connect(f1)\nf1.connect(f2)\nf2.connect(c)\n```\n\n* Register to `Application`\n\n```python\napp = actfw_core.Application()\napp.register_task(p)\napp.register_task(f1)\napp.register_task(f2)\napp.register_task(c)\n```\n\n* Execute application\n\n```python\napp.run()\n```\n\n## Development Guide\n\n### Installation of dev requirements\n\n```console\npip3 install poetry\npoetry install\n```\n\n### Running tests\n\n```console\npoetry run nose2 -v\n```\n\n### Releasing package & API doc\n\nCI will automatically do.\nFollow the following branch/tag rules.\n\n1. Make changes for next version in `master` branch (via pull-requests).\n2. Make a PR that updates version in `pyproject.toml` and merge it to `master` branch.\n3. Create Git tag from `master` branch's HEAD named `release-<New version>`. E.g. `release-1.4.0`.\n4. Then CI will build/upload package to PyPI & API doc to GitHub Pages.\n",
-    'author': 'Idein Inc.',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Idein/actfw-core',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

