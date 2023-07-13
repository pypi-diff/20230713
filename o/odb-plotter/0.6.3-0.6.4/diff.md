# Comparing `tmp/odb-plotter-0.6.3.tar.gz` & `tmp/odb-plotter-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.3.tar", last modified: Thu Jun 22 22:32:00 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.4.tar", last modified: Thu Jul 13 17:03:45 2023, max compression
```

## Comparing `odb-plotter-0.6.3.tar` & `odb-plotter-0.6.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.3/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3991 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     2025 2023-06-22 22:31:54.000000 odb-plotter-0.6.3/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.3/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.644376 odb-plotter-0.6.3/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3991 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 22:31:54.000000 odb-plotter-0.6.3/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.3/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.3/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.3/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    37294 2023-06-22 22:29:35.000000 odb-plotter-0.6.3/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.3/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.4/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     4035 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     2069 2023-07-13 17:01:36.000000 odb-plotter-0.6.4/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.4/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.184566 odb-plotter-0.6.4/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.184566 odb-plotter-0.6.4/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4035 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 17:03:18.000000 odb-plotter-0.6.4/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.4/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.4/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.4/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    37294 2023-06-22 22:29:35.000000 odb-plotter-0.6.4/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.4/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5382 2023-07-13 17:01:36.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.3/LICENSE` & `odb-plotter-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/PKG-INFO` & `odb-plotter-0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -74,12 +74,13 @@
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
+    * 0.6.4: Fixing Python2 Error Reporting
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.3/README.md` & `odb-plotter-0.6.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,12 +37,13 @@
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
+    * 0.6.4: Fixing Python2 Error Reporting
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.3/pyproject.toml` & `odb-plotter-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.4/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -74,12 +74,13 @@
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
+    * 0.6.4: Fixing Python2 Error Reporting
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.3/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.4/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/cli.py` & `odb-plotter-0.6.4/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/data/config.toml` & `odb-plotter-0.6.4/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/odb.py` & `odb-plotter-0.6.4/src/odbp/odb.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.4/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.4/src/odbp/py2_scripts/converter.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.4/src/odbp/py2_scripts/extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -111,14 +111,18 @@
                 target_nodesets.add(nodeset)
 
         target_nodesets = sorted(list(target_nodesets))
 
         if len(target_nodesets) == 0:
             target_nodesets = list(assembly.nodeSets.keys())
 
+    except Exception as e:
+        print("Error found in Abaqus")
+        print(e)
+
     finally:
         odb.close()
 
     extract(odb_path, save_path, target_nodesets, target_frames, temp_key)
 
 
 def extract(odb_path, save_path, target_nodesets, target_frames, temp_key):
```

### Comparing `odb-plotter-0.6.3/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.4/src/odbp/py2_scripts/state_collector.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/reader.py` & `odb-plotter-0.6.4/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/state.py` & `odb-plotter-0.6.4/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/util.py` & `odb-plotter-0.6.4/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.3/src/odbp/writer.py` & `odb-plotter-0.6.4/src/odbp/writer.py`

 * *Files identical despite different names*

