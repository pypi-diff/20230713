# Comparing `tmp/unitclass-1.0.3.tar.gz` & `tmp/unitclass-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.3.tar", last modified: Thu Jul 13 01:50:57 2023, max compression
+gzip compressed data, was "unitclass-1.0.4.tar", last modified: Thu Jul 13 02:30:00 2023, max compression
```

## Comparing `unitclass-1.0.3.tar` & `unitclass-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 01:50:57.469771 unitclass-1.0.3/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.3/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 01:50:57.469636 unitclass-1.0.3/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.3/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 01:50:49.000000 unitclass-1.0.3/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 01:50:57.469804 unitclass-1.0.3/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 01:50:57.469456 unitclass-1.0.3/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 01:50:57.000000 unitclass-1.0.3/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 01:50:57.000000 unitclass-1.0.3/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 01:50:57.000000 unitclass-1.0.3/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 01:50:57.000000 unitclass-1.0.3/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    43320 2023-07-13 01:50:38.000000 unitclass-1.0.3/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 02:30:00.131321 unitclass-1.0.4/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.4/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 02:30:00.131186 unitclass-1.0.4/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.4/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 02:29:51.000000 unitclass-1.0.4/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 02:30:00.131354 unitclass-1.0.4/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 02:30:00.131031 unitclass-1.0.4/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 02:30:00.000000 unitclass-1.0.4/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    43370 2023-07-13 02:29:37.000000 unitclass-1.0.4/unitclass.py
```

### Comparing `unitclass-1.0.3/LICENSE` & `unitclass-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.3/PKG-INFO` & `unitclass-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.3
+Version: 1.0.4
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.3/README.md` & `unitclass-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.3/pyproject.toml` & `unitclass-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.3/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.4/unitclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.3
+Version: 1.0.4
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.3/unitclass.py` & `unitclass-1.0.4/unitclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,19 +914,20 @@
             if qty in _defaults:
                 new_unit = _defaults[qty]
                 self.to(new_unit)
         return self
 
     def __format__(self, format_spec):
         unit_str = self.unit.translate(self.to_specials)
-        number = "{r:{f}}".format(r=self.value, f=format_spec)
         prefix = ''
         if 'USD' in unit_str:
             prefix = '$'
             unit_str = unit_str.replace('USD','')
+            format_spec = '.2f'
+        number = "{r:{f}}".format(r=self.value, f=format_spec)
         return "{}{} {}".format(prefix, number, unit_str).strip()
 
     def _true_repr(self):
         """
         This is the true __repr__ method that returns a representation that can 
         reconstruct the object. e.g.:
 
@@ -1106,15 +1107,15 @@
 
     # print(Unit(4, 'in2')/Unit(50.8,'mm'))
     # print(Unit(50.8,'mm2')/Unit(4, 'in'))
     # print(4/Unit('2 m'))
     # print(Unit('4 m')/Unit('2 m'))
     print(Unit('1 USD'))
     print(Unit('$1.00'))
-    print(Unit('1.00 USD/sqft'))
+    print("{:.10g}".format(Unit('1.00 USD/sqft')))
     # print(Unit('1 USD')/Unit('sqft'))
     # print(Unit('1 USD').to('pennies'))
     # print(Unit('4 m2')/Unit('2 m'))
     # print(Unit(50.8,'mm')*Unit(4, 'in'))
     # print(Unit('1 m')/Unit('1 m'))
     # print(Unit('1 m')/Unit('1 m') + Unit('1 m'))
     # print(Unit('1 m') + Unit('1 m')/Unit('1 m'))
```

