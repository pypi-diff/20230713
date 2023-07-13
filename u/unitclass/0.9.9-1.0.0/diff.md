# Comparing `tmp/unitclass-0.9.9.tar.gz` & `tmp/unitclass-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-0.9.9.tar", last modified: Wed Mar 22 23:15:12 2023, max compression
+gzip compressed data, was "unitclass-1.0.0.tar", last modified: Thu Jul 13 00:06:34 2023, max compression
```

## Comparing `unitclass-0.9.9.tar` & `unitclass-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-03-22 23:15:12.397150 unitclass-0.9.9/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-0.9.9/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-03-22 23:15:12.396978 unitclass-0.9.9/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-0.9.9/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-03-22 23:14:13.000000 unitclass-0.9.9/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-03-22 23:15:12.397188 unitclass-0.9.9/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-03-22 23:15:12.396769 unitclass-0.9.9/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-03-22 23:15:12.000000 unitclass-0.9.9/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-03-22 23:15:12.000000 unitclass-0.9.9/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-03-22 23:15:12.000000 unitclass-0.9.9/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-03-22 23:15:12.000000 unitclass-0.9.9/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    42975 2023-03-22 23:13:52.000000 unitclass-0.9.9/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:06:34.515886 unitclass-1.0.0/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.0/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:06:34.515750 unitclass-1.0.0/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.0/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 00:05:55.000000 unitclass-1.0.0/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 00:06:34.515920 unitclass-1.0.0/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:06:34.515567 unitclass-1.0.0/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    42813 2023-07-13 00:03:52.000000 unitclass-1.0.0/unitclass.py
```

### Comparing `unitclass-0.9.9/LICENSE` & `unitclass-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-0.9.9/PKG-INFO` & `unitclass-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 0.9.9
+Version: 1.0.0
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-0.9.9/README.md` & `unitclass-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-0.9.9/pyproject.toml` & `unitclass-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "0.9.9"
+version = "1.0.0"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-0.9.9/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.0/unitclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 0.9.9
+Version: 1.0.0
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-0.9.9/unitclass.py` & `unitclass-1.0.0/unitclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     'luminous_intensity': [['luminous_intensity'], []],
     'force': [['force'], []],
     'angle': [['angle'], []],
     'unitless': [['unitless'], []],
     # Other special purpose
     'concentration': [['unitless'], []],
     'data': [['data'], []],
+    'currency': [['currency'], []],
     # SI
     'mass': [['force', 'time', 'time'], ['length']],  # force/acceleration
     'energy': [['force', 'length'], []],
     'charge': [['current', 'time'], []],
     'catalytic_activity': [['amount'], ['time']],
     'illuminance': [['luminous_intensity', 'angle', 'angle'], ['length'] * 2],
     'power': [['force', 'length'], ['time']],
@@ -278,14 +279,19 @@
     ('data', 'B', 'byte bytes', 1, ''),
     ('data', 'KB', 'kilobyte kilobytes', 1024, 'B'),
     ('data', 'MB', 'megabyte megabytes', 1024, 'KB'),
     ('data', 'GB', 'gigabyte gigabytes', 1024, 'MB'),
     ('data', 'TB', 'terabyte terabytes', 1024, 'GB'),
     ('data', 'PB', 'petabyte petabytes', 1024, 'TB'),
     ('data', 'EB', 'exabyte exabytes', 1024, 'PB'),
+    ('currency', 'USD', 'dollars dollar usdollar', 1, ''),
+    ('currency', 'pennies', 'penny', 0.01, 'USD'),
+    ('currency', 'nickles', 'nickle', 0.05, 'USD'),
+    ('currency', 'dimes', 'dime', 0.10, 'USD'),
+    ('currency', 'quarters', 'quarter', 0.25, 'USD'),
     ('speed', 'mph', 'mileperhour', 1, 'mi/hr'),
     ('speed', 'kph', 'kmperhour', 1, 'km/hr'),
     ('speed', 'c', 'lightspeed', 299792458, 'm/s'),
     ('speed', 'mach', 'Ma mach_sealevel_15C', 340.3, 'm/s'),
     ('angular speed', 'rpm', 'RPM RPMS rpms', 1, 'rev/min'),
     ('concentration', '%', 'pct percent percentage', 0.01, 'unitless'),
     ('concentration', 'ppm', 'partspermillion', 1e-4, 'pct'),
@@ -331,36 +337,34 @@
     expand: will call _expand_units()
     """    
     if not numerator:
         numerator = []
     if not denominator:
         denominator = []
     text = text.strip()
-    # print("CALL",text, numerator, denominator)
     if divflip:
         numerator, denominator = denominator, numerator
 
     while match := re_oper.search(text):
         parens = match.group(1)
         term1 = match.group(3)
         op = match.group(4)
         term2 = match.group(5)
         term2_parens = match.group(6)
-        # print(text, '>>>', op, term1, term2, term2_parens, parens, match.span(), numerator, denominator)
 
-        if op == '*':
+        if op in ('*','×','·','•','⋅'):
             end = match.end()
             if term1: numerator.append(term1)
             if term2: numerator.append(term2)
             elif term2_parens:
                 numerator, denominator = _parse_unit(
                     term2_parens[1:-1], numerator, denominator, expand=False)
                 end += len(term2_parens)
             text = text[end:]
-        elif op == '/':
+        elif op in ('/','÷'):
             end = match.end()
             if term1: numerator.append(term1)
             if term2: denominator.append(term2)
             elif term2_parens:  # flip num/denom since it's being divided
                 numerator, denominator = _parse_unit(term2_parens[1:-1],
                                                           numerator,
                                                           denominator,
@@ -377,43 +381,14 @@
     if divflip:
         numerator, denominator = denominator, numerator
     if expand:
         numerator = _expand_units(numerator)
         denominator = _expand_units(denominator)
     return numerator, denominator
 
-def _parse_unit_simple(name, expand=True):
-    """Parse unit str and break down to indvidual components
-    e.g.:
-
-    >>> _parse_unit_simple(name='N*m/s*in')
-    (['N', 'm'], ['s', 'in'])
-
-    NOTE: This is a simplified function. It only allows for one
-        divsion operator and does not folow PEMDAS.
-        Everything on the left side of the division operator is multiplied and is the numerator.
-        Everything on the right side of the division operator is multiplied and is the denominator.
-
-    expand: will call _expand_units()
-    """
-    fractional = name.split("/")
-    if len(fractional) == 1:
-        num = fractional[0].split("*")
-        denom = []
-    else:
-        num, denom = fractional
-        num, denom = num.split("*"), denom.split("*")
-
-    if expand:
-        num = _expand_units(num)
-        denom = _expand_units(denom)
-
-    return num, denom
-
-
 def _get_unit(unit):
     """Returns unit dict, handling aliases too"""
     if unit in _units:
         return _units[unit]
     elif unit in _aliases:
         return _units[_aliases[unit]]
     else:
@@ -614,14 +589,20 @@
 
 def convert(value, from_unit, to_unit):
     """Convert value from original unit to new unit
     Example: convert(40, 'pcf', 'kg/m3') returns 640.7
     Special cases include temperature
     """
     # TODO: this doesn't handle compound units with temperature, like J/degC
+    
+    if (not to_unit) and (from_unit != '%'): # unitless, treat as same unit
+        return value
+    elif (not from_unit) and (to_unit != '%'): # unitless, treat as same unit
+        return value
+
     both = _get_unit_name(from_unit, ignore_error=True) + \
         _get_unit_name(to_unit, ignore_error=True)
     if both == '°C°F':
         newvalue = _convert_C2F(value)
     elif both == '°F°C':
         newvalue = _convert_F2C(value)
     elif both == '°K°C':
@@ -1011,40 +992,43 @@
 
     def __rtruediv__(self, other):
         return self.__truediv__(other, op='rdiv')
 
     def __add__(self, other):
         if isinstance(other, Unit):
             _check_consistent_units(other.unit, self.unit)
+            newunit = self.unit or other.unit
             other = convert(other.value, other.unit, self.unit)
+        else:
+            newunit = self.unit
         newvalue = self.value + other
-        if (not self.unit) and (not isinstance(other, Unit)):
-            return Unit(newvalue, '')
-        return Unit(newvalue, self.unit or other.unit)
+        return Unit(newvalue, newunit)
 
     def __radd__(self, other):
         return self.__add__(other)
 
     def __sub__(self, other):
         if isinstance(other, Unit):
             _check_consistent_units(other.unit, self.unit)
+            newunit = self.unit or other.unit
             other = convert(other.value, other.unit, self.unit)
+        else:
+            newunit = self.unit
         newvalue = self.value - other
-        if (not self.unit) and (not isinstance(other, Unit)):
-            return Unit(newvalue, '')
-        return Unit(newvalue, self.unit or other.unit)
+        return Unit(newvalue, newunit)
 
     def __rsub__(self, other):
         if isinstance(other, Unit):
             _check_consistent_units(other.unit, self.unit)
+            newunit = self.unit or other.unit
             other = convert(other.value, other.unit, self.unit)
+        else:
+            newunit = self.unit
         newvalue = other - self.value
-        if (not self.unit) and (not isinstance(other, Unit)):
-            return Unit(newvalue, '')
-        return Unit(newvalue, self.unit or other.unit)
+        return Unit(newvalue, newunit)
 
     def __pow__(self, other):
         return Unit(self.value**other, self._new_unit(other, op="pow"))
 
     def __float__(self):
         return float(self.value)  # type: ignore
 
@@ -1108,10 +1092,23 @@
     doctest.testfile('doctests.txt')
     doctest.testfile('README.md', optionflags=doctest.ELLIPSIS+doctest.NORMALIZE_WHITESPACE)
 
     # print(Unit(4, 'in2')/Unit(50.8,'mm'))
     # print(Unit(50.8,'mm2')/Unit(4, 'in'))
     # print(4/Unit('2 m'))
     # print(Unit('4 m')/Unit('2 m'))
-    # print(Unit('4 m')/2)
+    # print(Unit('1 USD'))
+    # print(Unit('1 USD')/Unit('sqft'))
+    # print(Unit('1 USD').to('pennies'))
     # print(Unit('4 m2')/Unit('2 m'))
     # print(Unit(50.8,'mm')*Unit(4, 'in'))
+    # print(Unit('1 m')/Unit('1 m'))
+    # print(Unit('1 m')/Unit('1 m') + Unit('1 m'))
+    # print(Unit('1 m') + Unit('1 m')/Unit('1 m'))
+    # a = Unit(1, 'in')
+    # b = Unit(1, 'm')/Unit(1, 'm')
+    # print(a)
+    # print(a.value,'>', a.unit)
+    # print(b)
+    # print(b.value,'>', b.unit)
+    # print(a+b)
+    # print(b+a)
```

