# Comparing `tmp/Navix-0.3.6.tar.gz` & `tmp/Navix-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.3.6.tar", last modified: Thu Jul 13 08:33:06 2023, max compression
+gzip compressed data, was "Navix-0.3.7.tar", last modified: Thu Jul 13 10:30:55 2023, max compression
```

## Comparing `Navix-0.3.6.tar` & `Navix-0.3.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-13 08:32:52.000000 Navix-0.3.6/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 08:32:52.000000 Navix-0.3.6/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 08:32:52.000000 Navix-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 08:32:52.000000 Navix-0.3.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 08:32:52.000000 Navix-0.3.6/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-13 08:32:52.000000 Navix-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 08:32:52.000000 Navix-0.3.6/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 08:33:06.000000 Navix-0.3.6/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 08:33:06.468160 Navix-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-13 08:32:52.000000 Navix-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.464160 Navix-0.3.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/performance.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 08:32:52.000000 Navix-0.3.6/docs/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/navix/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 08:32:52.000000 Navix-0.3.6/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 08:32:52.000000 Navix-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-13 08:32:52.000000 Navix-0.3.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-13 08:32:52.000000 Navix-0.3.6/scripts/release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:33:06.468160 Navix-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:33:06.468160 Navix-0.3.6/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/minigrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/minigrid_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations_keydoor_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/observations_room_report.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/performance/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 08:32:52.000000 Navix-0.3.6/tests/test_terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.380015 Navix-0.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.380015 Navix-0.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-13 10:30:34.000000 Navix-0.3.7/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-13 10:30:34.000000 Navix-0.3.7/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-13 10:30:34.000000 Navix-0.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 10:30:34.000000 Navix-0.3.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 10:30:34.000000 Navix-0.3.7/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-13 10:30:34.000000 Navix-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:30:34.000000 Navix-0.3.7/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 10:30:55.000000 Navix-0.3.7/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-13 10:30:55.388015 Navix-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-13 10:30:34.000000 Navix-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/performance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-13 10:30:34.000000 Navix-0.3.7/docs/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 10:30:34.000000 Navix-0.3.7/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 10:30:34.000000 Navix-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-13 10:30:34.000000 Navix-0.3.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.384015 Navix-0.3.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      808 2023-07-13 10:30:34.000000 Navix-0.3.7/scripts/release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:30:55.388015 Navix-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:30:55.388015 Navix-0.3.7/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/minigrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/minigrid_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations_keydoor_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/observations_room_report.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/performance/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-13 10:30:34.000000 Navix-0.3.7/tests/test_terminations.py
```

### Comparing `Navix-0.3.6/.github/workflows/CD.yml` & `Navix-0.3.7/.github/workflows/CD.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 name: CD
 
-on: workflow_dispatch
+on:
+  workflow_dispatch:
+  push:
+    branches:
+      - "main"
 
 jobs:
   release:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
```

### Comparing `Navix-0.3.6/.github/workflows/CI.yml` & `Navix-0.3.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/.gitignore` & `Navix-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/COPYRIGHT` & `Navix-0.3.7/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/LICENSE` & `Navix-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/Navix.egg-info/PKG-INFO` & `Navix-0.3.7/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.6
+Version: 0.3.7
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.3.6/Navix.egg-info/SOURCES.txt` & `Navix-0.3.7/Navix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/PKG-INFO` & `Navix-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.3.6
+Version: 0.3.7
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.3.6/README.md` & `Navix-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/docs/design_notes.md` & `Navix-0.3.7/docs/design_notes.md`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/docs/performance.ipynb` & `Navix-0.3.7/docs/performance.ipynb`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/docs/performance.py` & `Navix-0.3.7/docs/performance.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/__init__.py` & `Navix-0.3.7/navix/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/_version.py` & `Navix-0.3.7/navix/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `Navix-0.3.6/navix/actions.py` & `Navix-0.3.7/navix/actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/components.py` & `Navix-0.3.7/navix/components.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/entities.py` & `Navix-0.3.7/navix/entities.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/environments/__init__.py` & `Navix-0.3.7/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/environments/environment.py` & `Navix-0.3.7/navix/environments/environment.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/environments/keydoor.py` & `Navix-0.3.7/navix/environments/keydoor.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/environments/room.py` & `Navix-0.3.7/navix/environments/room.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/graphics.py` & `Navix-0.3.7/navix/graphics.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/grid.py` & `Navix-0.3.7/navix/grid.py`

 * *Files 15% similar despite different names*

```diff
@@ -151,57 +151,41 @@
     wall_at = jax.random.randint(key, (), 2, width - 2)
     grid = grid.at[1:-1, wall_at].set(-1)
     return grid, wall_at
 
 
 def crop(grid: Array, origin: Array, direction: Array, radius: int) -> Array:
     input_shape = grid.shape
-    max_dim = max(input_shape)
 
-    # pad to square and ensure non out of bounds
-    padding = []
-    for d in input_shape[:2]:
-        pad = max_dim - d
-        pad, rem = divmod(pad, 2)
-        pad = (pad + rem + radius, pad + radius)
-        padding.append(pad)
+    # pad with radius
+    padding = [(radius, radius), (radius, radius)]
     for _ in range(len(input_shape) - 2):
         padding.append((0, 0))
 
     padded = jnp.pad(grid, padding, constant_values=0)
-    origin = origin + jnp.asarray((padding[0][0] - radius, padding[1][0] - radius))
-    height, width = (padded.shape[0] - radius * 2, padded.shape[1] - radius * 2)
 
-    # rotate
-    rotated, centre = jax.lax.switch(
+    # translate the grid such that the agent is `radius` away from the top and left edges
+    translated = jnp.roll(padded, -jnp.asarray(origin), axis=(0, 1))
+
+    # crop such that the agent is in the centre of the grid
+    cropped = translated[: 2 * radius + 1, : 2 * radius + 1]
+
+    # rotate such that the agent is facing north
+    rotated = jax.lax.switch(
         direction,
         (
-            lambda x: (
-                jnp.rot90(x, 1),
-                (width - 1 - origin[1], origin[0]),
-            ),  # 0 = transpose, 1 = flip
-            lambda x: (
-                jnp.rot90(x, 2),
-                (height - 1 - origin[0], width - 1 - origin[1]),
-            ),  # 0 = flip, 1 = flip
-            lambda x: (
-                jnp.rot90(x, 3),
-                (origin[1], height - 1 - origin[0]),
-            ),  # 0 = flip, 1 = transpose
-            lambda x: (x, (origin[0], origin[1])),
+            lambda x: jnp.rot90(x, 1),  # 0 = transpose, 1 = flip
+            lambda x: jnp.rot90(x, 2),  # 0 = flip, 1 = flip
+            lambda x: jnp.rot90(x, 3),  # 0 = flip, 1 = transpose
+            lambda x: x,
         ),
-        padded,
+        cropped,
     )
 
-    # translate
-    translated = jnp.roll(rotated, -jnp.asarray(centre), axis=(0, 1))
-
-    # crop
-    cropped = translated[: radius + 1, : 2 * radius + 1]
-
+    cropped = rotated[:radius + 1]
     return jnp.asarray(cropped, dtype=grid.dtype)
 
 
 def view_cone(transparency_map: Array, origin: Array, radius: int) -> Array:
     # transparency_map is a boolean map of transparent (1) and opaque (0) tiles
 
     def fin_diff(array, _):
```

### Comparing `Navix-0.3.6/navix/observations.py` & `Navix-0.3.7/navix/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/tasks.py` & `Navix-0.3.7/navix/tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/navix/terminations.py` & `Navix-0.3.7/navix/terminations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/pyproject.toml` & `Navix-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/scripts/release.sh` & `Navix-0.3.7/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/grid.py` & `Navix-0.3.7/tests/performance/grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/minigrid.py` & `Navix-0.3.7/tests/performance/minigrid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/observations.py` & `Navix-0.3.7/tests/performance/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/observations_keydoor_report.txt` & `Navix-0.3.7/tests/performance/observations_keydoor_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/observations_room_report.txt` & `Navix-0.3.7/tests/performance/observations_room_report.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/performance/profiling.py` & `Navix-0.3.7/tests/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_actions.py` & `Navix-0.3.7/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_entities.py` & `Navix-0.3.7/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_environments.py` & `Navix-0.3.7/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_grid.py` & `Navix-0.3.7/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_observations.py` & `Navix-0.3.7/tests/test_observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_tasks.py` & `Navix-0.3.7/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.3.6/tests/test_terminations.py` & `Navix-0.3.7/tests/test_terminations.py`

 * *Files identical despite different names*

