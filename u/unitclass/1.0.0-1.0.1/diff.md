# Comparing `tmp/unitclass-1.0.0.tar.gz` & `tmp/unitclass-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.0.tar", last modified: Thu Jul 13 00:06:34 2023, max compression
+gzip compressed data, was "unitclass-1.0.1.tar", last modified: Thu Jul 13 00:13:40 2023, max compression
```

## Comparing `unitclass-1.0.0.tar` & `unitclass-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:06:34.515886 unitclass-1.0.0/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.0/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:06:34.515750 unitclass-1.0.0/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.0/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 00:05:55.000000 unitclass-1.0.0/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 00:06:34.515920 unitclass-1.0.0/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:06:34.515567 unitclass-1.0.0/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 00:06:34.000000 unitclass-1.0.0/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    42813 2023-07-13 00:03:52.000000 unitclass-1.0.0/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:13:40.223242 unitclass-1.0.1/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.1/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:13:40.223065 unitclass-1.0.1/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.1/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-13 00:13:33.000000 unitclass-1.0.1/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-13 00:13:40.223290 unitclass-1.0.1/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-13 00:13:40.222909 unitclass-1.0.1/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-13 00:13:40.000000 unitclass-1.0.1/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-13 00:13:40.000000 unitclass-1.0.1/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-13 00:13:40.000000 unitclass-1.0.1/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-13 00:13:40.000000 unitclass-1.0.1/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    42813 2023-07-13 00:13:26.000000 unitclass-1.0.1/unitclass.py
```

### Comparing `unitclass-1.0.0/LICENSE` & `unitclass-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.0/PKG-INFO` & `unitclass-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.0
+Version: 1.0.1
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.0/README.md` & `unitclass-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.0/pyproject.toml` & `unitclass-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.0/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.1/unitclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.0
+Version: 1.0.1
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.0/unitclass.py` & `unitclass-1.0.1/unitclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     ('data', 'MB', 'megabyte megabytes', 1024, 'KB'),
     ('data', 'GB', 'gigabyte gigabytes', 1024, 'MB'),
     ('data', 'TB', 'terabyte terabytes', 1024, 'GB'),
     ('data', 'PB', 'petabyte petabytes', 1024, 'TB'),
     ('data', 'EB', 'exabyte exabytes', 1024, 'PB'),
     ('currency', 'USD', 'dollars dollar usdollar', 1, ''),
     ('currency', 'pennies', 'penny', 0.01, 'USD'),
-    ('currency', 'nickles', 'nickle', 0.05, 'USD'),
+    ('currency', 'nickels', 'nickel', 0.05, 'USD'),
     ('currency', 'dimes', 'dime', 0.10, 'USD'),
     ('currency', 'quarters', 'quarter', 0.25, 'USD'),
     ('speed', 'mph', 'mileperhour', 1, 'mi/hr'),
     ('speed', 'kph', 'kmperhour', 1, 'km/hr'),
     ('speed', 'c', 'lightspeed', 299792458, 'm/s'),
     ('speed', 'mach', 'Ma mach_sealevel_15C', 340.3, 'm/s'),
     ('angular speed', 'rpm', 'RPM RPMS rpms', 1, 'rev/min'),
```

