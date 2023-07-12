# Comparing `tmp/forcedimension-0.1.5.tar.gz` & `tmp/forcedimension-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forcedimension-0.1.5.tar", last modified: Thu Jul 21 21:44:40 2022, max compression
+gzip compressed data, was "forcedimension-0.1.6.tar", last modified: Wed Jul 12 22:36:50 2023, max compression
```

## Comparing `forcedimension-0.1.5.tar` & `forcedimension-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2022-07-21 21:44:40.957806 forcedimension-0.1.5/
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    35149 2022-07-20 22:11:06.000000 forcedimension-0.1.5/LICENSE
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46037 2022-07-21 21:44:40.957806 forcedimension-0.1.5/PKG-INFO
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     4815 2022-07-20 22:45:01.000000 forcedimension-0.1.5/README.md
-drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2022-07-21 21:44:40.953806 forcedimension-0.1.5/forcedimension/
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    37805 2022-07-21 21:44:30.000000 forcedimension-0.1.5/forcedimension/__init__.py
-drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2022-07-21 21:44:40.957806 forcedimension-0.1.5/forcedimension/dhd/
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)   106033 2022-07-21 21:24:20.000000 forcedimension-0.1.5/forcedimension/dhd/__init__.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     8076 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/dhd/adaptors.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     3873 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/dhd/constants.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)   105828 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/dhd/expert.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     1820 2022-07-21 21:44:30.000000 forcedimension-0.1.5/forcedimension/dhd/os_independent.py
-drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2022-07-21 21:44:40.957806 forcedimension-0.1.5/forcedimension/drd/
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46373 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/drd/__init__.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     5368 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/runtime.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     1453 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/typing.py
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     9829 2022-07-20 22:11:06.000000 forcedimension-0.1.5/forcedimension/util.py
-drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2022-07-21 21:44:40.957806 forcedimension-0.1.5/forcedimension.egg-info/
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46037 2022-07-21 21:44:40.000000 forcedimension-0.1.5/forcedimension.egg-info/PKG-INFO
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)      522 2022-07-21 21:44:40.000000 forcedimension-0.1.5/forcedimension.egg-info/SOURCES.txt
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)        1 2022-07-21 21:44:40.000000 forcedimension-0.1.5/forcedimension.egg-info/dependency_links.txt
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       40 2022-07-21 21:44:40.000000 forcedimension-0.1.5/forcedimension.egg-info/requires.txt
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       15 2022-07-21 21:44:40.000000 forcedimension-0.1.5/forcedimension.egg-info/top_level.txt
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)      826 2022-07-21 21:44:30.000000 forcedimension-0.1.5/pyproject.toml
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       38 2022-07-21 21:44:40.957806 forcedimension-0.1.5/setup.cfg
--rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       69 2022-07-20 22:11:06.000000 forcedimension-0.1.5/setup.py
+drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2023-07-12 22:36:50.371765 forcedimension-0.1.6/
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    35149 2023-06-21 16:29:41.000000 forcedimension-0.1.6/LICENSE
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46037 2023-07-12 22:36:50.371765 forcedimension-0.1.6/PKG-INFO
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     4815 2022-07-20 22:45:01.000000 forcedimension-0.1.6/README.md
+drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2023-07-12 22:36:50.371765 forcedimension-0.1.6/forcedimension/
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    38206 2023-07-12 22:36:41.000000 forcedimension-0.1.6/forcedimension/__init__.py
+drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2023-07-12 22:36:50.371765 forcedimension-0.1.6/forcedimension/dhd/
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)   108732 2023-07-12 22:36:41.000000 forcedimension-0.1.6/forcedimension/dhd/__init__.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     8076 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/dhd/adaptors.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     3873 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/dhd/constants.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)   105828 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/dhd/expert.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     1636 2023-07-12 22:36:41.000000 forcedimension-0.1.6/forcedimension/dhd/os_independent.py
+drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2023-07-12 22:36:50.371765 forcedimension-0.1.6/forcedimension/drd/
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46373 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/drd/__init__.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     5368 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/runtime.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     1453 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/typing.py
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)     9829 2022-07-20 22:11:06.000000 forcedimension-0.1.6/forcedimension/util.py
+drwxrwxr-x   0 emdash00  (1000) emdash00  (1000)        0 2023-07-12 22:36:50.371765 forcedimension-0.1.6/forcedimension.egg-info/
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)    46037 2023-07-12 22:36:50.000000 forcedimension-0.1.6/forcedimension.egg-info/PKG-INFO
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)      522 2023-07-12 22:36:50.000000 forcedimension-0.1.6/forcedimension.egg-info/SOURCES.txt
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)        1 2023-07-12 22:36:50.000000 forcedimension-0.1.6/forcedimension.egg-info/dependency_links.txt
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       40 2023-07-12 22:36:50.000000 forcedimension-0.1.6/forcedimension.egg-info/requires.txt
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       15 2023-07-12 22:36:50.000000 forcedimension-0.1.6/forcedimension.egg-info/top_level.txt
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)      825 2023-07-12 22:36:41.000000 forcedimension-0.1.6/pyproject.toml
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       38 2023-07-12 22:36:50.371765 forcedimension-0.1.6/setup.cfg
+-rw-rw-r--   0 emdash00  (1000) emdash00  (1000)       69 2022-07-20 22:11:06.000000 forcedimension-0.1.6/setup.py
```

### Comparing `forcedimension-0.1.5/LICENSE` & `forcedimension-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/PKG-INFO` & `forcedimension-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcedimension
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Bindings for the ForceDimension SDK
 Author-email: Ember Chow <emberchow.business@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `forcedimension-0.1.5/README.md` & `forcedimension-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/__init__.py` & `forcedimension-0.1.6/forcedimension/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+.. module::forcedimension
+   :platform: Windows, Unix
+   :synopsis: ForceDimensionSDK high level wrappers.
+
+.. moduleauthor:: Ember "Emmy" Chow <emberchow.business@gmail.com>
+"""
 from math import nan
 from threading import Condition, Lock, Thread
 from time import monotonic, sleep
 from typing import Callable, List, MutableSequence, Optional
 from typing import cast
 
 import forcedimension.dhd as dhd
@@ -19,15 +26,15 @@
     EuclidianVector,
     ImmutableWrapper,
     JacobianMatrix,
     UpdateOpts,
 )
 
 
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 
 DefaultVecType = EuclidianVector
 
 try:
     from forcedimension.util import NumpyVector, NumpyJacobian
     DefaultVecType = NumpyVector
@@ -234,16 +241,17 @@
     def pos(self) -> Optional[ImmutableWrapper[MutFSeq]]:
         """
         Provides a copy of the last-known position of the HapticDevice's end
         effector. Thread-safe.
 
         :rtype: Optional[MutableSequence[float]]
 
-        :returns: A mutable sequence of [x, y, z] where x, y, and z are the
-        end-effector's position given in [m].
+        :returns:
+            A mutable sequence of [x, y, z] where x, y, and z are the
+            end-effector's position given in [m].
         """
         self.check_threadex()
         return self._pos_view
 
     @property
     def mass(self) -> Optional[float]:
         """
@@ -262,58 +270,62 @@
     def v(self) -> Optional[ImmutableWrapper[MutFSeq]]:
         """
         Provides a copy of the last-known linear velocity of the HapticDevice's
         end-effector. Thread-safe.
 
         :rtype: Optional[MutableSequence[float]]
 
-        :returns: A mutable sequence of [vx, vy, vz] where vx, vy, and vz are
-        the end-effector's linear velocity given in [m/s].
+        :returns:
+            A mutable sequence of [vx, vy, vz] where vx, vy, and vz are
+            the end-effector's linear velocity given in [m/s].
         """
         self.check_threadex()
         return self._v_view
 
     @property
     def w(self) -> Optional[ImmutableWrapper[MutFSeq]]:
         """
         Provides a copy of the last-known angular velocity of the
         HapticDevice's end-effector. Thread-safe.
 
         :rtype: Optional[MutableSequence[float]]
 
-        :returns: A mutable sequence of [wx, wy, wz] where wx, wy, and wz are
-        the end-effector's linear velocity given in [rad/s].
+        :returns:
+            A mutable sequence of [wx, wy, wz] where wx, wy, and wz are
+            the end-effector's linear velocity given in [rad/s].
         """
         self.check_threadex()
         return self._w_view
 
     @property
     def t(self) -> Optional[ImmutableWrapper[MutFSeq]]:
         """
         Provides a copy of the last-known applied torque of the HapticDevice's
         end-effector. Thread-safe.
 
         :rtype: Optional[MutableSequence[float]]
 
-        :returns: A mutable sequence of [tx, ty, tz] where tx, ty, and tz are
-        the torque experienced by the end-effector in [Nm]
+        :returns:
+            A mutable sequence of [tx, ty, tz] where tx, ty, and tz are
+            the torque experienced by the end-effector in [Nm]
         """
         self.check_threadex()
         return self._t_view
 
     @property
     def f(self) -> Optional[ImmutableWrapper[MutFSeq]]:
         """
         Provides a copy of the last-known applied force of the HapticDevice's
         end-effector. Thread-safe.
 
         :rtype: Optional[MutableSequence[float]]
 
-        :returns: A mutable sequence of [fx, fy, fz] where fx, fy, and fz are
-        the torque experienced by the end-effector in [N]
+        :returns:
+            A mutable sequence of [fx, fy, fz] where fx, fy, and fz are
+            the torque experienced by the end-effector in [N]
         """
 
         self.check_threadex()
         return self._f_view
 
     @property
     def left_handed(self) -> Optional[bool]:
@@ -549,15 +561,15 @@
 
     def submit(self):
         """
         Push the requested forces and torques to the device in a blocking send.
 
         See Also
         --------
-        :func:HapticDevice.req
+        :func:`HapticDevice.req`
 
         """
         self._req = False
         err = dhd.setForceAndTorque(
             self._f_req,
             self._t_req,
             cast(int, self._id)
@@ -688,33 +700,34 @@
             )
 
     def get_max_force(self) -> Optional[float]:
         """
         Retrieve the current limit (in N) to the force magnitude that can be
         applied by the haptic device.
 
-        :returns: The current limit (in N) to the force magnitude that can be
-        applied by the haptic device to the end-effector. If there is no limit,
-        None is returned instead.
+        :returns:
+            The current limit (in N) to the force magnitude that can be
+            applied by the haptic device to the end-effector. If there is no
+            limit, None is returned instead.
 
-        rtype: Optional[float]
+        :rtype: Optional[float]
         """
 
         limit = dhd.getMaxForce(ID=cast(int, self._id))
 
         return limit if limit > 0 else None
 
     def set_max_force(self, limit: Optional[float]) -> None:
         """
         Define or disable a limit (in N) to the force magnitude that can be
         applied by the haptic device.
 
-        :param Optional[float] limit: The desired limit (in N) to the force
-        magnitude that can be applied. If the limit is None, the force limit is
-        disabled.
+        :param Optional[float] limit:
+            The desired limit (in N) to the force magnitude that can be
+            applied. If the limit is None, the force limit is disabled.
         """
         if limit is None:
             err = dhd.setMaxForce(ID=cast(int, self._id), limit=-1.0)
         else:
             if limit < 0:
                 raise ValueError
 
@@ -724,33 +737,34 @@
             raise errno_to_exception(ErrorNum(dhd.errorGetLast()))
 
     def get_max_torque(self) -> Optional[float]:
         """
         Retrieve the current limit (in Nm) to the torque magnitude that can be
         applied by the haptic device.
 
-        :returns: The current limit (in Nm) to the force magnitude that can be
-        applied by the haptic device to the end-effector. If there is no limit,
-        None is returned instead.
+        :returns:
+            The current limit (in Nm) to the force magnitude that can be
+            applied by the haptic device to the end-effector. If there is no
+            limit, None is returned instead.
 
-        rtype: Optional[float]
+        :rtype: Optional[float]
         """
 
         limit = dhd.getMaxTorque(ID=cast(int, self._id))
 
         return limit if limit > 0 else None
 
     def set_max_torque(self, limit: Optional[float]) -> None:
         """
         Define or disable a limit (in N) to the force magnitude that can be
         applied by the haptic device.
 
-        :param Optional[float] limit: The desired limit (in N) to the force
-        magnitude that can be applied. If the limit is None, the force limit is
-        disabled.
+        :param Optional[float] limit:
+            The desired limit (in N) to the force magnitude that can be
+            applied. If the limit is None, the force limit is disabled.
         """
         if limit is None:
             err = dhd.setMaxTorque(ID=cast(int, self._id), limit=-1.0)
         else:
             if limit < 0:
                 raise ValueError
 
@@ -774,22 +788,23 @@
 
         dhd.stop(cast(int, self._id))
 
     def get_button(self, button_id: int = 0) -> bool:
         """
         See if the button on the device is being pressed.
 
+        See Also
+        --------
+        :class:`forcedimension.dhd.constants.NovintButtonID`
+
+
         :param int button_id: The button to check
 
         :rtype: bool
-        :returns: True if the button is being pressed, False otherwise.
-
-        See Also
-        --------
-        :class:forcedimension.dhd.dhd.constants.NovintButtonID
+        :returns: True if the button is being pressed, False otherwise
         """
         return bool(self._buttons & cast(int, 1 << button_id))
 
     def close(self):
         self.open = False
         if self._haptic_daemon is not None:
             self._haptic_daemon.stop()
@@ -807,14 +822,20 @@
     A high-level wrapper for methods and kinematic data of a Gripper on a
     HapticDevice.
 
     Certain kinds of HapticDevices opened will have grippers. If that is the
     case, a Gripper object will be instantiated as well containing methods to
     get kinematic information about the Gripper.
     """
+    _enc: int
+    _angle: float
+    _gap: float
+    _v: float
+    _w: float
+    _fg: float
 
     def __init__(
             self,
             parent: HapticDevice,
             ID: Optional[int] = None,
             vecgen: Callable[[], MutableSequence[float]] = EuclidianVector
     ):
@@ -823,20 +844,20 @@
             if (ID < 0):
                 raise ValueError("ID must be greater than 0.")
 
             self._id: int = ID
 
         VecType = vecgen
 
-        self._enc: int = 0
-        self._angle: float = nan
-        self._gap: float = nan
-        self._v: float = nan
-        self._w: float = nan
-        self._fg: float = nan
+        self._enc = 0
+        self._angle = nan
+        self._gap = nan
+        self._v = nan
+        self._w = nan
+        self._fg = nan
 
         self._thumb_pos: MutFSeq = VecType()
         self._finger_pos: MutFSeq = VecType()
 
         self._parent: HapticDevice = parent
 
         self._thumb_pos_view: ImmutableWrapper[MutFSeq] = (
@@ -879,33 +900,34 @@
         # raise NotImplementedError
 
     def get_max_force(self) -> Optional[float]:
         """
         Retrieve the current limit (in N) to the force magnitude that can be
         applied by the haptic device.
 
-        :returns: The current limit (in N) to the force magnitude that can be
-        applied by the haptic device to the end-effector. If there is no limit,
-        None is returned instead.
+        :returns:
+            The current limit (in N) to the force magnitude that can be
+            applied by the haptic device to the end-effector. If there is no
+            limit, None is returned instead.
 
-        rtype: Optional[float]
+        :rtype: Optional[float]
         """
 
         limit = dhd.getMaxGripperForce(ID=cast(int, self._id))
 
         return limit if limit > 0 else None
 
     def set_max_force(self, limit: Optional[float]) -> None:
         """
         Define or disable a limit (in N) to the force magnitude that can be
         applied by the haptic device.
 
-        :param Optional[float] limit: The desired limit (in N) to the force
-        magnitude that can be applied. If the limit is None, the force limit is
-        disabled.
+        :param Optional[float] limit:
+            The desired limit (in N) to the force magnitude that can be
+            applied. If the limit is None, the force limit is disabled.
         """
         if limit is None:
             err = dhd.setMaxGripperForce(ID=cast(int, self._id), limit=-1.0)
         else:
             if limit < 0:
                 raise ValueError
```

### Comparing `forcedimension-0.1.5/forcedimension/dhd/__init__.py` & `forcedimension-0.1.6/forcedimension/dhd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2532,14 +2532,111 @@
         t[1],
         t[2],
         fg,
         ID
     )
 
 
+_libdhd.dhdGetForceAndTorqueAndGripperForce.argtypes = [
+    POINTER(c_double),
+    POINTER(c_double),
+    POINTER(c_double),
+    POINTER(c_double),
+    POINTER(c_double),
+    POINTER(c_double),
+    POINTER(c_double),
+    c_byte
+]
+_libdhd.dhdGetForceAndTorqueAndGripperForce.restype = c_int
+
+def getForceAndTorqueAndGripperForce(
+    ID: int = -1,
+    f_out: Optional[MutableFloatVectorLike] = None,
+    t_out: Optional[MutableFloatVectorLike] = None
+) -> Tuple[
+    Union[MutableFloatVectorLike, List[float]],
+    Union[MutableFloatVectorLike, List[float]],
+    float,
+    int
+]:
+    """
+    Retrieve the force and torque vectors applied to the device end-effector.
+
+    :param int ID:
+         Device ID (see multiple devices section for details), defaults to -1.
+
+    :param Optional[MutableFloatVectorLike] f_out:
+        An output buffer to store the applied forces on the end-effector. If
+        specified, the return will contain a reference to this buffer rather to
+        a newly allocated list, optional.
+
+    :param Optional[MutableFloatVectorLike] t_out:
+        An output buffer to store the applied torques on the end-effector. If
+        specified, the return will contain a reference to this buffer rather to
+        a newly allocated list, optional.
+
+    :raises ValueError:
+        If ``ID`` is not implicitly convertible to C char.
+
+    :returns:
+        A tuple in the form  ``([fx, fy, fz], [tx, ty, tz], fg, err)``.
+        ``[fx, fy, fz]`` are translation forces applied to the end-effector
+        (in [N])  about the X, Y, and Z axes, respectively. ``[tx, ty, tz]``
+        refers to the torques applied to the end-effector (in [Nm]) about
+        the X, Y, and Z axes.  ``fg`` refers to the gripper force (in [Nm]).
+        ``err`` is 0, on success, -1 otherwise.
+
+    :rtype:
+        Tuple
+        [
+        Union[MutableFloatVectorLike, List[float]],
+        Union[MutableFloatVectorLike, List[float]],
+        int
+        ]
+
+    """
+
+    fx = c_double()
+    fy = c_double()
+    fz = c_double()
+
+    tx = c_double()
+    ty = c_double()
+    tz = c_double()
+
+    fg = c_double()
+
+    err = _libdhd.dhdGetForceAndTorqueAndGripperForce(
+        byref(fx), byref(fy), byref(fz),
+        byref(tx), byref(ty), byref(tz),
+        byref(fg),
+        ID
+    )
+
+    if f_out is None:
+        f_ret = [fx.value, fy.value, fz.value]
+    else:
+        f_ret = f_out
+
+        f_out[0] = fx.value
+        f_out[1] = fy.value
+        f_out[2] = fz.value
+
+    if t_out is None:
+        t_ret = [tx.value, ty.value, tz.value]
+    else:
+        t_ret = t_out
+
+        t_out[0] = tx.value
+        t_out[1] = ty.value
+        t_out[2] = tz.value
+
+    return (f_ret, t_ret, fg.value, err)
+
+
 _libdhd.dhdConfigLinearVelocity.argtypes = [c_int, c_int, c_byte]
 _libdhd.dhdConfigLinearVelocity.restype = c_int
 
 
 def configLinearVelocity(
     ms: int = VELOCITY_WINDOW,
     mode: int = VELOCITY_WINDOWING,
```

### Comparing `forcedimension-0.1.5/forcedimension/dhd/adaptors.py` & `forcedimension-0.1.6/forcedimension/dhd/adaptors.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/dhd/constants.py` & `forcedimension-0.1.6/forcedimension/dhd/constants.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/dhd/expert.py` & `forcedimension-0.1.6/forcedimension/dhd/expert.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/dhd/os_independent.py` & `forcedimension-0.1.6/forcedimension/dhd/os_independent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-.. module::expert
-   :platform: Windows, Unix
-   :synopsis: libdhd "OS Independent SDK" Python libdhd
-
-.. moduleauthor:: Ember "Emmy" Chow <emberchow.business@gmail.com>
-"""
-
 from ctypes import c_bool, c_byte, c_double
 from forcedimension import runtime
 
 _libdhd = runtime.load("libdrd")
 
 if _libdhd is None:
     raise ImportError("There were problems loading libdhd.")
@@ -64,22 +56,21 @@
         The current monotonic time in [s] from the high-resolution system
         counter.
     """
     return _libdhd.dhdGetTime()
 
 
 _libdhd.dhdSleep.argtypes = [c_double]
-_libdhd.dhd.restype = None
+_libdhd.dhdSleep.restype = None
 
 
 def sleep(sec: float) -> None:
     """
     Sleep for a given period of time in [s]. This function is OS independent.
 
     :rtype: None
     """
     _libdhd.dhdSleep(sec)
 
 
 def startThread():
-    # TODO implement startThread
-    pass
+    raise NotImplementedError()
```

### Comparing `forcedimension-0.1.5/forcedimension/drd/__init__.py` & `forcedimension-0.1.6/forcedimension/drd/__init__.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/runtime.py` & `forcedimension-0.1.6/forcedimension/runtime.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/typing.py` & `forcedimension-0.1.6/forcedimension/typing.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension/util.py` & `forcedimension-0.1.6/forcedimension/util.py`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/forcedimension.egg-info/PKG-INFO` & `forcedimension-0.1.6/forcedimension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forcedimension
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Bindings for the ForceDimension SDK
 Author-email: Ember Chow <emberchow.business@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `forcedimension-0.1.5/forcedimension.egg-info/SOURCES.txt` & `forcedimension-0.1.6/forcedimension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forcedimension-0.1.5/pyproject.toml` & `forcedimension-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "forcedimension"
-version = "0.1.5"
-authors = [ 
+version = "0.1.6"
+authors = [
     { name="Ember Chow", email="emberchow.business@gmail.com" },
 ]
 description = "Python Bindings for the ForceDimension SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file="LICENSE"}
 classifiers = [
```

