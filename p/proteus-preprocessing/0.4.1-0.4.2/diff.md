# Comparing `tmp/proteus_preprocessing-0.4.1.tar.gz` & `tmp/proteus_preprocessing-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_preprocessing-0.4.1.tar", max compression
+gzip compressed data, was "proteus_preprocessing-0.4.2.tar", max compression
```

## Comparing `proteus_preprocessing-0.4.1.tar` & `proteus_preprocessing-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       43 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/__init__.py
--rw-r--r--   0        0        0      909 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/ecl_deck.py
--rw-r--r--   0        0        0     8837 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/runspec.py
--rw-r--r--   0        0        0     2999 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/deck/section.py
--rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/__init__.py
--rw-r--r--   0        0        0     2509 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/flowline.py
--rw-r--r--   0        0        0     1461 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/facilities/network.py
--rw-r--r--   0        0        0        0 2023-07-12 14:37:41.812221 proteus_preprocessing-0.4.1/preprocessing/modular/__init__.py
--rw-r--r--   0        0        0      548 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/dat.py
--rw-r--r--   0        0        0    16684 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/data.py
--rw-r--r--   0        0        0      415 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/egrid.py
--rw-r--r--   0        0        0      365 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/grdecl.py
--rw-r--r--   0        0        0     2123 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/init.py
--rw-r--r--   0        0        0     5402 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/s.py
--rw-r--r--   0        0        0      178 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/modular/x.py
--rw-r--r--   0        0        0      221 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/patches.py
--rw-r--r--   0        0        0       71 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/__init__.py
--rw-r--r--   0        0        0     1062 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/expand_dates.py
--rw-r--r--   0        0        0      901 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/preprocessing/utils/expand_wcon.py
--rw-r--r--   0        0        0     1572 2023-07-12 14:37:41.816221 proteus_preprocessing-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 proteus_preprocessing-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/deck/__init__.py
+-rw-r--r--   0        0        0      909 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/deck/ecl_deck.py
+-rw-r--r--   0        0        0     8837 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/deck/runspec.py
+-rw-r--r--   0        0        0     2999 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/deck/section.py
+-rw-r--r--   0        0        0        0 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/facilities/__init__.py
+-rw-r--r--   0        0        0     2709 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/facilities/flowline.py
+-rw-r--r--   0        0        0     1511 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/facilities/network.py
+-rw-r--r--   0        0        0        0 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/dat.py
+-rw-r--r--   0        0        0    16684 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/data.py
+-rw-r--r--   0        0        0      415 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/egrid.py
+-rw-r--r--   0        0        0      365 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/grdecl.py
+-rw-r--r--   0        0        0     2123 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/init.py
+-rw-r--r--   0        0        0     5402 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/s.py
+-rw-r--r--   0        0        0      178 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/modular/x.py
+-rw-r--r--   0        0        0      221 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/patches.py
+-rw-r--r--   0        0        0       71 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/utils/__init__.py
+-rw-r--r--   0        0        0     1062 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/utils/expand_dates.py
+-rw-r--r--   0        0        0      901 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/preprocessing/utils/expand_wcon.py
+-rw-r--r--   0        0        0     1572 2023-07-13 12:38:35.861948 proteus_preprocessing-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 proteus_preprocessing-0.4.2/PKG-INFO
```

### Comparing `proteus_preprocessing-0.4.1/preprocessing/deck/ecl_deck.py` & `proteus_preprocessing-0.4.2/preprocessing/deck/ecl_deck.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/deck/runspec.py` & `proteus_preprocessing-0.4.2/preprocessing/deck/runspec.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/deck/section.py` & `proteus_preprocessing-0.4.2/preprocessing/deck/section.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/facilities/flowline.py` & `proteus_preprocessing-0.4.2/preprocessing/facilities/flowline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-import json
-import os
+from pathlib import Path
 
 import h5py
 import numpy as np
 
+from preprocessing.facilities.network import preprocess as preprocess_network
+
 VARIABLES = [
     "VolumeFlowrateOilStockTank",
     "VolumeFlowrateLiquidStockTank",
     "Pressure",
     "Watercut",
     "VolumeFlowrateOilInSitu",
     "VolumeFlowrateLiquidInSitu",
 ]
 
 
-def preprocess(download_func, output_source, base_output_source, input_files, **_):
-    network = get_processed_network_json(base_output_source)
+def preprocess(download_func, output_source, input_files, **_):
+    network_file_name = input_files[0]  # network.csv
+    input_file_names = input_files[1:]  # (cases/{group}/SIMULATION_{case}/flowline.csv, ...)
+    output_sub_directory = Path(input_file_names[0]).parents[1]  # cases/{group}  # noqa
+
+    network = preprocess_network(download_func, output_source, network_file_name, save=False)
 
-    download_raw_flowline_csvs(download_func, output_source, input_files)
+    download_raw_flowline_csvs(download_func, output_source, input_file_names)
 
     output_networks = []
     for n in range(len(network)):
         network_names = network[list(network.keys())[n]]["branches"]
         outputs = []
 
         for variable in VARIABLES:
             outputs_array = []
 
-            for input_file in input_files:
-                input_file_name = os.path.join(output_source.uri, input_file)
+            for input_file in input_file_names:
+                input_file_name = Path(output_source.uri) / input_file
                 data = np.loadtxt(input_file_name, delimiter=",", dtype=str)
                 values = []
 
                 for name_cluster in network_names:
                     values.append(
                         data[data[:, 2] == name_cluster, np.where(data[0, :] == variable)[0][0]].astype(np.float32)
                     )
 
                 outputs_array.append(np.concatenate(values))
 
             try:
                 outputs.append(np.stack(outputs_array))
 
             except Exception:
-                for i in range(len(input_files)):
+                for i in range(len(input_file_names)):
                     if len(outputs_array[i]) != len(outputs_array[0]):
                         print(
                             f"Error length does not match in simulation {i} it should be {len(outputs_array[0])}. "
                             f"However, the length is {len(outputs_array[i])}"
                         )
 
         output_networks.append(np.moveaxis(np.stack(outputs), 0, 1))
 
-    save_processed_flowline_h5(output_source, output_networks)
-
+    save_processed_flowline_h5(output_source, output_sub_directory, output_networks)
 
-def get_processed_network_json(base_output_source):
-    network_file_name = os.path.join(base_output_source.uri, "network.json")
-    with open(network_file_name, "r") as network_file:
-        return json.load(network_file)
+    return output_networks
 
 
 def download_raw_flowline_csvs(download_func, output_source, input_files):
     for input_file in input_files:
         download_func(input_file, output_source.uri)
 
 
-def save_processed_flowline_h5(output_source, output_networks):
-    output_file_name = os.path.join(output_source.uri, "flowline.h5")
+def save_processed_flowline_h5(output_source, output_directory, output_networks):
+    output_file_name = Path(output_source.uri) / output_directory / "flowline.h5"
     with h5py.File(output_file_name, "w") as output_file:
         for i in range(len(output_networks)):
-            output_file.create_dataset(f"arr_{i}", data=output_networks[i])
+            output_file.create_dataset(f"network_{i}", data=output_networks[i])
```

### Comparing `proteus_preprocessing-0.4.1/preprocessing/facilities/network.py` & `proteus_preprocessing-0.4.2/preprocessing/facilities/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
-import os
+
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 
-def preprocess(download_func, output_source, network, **_):
+def preprocess(download_func, output_source, network, save=True, **_):
     df = get_raw_network_dataframe(download_func, output_source, network)
 
     unique_counts = df.groupby(["Elevation", "Lat", "Long"]).transform("nunique")
     df["num_connections"] = unique_counts["BranchEquipment"]
     network_number = list(df["Network"].unique())
 
     network = {}
@@ -19,20 +20,23 @@
         network[n + 1]["measured_distance"] = np.concatenate(
             [df[df["BranchEquipment"] == b]["MeasuredDistance"].values for b in network[n + 1]["branches"]]
         ).tolist()
         network[n + 1]["numbers"] = np.cumsum(
             [len(df[df["BranchEquipment"] == b]["MeasuredDistance"].values) for b in network[n + 1]["branches"]]
         ).tolist()
 
-    save_processed_network_json(output_source, network)
+    if save:
+        save_processed_network_json(output_source, network)
+
+    return network
 
 
 def get_raw_network_dataframe(download_func, output_source, network):
     download_func(network, output_source.uri)
-    input_file_name = os.path.join(output_source.uri, network)
+    input_file_name = Path(output_source.uri) / network
     return pd.read_csv(input_file_name)
 
 
 def save_processed_network_json(output_source, network):
-    output_file_name = os.path.join(output_source.uri, "network.json")
+    output_file_name = Path(output_source.uri) / "network.json"
     with open(output_file_name, "w") as output_file:
         json.dump(network, output_file)
```

### Comparing `proteus_preprocessing-0.4.1/preprocessing/modular/dat.py` & `proteus_preprocessing-0.4.2/preprocessing/modular/dat.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/modular/data.py` & `proteus_preprocessing-0.4.2/preprocessing/modular/data.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/modular/init.py` & `proteus_preprocessing-0.4.2/preprocessing/modular/init.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/modular/s.py` & `proteus_preprocessing-0.4.2/preprocessing/modular/s.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/utils/expand_dates.py` & `proteus_preprocessing-0.4.2/preprocessing/utils/expand_dates.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/preprocessing/utils/expand_wcon.py` & `proteus_preprocessing-0.4.2/preprocessing/utils/expand_wcon.py`

 * *Files identical despite different names*

### Comparing `proteus_preprocessing-0.4.1/pyproject.toml` & `proteus_preprocessing-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-preprocessing"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = []
 packages = [
     { include = "preprocessing/modular" },
     { include = "preprocessing/deck" },
     { include = "preprocessing/facilities" },
     { include = "preprocessing/utils" },
```

### Comparing `proteus_preprocessing-0.4.1/PKG-INFO` & `proteus_preprocessing-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-preprocessing
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

