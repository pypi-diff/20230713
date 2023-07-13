# Comparing `tmp/odb-plotter-0.6.6.tar.gz` & `tmp/odb-plotter-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.6.tar", last modified: Thu Jul 13 17:49:40 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.7.tar", last modified: Thu Jul 13 19:01:02 2023, max compression
```

## Comparing `odb-plotter-0.6.6.tar` & `odb-plotter-0.6.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.6/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     4134 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     2168 2023-07-13 17:49:35.000000 odb-plotter-0.6.6/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.6/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.540992 odb-plotter-0.6.6/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     4134 2023-07-13 17:49:40.000000 odb-plotter-0.6.6/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 17:49:40.000000 odb-plotter-0.6.6/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 17:49:40.000000 odb-plotter-0.6.6/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 17:49:40.000000 odb-plotter-0.6.6/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 17:49:40.000000 odb-plotter-0.6.6/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 17:49:35.000000 odb-plotter-0.6.6/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.6/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.6/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.6/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.6/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    37298 2023-07-13 17:49:35.000000 odb-plotter-0.6.6/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.6/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 17:49:40.544325 odb-plotter-0.6.6/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)    10579 2023-07-13 17:33:44.000000 odb-plotter-0.6.6/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5522 2023-07-13 17:33:44.000000 odb-plotter-0.6.6/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3196 2023-07-13 17:33:44.000000 odb-plotter-0.6.6/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.6/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.6/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.6/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.6/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.7/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     4253 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     2287 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.7/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.424299 odb-plotter-0.6.7/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.424299 odb-plotter-0.6.7/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4253 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-07-13 19:01:02.000000 odb-plotter-0.6.7/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.7/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.7/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.7/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    37876 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.7/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-07-13 19:01:02.427633 odb-plotter-0.6.7/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)    10576 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5522 2023-07-13 17:33:44.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3196 2023-07-13 17:33:44.000000 odb-plotter-0.6.7/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.7/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3909 2023-07-13 19:00:56.000000 odb-plotter-0.6.7/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.6/LICENSE` & `odb-plotter-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/PKG-INFO` & `odb-plotter-0.6.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -77,12 +77,13 @@
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
+    * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.6/README.md` & `odb-plotter-0.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,12 +40,13 @@
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
+    * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.6/pyproject.toml` & `odb-plotter-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.7/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -77,12 +77,13 @@
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
     * 0.6.3: Actually filtering 3D plots.
     * 0.6.4: Fixing Python2 Error Reporting
     * 0.6.5: Fixing Python2 Error Reporting in more places
     * 0.6.6: Fixing conversion problems
+    * 0.6.7: Implementing tools for .odbs with coords in only some steps or tools for frame steps with different sizes
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.6/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.7/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/cli.py` & `odb-plotter-0.6.7/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/data/config.toml` & `odb-plotter-0.6.7/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/odb.py` & `odb-plotter-0.6.7/src/odbp/odb.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import subprocess
 import shutil
 import pathlib
 import pickle
 import multiprocessing
+import sys
 
 import numpy as np
 import pandas as pd
 
 from typing import TextIO, Union, Any, Tuple, List, Dict, Optional, Iterator
 from abc import abstractmethod
 
@@ -842,16 +843,22 @@
         ]
 
         # shell=True is BAD PRACTICE, but abaqus python won't run without it
         subprocess.run(odb_convert_args, shell=True)
 
         result_file: TextIO
         result_dir: pathlib.Path
-        with open(self._convert_result_path, "rb") as result_file:
-            result_dir = pathlib.Path(pickle.load(result_file))
+        
+        try:
+            with open(self._convert_result_path, "rb") as result_file:
+                result_dir = pathlib.Path(pickle.load(result_file))
+
+        except FileNotFoundError:
+            print(f"File {self._convert_result_path} was not found. See previous Python 2 errors")
+            sys.exit(-1)
 
         pathlib.Path.unlink(self._convert_result_path)
 
         convert_npz_to_hdf(hdf_path, result_dir)
 
         if result_dir.exists():
             shutil.rmtree(result_dir)
@@ -924,19 +931,24 @@
             self._extract_result_path
             ]
 
         # shell=True is bad practice, but abaqus python will not run without it.
         subprocess.run(args_list, shell=True)
 
         temp_file: TextIO
-        with open(self._extract_result_path, "rb") as temp_file:
-            # From the Pickle spec, decoding python 2 numpy arrays must use
-            # "latin-1" encoding
-            results: List[Dict[str, float]]
-            results = pickle.load(temp_file, encoding="latin-1")
+        try:
+            with open(self._extract_result_path, "rb") as temp_file:
+                # From the Pickle spec, decoding python 2 numpy arrays must use
+                # "latin-1" encoding
+                results: List[Dict[str, float]]
+                results = pickle.load(temp_file, encoding="latin-1")
+
+        except FileNotFoundError:
+            print(f"File {self._extract_result_path} was not found. See previous Python 2 errors")
+            sys.exit(-1)
 
         results = sorted(results, key=lambda d: d["time"])
 
         results_df_list: List[DataFrameType] = list()
         for result in results:
             time = result.pop("time")
             results_df_list.append(pd.DataFrame.from_dict({time: result}, orient="index"))
@@ -1033,16 +1045,21 @@
             "python",
             self._collect_state_script_path,
             path,
             self._collect_state_result_path
             ], shell=True)
 
         result_file: TextIO
-        with open(self._collect_state_result_path, "rb") as result_file:
-            return pickle.load(result_file)
+        try:
+            with open(self._collect_state_result_path, "rb") as result_file:
+                return pickle.load(result_file)
+
+        except FileNotFoundError:
+            print(f"File {self._collect_state_result_path} was not found. See previous Python 2 errors")
+            sys.exit(-1)
 
 
     def load_hdf(self) -> None:
 
         if not hasattr(self, "hdf_path"):
             raise AttributeError("hdf_path attribute must be set before "
                     "calling load_hdf method.")
```

### Comparing `odb-plotter-0.6.6/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.7/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.7/src/odbp/py2_scripts/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,16 @@
             for frame in user_frames:
                 target_frames.add(frame.frameId)
 
         target_frames = sorted(list(target_frames))
 
         if len(target_frames) == 0:
             for step_data in steps.values():
-                for frame in step_data.frames:
-                    target_frames.append(frame.frameId) 
+                for i, _ in enumerate(step_data.frames):
+                    target_frames.append(i) 
 
         target_nodesets = set()
         if user_nodes is not None:
             if isinstance(user_nodes, collections.Mapping):
                 for key, val in user_nodes.items():
                     assembly.NodeSetFromNodeLabels(name=key, nodeLabels=(val,))
                     target_nodesets.add(key)
@@ -317,15 +317,14 @@
                 for item in coords.values:
                     node = item.nodeLabel
                     coord = item.data
                     xyz = [node]
                     for axis in coord:
                         xyz.append(axis)
                     results_list.append(xyz)
-
                 np.savez_compressed(coord_file, np.array(results_list))
 
             except KeyError:
                 pass
 
         finally:
             odb.close()
```

### Comparing `odb-plotter-0.6.6/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.7/src/odbp/py2_scripts/extractor.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.7/src/odbp/py2_scripts/state_collector.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/reader.py` & `odb-plotter-0.6.7/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/state.py` & `odb-plotter-0.6.7/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/util.py` & `odb-plotter-0.6.7/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.6/src/odbp/writer.py` & `odb-plotter-0.6.7/src/odbp/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
             i: int
             items: Tuple[str, NDArrayType]
             for i, items in enumerate(temp_dict[step].items()):
                 file: str
                 node_data: NDArrayType
                 file, node_data = items
                 frame: str = pathlib.Path(file).stem
-                print(frame)
                 target_len: int = len(node_data)
                 hdf5_file.create_dataset(
                         f"nodes/{step}/{frame}",
                         data = np.hstack((
                             node_data,
                             np.vstack(
                                 np.full(
```

