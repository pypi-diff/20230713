# Comparing `tmp/bond_async-0.1.23.tar.gz` & `tmp/bond_async-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bond_async-0.1.23.tar", last modified: Mon Mar 13 22:22:09 2023, max compression
+gzip compressed data, was "bond_async-0.2.0.tar", last modified: Thu Jul 13 18:31:10 2023, max compression
```

## Comparing `bond_async-0.1.23.tar` & `bond_async-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:22:09.090111 bond_async-0.1.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-13 22:21:57.000000 bond_async-0.1.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-13 22:22:09.090111 bond_async-0.1.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-13 22:21:57.000000 bond_async-0.1.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:22:09.086111 bond_async-0.1.23/bond_async/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/bond_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/bpup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-13 22:21:57.000000 bond_async-0.1.23/bond_async/device_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:22:09.090111 bond_async-0.1.23/bond_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-13 22:22:09.000000 bond_async-0.1.23/bond_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 22:22:09.000000 bond_async-0.1.23/bond_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 22:22:09.000000 bond_async-0.1.23/bond_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-13 22:22:09.000000 bond_async-0.1.23/bond_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-13 22:22:09.000000 bond_async-0.1.23/bond_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 22:22:09.090111 bond_async-0.1.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-13 22:21:57.000000 bond_async-0.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:31:10.696611 bond_async-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 18:31:01.000000 bond_async-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-13 18:31:10.696611 bond_async-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-13 18:31:01.000000 bond_async-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:31:10.696611 bond_async-0.2.0/bond_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/bond_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/bpup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 18:31:01.000000 bond_async-0.2.0/bond_async/requestor_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:31:10.696611 bond_async-0.2.0/bond_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-13 18:31:10.000000 bond_async-0.2.0/bond_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 18:31:10.000000 bond_async-0.2.0/bond_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:31:10.000000 bond_async-0.2.0/bond_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 18:31:10.000000 bond_async-0.2.0/bond_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 18:31:10.000000 bond_async-0.2.0/bond_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:31:10.696611 bond_async-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-13 18:31:01.000000 bond_async-0.2.0/setup.py
```

### Comparing `bond_async-0.1.23/LICENSE` & `bond_async-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bond_async-0.1.23/PKG-INFO` & `bond_async-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bond_async
-Version: 0.1.23
+Version: 0.2.0
 Summary: Asynchronous Python wrapper library over Bond Local API
 Home-page: https://github.com/bondhome/bond-async
 Author: Olibra LLC
 Author-email: mobiledev@olibra.io
 License: MIT
 Keywords: bond local api async
 Classifier: Intended Audience :: Developers
```

### Comparing `bond_async-0.1.23/README.md` & `bond_async-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bond_async-0.1.23/bond_async/action.py` & `bond_async-0.2.0/bond_async/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     STOP = "Stop"
     TURN_ON = "TurnOn"
     TURN_OFF = "TurnOff"
     TOGGLE_POWER = "TogglePower"
     SET_TIMER = "SetTimer"
     SWITCH_MODE = "SwitchMode"
     SET_STATE_BELIEF = "state"
+    HOME_SHIELD_ON = "HomeShieldOn"
+    HOME_SHIELD_OFF = "HomeShieldOff"
+    HOME_SHIELD_TOGGLE = "HomeShieldToggle"
 
     # Lights
     TURN_LIGHT_ON = "TurnLightOn"
     TURN_LIGHT_OFF = "TurnLightOff"
     TOGGLE_LIGHT = "ToggleLight"
     SET_BRIGHTNESS = "SetBrightness"
     INCREASE_BRIGHTNESS = "IncreaseBrightness"
```

### Comparing `bond_async-0.1.23/bond_async/bond_type.py` & `bond_async-0.2.0/bond_async/bond_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """Bond type enumeration."""
 from enum import Enum
 import re
 
 regexes = {
-    "bridge_snowbird": "^[A-C]\w*$",
-    "bridge_zermatt": "^Z(Z|X)\w*$",
-    "bridge_pro": "^ZP\w*$",
-    "sbb_lights": "^T\w*$",
-    "sbb_ceiling_fan": "^K\w*$",
-    "sbb_plug": "^P\w*$",
+    "bridge_snowbird": r"^[A-C]\w*$",
+    "bridge_zermatt": r"^Z(Z|X)\w*$",
+    "bridge_pro": r"^ZP\w*$",
+    "sbb_lights": r"^T\w*$",
+    "sbb_ceiling_fan": r"^K\w*$",
+    "sbb_plug": r"^P\w*$",
 }
 
 
 class BondType(Enum):
     """Bond type enumeration."""
 
     BRIDGE_SNOWBIRD = "bridge_snowbird"
     BRIDGE_ZERMATT = "bridge_zermatt"
     BRIDGE_PRO = "bridge_pro"
     SBB_LIGHTS = "sbb_lights"
     SBB_CEILING_FAN = "sbb_ceiling_fan"
     SBB_PLUG = "sbb_plug"
 
     def is_sbb(self) -> bool:
+        """Checks if BondType is a Smart by Bond product."""
         return self.value.startswith("sbb_")
 
     def is_bridge(self) -> bool:
+        """Checks if BondType is a Bond Bridge/Bond Bridge Pro."""
         return self.value.startswith("bridge_")
 
     @classmethod
     def from_serial(cls, serial: str):
         """Returns a BondType for a serial number"""
-        for type in regexes:
-            if re.search(regexes[type], serial):
-                return cls(type)
+        for (bond_type, regex) in regexes.items():
+            if re.search(regex, serial):
+                return cls(bond_type)
         return None
 
     @staticmethod
     def is_sbb_from_serial(serial: str) -> bool:
         """Checks if specified Bond serial number is a Smart by Bond product."""
-        bondType = BondType.from_serial(serial)
-        if bondType:
-            return bondType.is_sbb()
-        else:
-            return False
+        bond_type = BondType.from_serial(serial)
+        if bond_type:
+            return bond_type.is_sbb()
+        return False
 
     @staticmethod
     def is_bridge_from_serial(serial: str) -> bool:
         """Checks if specified Bond serial number is a Bond Bridge."""
-        bondType = BondType.from_serial(serial)
-        if bondType:
-            return bondType.is_bridge()
-        else:
-            return False
+        bond_type = BondType.from_serial(serial)
+        if bond_type:
+            return bond_type.is_bridge()
+        return False
```

### Comparing `bond_async-0.1.23/bond_async/bpup.py` & `bond_async-0.2.0/bond_async/bpup.py`

 * *Files identical despite different names*

### Comparing `bond_async-0.1.23/bond_async/device_type.py` & `bond_async-0.2.0/bond_async/device_type.py`

 * *Files identical despite different names*

### Comparing `bond_async-0.1.23/bond_async.egg-info/PKG-INFO` & `bond_async-0.2.0/bond_async.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bond-async
-Version: 0.1.23
+Version: 0.2.0
 Summary: Asynchronous Python wrapper library over Bond Local API
 Home-page: https://github.com/bondhome/bond-async
 Author: Olibra LLC
 Author-email: mobiledev@olibra.io
 License: MIT
 Keywords: bond local api async
 Classifier: Intended Audience :: Developers
```

### Comparing `bond_async-0.1.23/setup.py` & `bond_async-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="bond_async",
-    version="0.1.23",
+    version="0.2.0",
     packages=find_packages(exclude=['tests']),
 
     author="Olibra LLC",
     author_email="mobiledev@olibra.io",
     description="Asynchronous Python wrapper library over Bond Local API",
     long_description=README,
     long_description_content_type="text/markdown",
```

