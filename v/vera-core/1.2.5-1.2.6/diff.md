# Comparing `tmp/vera-core-1.2.5.tar.gz` & `tmp/vera-core-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vera-core-1.2.5.tar", last modified: Wed Jan 11 20:55:48 2023, max compression
+gzip compressed data, was "vera-core-1.2.6.tar", last modified: Thu Jul 13 00:36:42 2023, max compression
```

## Comparing `vera-core-1.2.5.tar` & `vera-core-1.2.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.583441 vera-core-1.2.5/
--rw-r--r--   0 root         (0) root         (0)      583 2023-01-11 20:55:10.000000 vera-core-1.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      112 2023-01-11 20:55:10.000000 vera-core-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2023-01-11 20:55:48.583441 vera-core-1.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1558 2023-01-11 20:55:10.000000 vera-core-1.2.5/README.rst
--rw-r--r--   0 root         (0) root         (0)     1149 2023-01-11 20:55:48.583441 vera-core-1.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-11 20:55:10.000000 vera-core-1.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.575441 vera-core-1.2.5/vera_core/
--rw-r--r--   0 root         (0) root         (0)      583 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/LICENSE
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/app/
--rw-r--r--   0 root         (0) root         (0)       50 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/app/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7427 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/core/vera_out_file.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/app/ui/
--rw-r--r--   0 root         (0) root         (0)    12363 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2508 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/assembly_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/app/ui/assets/
--rw-r--r--   0 root         (0) root         (0)      158 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4962 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/assets/logo.svg
--rw-r--r--   0 root         (0) root         (0)     3131 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/axial_plot.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/core_view.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/empty.py
--rw-r--r--   0 root         (0) root         (0)     2606 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/table_view.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/time_plot.py
--rw-r--r--   0 root         (0) root         (0)     6973 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/volume_view.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/x_axial_view.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/app/ui/y_axial_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/module/
--rw-r--r--   0 root         (0) root         (0)      476 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core/module/serve/
--rw-r--r--   0 root         (0) root         (0)      365 2023-01-11 20:55:45.000000 vera-core-1.2.5/vera_core/module/serve/vue-vera_core.css
--rw-r--r--   0 root         (0) root         (0)   233904 2023-01-11 20:55:45.000000 vera-core-1.2.5/vera_core/module/serve/vue-vera_core.umd.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.583441 vera-core-1.2.5/vera_core/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-01-11 20:55:10.000000 vera-core-1.2.5/vera_core/widgets/vera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 20:55:48.579441 vera-core-1.2.5/vera_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-11 20:55:48.000000 vera-core-1.2.5/vera_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-13 00:35:53.000000 vera-core-1.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-13 00:35:53.000000 vera-core-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-13 00:36:42.010626 vera-core-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-13 00:35:53.000000 vera-core-1.2.6/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-13 00:36:42.010626 vera-core-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 00:35:53.000000 vera-core-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.002626 vera-core-1.2.6/vera_core/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7741 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/core/vera_out_file.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.006626 vera-core-1.2.6/vera_core/app/ui/
+-rw-r--r--   0 root         (0) root         (0)    12376 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assembly_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/app/ui/assets/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4962 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/assets/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/axial_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/core_view.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/empty.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/table_view.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/time_plot.py
+-rw-r--r--   0 root         (0) root         (0)     6973 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/volume_view.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/x_axial_view.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/app/ui/y_axial_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/module/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-13 00:36:38.000000 vera-core-1.2.6/vera_core/module/serve/vue-vera_core.css
+-rw-r--r--   0 root         (0) root         (0)   233904 2023-07-13 00:36:38.000000 vera-core-1.2.6/vera_core/module/serve/vue-vera_core.umd.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.010626 vera-core-1.2.6/vera_core/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-13 00:35:53.000000 vera-core-1.2.6/vera_core/widgets/vera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 00:36:42.002626 vera-core-1.2.6/vera_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 00:36:41.000000 vera-core-1.2.6/vera_core.egg-info/top_level.txt
```

### Comparing `vera-core-1.2.5/LICENSE` & `vera-core-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/PKG-INFO` & `vera-core-1.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vera-core
-Version: 1.2.5
+Version: 1.2.6
 Summary: VERACore let you visualize and interpret the output data from VERA codes
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,14 +19,16 @@
 
 VERACore
 ========================================
 
 VERACore is a Python application for visualization and engineering analyses of output data from VERA (Virtual Environment for Reactor Applications).
 Implemented in Python, it provides instantaneous 2D and 3D images, 1D plots, and alphanumeric data from VERA multi-physics simulations.
 
+For an interactive online example, see `here <https://pvw.kitware.com/vera/>`_.
+
 Installing
 ----------------------------------------
 
 VERACore can be installed via pip and can run locally or deployed as a service.
 To use it locally within a virtual environment, you can run the following commands:
 
 .. code-block:: console
```

### Comparing `vera-core-1.2.5/README.rst` & `vera-core-1.2.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 VERACore
 ========================================
 
 VERACore is a Python application for visualization and engineering analyses of output data from VERA (Virtual Environment for Reactor Applications).
 Implemented in Python, it provides instantaneous 2D and 3D images, 1D plots, and alphanumeric data from VERA multi-physics simulations.
 
+For an interactive online example, see `here <https://pvw.kitware.com/vera/>`_.
+
 Installing
 ----------------------------------------
 
 VERACore can be installed via pip and can run locally or deployed as a service.
 To use it locally within a virtual environment, you can run the following commands:
 
 .. code-block:: console
```

### Comparing `vera-core-1.2.5/setup.cfg` & `vera-core-1.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vera-core
-version = 1.2.5
+version = 1.2.6
 description = VERACore let you visualize and interpret the output data from VERA codes
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `vera-core-1.2.5/vera_core/LICENSE` & `vera-core-1.2.6/vera_core/LICENSE`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/core/vera_out_file.py` & `vera-core-1.2.6/vera_core/app/core/vera_out_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,22 +76,29 @@
         return self._f[f"{self._path}/{name}"]
 
     def _cache(self, name):
         # Set the attribute to be the loaded numpy array
         if name not in self._dataset_names:
             raise AttributeError(name)
 
-        setattr(self, name, self._load_dataset(name)[:])
+        dataset = self._load_dataset(name)[()]
+        if not isinstance(dataset, np.ndarray):
+            dataset = np.array([dataset])
+        setattr(self, name, dataset)
 
     def _uncache(self, name):
         # Set the attribute to be the h5py dataset
         if name not in self._dataset_names:
             raise AttributeError(name)
 
-        setattr(self, name, self._load_dataset(name))
+        # to fix issue with scalar datasets being indexed with a [0]
+        dataset = self._load_dataset(name)[()]
+        if not isinstance(dataset, np.ndarray):
+            dataset = np.array([dataset])
+        setattr(self, name, dataset)
 
     def _cache_all(self):
         for name in self._dataset_names:
             self._cache(name)
 
     def _uncache_all(self):
         for name in self._dataset_names:
@@ -199,20 +206,20 @@
     def reduced_core_map_column_label(self, assembly_idx):
         i, j = self.reduced_core_map_ij(assembly_idx)
         return self.reduced_core_map_column_labels[i]
 
 
 class VeraOutState(LazyHDF5Loader):
     # These are the attributes that will be read from the HDF5 file
-    crit_boron: H5_ARRAY_TYPE = None
+    boron: H5_ARRAY_TYPE = None
     detector_response: H5_ARRAY_TYPE = None
     exposure: H5_ARRAY_TYPE = None
     keff: H5_ARRAY_TYPE = None
-    pin_cladtemps: H5_ARRAY_TYPE = None
-    pin_fueltemps: H5_ARRAY_TYPE = None
-    pin_moddens: H5_ARRAY_TYPE = None
-    pin_modtemps: H5_ARRAY_TYPE = None
+    pin_max_clad_surface_temp: H5_ARRAY_TYPE = None
+    pin_fuel_temp: H5_ARRAY_TYPE = None
+    pin_mod_dens: H5_ARRAY_TYPE = None
+    pin_mod_temp: H5_ARRAY_TYPE = None
     pin_powers: H5_ARRAY_TYPE = None
 
     def __init__(self, f, idx):
         super().__init__(f, f"/STATE_{idx:04}", list(self.__annotations__))
         self._index = idx
```

### Comparing `vera-core-1.2.5/vera_core/app/jupyter.py` & `vera-core-1.2.6/vera_core/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/main.py` & `vera-core-1.2.6/vera_core/app/main.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/__init__.py` & `vera-core-1.2.6/vera_core/app/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,18 +197,18 @@
 
             vuetify.VSelect(
                 v_model=("selected_array", "pin_powers"),
                 items=(
                     "available_arrays",
                     [
                         dict(text="Pin Powers", value="pin_powers"),
-                        dict(text="Pin Clad Temps", value="pin_cladtemps"),
-                        dict(text="Pin Fuel Temps", value="pin_fueltemps"),
-                        dict(text="Pin Moderator Density", value="pin_moddens"),
-                        dict(text="Pin Moderator Temps", value="pin_modtemps"),
+                        dict(text="Pin Clad Temps", value="pin_max_clad_surface_temp"),
+                        dict(text="Pin Fuel Temps", value="pin_fuel_temp"),
+                        dict(text="Pin Moderator Density", value="pin_mod_dens"),
+                        dict(text="Pin Moderator Temps", value="pin_mod_temp"),
                         dict(text="Pin Volumes", value="pin_volumes"),
                     ],
                 ),
                 hide_details=True,
                 dense=True,
                 style="max-width: 220px",
             )
```

### Comparing `vera-core-1.2.5/vera_core/app/ui/assembly_view.py` & `vera-core-1.2.6/vera_core/app/ui/assembly_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/assets/logo.svg` & `vera-core-1.2.6/vera_core/app/ui/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/axial_plot.py` & `vera-core-1.2.6/vera_core/app/ui/axial_plot.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/core_view.py` & `vera-core-1.2.6/vera_core/app/ui/core_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/table_view.py` & `vera-core-1.2.6/vera_core/app/ui/table_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         indices = tuple(map(int, indices))
 
         array = vera_out_file.array(selected_array)
         value = array[indices]
 
         data_dict = {
             selected_array: value,
-            "crit_boron": vera_out_file.active_state.crit_boron[0],
+            "boron": vera_out_file.active_state.boron[0],
             "exposure": vera_out_file.active_state.exposure[0],
             "keff": vera_out_file.active_state.keff[0],
         }
 
         # Round floats so we don't display too many sig figs.
         # 7 sig figs matches veraview.
         sig_figs = 7
```

### Comparing `vera-core-1.2.5/vera_core/app/ui/time_plot.py` & `vera-core-1.2.6/vera_core/app/ui/time_plot.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/volume_view.py` & `vera-core-1.2.6/vera_core/app/ui/volume_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/x_axial_view.py` & `vera-core-1.2.6/vera_core/app/ui/x_axial_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/app/ui/y_axial_view.py` & `vera-core-1.2.6/vera_core/app/ui/y_axial_view.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/module/serve/vue-vera_core.umd.min.js` & `vera-core-1.2.6/vera_core/module/serve/vue-vera_core.umd.min.js`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core/widgets/vera.py` & `vera-core-1.2.6/vera_core/widgets/vera.py`

 * *Files identical despite different names*

### Comparing `vera-core-1.2.5/vera_core.egg-info/PKG-INFO` & `vera-core-1.2.6/vera_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vera-core
-Version: 1.2.5
+Version: 1.2.6
 Summary: VERACore let you visualize and interpret the output data from VERA codes
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,14 +19,16 @@
 
 VERACore
 ========================================
 
 VERACore is a Python application for visualization and engineering analyses of output data from VERA (Virtual Environment for Reactor Applications).
 Implemented in Python, it provides instantaneous 2D and 3D images, 1D plots, and alphanumeric data from VERA multi-physics simulations.
 
+For an interactive online example, see `here <https://pvw.kitware.com/vera/>`_.
+
 Installing
 ----------------------------------------
 
 VERACore can be installed via pip and can run locally or deployed as a service.
 To use it locally within a virtual environment, you can run the following commands:
 
 .. code-block:: console
```

### Comparing `vera-core-1.2.5/vera_core.egg-info/SOURCES.txt` & `vera-core-1.2.6/vera_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

