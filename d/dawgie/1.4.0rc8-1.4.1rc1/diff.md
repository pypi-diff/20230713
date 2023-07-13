# Comparing `tmp/dawgie-1.4.0rc8.tar.gz` & `tmp/dawgie-1.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.0rc8.tar", last modified: Mon Dec 19 14:44:38 2022, max compression
+gzip compressed data, was "dawgie-1.4.1rc1.tar", last modified: Thu Jul 13 00:49:53 2023, max compression
```

## Comparing `dawgie-1.4.0rc8.tar` & `dawgie-1.4.1rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2022-12-19 14:44:38.622273 dawgie-1.4.0rc8/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2022-12-19 14:44:17.000000 dawgie-1.4.0rc8/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9503 2022-12-19 14:44:38.622273 dawgie-1.4.0rc8/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8904 2022-12-19 14:44:17.000000 dawgie-1.4.0rc8/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2022-12-19 14:44:38.622273 dawgie-1.4.0rc8/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9503 2022-12-19 14:44:38.000000 dawgie-1.4.0rc8/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6061 2022-12-19 14:44:38.000000 dawgie-1.4.0rc8/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2022-12-19 14:44:38.000000 dawgie-1.4.0rc8/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      255 2022-12-19 14:44:38.000000 dawgie-1.4.0rc8/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2022-12-19 14:44:38.000000 dawgie-1.4.0rc8/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2022-12-19 14:44:38.622273 dawgie-1.4.0rc8/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6321 2022-12-19 04:36:38.000000 dawgie-1.4.0rc8/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6015 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 00:49:53.000000 dawgie-1.4.1rc1/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 00:49:53.413623 dawgie-1.4.1rc1/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6321 2023-06-28 21:20:21.000000 dawgie-1.4.1rc1/setup.py
```

### Comparing `dawgie-1.4.0rc8/LICENSE` & `dawgie-1.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.0rc8/PKG-INFO` & `dawgie-1.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.0rc8
+Version: 1.4.1rc1
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -81,21 +80,21 @@
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>THe username:password for the database named with DAWGIE_DB_NAME.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the POSTGRESQL server. When DAWGIE_DB_IMPL is 'post', this value defaults to 5432 because POSTGRESQL is independent of DAWGIE.</dd>
 </dl>
 
-##### Shelf
+##### Shelve
 
 <dl>
   <dt>DAWGIE_DB_HOST --context-db-host</dt>
   <dd>The IP hostname of the machine running DAWGIE.</dd>
   <dt>DAWGIE_DB_IMPL --context-db-impl</dt>
-  <dd>Must be 'shelf'</dd>
+  <dd>Must be 'shelve'</dd>
   <dt>DAWGIE_DB_NAME --context-db-name</dt>
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>The directory path on DAWGIE_DB_HOST to write the shelve files.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the DAWGIE DB interface. In is automatically computed from the general port number where DAWGIE is being served (see --port)</dd>
 </dl>
@@ -141,9 +140,7 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
-
-
```

### Comparing `dawgie-1.4.0rc8/README.md` & `dawgie-1.4.1rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,21 @@
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>THe username:password for the database named with DAWGIE_DB_NAME.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the POSTGRESQL server. When DAWGIE_DB_IMPL is 'post', this value defaults to 5432 because POSTGRESQL is independent of DAWGIE.</dd>
 </dl>
 
-##### Shelf
+##### Shelve
 
 <dl>
   <dt>DAWGIE_DB_HOST --context-db-host</dt>
   <dd>The IP hostname of the machine running DAWGIE.</dd>
   <dt>DAWGIE_DB_IMPL --context-db-impl</dt>
-  <dd>Must be 'shelf'</dd>
+  <dd>Must be 'shelve'</dd>
   <dt>DAWGIE_DB_NAME --context-db-name</dt>
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>The directory path on DAWGIE_DB_HOST to write the shelve files.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the DAWGIE DB interface. In is automatically computed from the general port number where DAWGIE is being served (see --port)</dd>
 </dl>
```

### Comparing `dawgie-1.4.0rc8/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc1/dawgie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.0rc8
+Version: 1.4.1rc1
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -81,21 +80,21 @@
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>THe username:password for the database named with DAWGIE_DB_NAME.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the POSTGRESQL server. When DAWGIE_DB_IMPL is 'post', this value defaults to 5432 because POSTGRESQL is independent of DAWGIE.</dd>
 </dl>
 
-##### Shelf
+##### Shelve
 
 <dl>
   <dt>DAWGIE_DB_HOST --context-db-host</dt>
   <dd>The IP hostname of the machine running DAWGIE.</dd>
   <dt>DAWGIE_DB_IMPL --context-db-impl</dt>
-  <dd>Must be 'shelf'</dd>
+  <dd>Must be 'shelve'</dd>
   <dt>DAWGIE_DB_NAME --context-db-name</dt>
   <dd>The name of the database to use.</dd>
   <dt>DAWGIE_DB_PATH --context-db-path</dt>
   <dd>The directory path on DAWGIE_DB_HOST to write the shelve files.</dd>
   <dt>DAWGIE_DB_PORT  --context-db-port</dt>
   <dd>The IP port number of the DAWGIE DB interface. In is automatically computed from the general port number where DAWGIE is being served (see --port)</dd>
 </dl>
@@ -141,9 +140,7 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
-
-
```

### Comparing `dawgie-1.4.0rc8/dawgie.egg-info/SOURCES.txt` & `dawgie-1.4.1rc1/dawgie.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,109 @@
 LICENSE
 README.md
 setup.py
 ../LICENSE.txt
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/context.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/security.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/util.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/lockview.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/post.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/shelf.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/test.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/testdata.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/dbsinfo.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/extract.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/inter.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/list.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/post2shelve.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/purge.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/sandbox.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/util.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/tools/worm.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/util/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/db/util/aspect.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/de/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/de/html.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/__main__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/app.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/requirements.txt
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/submit.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/svrender.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/images/loading.gif
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/algorithms_table.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/application.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/db.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/schedule.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/tasks_table.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/javascripts/welcome.js
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/about/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/algorithms/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/command/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/database/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/database/primary_table/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/database/targets/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/database/tasks/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/database/versions/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/exoplanet_systems/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/logs/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/pipelines/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/schedule/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/search/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/pages/tasks/index.html
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/fe/stylesheets/application.css
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/__main__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/dag.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/farm.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/jobinfo.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/message.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/promotion.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/resources.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/scan.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/schedule.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/state.dot
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/state.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/util.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/version.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/logger/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/logger/fe.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/worker/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/worker/__main__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/worker/aws.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/pl/worker/cluster.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/__init__.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/compliant.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/dag.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/detach.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/logfile.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/resources.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/submit.py
-/tmp/tmp.k3dtsmQMpq/Python/dawgie/tools/trace.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/context.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/security.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/util.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/lockview.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/post.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/test.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/testdata.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/dbsinfo.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/extract.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/inter.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/list.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/post2shelve.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/purge.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/sandbox.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/util.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/tools/worm.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/util/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/db/util/aspect.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/de/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/de/html.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/__main__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/app.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/requirements.txt
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/submit.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/svrender.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.eot
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.svg
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.ttf
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-300.woff2
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.eot
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.svg
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.ttf
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-700.woff2
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.eot
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.svg
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.ttf
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/open-sans-v13-latin-regular.woff2
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.eot
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.svg
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.ttf
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/fonts/bootstrap/glyphicons-halflings-regular.woff2
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/images/loading.gif
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/algorithms_table.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/application.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/db.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/schedule.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/tasks_table.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/javascripts/welcome.js
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/about/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/algorithms/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/command/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/primary_table/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/targets/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/tasks/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/database/versions/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/exoplanet_systems/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/logs/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/pipelines/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/schedule/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/search/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/pages/tasks/index.html
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/fe/stylesheets/application.css
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/__main__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/dag.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/farm.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/jobinfo.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/message.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/promotion.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/resources.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/scan.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/schedule.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/state.dot
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/state.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/util.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/version.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/logger/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/logger/fe.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/__main__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/aws.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/pl/worker/cluster.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/__init__.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/compliant.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/dag.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/detach.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/logfile.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/resources.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/submit.py
+/tmp/tmp.aZ0zPmgs1d/Python/dawgie/tools/trace.py
 dawgie.egg-info/PKG-INFO
 dawgie.egg-info/SOURCES.txt
 dawgie.egg-info/dependency_links.txt
 dawgie.egg-info/requires.txt
 dawgie.egg-info/top_level.txt
```

### Comparing `dawgie-1.4.0rc8/setup.py` & `dawgie-1.4.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python3
 '''
 
 COPYRIGHT:
-Copyright (c) 2015-2022, California Institute of Technology ("Caltech").
+Copyright (c) 2015-2023, California Institute of Technology ("Caltech").
 U.S. Government sponsorship acknowledged.
 
 All rights reserved.
 
 LICENSE:
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

