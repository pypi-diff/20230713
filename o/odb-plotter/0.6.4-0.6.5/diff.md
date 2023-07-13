# Comparing `tmp/odb-plotter-0.6.4.tar.gz` & `tmp/odb-plotter-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.4.tar", last modified: Thu Jul 13 17:03:45 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.5.tar", last modified: Thu Jul 13 17:33:50 2023, max compression
```

## Comparing `odb-plotter-0.6.4.tar` & `odb-plotter-0.6.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.4/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     4035 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     2069 2023-07-13 17:01:36.000000 odb-plotter-0.6.4/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.4/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.184566 odb-plotter-0.6.4/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.184566 odb-plotter-0.6.4/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     4035 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 17:03:45.000000 odb-plotter-0.6.4/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 17:03:18.000000 odb-plotter-0.6.4/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.4/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.4/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.4/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    37294 2023-06-22 22:29:35.000000 odb-plotter-0.6.4/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.4/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:03:45.187899 odb-plotter-0.6.4/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5382 2023-07-13 17:01:36.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.4/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.780971 odb-plotter-0.6.5/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.5/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     4094 2023-07-13 17:33:50.780971 odb-plotter-0.6.5/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     2128 2023-07-13 17:33:44.000000 odb-plotter-0.6.5/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.5/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 17:33:50.780971 odb-plotter-0.6.5/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.777638 odb-plotter-0.6.5/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.777638 odb-plotter-0.6.5/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4094 2023-07-13 17:33:50.000000 odb-plotter-0.6.5/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 17:33:50.000000 odb-plotter-0.6.5/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 17:33:50.000000 odb-plotter-0.6.5/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 17:33:50.000000 odb-plotter-0.6.5/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 17:33:50.000000 odb-plotter-0.6.5/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.777638 odb-plotter-0.6.5/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 17:33:44.000000 odb-plotter-0.6.5/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.5/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.5/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.777638 odb-plotter-0.6.5/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.5/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.5/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    37294 2023-06-22 22:29:35.000000 odb-plotter-0.6.5/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.5/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:33:50.780971 odb-plotter-0.6.5/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)    10579 2023-07-13 17:33:44.000000 odb-plotter-0.6.5/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5522 2023-07-13 17:33:44.000000 odb-plotter-0.6.5/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3196 2023-07-13 17:33:44.000000 odb-plotter-0.6.5/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.5/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.5/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.5/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.5/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.4/LICENSE` & `odb-plotter-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/PKG-INFO` & `odb-plotter-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -75,12 +75,13 @@
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
+    * 0.6.5: Fixing Python2 Error Reporting in more places
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.4/README.md` & `odb-plotter-0.6.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,12 +38,13 @@
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
+    * 0.6.5: Fixing Python2 Error Reporting in more places
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.4/pyproject.toml` & `odb-plotter-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.5/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -75,12 +75,13 @@
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
+    * 0.6.5: Fixing Python2 Error Reporting in more places
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.4/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.5/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/cli.py` & `odb-plotter-0.6.5/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/data/config.toml` & `odb-plotter-0.6.5/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/odb.py` & `odb-plotter-0.6.5/src/odbp/odb.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.5/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.5/src/odbp/py2_scripts/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 compressed numpy arrays. This is used to translate .odb data from the Python 2
 environment to a modern Python 3 environment
 
 Originally authored by CMML member CJ Nguyen, based before on extraction
 script written by CMML members Will Furr and Matt Dantin
 """
 
-
+import sys
 import os
 import pickle
 import numpy as np
 import argparse
 import multiprocessing
 import collections
 from odbAccess import openOdb
@@ -121,14 +121,20 @@
     time_dir = os.path.join(parent_dir, "step_frame_times")
     if not os.path.exists(time_dir):
         os.mkdir(time_dir)
 
     try:
         odb = openOdb(odb_path, readOnly=True)
 
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
+
+    try:
         steps = odb.steps
 
         base_times = [
             (step_key, step_val.totalTime) for step_key, step_val in steps.items()
             ]
 
         assembly = odb.rootAssembly
@@ -187,115 +193,143 @@
             read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key)
             read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus)
 
     return parent_dir
 
 
 def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, target_frames, nodeset, temp_key, num_cpus):
-    odb = openOdb(odb_path, readOnly=True)
-    steps = odb.steps
+    try:
+        odb = openOdb(odb_path, readOnly=True)
 
-    curr_step_dir = os.path.join(temps_dir, step_key)
-    if not os.path.exists(curr_step_dir):
-        os.mkdir(curr_step_dir)
-
-    max_frame = max(target_frames)
-
-    max_pad = len(str(max_frame))
-
-    manager = multiprocessing.Manager()
-    frame_times = manager.list()
-    if len(steps[step_key].frames) > 0:
-        idx_list = [i for i in range(len(steps[step_key].frames))]
-        idx_list_len = len(idx_list)
-        # TODO: what if the length isn't divisible by the number of processors (is it now?)
-        final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
-        odb.close()
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
 
-        temp_procs = list()
-        for idx_list in final_idx_list:
-            p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key))
-            p.start()
-            temp_procs.append(p)
-
-        for p in temp_procs:
-            p.join()
-
-        np.savez_compressed(
-            "{}.npz".format(
-                os.path.join(
-                    time_dir,
-                    step_key
-                    )
-                ),
-            np.sort(
-                np.array(
-                    frame_times
+    try:
+        steps = odb.steps
+
+        curr_step_dir = os.path.join(temps_dir, step_key)
+        if not os.path.exists(curr_step_dir):
+            os.mkdir(curr_step_dir)
+
+        max_frame = max(target_frames)
+
+        max_pad = len(str(max_frame))
+
+        manager = multiprocessing.Manager()
+        frame_times = manager.list()
+        if len(steps[step_key].frames) > 0:
+            idx_list = [i for i in range(len(steps[step_key].frames))]
+            idx_list_len = len(idx_list)
+            # TODO: what if the length isn't divisible by the number of processors (is it now?)
+            final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
+
+            temp_procs = list()
+            for idx_list in final_idx_list:
+                p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key))
+                p.start()
+                temp_procs.append(p)
+
+            for p in temp_procs:
+                p.join()
+
+            np.savez_compressed(
+                "{}.npz".format(
+                    os.path.join(
+                        time_dir,
+                        step_key
+                        )
+                    ),
+                np.sort(
+                    np.array(
+                        frame_times
+                        )
                     )
                 )
-            )
+
+    finally:
+        odb.close()
 
 
 def read_single_frame_temp(odb_path, idx_list, max_pad, target_frames, step_key, curr_step_dir, frame_times, base_time, nodeset, temp_key):
 
-    odb = openOdb(odb_path, readOnly=True)
-    steps = odb.steps
-    assembly = odb.rootAssembly
-
-    for idx in idx_list:
-        if idx not in target_frames:
-            continue
-        
-        frame = steps[step_key].frames[idx]
-
-        field = frame.fieldOutputs[temp_key].getSubset(region=assembly.nodeSets[nodeset])
-        frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
-        node_temps = list()
-        for item in field.values:
-            temp = item.data
-            node_temps.append(temp)
-
-        num = str(idx + 1).zfill(max_pad)
-        np.savez_compressed(
-                os.path.join(
-                    curr_step_dir,
-                    "frame_{}".format(num)
-                    ),
-                np.array(node_temps)
-                )
+    try:
+        odb = openOdb(odb_path, readOnly=True)
+
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
 
-    odb.close()
+    try:
+        steps = odb.steps
+        assembly = odb.rootAssembly
+
+        for idx in idx_list:
+            if idx not in target_frames:
+                continue
+            
+            frame = steps[step_key].frames[idx]
+
+            field = frame.fieldOutputs[temp_key].getSubset(region=assembly.nodeSets[nodeset])
+            frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
+            node_temps = list()
+            for item in field.values:
+                temp = item.data
+                node_temps.append(temp)
+
+            num = str(idx + 1).zfill(max_pad)
+            np.savez_compressed(
+                    os.path.join(
+                        curr_step_dir,
+                        "frame_{}".format(num)
+                        ),
+                    np.array(node_temps)
+                    )
+
+    finally:
+        odb.close()
 
 
 def read_nodeset_coords(odb_path, nodeset, coord_file, step_key, coord_key):
 
     # Only extract coordinates from the first given nodeset/step
     if not os.path.exists(coord_file):
 
-        odb = openOdb(odb_path, readOnly=True)
-        assembly = odb.rootAssembly
-        steps = odb.steps
+        try:
+            odb = openOdb(odb_path, readOnly=True)
 
-        frame = steps[step_key].frames[0]
+        except Exception as e:
+            print("Abaqus Error:")
+            print(e)
+            sys.exit(1)
 
         try:
-            coords = frame.fieldOutputs[coord_key].getSubset(region=assembly.nodeSets[nodeset])
+            assembly = odb.rootAssembly
+            steps = odb.steps
 
-            results_list = list()
-            for item in coords.values:
-                node = item.nodeLabel
-                coord = item.data
-                xyz = [node]
-                for axis in coord:
-                    xyz.append(axis)
-                results_list.append(xyz)
+            frame = steps[step_key].frames[0]
 
-            np.savez_compressed(coord_file, np.array(results_list))
+            try:
+                coords = frame.fieldOutputs[coord_key].getSubset(region=assembly.nodeSets[nodeset])
 
-        except KeyError:
-            pass
+                results_list = list()
+                for item in coords.values:
+                    node = item.nodeLabel
+                    coord = item.data
+                    xyz = [node]
+                    for axis in coord:
+                        xyz.append(axis)
+                    results_list.append(xyz)
 
-        odb.close()
+                np.savez_compressed(coord_file, np.array(results_list))
+
+            except KeyError:
+                pass
+
+        finally:
+            odb.close()
 
     
 if __name__ == "__main__":
     main()
```

### Comparing `odb-plotter-0.6.4/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.5/src/odbp/py2_scripts/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 extracts as one 2D array to be split in the corresponding 
 Python 3 script: 
 
 """
 """
 Updated by Clark Hensley for CMML
 """
+
+import sys
 import pickle
 import argparse
 import collections
 import numpy as np
 from odbAccess import openOdb
 
 
@@ -63,14 +65,21 @@
     else:
         user_steps = None
 
     temp_key = str(input_dict.get("temp_key", "NT11"))
 
     try:
         odb = openOdb(odb_path, readOnly=True)
+
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
+
+    try:
         steps = odb.steps
         assembly = odb.rootAssembly
 
         target_frames = set()
         if user_steps is not None:
             for step in user_steps:
                 step_data = steps[step]
@@ -111,28 +120,31 @@
                 target_nodesets.add(nodeset)
 
         target_nodesets = sorted(list(target_nodesets))
 
         if len(target_nodesets) == 0:
             target_nodesets = list(assembly.nodeSets.keys())
 
-    except Exception as e:
-        print("Error found in Abaqus")
-        print(e)
-
     finally:
         odb.close()
 
     extract(odb_path, save_path, target_nodesets, target_frames, temp_key)
 
 
 def extract(odb_path, save_path, target_nodesets, target_frames, temp_key):
 
     try:
         odb = openOdb(odb_path, readOnly=True)
+
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
+
+    try:
         steps = odb.steps
         assembly = odb.rootAssembly
 
         final_record = list()
         for step in steps.keys():
             step_start_time = steps[step].totalTime
             for frame in steps[step].frames:
```

### Comparing `odb-plotter-0.6.4/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.5/src/odbp/py2_scripts/state_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 compressed numpy arrays. This is used to translate .odb data from the Python 2
 environment to a modern Python 3 environment
 
 Originally authored by CMML member CJ Nguyen, based before on extraction
 script written by CMML members Will Furr and Matt Dantin
 """
 
+import sys
 import argparse
 import pickle
 from odbAccess import openOdb
 
 def main():
     input_args = "input args"
     parser = argparse.ArgumentParser()
@@ -33,14 +34,21 @@
         result_file.close()
 
 def collect_state(odb_path):
     result = dict()
     try:
         odb = openOdb(odb_path, readOnly=True)
 
+    except Exception as e:
+        print("Abaqus Error:")
+        print(e)
+        sys.exit(1)
+
+    try:
+
         # What are our targets:
         # Frames
         # Steps --> Frames
         # Nodesets
         # Parts --> Nodesets
         # # Nodes --> Nodesets
         steps = odb.steps
```

### Comparing `odb-plotter-0.6.4/src/odbp/reader.py` & `odb-plotter-0.6.5/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/state.py` & `odb-plotter-0.6.5/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/util.py` & `odb-plotter-0.6.5/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.4/src/odbp/writer.py` & `odb-plotter-0.6.5/src/odbp/writer.py`

 * *Files identical despite different names*

