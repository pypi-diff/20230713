# Comparing `tmp/flowchem-test-0.1b2.tar.gz` & `tmp/flowchem-test-0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchem-test-0.1b2.tar", last modified: Thu Jul 13 17:43:21 2023, max compression
+gzip compressed data, was "flowchem-test-0.1b3.tar", last modified: Thu Jul 13 17:43:25 2023, max compression
```

## Comparing `flowchem-test-0.1b2.tar` & `flowchem-test-0.1b3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:21.081979 flowchem-test-0.1b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 17:43:21.081979 flowchem-test-0.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:43:21.081979 flowchem-test-0.1b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:21.077979 flowchem-test-0.1b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:21.077979 flowchem-test-0.1b2/src/flowchem_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/src/flowchem_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/src/flowchem_test/fakedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/src/flowchem_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-13 17:43:11.000000 flowchem-test-0.1b2/src/flowchem_test/test_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:21.077979 flowchem-test-0.1b2/src/flowchem_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 17:43:21.000000 flowchem-test-0.1b2/src/flowchem_test.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:25.308382 flowchem-test-0.1b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 17:43:25.308382 flowchem-test-0.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:43:25.308382 flowchem-test-0.1b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:25.304382 flowchem-test-0.1b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:25.308382 flowchem-test-0.1b3/src/flowchem_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/src/flowchem_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/src/flowchem_test/fakedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:14.000000 flowchem-test-0.1b3/src/flowchem_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:25.308382 flowchem-test-0.1b3/src/flowchem_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 17:43:25.000000 flowchem-test-0.1b3/src/flowchem_test.egg-info/top_level.txt
```

### Comparing `flowchem-test-0.1b2/LICENSE` & `flowchem-test-0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchem-test-0.1b2/PKG-INFO` & `flowchem-test-0.1b3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchem-test
-Version: 0.1b2
+Version: 0.1b3
 Summary: Add support for test devices in flowchem.
 Author-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 Maintainer-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/cambiegroup/flowchem-test
 Keywords: chemistry,automation,laboratory,testing
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flowchem-test-0.1b2/pyproject.toml` & `flowchem-test-0.1b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 flowchem_test = ["py.typed"]
 
 [project]
 name = "flowchem-test"
-version = "0.1b2"
+version = "0.1b3"
 description = "Add support for test devices in flowchem."
 readme = "README.md"
 requires-python = ">=3.10"
 license =  { text = "MIT" }
 keywords = ["chemistry", "automation", "laboratory", "testing"]
 authors = [
     { name = "Dario Cambié", email = "2422614+dcambie@users.noreply.github.com" },
```

### Comparing `flowchem-test-0.1b2/src/flowchem_test/fakedevice.py` & `flowchem-test-0.1b3/src/flowchem_test/fakedevice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Fake device for testing purposes. No parameters needed."""
-from collections.abc import Iterable
-
 from flowchem.components.base_component import FlowchemComponent
 from flowchem.devices.flowchem_device import DeviceInfo
 from flowchem.devices.flowchem_device import FlowchemDevice
+
 from flowchem.utils.people import dario
 
-from .test_component import TestComponent
+
+class TestComponent(FlowchemComponent):
+    def __init__(self, name: str, hw_device: FlowchemDevice):
+        """Initialize a TestComponent with the provided endpoints."""
+        super().__init__(name, hw_device)
+        self.add_api_route("/test", lambda: True, methods=["GET"])
 
 
 class FakeDevice(FlowchemDevice):
     device_info = DeviceInfo(
-        authors=[dario],
-        maintainers=[dario],
-        manufacturer="virtual-device",
-        model="FakeDevice",
-        serial_number=42,
-        version="v1.0",
-    )
-
-    def components(self) -> Iterable[FlowchemComponent]:
-        """Returns a test Component."""
-        component = TestComponent(name="test-component", hw_device=self)
-        component.add_api_route("/test", lambda: True, methods=["GET"])
-        return (component,)
+            authors=[dario],
+            maintainers=[dario],
+            manufacturer="virtual-device",
+            model="FakeDevice",
+            serial_number=42,
+            version="v1.0",
+        )
+
+    async def initialize(self):
+        """Add component to device."""
+        self.components.append(TestComponent(name="test-component", hw_device=self))
```

### Comparing `flowchem-test-0.1b2/src/flowchem_test.egg-info/PKG-INFO` & `flowchem-test-0.1b3/src/flowchem_test.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchem-test
-Version: 0.1b2
+Version: 0.1b3
 Summary: Add support for test devices in flowchem.
 Author-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 Maintainer-email: Dario Cambié <2422614+dcambie@users.noreply.github.com>
 License: MIT
 Project-URL: repository, https://github.com/cambiegroup/flowchem-test
 Keywords: chemistry,automation,laboratory,testing
 Classifier: License :: OSI Approved :: MIT License
```

