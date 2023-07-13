# Comparing `tmp/chaostoolkit-lib-1.8.1.tar.gz` & `tmp/chaostoolkit-lib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chaostoolkit-lib-1.8.1.tar", last modified: Thu Feb 20 09:50:50 2020, max compression
+gzip compressed data, was "dist/chaostoolkit-lib-1.9.0.tar", last modified: Wed Apr 29 14:04:16 2020, max compression
```

## Comparing `chaostoolkit-lib-1.8.1.tar` & `chaostoolkit-lib-1.9.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7397 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2981 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10040 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    28754 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      193 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      123 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10040 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/pytest.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaoslib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7061 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/notification.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaoslib/control/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13178 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/control/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5478 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/control/python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/extension.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4033 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      822 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/settings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaoslib/provider/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4097 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/provider/http.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/provider/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3630 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/provider/process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5115 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/provider/python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9440 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/activity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3760 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1424 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/rollback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/caching.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-20 09:50:50.000000 chaostoolkit-lib-1.8.1/chaoslib/discovery/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6543 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/discovery/discover.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3639 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/discovery/package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/discovery/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9341 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/secret.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13236 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2403 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/deprecation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12108 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/hypothesis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-02-20 09:50:23.000000 chaostoolkit-lib-1.8.1/chaoslib/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7397 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2981 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      229 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10040 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29516 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      193 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       94 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      127 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      123 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10040 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/pytest.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaoslib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7061 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/notification.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaoslib/control/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13178 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/control/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5478 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/control/python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2766 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/extension.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4237 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/settings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaoslib/provider/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4097 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/provider/http.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/provider/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3649 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/provider/process.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5115 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/provider/python.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9440 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/activity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3760 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1424 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/rollback.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/caching.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-29 14:04:16.000000 chaostoolkit-lib-1.9.0/chaoslib/discovery/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6543 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/discovery/discover.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3639 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/discovery/package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/discovery/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2105 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/configuration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9341 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/secret.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13377 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/experiment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2403 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/deprecation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12108 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/hypothesis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-04-29 14:03:48.000000 chaostoolkit-lib-1.9.0/chaoslib/types.py
```

### Comparing `chaostoolkit-lib-1.8.1/README.md` & `chaostoolkit-lib-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/setup.py` & `chaostoolkit-lib-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/LICENSE` & `chaostoolkit-lib-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/PKG-INFO` & `chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-lib
-Version: 1.8.1
+Version: 1.9.0
 Summary: Chaos engineering toolkit core library
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License 2.0
 Description: # chaostoolkit-lib
         
@@ -210,10 +210,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.5.*
 Description-Content-Type: text/markdown
+Provides-Extra: jsonpath
 Provides-Extra: vault
 Provides-Extra: decoders
-Provides-Extra: jsonpath
```

### Comparing `chaostoolkit-lib-1.8.1/chaostoolkit_lib.egg-info/SOURCES.txt` & `chaostoolkit-lib-1.9.0/chaostoolkit_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/CHANGELOG.md` & `chaostoolkit-lib-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 # Changelog
 
 ## [Unreleased][]
 
-[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.8.1...HEAD
+[Unreleased]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.9.0...HEAD
+
+## [1.9.0][] - 2020-04-29
+
+[1.9.0]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.8.1...1.9.0
+
+### Added
+
+- Only apply rollbacks if experiment has progressed past the initial steady state hypothesis [#168](168)
+- Allow to not verify certificates when connecting to a HTTPS endpoint using [#163](163)
+  self-signed certificate.
+
+[168]: https://github.com/chaostoolkit/chaostoolkit-lib/issues/168
+[163]: https://github.com/chaostoolkit/chaostoolkit-lib/issues/163
+
+### Changed
+
+- Fix error on empty string variables call [#165][165]
+
+[165]: https://github.com/chaostoolkit/chaostoolkit-lib/issues/165
+
 
 ## [1.8.1][] - 2020-02-20
 
 [1.8.1]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.8.0...1.8.1
 
 ### Added
 
@@ -23,20 +43,23 @@
 [1.8.0]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.7.1...1.8.0
 
 ### Added
 
 - Optional default value for environment variable in configuration
 - Warn the user for an action process returning a non-zero exit code 
 - Support for process path relative to homedir ~
+- Indicate path in validation when path is not found nor executable [#159][159]
 
 ### Changed
 
 - Changed the method's one-step minimum requirement. 
   An experiment with an empty method (without any activities) is now valid.
 
+[159]: https://github.com/chaostoolkit/chaostoolkit-lib/issues/159
+
 ## [1.7.1][] - 2019-09-27
 
 [1.7.1]: https://github.com/chaostoolkit/chaostoolkit-lib/compare/1.7.0...1.7.1
 
 ### Added
 
 - Catch `InterruptExecution` during rollbacks so that the experiment terminates
```

### Comparing `chaostoolkit-lib-1.8.1/PKG-INFO` & `chaostoolkit-lib-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaostoolkit-lib
-Version: 1.8.1
+Version: 1.9.0
 Summary: Chaos engineering toolkit core library
 Home-page: http://chaostoolkit.org
 Author: chaostoolkit Team
 Author-email: contact@chaostoolkit.org
 License: Apache License 2.0
 Description: # chaostoolkit-lib
         
@@ -210,10 +210,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.5.*
 Description-Content-Type: text/markdown
+Provides-Extra: jsonpath
 Provides-Extra: vault
 Provides-Extra: decoders
-Provides-Extra: jsonpath
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/info.py` & `chaostoolkit-lib-1.9.0/chaoslib/info.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/notification.py` & `chaostoolkit-lib-1.9.0/chaoslib/notification.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/control/__init__.py` & `chaostoolkit-lib-1.9.0/chaoslib/control/__init__.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/control/python.py` & `chaostoolkit-lib-1.9.0/chaoslib/control/python.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/extension.py` & `chaostoolkit-lib-1.9.0/chaoslib/extension.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/loader.py` & `chaostoolkit-lib-1.9.0/chaoslib/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             except yaml.YAMLError:
                 pass
 
     raise InvalidExperiment(
         "only files with json, yaml or yml extensions are supported")
 
 
-def load_experiment(experiment_source: str,
-                    settings: Settings = None) -> Experiment:
+def load_experiment(experiment_source: str, settings: Settings = None,
+                    verify_tls: bool = True) -> Experiment:
     """
     Load an experiment from the given source.
 
     The source may be a local file or a HTTP(s) URL. If the endpoint requires
     authentication, please set the appropriate entry in the settings file,
     under the `auths:` section, keyed by domain. For instance:
 
@@ -86,14 +86,18 @@
       otherdomain.com:
         type: bearer
         value: UIY
       localhost:8081:
         type: digest
         value: UIY
     ```
+
+    Set `verify_tls` to `False` if the source is a over a self-signed
+    certificate HTTP endpoint to instruct the loader to not verify the
+    certificates.
     """
     with controls(level="loader", context=experiment_source) as control:
         if os.path.exists(experiment_source):
             parsed = parse_experiment_from_file(experiment_source)
             control.with_state(parsed)
             return parsed
 
@@ -113,15 +117,15 @@
             for domain in auths:
                 if domain == p.netloc:
                     auth = auths[domain]
                     headers["Authorization"] = '{} {}'.format(
                         auth["type"], auth["value"])
                     break
 
-        r = requests.get(experiment_source, headers=headers)
+        r = requests.get(experiment_source, headers=headers, verify=verify_tls)
         if r.status_code != 200:
             raise InvalidSource(
                 "Failed to fetch the experiment: {}".format(r.text))
 
         logger.debug("Fetched experiment: \n{}".format(r.text))
         parsed = parse_experiment_from_http(r)
         control.with_state(parsed)
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/exceptions.py` & `chaostoolkit-lib-1.9.0/chaoslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/settings.py` & `chaostoolkit-lib-1.9.0/chaoslib/settings.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/provider/http.py` & `chaostoolkit-lib-1.9.0/chaoslib/provider/http.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/provider/process.py` & `chaostoolkit-lib-1.9.0/chaoslib/provider/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,21 +90,21 @@
     In all failing cases, raises :exc:`InvalidActivity`.
 
     This should be considered as a private function.
     """
     name = activity["name"]
     provider = activity["provider"]
 
-    path = provider.get("path")
+    path = raw_path = provider.get("path")
     if not path:
         raise InvalidActivity("a process activity must have a path")
 
     path = shutil.which(path)
     if not path:
         raise InvalidActivity(
             "path '{path}' cannot be found, in activity '{name}'".format(
-                path=path, name=name))
+                path=raw_path, name=name))
 
     if not os.access(path, os.X_OK):
         raise InvalidActivity(
             "no access permission to '{path}', in activity '{name}'".format(
-                path=path, name=name))
+                path=raw_path, name=name))
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/provider/python.py` & `chaostoolkit-lib-1.9.0/chaoslib/provider/python.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/activity.py` & `chaostoolkit-lib-1.9.0/chaoslib/activity.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/__init__.py` & `chaostoolkit-lib-1.9.0/chaoslib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         HAS_CHARDET = False
 from logzero import logger
 
 from chaoslib.exceptions import ActivityFailed
 from chaoslib.types import Configuration, Secrets
 
 __all__ = ["__version__", "decode_bytes", "substitute"]
-__version__ = '1.8.1'
+__version__ = '1.9.0'
 
 
 def substitute(data: Union[None, str, Dict[str, Any], List],
                configuration: Configuration,
                secrets: Secrets) -> Dict[str, Any]:
     """
     Replace forms such as `${name}` with the first value found in either the
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/rollback.py` & `chaostoolkit-lib-1.9.0/chaoslib/rollback.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/caching.py` & `chaostoolkit-lib-1.9.0/chaoslib/caching.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/discovery/discover.py` & `chaostoolkit-lib-1.9.0/chaoslib/discovery/discover.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/discovery/package.py` & `chaostoolkit-lib-1.9.0/chaoslib/discovery/package.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/configuration.py` & `chaostoolkit-lib-1.9.0/chaoslib/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     conf = {}
 
     for (key, value) in config_info.items():
         if isinstance(value, dict) and "type" in value:
             if value["type"] == "env":
                 env_key = value["key"]
                 env_default = value.get("default")
-                if env_key not in env and not env_default:
+                if (env_key not in env) and (env_default is None):
                     raise InvalidExperiment(
                         "Configuration makes reference to an environment key"
                         " that does not exist: {}".format(env_key))
                 conf[key] = env.get(env_key, env_default)
         else:
             conf[key] = value
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/secret.py` & `chaostoolkit-lib-1.9.0/chaoslib/secret.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/experiment.py` & `chaostoolkit-lib-1.9.0/chaoslib/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 import platform
 import time
 from typing import List
 
 from logzero import logger
 
-from chaoslib import __version__
+from chaoslib import __version__, substitute
 from chaoslib.activity import ensure_activity_is_valid, run_activities
 from chaoslib.caching import with_cache, lookup_activity
 from chaoslib.control import initialize_controls, controls, cleanup_controls, \
     validate_controls, Control, initialize_global_controls, \
     cleanup_global_controls
 from chaoslib.deprecation import warn_about_deprecated_features
 from chaoslib.exceptions import ActivityFailed, ChaosException, \
@@ -175,28 +175,29 @@
     abnormally (Ctrl-C, SIGTERM...). Afterall, there is a chance we actually
     cannot afford to rollback properly. Better bailing to a conservative
     approach. This means we swallow :exc:`KeyboardInterrupt` and
     :exc:`SystemExit` and do not bubble it back up to the caller. We when were
     interrupted, we set the `interrupted` flag of the result accordingly to
     notify the caller this was indeed not terminated properly.
     """
-    logger.info("Running experiment: {t}".format(t=experiment["title"]))
-
     dry = experiment.get("dry", False)
     if dry:
         logger.warning("Dry mode enabled")
 
     started_at = time.time()
     settings = settings if settings is not None else get_loaded_settings()
     config = load_configuration(experiment.get("configuration", {}))
     secrets = load_secrets(experiment.get("secrets", {}), config)
     initialize_global_controls(experiment, config, secrets, settings)
     initialize_controls(experiment, config, secrets)
     activity_pool, rollback_pool = get_background_pools(experiment)
 
+    experiment["title"] = substitute(experiment["title"], config, secrets)
+    logger.info("Running experiment: {t}".format(t=experiment["title"]))
+
     control = Control()
     journal = initialize_run_journal(experiment)
 
     try:
         try:
             control.begin(
                 "experiment", experiment, experiment, config, secrets)
@@ -211,15 +212,15 @@
                     raise ActivityFailed(
                         "Steady state probe '{p}' is not in the given "
                         "tolerance so failing this experiment".format(
                             p=p["activity"]["name"]))
             except ActivityFailed as a:
                 journal["steady_states"]["before"] = state
                 journal["status"] = "failed"
-                logger.fatal(str(a))
+                raise
             else:
                 try:
                     journal["run"] = apply_activities(
                         experiment, config, secrets, activity_pool, dry)
                 except InterruptExecution:
                     raise
                 except Exception:
@@ -238,14 +239,16 @@
                             raise ActivityFailed(
                                 "Steady state probe '{p}' is not in the given "
                                 "tolerance so failing this experiment".format(
                                     p=p["activity"]["name"]))
                     except ActivityFailed as a:
                         journal["status"] = "failed"
                         logger.fatal(str(a))
+        except ActivityFailed as a:
+            logger.fatal(str(a))
         except InterruptExecution as i:
             journal["status"] = "interrupted"
             logger.fatal(str(i))
         except (KeyboardInterrupt, SystemExit):
             journal["status"] = "interrupted"
             logger.warning("Received an exit signal, "
                            "leaving without applying rollbacks.")
```

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/deprecation.py` & `chaostoolkit-lib-1.9.0/chaoslib/deprecation.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/hypothesis.py` & `chaostoolkit-lib-1.9.0/chaoslib/hypothesis.py`

 * *Files identical despite different names*

### Comparing `chaostoolkit-lib-1.8.1/chaoslib/types.py` & `chaostoolkit-lib-1.9.0/chaoslib/types.py`

 * *Files identical despite different names*

