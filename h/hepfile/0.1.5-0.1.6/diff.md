# Comparing `tmp/hepfile-0.1.5.tar.gz` & `tmp/hepfile-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hepfile-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hepfile-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hepfile-0.1.5.tar` & `hepfile-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11389 2023-07-10 16:29:56.189257 hepfile-0.1.5/LICENSE
--rw-r--r--   0        0        0     8357 2023-07-10 16:29:56.189257 hepfile-0.1.5/README.md
--rw-r--r--   0        0        0     1912 2023-07-10 16:29:56.209257 hepfile-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1346 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/__init__.py
--rw-r--r--   0        0        0       76 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/_version.py
--rw-r--r--   0        0        0     8051 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/awkward_tools.py
--rw-r--r--   0        0        0      402 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/constants.py
--rw-r--r--   0        0        0     1764 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/csv_tools.py
--rw-r--r--   0        0        0     8548 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/df_tools.py
--rw-r--r--   0        0        0     7291 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/dict_tools.py
--rw-r--r--   0        0        0     1935 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/errors.py
--rw-r--r--   0        0        0        0 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/py.typed
--rw-r--r--   0        0        0    21588 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/read.py
--rw-r--r--   0        0        0    28372 2023-07-10 16:29:56.213257 hepfile-0.1.5/src/hepfile/write.py
--rw-r--r--   0        0        0    10227 1970-01-01 00:00:00.000000 hepfile-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11389 2023-07-13 17:01:59.486751 hepfile-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8348 2023-07-13 17:01:59.486751 hepfile-0.1.6/README.md
+-rw-r--r--   0        0        0     1939 2023-07-13 17:01:59.502752 hepfile-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1245 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/_version.py
+-rw-r--r--   0        0        0     8110 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/awkward_tools.py
+-rw-r--r--   0        0        0      402 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/constants.py
+-rw-r--r--   0        0        0     1962 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/csv_tools.py
+-rw-r--r--   0        0        0     8841 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/df_tools.py
+-rw-r--r--   0        0        0     7229 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/dict_tools.py
+-rw-r--r--   0        0        0     1935 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/errors.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/py.typed
+-rw-r--r--   0        0        0    21714 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/read.py
+-rw-r--r--   0        0        0    28920 2023-07-13 17:01:59.506752 hepfile-0.1.6/src/hepfile/write.py
+-rw-r--r--   0        0        0    10302 1970-01-01 00:00:00.000000 hepfile-0.1.6/PKG-INFO
```

### Comparing `hepfile-0.1.5/LICENSE` & `hepfile-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hepfile-0.1.5/README.md` & `hepfile-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![PyPI version](https://badge.fury.io/py/hepfile.svg)][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![codecov](https://codecov.io/gh/mattbellis/hepfile/branch/main/graph/badge.svg?token=4OADJIUAPU)](https://codecov.io/gh/mattbellis/hepfile)
 [![Code style: black][black-badge]][black-link]
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mattbellis/hepfile/HEAD?urlpath=lab/tree/docs/examples/example_nb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mattbellis/hepfile/HEAD?urlpath=lab/tree/docs/example_nb)
 [![DOI](https://zenodo.org/badge/378834559.svg)](https://zenodo.org/badge/latestdoi/378834559)
 [![Gitter][gitter-badge]][gitter-link]
 
 [actions-badge]:            https://github.com/mattbellis/hepfile/workflows/CI/badge.svg
 [actions-link]:             https://github.com/mattbellis/hepfile/actions
 [black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]:               https://github.com/psf/black
```

### Comparing `hepfile-0.1.5/pyproject.toml` & `hepfile-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 docs = [
   "hepfile[all]",
   "Sphinx>=3.0.0",
   "myst_parser>=0.13",
   "nbsphinx>=0.9.1",
   "sphinx-book-theme>=0.0.33",
   "sphinx_copybutton",
+  "autodoc",
+  "ipykernel"
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra -Wd"
 testpaths = ["tests"]
 
 [tool.mypy]
```

### Comparing `hepfile-0.1.5/src/hepfile/__init__.py` & `hepfile-0.1.6/src/hepfile/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,19 +40,14 @@
 
 # put all these variables in __all__
 __all__ = ("__version__", "__package__", "_AWKWARD", "_PANDAS")
 
 
 # override getattr
 def __getattr__(name: str) -> bool:
-    if name == "_AWKWARD":
-        return _AWKWARD
-    if name == "_PANDAS":
-        return _PANDAS
-
     if not _AWKWARD and name == "awkward_tools":
         raise MissingOptionalDependency("awkward")
 
     if not _PANDAS and name == "csv_tools" or name == "df_tools":
         raise MissingOptionalDependency("pandas")
 
     raise AttributeError
```

### Comparing `hepfile-0.1.5/src/hepfile/awkward_tools.py` & `hepfile-0.1.6/src/hepfile/awkward_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """
 These are tools to make working with and translating between awkward arrays
 and hepfile data objects easier.
+
+Note: The base installation package does not contain these tools!
+You must have installed hepfile with either
+1) 'python -m pip install hepfile[awkward]', or
+2) 'python -m pip install hepfile[all]'
 """
 from __future__ import annotations
 
 import warnings
 import awkward as ak
 import numpy as np
 from hepfile.write import (
@@ -25,64 +30,66 @@
     """
     Converts all (or a subset of) the output data from `hepfile.read.load` to
     a dictionary of awkward arrays.
 
     Args:
         data (dict): Output data dictionary from the `hepfile.read.load` function.
         groups (list): list of groups to pull from data and convert to awkward arrays.
-        datasets (list): list of datasets to pull from data and include in the awkward arrays.
+        datasets (list): list of full dataset paths (ex. 'jet/px' not 'px') to pull
+        from data and include in the awkward arrays.
 
     Returns:
         ak_arrays (dict): dictionary of awkward arrays with the data.
     """
 
-    if datasets is None:
-        datasets = data["_LIST_OF_DATASETS_"]
+    if isinstance(groups, str):
+        groups = [groups]
 
     if groups is None:
         groups = list(data["_GROUPS_"].keys())
 
     ak_arrays = {}
 
     # turn a few things into sets for faster searching
     list_of_counters = set(data["_LIST_OF_COUNTERS_"])
-    singletons_group = set(data["_SINGLETONS_GROUP_"])
+    singletons_group = set(data["_GROUPS_"]["_SINGLETONS_GROUP_"])
 
     for group in groups:
         for dset in data["_GROUPS_"][group]:
             if dset in singletons_group:
                 dataset = dset
             else:
                 dataset = f"{group}/{dset}"
 
             if dataset in list_of_counters:
                 continue
 
             if dataset not in data.keys():
                 continue
 
+            if datasets is not None and dataset not in datasets:
+                continue
+
             if (
                 len(data[dataset]) != 0
-                and isinstance(data[dataset], np.ndarray)
+                and isinstance(data[dataset], (np.ndarray, list))
                 and isinstance(data[dataset][0], bytes)
             ):
                 data[dataset] = np.array([val.decode() for val in data[dataset]])
 
             if dataset in singletons_group:
                 if dataset in data.keys():  # skip if it isn't in data
                     ak_arrays[dataset] = ak.Array(data[dataset])
                 continue
 
             nkey = data["_MAP_DATASETS_TO_COUNTERS_"][dataset]
 
             num = data[nkey]
             vals = data[dataset]
 
-            if len(vals) > 0 and isinstance(vals[0], str):
-                vals = vals.astype(str)
             ak_array = ak.unflatten(list(vals), list(num))
 
             if group not in ak_arrays:
                 ak_arrays[group] = {}
             ak_arrays[group][dset] = ak_array
 
     try:
@@ -104,24 +111,29 @@
         ) from err
 
     return awk
 
 
 ################################################################################
 def awkward_to_hepfile(
-    ak_array: ak.Record, outfile: str = None, write_hepfile: bool = True
+    ak_array: ak.Record,
+    outfile: str = None,
+    write_hepfile: bool = True,
+    verbose: bool = False,
+    **kwargs,
 ) -> dict:
     """
     Converts a dictionary of awkward arrays to a hepfile
 
     Args:
         ak_array (Awkward Array): dictionary of Awkward Arrays to write to a hepfile
         outfile (str): path to write output hdf5 file to
         write_hepfile (bool): if True, writes data to outfile.
                               If False, just converts to hepfile format and returns
+        verbose (bool): if true print some stuff
         **kwargs (None): Passed to `hepfile.write.write_to_file`
 
     Returns:
         Dictionary of hepfile data
     """
 
     # perform IO checks
@@ -167,39 +179,35 @@
             for dataset in data_dict[group].fields:
                 name = f"{group}/{dataset}"
                 bucket[name] = data_dict[group][dataset].to_list()
         pack(data, bucket)
 
     # then write it out to a file
     if write_hepfile:
-        print("Writing the hdf5 file from the awkward array...")
-
-        for key, item in data.items():
-            if isinstance(item, (ak.Record, ak.Array)):
-                try:
-                    data[key] = ak.to_numpy(item)
-                except:
-                    data[key] = ak.to_list(item)
+        if verbose:
+            print("Writing the hdf5 file from the awkward array...")
 
         write_to_file(outfile, data)
 
     return data
 
 
 def _awkward_depth(ak_array: ak.Record) -> int:
     max_depth = 0
     for item in ak_array.to_list():
-        item_depth = -1
+        item_depth = 0
         for string in str(item):
             if string == "{":
                 item_depth += 1
+
+            if item_depth > max_depth:
+                max_depth = item_depth
+
             if string == "}":
                 item_depth -= 1
-        if item_depth > max_depth:
-            max_depth = item_depth
 
     return max_depth
 
 
 def _is_valid_awkward(ak_array: ak.Record):
     """
     Checks if the input awkward array is valid and raises an exception if not
@@ -208,15 +216,15 @@
         ak_array (ak.Array): awkward array to check
     """
 
     # validate input array
     if not isinstance(ak_array, (ak.Array, ak.Record)):
         raise AwkwardStructureError("Please input an Awkward Array or Awkward Record")
 
-    if ak_array.fields == 0:
+    if len(ak_array.fields) == 0:
         raise AwkwardStructureError(
             "Your input Awkward Array must be a Record. \
             This means it needs to have fields in it."
         )
 
     # check input array only has a "depth" of 2
     # this can be removed once hepfiles support unlimited depth of groups!
@@ -225,16 +233,14 @@
             "Hepfile only supports awkward arrays with a depth <= 2! \
             Please ensure your input follows this guideline."
         )
 
 
 def _get_awkward_type(ak_array: ak.Record) -> type:
     ndim = ak_array.ndim
-    if ndim < 1:
-        raise InputError("Cannot check type with depth < 1")
     try:
         if isinstance(ak_array[0], (ak.Record, ak.Array)):
             arr = ak_array
             type_str = ak_array.type.content
             if isinstance(type_str, ak.types.NumpyType):
                 dtype = type_str.primitive
             else:
```

### Comparing `hepfile-0.1.5/src/hepfile/csv_tools.py` & `hepfile-0.1.6/src/hepfile/csv_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 """
 Tools to help with managing csvs with hepfile
+
+Note: The base installation package does not contain these tools!
+You must have installed hepfile with either
+1) 'python -m pip install hepfile[pandas]', or
+2) 'python -m pip install hepfile[all]'
 """
 from __future__ import annotations
 
 import os
 from typing import Optional
 
 import pandas as pd
```

### Comparing `hepfile-0.1.5/src/hepfile/df_tools.py` & `hepfile-0.1.6/src/hepfile/df_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 """
 Tools to work with Pandas DataFrames and Hepfile data
+
+Note: The base installation package does not contain these tools!
+You must have installed hepfile with either
+1) 'python -m pip install hepfile[pandas]', or
+2) 'python -m pip install hepfile[all]'
 """
 from __future__ import annotations
 
 import pandas as pd
 import hepfile as hf
 from hepfile.errors import InputError, MissingOptionalDependency
 from hepfile.dict_tools import dictlike_to_hepfile
@@ -96,14 +101,16 @@
     groups: list[str] = None,
     events: list[int] = None,
 ) -> dict[pd.DataFrame]:
     """
     Converts an awkward array of hepfile data to a dataframe. Does the same thing
     as hepfile_to_df but given an awkward array.
 
+    Note: You must have installed with 'python -m pip install hepfile[all]' to use this tool!
+
     Args:
         ak_array [ak.Array]: awkward array in the format of a hepfile
         groups [list]: groups to include, None (default) means include all groups
         events [list]: list of event indexes to include
 
     Returns:
         Dictionary of requested groups as dataframes where the keys are the group names.
```

### Comparing `hepfile-0.1.5/src/hepfile/dict_tools.py` & `hepfile-0.1.6/src/hepfile/dict_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,25 +39,26 @@
 
     Args:
         dict_list (list): list of dictionaries or dataframes where each dictionary/df
                           holds information on an event
         outfile (str): path to write output hepfile to
         how_to_pack (str): how to pack the input dataset. Options are 'awkward' or 'classic'.
                       'awkward' called awkward_to_hepfile, 'classic' does it more traditional.
-                      default is 'awkward'.
+                      default is 'classic'. To use how_to_pack='awkward', make sure you
+                      installed hepfile with the 'awkward' or 'all' optional dependency!
         **kwargs: passed to `hepfile.write.write_to_file` if 'awkward'. Can only be
                   'write_to_hepfile' and 'ignore_protected' if 'classic'.
     Returns:
         Dictionary of Awkward Arrays with the data stored in outfile
     """
 
     # check if it is a list of dictionaries or dataframe
-    if not isinstance(dict_list, list):
+    if not isinstance(dict_list[0], dict):
         try:  # try convert from dataframe to list of dictionaries
-            dict_list = [dict_list[key].to_dict() for key in dict_list.to_dict()]
+            dict_list = [item.to_dict() for item in dict_list]
         except Exception as exc:
             raise InputError(
                 "Please input either a dataframe or list \
             of dictionaries"
             ) from exc
 
     if how_to_pack == "awkward" and not hf._AWKWARD:
@@ -71,30 +72,14 @@
                 "Keys must match across the entire input dictionary list!!!"
             )
 
     if how_to_pack == "awkward":
         return _awkward(dict_list, outfile, **kwargs)
 
     if how_to_pack == "classic":
-        # check kwargs
-        test = {}
-        test.update(**kwargs)
-        try:
-            test.pop("write_hepfile")
-        except KeyError:
-            pass
-        try:
-            test.pop("ignore_protected")
-        except KeyError:
-            pass
-        if len(test) > 0:
-            warnings.warn(
-                "Since how_to_pack=classic, only write_hepfile will be passed along!"
-            )
-
         return _classic(dict_list, outfile, **kwargs)
 
     raise InputError("how_to_pack should either be 'awkward' or 'classic'")
 
 
 def _classic(
     dict_list: dict, outfile: str = None, write_hepfile=True, ignore_protected=False
@@ -122,15 +107,17 @@
             )
 
             continue
 
         create_group(data, group_name, counter=f"n{group_name}")
         for dataset_name in temp_dict[group_name]:
             if not isinstance(temp_dict[group_name][dataset_name], (list, np.ndarray)):
-                raise DictStructureError("Subdictionaries must be made up of lists!")
+                temp_dict[group_name][dataset_name] = [
+                    temp_dict[group_name][dataset_name]
+                ]
 
             test_list = temp_dict[group_name][dataset_name]
 
             dtype = _get_dtype(test_list)
             create_dataset(data, dataset_name, group=group_name, dtype=dtype)
 
     # now pack the data from each data dictionary
@@ -176,14 +163,19 @@
     return out_ak
 
 
 def append(ak_dict: ak.Record, new_dict: dict) -> ak.Record:
     """
     Append a new event to an existing awkward dictionary with events
 
+    Note: This tool requires awkward to be installed. Make sure you installed with
+    either
+    1) 'python -m pip install hepfile[awkward]' or,
+    2) 'python -m pip install hepfile[all]'
+
     Args:
         ak_dict (ak.Record): awkward Record of data
         new_dict (dict): Dictionary of value to append to ak_dict. All keys must match ak_dict!
     Return:
         Awkward Record of awkward arrays with the new_dict appended
     """
     if not hf._AWKWARD:
```

### Comparing `hepfile-0.1.5/src/hepfile/errors.py` & `hepfile-0.1.6/src/hepfile/errors.py`

 * *Files identical despite different names*

### Comparing `hepfile-0.1.5/src/hepfile/read.py` & `hepfile-0.1.6/src/hepfile/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         verbose (boolean): True if debug output is required
 
         desired_groups (list): Groups to be read from input file,
 
         subset (int): Number of buckets to be read from input file
 
         return_type (str): Type to return. Options are 'dictionary', 'awkward', and 'pandas'.
-                           Default is 'dictionary'.
+                           Default is 'dictionary'. Note: the 'awkward' option requires
+                           hepfile to be installed with the awkward or all option and the
+                           'pandas' option requires hepfile to be installed with the pandas
+                           or all option!
 
     Returns:
         data (dict): Selected data from HDF5 file
 
         bucket (dict): An empty bucket dictionary to be filled by data from select buckets
 
     """
@@ -78,18 +81,23 @@
 
         # We might only read in a subset of the data though!
         if subset is not None:
             if isinstance(subset, tuple):
                 subset = list(subset)
 
             if isinstance(subset, int):
-                print(
-                    "Single subset value of {subset} being interpreted as a high range"
-                )
-                print(f"subset being set to a range of (0,{subset})\n")
+                if verbose:
+                    warning = "\n".join(
+                        (
+                            "Single subset value of {subset} being interpreted as a high range",
+                            f"subset being set to a range of (0,{subset})\n",
+                        )
+                    )
+                    warnings.warn(warning)
+
                 subset = [0, subset]
 
             # If the user has specified `subset` incorrectly, then let's return
             # an empty data and bucket
             if subset[1] - subset[0] <= 0:
                 raise RangeSubsetError(
                     f"The range in subset is either 0 or negative! \
@@ -112,20 +120,21 @@
                     be set to {nbuckets}\n"
                 )
                 subset[1] = nbuckets
 
             data["_NUMBER_OF_BUCKETS_"] = subset[1] - subset[0]
             nbuckets = data["_NUMBER_OF_BUCKETS_"]
 
-            print("Will read in a subset of the file!")
-            print(
-                f"From bucket {subset[0]} (inclusive) through bucket {subset[1]-1} (inclusive)"
-            )
-            print(f"Bucket {subset[1]} is not read in")
-            print(f"Reading in {nbuckets} buckets\n")
+            if verbose:
+                print("Will read in a subset of the file!")
+                print(
+                    f"From bucket {subset[0]} (inclusive) through bucket {subset[1]-1} (inclusive)"
+                )
+                print(f"Bucket {subset[1]} is not read in")
+                print(f"Reading in {nbuckets} buckets\n")
 
         ############################################################################
         # Get the datasets and counters
         ############################################################################
         allvalues = infile["_MAP_DATASETS_TO_COUNTERS_"]
         for vals in allvalues:
             if verbose:
@@ -187,15 +196,16 @@
                 # of the dataset
                 for desdat in desired_groups:
                     if desdat in entry:
                         is_dropped = False
                         break
 
                 if is_dropped is True:
-                    print(f"Not reading out {entry} from the file....")
+                    if verbose:
+                        print(f"Not reading out {entry} from the file....")
                     all_datasets.remove(entry)
 
                 i -= 1
 
             if verbose:
                 print("After only selecting certain datasets ----- ")
                 print(f"all_datasets: {all_datasets}")
@@ -212,17 +222,17 @@
             print("\n_SINGLETONS_GROUP_/COUNTER:")
             print(data["_SINGLETONS_GROUP_/COUNTER"])
             print("\n")
 
         ############################################################################
         # Pull out the counters and build the indices
         ############################################################################
-        print("Building the indices...\n")
 
         if verbose:
+            print("Building the indices...\n")
             print("data.keys()")
             print(data.keys())
             print("\n")
 
         # We will need to keep track of the indices in the entire file
         # This way, if the user specifies a subset of the data, we have the full
         # indices already calculated
@@ -235,21 +245,14 @@
             full_file_counters = infile[counter_name]
             full_file_index = calculate_index_from_counters(full_file_counters)
 
             if verbose:
                 print(f"full file counters: {full_file_counters}\n")
                 print(f"full file index: {full_file_index}\n")
 
-            # If we passed in subset, grab that slice of the data from the file
-            if subset is not None and subset[1] <= subset[0]:
-                raise RangeSubsetError(
-                    f"Unable to read anything in! High range of {subset[1]} is \
-                    less than or equal to low range of {subset[0]}"
-                )
-
             if subset is not None:
                 # We tack on +1 to the high range of subset when we pull out the counters
                 # and index because we want to get all of the entries for the last entry.
                 data[counter_name] = infile[counter_name][subset[0] : subset[1] + 1]
                 index = full_file_index[subset[0] : subset[1] + 1]
             else:
                 data[counter_name] = infile[counter_name][:]
@@ -262,17 +265,16 @@
                 subset_index = index - index[0]
 
             index_name = f"{counter_name}_INDEX"
 
             data[index_name] = subset_index
             full_file_indices[index_name] = index
 
-        print("Built the indices!")
-
         if verbose:
+            print("Built the indices!")
             print("full_file_index: ")
             print(f"{full_file_indices}\n")
 
         # Loop over the all_datasets we want and pull out the data.
         for name in all_datasets:
             # If this is a counter, we're going to have to grab the indices
             # differently than for a "normal" dataset
@@ -314,15 +316,16 @@
                 if verbose:
                     print(dataset)
 
             # write the metadata for that group to data if it exists
             if name not in constants.protected_names and "meta" in dataset.attrs.keys():
                 data["_META_"][name] = dataset.attrs["meta"]
 
-    print("Data is read in and input file is closed.")
+    if verbose:
+        print("Data is read in and input file is closed.")
 
     # edit data so it matches the format of the data dict that was saved to the file
     # this makes it so that data can be directly passed to write_to_file
     # 1) add back in _GROUP_
     datasets = np.array(data["_LIST_OF_DATASETS_"])
 
     allgroups = np.array([d.split("/")[0] for d in datasets])
@@ -500,17 +503,15 @@
 
     if return_type in {"df", "dataframe"}:
         if not hf._PANDAS:
             raise MissingOptionalDependency("pandas")
         import pandas as pd
 
     if return_type is not None and return_type not in ["dict", "df", "dataframe"]:
-        print("'return_type' must be 'dict', 'df', or 'dataframe'")
-        print("Not returning any header information")
-        return None
+        raise InputError("'return_type' must be 'dict', 'df', or 'dataframe!")
 
     with h5.File(filename, "r+") as infile:
         if "_HEADER_" not in infile:
             raise HeaderNotFound(
                 f"No header data in file {filename}! File has no _HEADER_ group.\n"
             )
 
@@ -539,15 +540,15 @@
     """Pretty print the file metadata"""
 
     output = ""
 
     try:
         metadata = get_file_metadata(filename)
     except MetadataNotFound:
-        print(f"No Metadata in {filename}!")
+        warnings.warn(f"No Metadata in {filename}!")
         return output
 
     keys = list(metadata.keys())
 
     first_keys_to_print = ["date", "_NUMBER_OF_BUCKETS_"]
 
     keys_already_printed = []
@@ -575,15 +576,14 @@
             continue
 
         val = metadata[key]
         output += f"{key:<20s} : {val}\n"
         keys_already_printed.append(key)
 
     print(output)
-
     return output
 
 
 ################################################################################
 
 
 def print_file_header(filename: str) -> str:
```

### Comparing `hepfile-0.1.5/src/hepfile/write.py` & `hepfile-0.1.6/src/hepfile/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,72 +124,82 @@
         raise InputError(
             f"{group_name} is protected, please choose a different group name!"
         )
 
     # Check for slashes in the group name. We can't have them.
     if "/" in group_name:
         new_group_name = group_name.replace("/", "-")
-        print("----------------------------------------------------")
-        print("Slashes / are not allowed in group names")
-        print(f"Replacing / with - in group name {group_name}")
-        print(f"The new name will be {new_group_name}")
-        print("----------------------------------------------------")
+        warning = "\n".join(
+            (
+                "----------------------------------------------------",
+                "Slashes / are not allowed in group names",
+                f"Replacing / with - in group name {group_name}",
+                f"The new name will be {new_group_name}",
+                "----------------------------------------------------",
+            )
+        )
+        warnings.warn(warning)
         group_name = new_group_name
 
     # Change name of variable, just to keep code more understandable
     counter_name = counter
 
     # Create a counter_name if the user has not specified one
     if counter_name is None:
-        print("----------------------------------------------------")
-        print(f"There is no counter to go with group \033[1m{group_name}\033[0m")
-        print("Are you sure that's what you want?")
         counter_name = f"N_{group_name}"
-        print(f"Creating a counter called \033[1m{counter_name}\033[0m")
-        print("-----------------------------------------------------")
+        warning = "\n".join(
+            (
+                "----------------------------------------------------",
+                f"There is no counter to go with group \033[1m{group_name}\033[0m",
+                "Are you sure that's what you want?",
+                f"Creating a counter called \033[1m{counter_name}\033[0m",
+                "-----------------------------------------------------",
+            )
+        )
+        warnings.warn(warning)
 
     # Check for slashes in the counter name. We can't have them.
     if "/" in counter_name:
         new_counter_name = counter_name.replace("/", "-")
-        print("----------------------------------------------------")
-        print("Slashes / are not allowed in counter names")
-        print(f"Replacing / with - in counter name {counter_name}")
-        print(f"The new name will be {new_counter_name}")
-        print("----------------------------------------------------")
+        warning = "\n".join(
+            (
+                "----------------------------------------------------",
+                "Slashes / are not allowed in counter names",
+                f"Replacing / with - in counter name {counter_name}",
+                "The new name will be {new_counter_name}",
+                "----------------------------------------------------",
+            )
+        )
+        warnings.warn(warning)
         counter_name = new_counter_name
 
     keys = data.keys()
 
     # Then put the group and any datasets in there next.
-    keyfound = False
-    if group_name in keys:
-        print(f"\033[1m{group_name}\033[0m is already in the dictionary!")
-        keyfound = True
+    if group_name in data["_GROUPS_"]:
+        raise ValueError(f"\033[1m{group_name}\033[0m is already in the dictionary!")
 
-    if not keyfound:
-        data["_GROUPS_"][group_name] = []
-        if verbose:
-            print(f"Adding group \033[1m{group_name}\033[0m")
-
-        data["_GROUPS_"][group_name].append(counter_name)
-        full_counter_name = f"{group_name}/{counter_name}"
-
-        data["_MAP_DATASETS_TO_COUNTERS_"][group_name] = full_counter_name
-        data["_MAP_DATASETS_TO_DATA_TYPES_"][full_counter_name] = int
-
-        if full_counter_name not in data["_LIST_OF_COUNTERS_"]:
-            data["_LIST_OF_COUNTERS_"].append(full_counter_name)
-
-        data[full_counter_name] = []
-        if verbose:
-            print(
-                f"Adding a counter for \033[1m{group_name}\033[0m as \033[1m{counter_name}\033[0m"
-            )
-
-    return 0
+    data["_GROUPS_"][group_name] = []
+    if verbose:
+        print(f"Adding group \033[1m{group_name}\033[0m")
+
+    data["_GROUPS_"][group_name].append(counter_name)
+    full_counter_name = f"{group_name}/{counter_name}"
+
+    data["_MAP_DATASETS_TO_COUNTERS_"][group_name] = full_counter_name
+    data["_MAP_DATASETS_TO_DATA_TYPES_"][full_counter_name] = int
+
+    if full_counter_name not in data["_LIST_OF_COUNTERS_"]:
+        data["_LIST_OF_COUNTERS_"].append(full_counter_name)
+
+    data[full_counter_name] = []
+    if verbose:
+        print(
+            f"Adding a counter for \033[1m{group_name}\033[0m as \033[1m{counter_name}\033[0m"
+        )
 
 
 ################################################################################
 
 
 ################################################################################
 # This adds a dataset to the dictionary, similar to
@@ -230,92 +240,87 @@
         if not ignore_protected and tempname in constants.protected_names:
             raise InputError(
                 f"{tempname} is protected, please choose a different dataset name!"
             )
 
         if "/" in tempname:
             new_dataset_name = tempname.replace("/", "-")
-            print("----------------------------------------------------")
-            print("Slashes / are not allowed in dataset names")
-            print(f"Replacing / with - in dataset name {tempname}")
-            print(f"The new name will be {new_dataset_name}")
-            print("----------------------------------------------------")
+            warning = "\n".join(
+                (
+                    "----------------------------------------------------",
+                    "Slashes / are not allowed in dataset names",
+                    f"Replacing / with - in dataset name {tempname}",
+                    f"The new name will be {new_dataset_name}",
+                    "----------------------------------------------------",
+                )
+            )
+            warnings.warn(warning)
             datasets[i] = new_dataset_name
 
     keys = data.keys()
 
     # These will be entries for the SINGLETON_GROUP, if there is no group passed in
     if group is None:
         for dataset in datasets:
-            keyfound = False
-
             if dataset in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
-                print(f"\033[1m{dataset}\033[0m is already in the dictionary!")
-                keyfound = True
-
-            if not keyfound:
-                if verbose:
-                    print(
-                        f"Adding dataset \033[1m{dataset}\033[0m to the dictionary as a SINGLETON."
-                    )
-                data["_GROUPS_"]["_SINGLETONS_GROUP_"].append(dataset)
-                data[dataset] = []
-                data["_MAP_DATASETS_TO_COUNTERS_"][
-                    dataset
-                ] = "_SINGLETONS_GROUP_/COUNTER"
+                warnings.warn(
+                    f"\033[1m{dataset}\033[0m is already in the dictionary! Skipping!"
+                )
+                continue
 
-                data["_MAP_DATASETS_TO_DATA_TYPES_"][dataset] = dtype
+            if verbose:
+                print(
+                    f"Adding dataset \033[1m{dataset}\033[0m to the dictionary as a SINGLETON."
+                )
+            data["_GROUPS_"]["_SINGLETONS_GROUP_"].append(dataset)
+            data[dataset] = []
+            data["_MAP_DATASETS_TO_COUNTERS_"][dataset] = "_SINGLETONS_GROUP_/COUNTER"
 
-        return 0
+            data["_MAP_DATASETS_TO_DATA_TYPES_"][dataset] = dtype
 
-    # Put the counter in the dictionary first.
-    keyfound = group in data["_GROUPS_"]
+        return
 
-    # NEED TO FIX THIS PART SO THAT IT FINDS THE RIGHT COUNTER FROM THE GROUP
-    if not keyfound:
+    # check if the group is in the dataset
+    if group not in data["_GROUPS_"]:
         counter = f"N_{group}"
         warnings.warn(
             f"Your group, \033[1m{group}\033[0m is not in the dictionary yet! \
             Adding it, along with a counter of \033[1m{counter}\033[0m"
         )
         create_group(data, group, counter=counter)
 
     for dataset in datasets:
-        keyfound = False
         name = f"{group}/{dataset}"
 
         # check that tempname isn't in protected_names
         if not ignore_protected and name in constants.protected_names:
             raise InputError(
                 f"{name} is protected, please choose a different dataset or group name!"
             )
 
         if name in keys:
             warnings.warn(
                 f"\033[1m{name}\033[0m is already in the dictionary! Skipping!!!"
             )
-            keyfound = True
-
-        if not keyfound:
-            if verbose:
-                print(
-                    f"Adding dataset \033[1m{dataset}\033[0m to the dictionary \
-                    under group \033[1m{group}\033[0m."
-                )
-            data[name] = []
-            data["_GROUPS_"][group].append(dataset)
+            continue
 
-            # Add a counter for this dataset for the group with which it is associated.
-            counter = data["_MAP_DATASETS_TO_COUNTERS_"][group]
-            # counter_name = "%s/%s" % (group,counter)
-            data["_MAP_DATASETS_TO_COUNTERS_"][name] = counter
+        if verbose:
+            print(
+                f"Adding dataset \033[1m{dataset}\033[0m to the dictionary \
+                under group \033[1m{group}\033[0m."
+            )
+        data[name] = []
+        data["_GROUPS_"][group].append(dataset)
 
-            data["_MAP_DATASETS_TO_DATA_TYPES_"][name] = dtype
+        # Add a counter for this dataset for the group with which it is associated.
+        counter = data["_MAP_DATASETS_TO_COUNTERS_"][group]
+        # counter_name = "%s/%s" % (group,counter)
+        data["_MAP_DATASETS_TO_COUNTERS_"][name] = counter
 
-    return 0
+        data["_MAP_DATASETS_TO_DATA_TYPES_"][name] = dtype
 
 
 ###############################################################################
 def add_meta(data: dict, name: str, meta_data: list):
     """
     Create metadata for a group (or singleton) and add it to data
 
@@ -422,26 +427,35 @@
         if key in {
             "_MAP_DATASETS_TO_COUNTERS_",
             "_GROUPS_",
             "_LIST_OF_COUNTERS_",
             "_MAP_DATASETS_TO_DATA_TYPES_",
             "_META_",
             "_PROTECTED_NAMES_",
+            "_MAP_DATASETS_TO_INDEX_",
+            "_LIST_OF_DATASETS",
+            "_SINGLETONS_GROUP_",
+            "_HEADER_",
+            "_NUMBER_OF_BUCKETS_",
         }:
             continue
 
+        if isinstance(data[key], np.ndarray):
+            data[key] = data[key].tolist()
+
+        if isinstance(bucket[key], np.ndarray):
+            bucket[key] = bucket[key].tolist()
+
         # The singletons will only have 1 entry per bucket
         if key == "_SINGLETONS_GROUP_/COUNTER":
             data[key].append(1)
             continue
 
-        if isinstance(bucket[key], (list, np.ndarray)):
+        if isinstance(bucket[key], list):
             value = bucket[key]
-            if isinstance(value, np.ndarray):
-                value = value.tolist()
             if len(value) > 0:
                 data[key] += value
         else:
             # This is for counters and SINGLETONS
             if key in data["_GROUPS_"]["_SINGLETONS_GROUP_"]:
                 if bucket[key] is None:
                     raise MissingSingletonValue(
@@ -455,16 +469,14 @@
             else:
                 data[key].append(bucket[key])
 
     # Clear out the bucket after it's been packed if that's what we want
     if EMPTY_OUT_BUCKET:
         clear_bucket(bucket)
 
-    return 0
-
 
 ################################################################################
 
 
 def _convert_list_and_key_to_string_data(datalist: list[any], key: str) -> str:
     """Converts data dictionary to a string
 
@@ -523,28 +535,30 @@
 # This function writes default attributes and metadata to a file.
 ################################################################################
 def write_file_metadata(
     filename: str,
     mydict: dict = None,
     write_default_values: bool = True,
     append: bool = True,
+    verbose: bool = False,
 ) -> h5.File:
     """Writes file metadata in the attributes of an HDF5 file
 
     Args:
     filename (string): Name of output file
 
     mydict (dictionary): Metadata desired by user
 
     write_default_values (boolean): True if user wants to write/update the
                                         default metadata: date, hepfile version,
                                         h5py version, numpy version, and Python
                                         version, false if otherwise.
 
     append (boolean): True if user wants to keep older metadata, false otherwise.
+    verbose (boolean): True to print out statements as it goes
 
     Returns:
     hdoutfile (HDF5): File with new metadata
 
     """
 
     with h5.File(filename, "a") as hdoutfile:
@@ -564,35 +578,39 @@
             hdoutfile.attrs["h5py_version"] = h5.__version__
             hdoutfile.attrs["python_version"] = sys.version
 
         if mydict is not None:
             for key in mydict:
                 hdoutfile.attrs[key] = mydict[key]
 
-    print("Metadata added")
+    if verbose:
+        print("Metadata added")
+
     return hdoutfile
 
 
 ################################################################################
 # This function writes a set of user-defined header information to the
 # hepfile
 ################################################################################
-def write_file_header(filename: str, mydict: dict) -> h5.File:
+def write_file_header(filename: str, mydict: dict, verbose: bool = False) -> h5.File:
     """
     Writes header data to a protected group in an HDF5 file.
 
     If there is already header information, it is overwritten
     by this function.
 
     Args:
         filename (string): Name of file to write to (file should already exist
                            and the group will be appended to it.)
 
         mydict (dictionary): Header data passed in by user
 
+        verbose (bool): True to print out info as it runs
+
     Returns:
         hdoutfile (HDF5): Returns the file with new metadata
 
     """
 
     if len(mydict.keys()) == 0:
         raise InputError("Please provide header data to write to the header!")
@@ -608,35 +626,40 @@
             del hdoutfile["_HEADER_"]
 
         header_group = hdoutfile.create_group("_HEADER_")
 
         for key in mydict.keys():
             values = mydict[key]
 
+            # If value is just a str, int, or float, make it an array
+            if isinstance(values, (str, float, int)):
+                values = [values]
+
             # check that values can be converted to a np.array
             try:
                 values = np.array(values)
             except Exception as err:
                 raise InputError(
                     "Unable to convert header data to a numpy array!"
                 ) from err
 
-            # If value is just a str, int, or float, make it an array
-            if isinstance(values, (str, float, int)):
+            # check the datatype of values
+            if isinstance(values[0], np.number):
                 values = values.astype(str)
 
             # When we pass in the values, we need to do it as a list (NOT SURE WHY?)
             header_group.create_dataset(
                 key, (len(values), 1), dtype=dtype, data=values.tolist()
             )
 
     # DO WE WANT TO DO THIS HERE?
     hdoutfile.close()
 
-    print("Header data added")
+    if verbose:
+        print("Header data added")
     return hdoutfile
 
 
 ################################################################################
 
 ################################################################################
 
@@ -713,23 +736,23 @@
             for dataset in datasets:
                 name = None
                 if group == "_SINGLETONS_GROUP_" and dataset != "COUNTER":
                     name = dataset
                 else:
                     name = f"{group}/{dataset}"
 
-                if verbose is True:
+                if verbose:
                     print(f"Writing {name} to file")
 
                 x = data[name]
 
                 dataset_dtype = data["_MAP_DATASETS_TO_DATA_TYPES_"][name]
 
                 if isinstance(x, list):
-                    if verbose is True:
+                    if verbose:
                         print("\tConverting list to array...")
                     x = np.array(x)
 
                 # Do single precision only, unless specified
                 if force_single_precision:
                     # different type calls depending on input datastructure
                     if isinstance(x, np.ndarray):
@@ -737,21 +760,21 @@
                     else:
                         dtype = None
                         warnings.warn(
                             "Not a proper data type to convert to single precision, skipping!"
                         )
 
                     if dtype == np.float64:
-                        if verbose is True:
+                        if verbose:
                             print("\tConverting array to single precision...")
                         x = x.astype(np.float32)
                         dataset_dtype = np.float32
 
                 if dataset_dtype is not str:
-                    if verbose is True:
+                    if verbose:
                         print("\tWriting to file...")
                     hdoutfile.create_dataset(
                         name,
                         data=x,
                         compression=comp_type,
                         compression_opts=comp_opts,
                         dtype=dataset_dtype,
@@ -798,12 +821,11 @@
                 # SHOULD WE EXIT ON THIS?
 
             num_buckets = max(num_buckets, ncounter)
 
             prevcounter = countername
 
         hdoutfile.attrs["_NUMBER_OF_BUCKETS_"] = num_buckets
-        # hdoutfile.close()
 
     write_file_metadata(filename)
 
     return hdoutfile
```

### Comparing `hepfile-0.1.5/PKG-INFO` & `hepfile-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepfile
-Version: 0.1.5
+Version: 0.1.6
 Summary: A file description modeled after the ROOT analysis toolkit and common use-cases
 Author-email: Matt Bellis <mbellis@siena.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
@@ -28,14 +28,16 @@
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: hepfile[all] ; extra == "docs"
 Requires-Dist: Sphinx>=3.0.0 ; extra == "docs"
 Requires-Dist: myst_parser>=0.13 ; extra == "docs"
 Requires-Dist: nbsphinx>=0.9.1 ; extra == "docs"
 Requires-Dist: sphinx-book-theme>=0.0.33 ; extra == "docs"
 Requires-Dist: sphinx_copybutton ; extra == "docs"
+Requires-Dist: autodoc ; extra == "docs"
+Requires-Dist: ipykernel ; extra == "docs"
 Requires-Dist: hepfile[pandas,awkward] ; extra == "learn"
 Requires-Dist: astropy ; extra == "learn"
 Requires-Dist: pandas ; extra == "pandas"
 Project-URL: Documentation, https://hepfile.github.io
 Project-URL: Home, https://github.com/mattbellis/hepfile
 Provides-Extra: all
 Provides-Extra: awkward
@@ -54,15 +56,15 @@
 [![PyPI version](https://badge.fury.io/py/hepfile.svg)][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![codecov](https://codecov.io/gh/mattbellis/hepfile/branch/main/graph/badge.svg?token=4OADJIUAPU)](https://codecov.io/gh/mattbellis/hepfile)
 [![Code style: black][black-badge]][black-link]
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mattbellis/hepfile/HEAD?urlpath=lab/tree/docs/examples/example_nb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mattbellis/hepfile/HEAD?urlpath=lab/tree/docs/example_nb)
 [![DOI](https://zenodo.org/badge/378834559.svg)](https://zenodo.org/badge/latestdoi/378834559)
 [![Gitter][gitter-badge]][gitter-link]
 
 [actions-badge]:            https://github.com/mattbellis/hepfile/workflows/CI/badge.svg
 [actions-link]:             https://github.com/mattbellis/hepfile/actions
 [black-badge]:              https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]:               https://github.com/psf/black
```

