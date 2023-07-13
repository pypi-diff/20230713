# Comparing `tmp/dawgie-1.4.1rc1.tar.gz` & `tmp/dawgie-1.4.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.1rc1.tar", last modified: Thu Jul 13 00:49:53 2023, max compression
+gzip compressed data, was "dawgie-1.4.1rc2.tar", last modified: Thu Jul 13 15:26:01 2023, max compression
```

## Comparing `dawgie-1.4.1rc1.tar` & `dawgie-1.4.1rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6015 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6321 2023-06-28 21:20:21.000000 dawgie-1.4.1rc1/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 15:25:38.000000 dawgie-1.4.1rc2/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 15:25:38.000000 dawgie-1.4.1rc2/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 15:26:01.000000 dawgie-1.4.1rc2/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 15:26:01.282250 dawgie-1.4.1rc2/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 00:36:01.000000 dawgie-1.4.1rc2/setup.py
```

### Comparing `dawgie-1.4.1rc1/LICENSE` & `dawgie-1.4.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc1/PKG-INFO` & `dawgie-1.4.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc1
+Version: 1.4.1rc2
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -140,7 +141,9 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
+
+
```

### Comparing `dawgie-1.4.1rc1/README.md` & `dawgie-1.4.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc1/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc2/dawgie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc1
+Version: 1.4.1rc2
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -140,7 +141,9 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
+
+
```

### Comparing `dawgie-1.4.1rc1/dawgie.egg-info/SOURCES.txt` & `dawgie-1.4.1rc2/dawgie.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,116 @@
 LICENSE
 README.md
 setup.py
 ../LICENSE.txt
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/context.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/security.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/util.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/lockview.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/post.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/test.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/testdata.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/dbsinfo.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/extract.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/inter.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/list.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/post2shelve.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/purge.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/sandbox.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/util.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/worm.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/util/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/util/aspect.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/de/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/de/html.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/__main__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/app.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/requirements.txt
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/submit.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/svrender.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/images/loading.gif
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/algorithms_table.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/application.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/db.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/schedule.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/tasks_table.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/welcome.js
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/about/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/algorithms/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/command/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/primary_table/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/targets/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/tasks/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/versions/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/exoplanet_systems/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/logs/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/pipelines/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/schedule/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/search/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/tasks/index.html
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/stylesheets/application.css
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/__main__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/dag.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/farm.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/jobinfo.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/message.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/promotion.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/resources.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/scan.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/schedule.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/state.dot
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/state.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/util.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/version.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/logger/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/logger/fe.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/__main__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/aws.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/cluster.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/__init__.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/compliant.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/dag.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/detach.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/logfile.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/resources.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/submit.py
-/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/trace.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/context.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/security.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/util.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/lockview.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/post.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/test.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/testdata.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/comms.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/enums.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/model.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/state.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/shelve/util.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/dbsinfo.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/extract.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/inter.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/list.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/post2shelve.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/purge.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/sandbox.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/util.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/tools/worm.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/util/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/db/util/aspect.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/de/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/de/html.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/__main__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/app.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/requirements.txt
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/submit.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/svrender.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/images/loading.gif
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/algorithms_table.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/application.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/db.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/schedule.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/tasks_table.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/javascripts/welcome.js
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/about/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/algorithms/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/command/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/database/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/database/primary_table/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/database/targets/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/database/tasks/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/database/versions/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/exoplanet_systems/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/logs/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/pipelines/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/schedule/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/search/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/pages/tasks/index.html
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/fe/stylesheets/application.css
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/__main__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/dag.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/farm.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/jobinfo.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/message.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/promotion.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/resources.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/scan.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/schedule.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/snapshot.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/state.dot
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/state.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/util.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/version.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/logger/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/logger/fe.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/worker/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/worker/__main__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/worker/aws.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/pl/worker/cluster.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/__init__.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/compliant.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/dag.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/detach.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/logfile.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/resources.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/submit.py
+/tmp/tmp.rhIaMUwMMI/Python/dawgie/tools/trace.py
 dawgie.egg-info/PKG-INFO
 dawgie.egg-info/SOURCES.txt
 dawgie.egg-info/dependency_links.txt
 dawgie.egg-info/requires.txt
 dawgie.egg-info/top_level.txt
```

### Comparing `dawgie-1.4.1rc1/setup.py` & `dawgie-1.4.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         f.write ('\n')
         pass
     pass
 setuptools.setup(name='dawgie',
                  version=version,
                  packages=['dawgie',
                            'dawgie.db',
+                           'dawgie.db.shelve',
                            'dawgie.db.tools',
                            'dawgie.db.util',
                            'dawgie.de',
                            'dawgie.fe',
                            'dawgie.pl',
                            'dawgie.pl.logger',
                            'dawgie.pl.worker',
```

