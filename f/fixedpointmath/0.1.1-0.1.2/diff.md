# Comparing `tmp/fixedpointmath-0.1.1.tar.gz` & `tmp/fixedpointmath-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixedpointmath-0.1.1.tar", last modified: Thu Jun 29 18:47:36 2023, max compression
+gzip compressed data, was "fixedpointmath-0.1.2.tar", last modified: Wed Jul 12 22:39:45 2023, max compression
```

## Comparing `fixedpointmath-0.1.1.tar` & `fixedpointmath-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.079268 fixedpointmath-0.1.1/
--rw-r--r--   0 slundquist   (501) staff       (20)     2075 2023-06-29 18:47:36.079158 fixedpointmath-0.1.1/PKG-INFO
--rw-r--r--   0 slundquist   (501) staff       (20)     1429 2023-06-29 18:44:26.000000 fixedpointmath-0.1.1/README.md
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.077742 fixedpointmath-0.1.1/fixedpointmath/
--rw-r--r--   0 slundquist   (501) staff       (20)      503 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/__init__.py
--rw-r--r--   0 slundquist   (501) staff       (20)      213 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/errors.py
--rw-r--r--   0 slundquist   (501) staff       (20)    30490 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point.py
--rw-r--r--   0 slundquist   (501) staff       (20)    11036 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point_integer_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     1823 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/fixedpointmath/fixed_point_math.py
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.078171 fixedpointmath-0.1.1/fixedpointmath.egg-info/
--rw-r--r--   0 slundquist   (501) staff       (20)     2075 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/PKG-INFO
--rw-r--r--   0 slundquist   (501) staff       (20)      513 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/SOURCES.txt
--rw-r--r--   0 slundquist   (501) staff       (20)        1 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/dependency_links.txt
--rw-r--r--   0 slundquist   (501) staff       (20)       15 2023-06-29 18:47:36.000000 fixedpointmath-0.1.1/fixedpointmath.egg-info/top_level.txt
--rw-r--r--   0 slundquist   (501) staff       (20)      738 2023-06-29 18:47:24.000000 fixedpointmath-0.1.1/pyproject.toml
--rw-r--r--   0 slundquist   (501) staff       (20)       38 2023-06-29 18:47:36.079301 fixedpointmath-0.1.1/setup.cfg
-drwxr-xr-x   0 slundquist   (501) staff       (20)        0 2023-06-29 18:47:36.078985 fixedpointmath-0.1.1/tests/
--rw-r--r--   0 slundquist   (501) staff       (20)    23960 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_arithmetic_sugar.py
--rw-r--r--   0 slundquist   (501) staff       (20)    13308 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_class.py
--rw-r--r--   0 slundquist   (501) staff       (20)    17686 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_integer_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     4959 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_math.py
--rw-r--r--   0 slundquist   (501) staff       (20)     2281 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_nonfinite_checks.py
--rw-r--r--   0 slundquist   (501) staff       (20)     4527 2023-06-28 23:35:55.000000 fixedpointmath-0.1.1/tests/test_fp_relational_sugar.py
+drwxr-xr-x   0 matthewbrown   (501) staff       (20)        0 2023-07-12 22:39:45.763519 fixedpointmath-0.1.2/
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     2075 2023-07-12 22:39:45.763375 fixedpointmath-0.1.2/PKG-INFO
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     1429 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/README.md
+drwxr-xr-x   0 matthewbrown   (501) staff       (20)        0 2023-07-12 22:39:45.761058 fixedpointmath-0.1.2/fixedpointmath/
+-rw-r--r--   0 matthewbrown   (501) staff       (20)      503 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/fixedpointmath/__init__.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)      213 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/fixedpointmath/errors.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)    30368 2023-07-12 22:36:24.000000 fixedpointmath-0.1.2/fixedpointmath/fixed_point.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)    11289 2023-07-12 22:36:24.000000 fixedpointmath-0.1.2/fixedpointmath/fixed_point_integer_math.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     1823 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/fixedpointmath/fixed_point_math.py
+drwxr-xr-x   0 matthewbrown   (501) staff       (20)        0 2023-07-12 22:39:45.762014 fixedpointmath-0.1.2/fixedpointmath.egg-info/
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     2075 2023-07-12 22:39:45.000000 fixedpointmath-0.1.2/fixedpointmath.egg-info/PKG-INFO
+-rw-r--r--   0 matthewbrown   (501) staff       (20)      513 2023-07-12 22:39:45.000000 fixedpointmath-0.1.2/fixedpointmath.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewbrown   (501) staff       (20)        1 2023-07-12 22:39:45.000000 fixedpointmath-0.1.2/fixedpointmath.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewbrown   (501) staff       (20)       15 2023-07-12 22:39:45.000000 fixedpointmath-0.1.2/fixedpointmath.egg-info/top_level.txt
+-rw-r--r--   0 matthewbrown   (501) staff       (20)      738 2023-07-12 22:38:56.000000 fixedpointmath-0.1.2/pyproject.toml
+-rw-r--r--   0 matthewbrown   (501) staff       (20)       38 2023-07-12 22:39:45.763561 fixedpointmath-0.1.2/setup.cfg
+drwxr-xr-x   0 matthewbrown   (501) staff       (20)        0 2023-07-12 22:39:45.763166 fixedpointmath-0.1.2/tests/
+-rw-r--r--   0 matthewbrown   (501) staff       (20)    23960 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/tests/test_fp_arithmetic_sugar.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)    13308 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/tests/test_fp_class.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)    17846 2023-07-12 22:36:24.000000 fixedpointmath-0.1.2/tests/test_fp_integer_math.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     4959 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/tests/test_fp_math.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     2281 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/tests/test_fp_nonfinite_checks.py
+-rw-r--r--   0 matthewbrown   (501) staff       (20)     4527 2023-07-12 20:23:42.000000 fixedpointmath-0.1.2/tests/test_fp_relational_sugar.py
```

### Comparing `fixedpointmath-0.1.1/PKG-INFO` & `fixedpointmath-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixedpointmath
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fixed-point arithmetic and type that mirrors popular Solidity implementations
 Author-email: Dylan Paiton <dylan@delv.tech>, Mihai Cosma <mihai@delv.tech>, Matthew Brown <matt@delv.tech>, Sheng Lundquist <sheng@delv.tech>
 Project-URL: Homepage, https://github.com/delvtech/agent_0
 Project-URL: Bug Tracker, https://github.com/delvtech/agent_0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fixedpointmath-0.1.1/README.md` & `fixedpointmath-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/fixedpointmath/fixed_point.py` & `fixedpointmath-0.1.2/fixedpointmath/fixed_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,17 +563,15 @@
         r"""Cast to int"""
         if self.special_value is not None:
             raise ValueError(f"cannot convert FixedPoint {self.special_value} to integer")
         return int(self.scaled_value // 10**self.decimal_places)
 
     def __float__(self) -> float:
         r"""Cast to float"""
-        if self.special_value is not None:
-            return float(self.special_value)
-        return float(self.scaled_value) / 10**self.decimal_places
+        return float(str(self))
 
     def __bool__(self) -> bool:
         r"""Cast to bool"""
         if self.is_finite() and self != FixedPoint(0):
             return True
         return False
 
@@ -621,15 +619,15 @@
         memo[id(self)] = self
         return self
 
     # additional arethmitic & helper functions
     def div_up(self, other: OtherTypes | FixedPoint) -> FixedPoint:
         r"""Divide self by other, rounding up"""
         other = self._coerce_other(other)
-        if other <= FixedPoint("0.0"):
+        if other == FixedPoint("0.0"):
             raise errors.DivisionByZero
         return FixedPoint(
             scaled_value=FixedPointIntegerMath.div_up(self.scaled_value, other.scaled_value),
             decimal_places=self.decimal_places,
             signed=self.signed,
         )
```

### Comparing `fixedpointmath-0.1.1/fixedpointmath/fixed_point_integer_math.py` & `fixedpointmath-0.1.2/fixedpointmath/fixed_point_integer_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 
 from . import errors
 
 # we will use single letter names for the FixedPointIntegerMath class since all functions do basic arithmetic
 # pylint: disable=invalid-name
 
 
+def sign(value: int) -> int:
+    """Get the sign of an integer value."""
+    if value < 0:
+        return -1
+    return 1
+
+
 class FixedPointIntegerMath:
     """Safe integer arithmetic that assumes a 18-decimal fixed-point representation
 
     .. note::
         Most arithmetic adopted from `HyperDrive <https://github.com/delvtech/hyperdrive/blob/main/contracts/src/libraries/FixedPointMath.sol`_
         Credit to
             - `Solmate <https://github.com/transmissions11/solmate/blob/main/src/utils/FixedPointMathLib.sol>`_
@@ -89,15 +96,17 @@
     def mul_up(a: int, b: int) -> int:
         """Multiply a and b, rounding up."""
         return FixedPointIntegerMath.mul_div_up(a, b, FixedPointIntegerMath.ONE_18)
 
     @staticmethod
     def div_up(a: int, b: int) -> int:
         r"""Divide a by b, rounding up."""
-        return FixedPointIntegerMath.mul_div_up(a, FixedPointIntegerMath.ONE_18, b)
+
+        # mul_div_up expects positive values to do the rounding correctly.  handle the sign here.
+        return sign(a) * sign(b) * FixedPointIntegerMath.mul_div_up(abs(a), FixedPointIntegerMath.ONE_18, abs(b))
 
     @staticmethod
     def ilog2(x: int) -> int:
         r"""Returns floor(log2(x)) if x is nonzero, otherwise 0.
 
         This is the same as the location of the highest set bit.
         """
```

### Comparing `fixedpointmath-0.1.1/fixedpointmath/fixed_point_math.py` & `fixedpointmath-0.1.2/fixedpointmath/fixed_point_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/fixedpointmath.egg-info/PKG-INFO` & `fixedpointmath-0.1.2/fixedpointmath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixedpointmath
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fixed-point arithmetic and type that mirrors popular Solidity implementations
 Author-email: Dylan Paiton <dylan@delv.tech>, Mihai Cosma <mihai@delv.tech>, Matthew Brown <matt@delv.tech>, Sheng Lundquist <sheng@delv.tech>
 Project-URL: Homepage, https://github.com/delvtech/agent_0
 Project-URL: Bug Tracker, https://github.com/delvtech/agent_0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fixedpointmath-0.1.1/fixedpointmath.egg-info/SOURCES.txt` & `fixedpointmath-0.1.2/fixedpointmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/pyproject.toml` & `fixedpointmath-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixedpointmath"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "Dylan Paiton", email = "dylan@delv.tech" },
     { name = "Mihai Cosma", email = "mihai@delv.tech" },
     { name = "Matthew Brown", email = "matt@delv.tech" },
     { name = "Sheng Lundquist", email = "sheng@delv.tech" },
 ]
 description = "Fixed-point arithmetic and type that mirrors popular Solidity implementations"
```

### Comparing `fixedpointmath-0.1.1/tests/test_fp_arithmetic_sugar.py` & `fixedpointmath-0.1.2/tests/test_fp_arithmetic_sugar.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/tests/test_fp_class.py` & `fixedpointmath-0.1.2/tests/test_fp_class.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/tests/test_fp_integer_math.py` & `fixedpointmath-0.1.2/tests/test_fp_integer_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """FixedPoint integer math tests inspired from solidity hyperdrive implementation"""
 import math
 import unittest
 
-from fixedpointmath import errors
-from fixedpointmath import FixedPointIntegerMath
+from fixedpointmath import FixedPointIntegerMath, errors
 
 # pylint: disable=too-many-public-methods
 
 
 class TestFixedPointIntegerMath(unittest.TestCase):
     """Unit tests to verify that the fixed-point integer implementations are correct.
     The tests assume everything is in 1e18 precision.
@@ -130,14 +129,16 @@
         )
         self.assertEqual(
             FixedPointIntegerMath.div_up(3 * FixedPointIntegerMath.ONE_18, FixedPointIntegerMath.ONE_18),
             3 * FixedPointIntegerMath.ONE_18,
         )
         self.assertEqual(FixedPointIntegerMath.div_up(2 * FixedPointIntegerMath.ONE_18, int(1e19 * 1e18)), 1)
         self.assertEqual(FixedPointIntegerMath.div_up(0, FixedPointIntegerMath.ONE_18), 0)
+        self.assertEqual(FixedPointIntegerMath.div_up(-1, 1), -FixedPointIntegerMath.ONE_18)
+        self.assertEqual(FixedPointIntegerMath.div_up(1, -1), -FixedPointIntegerMath.ONE_18)
 
     def test_fail_div_up_zero_denominator(self):
         """Test error when dividing by zero"""
         with self.assertRaises(ValueError):
             FixedPointIntegerMath.div_up(FixedPointIntegerMath.ONE_18, 0)
 
     def test_mul_div_down(self):
```

### Comparing `fixedpointmath-0.1.1/tests/test_fp_math.py` & `fixedpointmath-0.1.2/tests/test_fp_math.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/tests/test_fp_nonfinite_checks.py` & `fixedpointmath-0.1.2/tests/test_fp_nonfinite_checks.py`

 * *Files identical despite different names*

### Comparing `fixedpointmath-0.1.1/tests/test_fp_relational_sugar.py` & `fixedpointmath-0.1.2/tests/test_fp_relational_sugar.py`

 * *Files identical despite different names*

