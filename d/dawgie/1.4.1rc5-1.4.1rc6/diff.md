# Comparing `tmp/dawgie-1.4.1rc5.tar.gz` & `tmp/dawgie-1.4.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.1rc5.tar", last modified: Thu Jul 13 19:16:17 2023, max compression
+gzip compressed data, was "dawgie-1.4.1rc6.tar", last modified: Thu Jul 13 20:59:54 2023, max compression
```

## Comparing `dawgie-1.4.1rc5.tar` & `dawgie-1.4.1rc6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 19:16:17.089563 dawgie-1.4.1rc5/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 19:16:01.000000 dawgie-1.4.1rc5/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 19:16:17.089563 dawgie-1.4.1rc5/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 19:16:01.000000 dawgie-1.4.1rc5/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 19:16:17.085563 dawgie-1.4.1rc5/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 19:16:17.000000 dawgie-1.4.1rc5/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 19:16:17.000000 dawgie-1.4.1rc5/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 19:16:17.000000 dawgie-1.4.1rc5/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 19:16:17.000000 dawgie-1.4.1rc5/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 19:16:17.000000 dawgie-1.4.1rc5/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 19:16:17.089563 dawgie-1.4.1rc5/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 19:06:38.000000 dawgie-1.4.1rc5/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 20:59:36.000000 dawgie-1.4.1rc6/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 20:59:36.000000 dawgie-1.4.1rc6/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 20:40:38.000000 dawgie-1.4.1rc6/setup.py
```

### Comparing `dawgie-1.4.1rc5/LICENSE` & `dawgie-1.4.1rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc5/PKG-INFO` & `dawgie-1.4.1rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc5
+Version: 1.4.1rc6
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Platform: UNKNOWN
```

### Comparing `dawgie-1.4.1rc5/README.md` & `dawgie-1.4.1rc6/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc5/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc6/dawgie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc5
+Version: 1.4.1rc6
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
 Platform: UNKNOWN
```

### Comparing `dawgie-1.4.1rc5/dawgie.egg-info/SOURCES.txt` & `dawgie-1.4.1rc6/dawgie.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,116 @@
 LICENSE
 README.md
 setup.py
 ../LICENSE.txt
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/context.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/security.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/util.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/lockview.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/post.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/test.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/testdata.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/comms.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/enums.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/model.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/state.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/shelve/util.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/dbsinfo.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/extract.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/inter.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/list.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/post2shelve.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/purge.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/sandbox.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/util.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/tools/worm.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/util/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/db/util/aspect.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/de/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/de/html.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/__main__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/app.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/requirements.txt
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/submit.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/svrender.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/images/loading.gif
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/algorithms_table.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/application.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/db.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/schedule.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/tasks_table.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/javascripts/welcome.js
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/about/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/algorithms/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/command/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/database/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/database/primary_table/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/database/targets/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/database/tasks/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/database/versions/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/exoplanet_systems/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/logs/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/pipelines/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/schedule/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/search/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/pages/tasks/index.html
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/fe/stylesheets/application.css
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/__main__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/dag.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/farm.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/jobinfo.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/message.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/promotion.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/resources.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/scan.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/schedule.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/snapshot.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/state.dot
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/state.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/util.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/version.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/logger/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/logger/fe.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/worker/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/worker/__main__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/worker/aws.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/pl/worker/cluster.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/__init__.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/compliant.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/dag.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/detach.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/logfile.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/resources.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/submit.py
-/tmp/tmp.IxG6YbmuOO/Python/dawgie/tools/trace.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/context.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/security.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/util.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/lockview.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/post.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/test.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/testdata.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/comms.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/enums.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/model.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/state.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/shelve/util.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/dbsinfo.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/extract.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/inter.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/list.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/post2shelve.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/purge.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/sandbox.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/util.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/tools/worm.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/util/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/db/util/aspect.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/de/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/de/html.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/__main__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/app.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/requirements.txt
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/submit.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/svrender.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/images/loading.gif
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/algorithms_table.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/application.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/db.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/schedule.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/tasks_table.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/javascripts/welcome.js
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/about/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/algorithms/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/command/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/database/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/database/primary_table/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/database/targets/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/database/tasks/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/database/versions/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/exoplanet_systems/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/logs/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/pipelines/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/schedule/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/search/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/pages/tasks/index.html
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/fe/stylesheets/application.css
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/__main__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/dag.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/farm.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/jobinfo.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/message.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/promotion.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/resources.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/scan.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/schedule.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/snapshot.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/state.dot
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/state.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/util.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/version.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/logger/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/logger/fe.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/worker/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/worker/__main__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/worker/aws.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/pl/worker/cluster.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/__init__.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/compliant.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/dag.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/detach.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/logfile.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/resources.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/submit.py
+/tmp/tmp.YjhQaWe0Ae/Python/dawgie/tools/trace.py
 dawgie.egg-info/PKG-INFO
 dawgie.egg-info/SOURCES.txt
 dawgie.egg-info/dependency_links.txt
 dawgie.egg-info/requires.txt
 dawgie.egg-info/top_level.txt
```

### Comparing `dawgie-1.4.1rc5/setup.py` & `dawgie-1.4.1rc6/setup.py`

 * *Files identical despite different names*

