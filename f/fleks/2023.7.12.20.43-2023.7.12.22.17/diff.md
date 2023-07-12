# Comparing `tmp/fleks-2023.7.12.20.43.tar.gz` & `tmp/fleks-2023.7.12.22.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleks-2023.7.12.20.43.tar", last modified: Wed Jul 12 20:43:51 2023, max compression
+gzip compressed data, was "fleks-2023.7.12.22.17.tar", last modified: Wed Jul 12 22:17:04 2023, max compression
```

## Comparing `fleks-2023.7.12.20.43.tar` & `fleks-2023.7.12.22.17.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.102328 fleks-2023.7.12.20.43/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.102328 fleks-2023.7.12.20.43/src/fleks/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 20:43:46.000000 fleks-2023.7.12.20.43/src/fleks/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/src/fleks/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-12 20:42:59.000000 fleks-2023.7.12.20.43/src/fleks/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/src/fleks/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/meta/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-12 20:42:59.000000 fleks-2023.7.12.20.43/src/fleks/meta/oop.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/src/fleks/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-12 20:42:15.000000 fleks-2023.7.12.20.43/src/fleks/util/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-12 20:42:59.000000 fleks-2023.7.12.20.43/src/fleks/util/lme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-12 20:42:59.000000 fleks-2023.7.12.20.43/src/fleks/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:43:51.106329 fleks-2023.7.12.20.43/src/fleks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 20:43:51.000000 fleks-2023.7.12.20.43/src/fleks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.293778 fleks-2023.7.12.22.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.293778 fleks-2023.7.12.22.17/src/fleks/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 22:16:59.000000 fleks-2023.7.12.22.17/src/fleks/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/src/fleks/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 22:16:03.000000 fleks-2023.7.12.22.17/src/fleks/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/src/fleks/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-12 22:16:05.000000 fleks-2023.7.12.22.17/src/fleks/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-12 22:16:04.000000 fleks-2023.7.12.22.17/src/fleks/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/src/fleks/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/meta/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-12 22:16:05.000000 fleks-2023.7.12.22.17/src/fleks/meta/oop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.297778 fleks-2023.7.12.22.17/src/fleks/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-12 22:15:15.000000 fleks-2023.7.12.22.17/src/fleks/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-12 22:16:05.000000 fleks-2023.7.12.22.17/src/fleks/util/lme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-12 22:16:05.000000 fleks-2023.7.12.22.17/src/fleks/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:17:04.293778 fleks-2023.7.12.22.17/src/fleks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 22:17:04.000000 fleks-2023.7.12.22.17/src/fleks.egg-info/top_level.txt
```

### Comparing `fleks-2023.7.12.20.43/PKG-INFO` & `fleks-2023.7.12.22.17/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2023.7.12.20.43
+Version: 2023.7.12.22.17
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any
 Classifier: Programming Language :: Python
-Requires-Python: >3.6
+Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
 Provides-Extra: publish
 
 See the project README
```

### Comparing `fleks-2023.7.12.20.43/README.md` & `fleks-2023.7.12.22.17/README.md`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/setup.cfg` & `fleks-2023.7.12.22.17/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -18,19 +18,22 @@
 [options]
 zip_safe = False
 zip_ok = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >3.6
+python_requires = >3.7
 install_requires = 
 	memoized-property==1.0.3
+	pydantic==1.10.11
+	blinker==1.6.2
 	rich==13.3.4
 	click==8.1.4
+	enlighten==1.11.2
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `fleks-2023.7.12.20.43/setup.py` & `fleks-2023.7.12.22.17/setup.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/cli/click.py` & `fleks-2023.7.12.22.17/src/fleks/cli/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/meta/namespace.py` & `fleks-2023.7.12.22.17/src/fleks/meta/namespace.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/meta/oop.py` & `fleks-2023.7.12.22.17/src/fleks/meta/oop.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/plugin.py` & `fleks-2023.7.12.22.17/src/fleks/plugin.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/util/__init__.py` & `fleks-2023.7.12.22.17/src/fleks/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/util/click.py` & `fleks-2023.7.12.22.17/src/fleks/util/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/util/lme.py` & `fleks-2023.7.12.22.17/src/fleks/util/lme.py`

 * *Files identical despite different names*

### Comparing `fleks-2023.7.12.20.43/src/fleks/util/typing.py` & `fleks-2023.7.12.22.17/src/fleks/util/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
 class classproperty:
     """ """
 
     def __init__(self, fxn):
         self.fxn = fxn
 
-    def __get__(self, obj, owner) -> OptionalAny:
-        assert obj
+    def __get__(self, obj, owner) -> OptionalAny:  # noqa
+        # assert obj
         return self.fxn(owner)
 
 
 class classproperty_cached(classproperty):
     """ """
 
     CLASSPROP_CACHES = {}
 
-    def __get__(self, obj, owner) -> OptionalAny:
-        assert obj
+    def __get__(self, obj, owner) -> OptionalAny:  # noqa
+        # assert obj
         result = self.__class__.CLASSPROP_CACHES.get(self.fxn, self.fxn(owner))
         self.__class__.CLASSPROP_CACHES[self.fxn] = result
         return self.__class__.CLASSPROP_CACHES[self.fxn]
```

### Comparing `fleks-2023.7.12.20.43/src/fleks.egg-info/PKG-INFO` & `fleks-2023.7.12.22.17/src/fleks.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2023.7.12.20.43
+Version: 2023.7.12.22.17
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any
 Classifier: Programming Language :: Python
-Requires-Python: >3.6
+Requires-Python: >3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: testing
 Provides-Extra: lint
 Provides-Extra: publish
 
 See the project README
```

### Comparing `fleks-2023.7.12.20.43/src/fleks.egg-info/SOURCES.txt` & `fleks-2023.7.12.22.17/src/fleks.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 src/fleks/plugin.py
 src/fleks.egg-info/PKG-INFO
 src/fleks.egg-info/SOURCES.txt
 src/fleks.egg-info/dependency_links.txt
 src/fleks.egg-info/not-zip-safe
 src/fleks.egg-info/requires.txt
 src/fleks.egg-info/top_level.txt
+src/fleks/app/__init__.py
 src/fleks/cli/__init__.py
+src/fleks/cli/arguments.py
 src/fleks/cli/click.py
+src/fleks/cli/options.py
 src/fleks/meta/__init__.py
 src/fleks/meta/namespace.py
 src/fleks/meta/oop.py
 src/fleks/util/__init__.py
 src/fleks/util/click.py
 src/fleks/util/lme.py
 src/fleks/util/typing.py
```

