# Comparing `tmp/ewoksdata-0.2.7.tar.gz` & `tmp/ewoksdata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.7.tar", last modified: Tue May 30 13:06:15 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.3.0.tar", last modified: Thu Jul 13 09:18:38 2023, max compression
```

## Comparing `ewoksdata-0.2.7.tar` & `ewoksdata-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 13:04:09.000000 ewoksdata-0.2.7/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:06:09.000000 ewoksdata-0.2.7/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8552 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     9870 2023-05-30 12:59:48.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:06:09.000000 ewoksdata-0.2.7/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3771 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4200 2023-05-30 12:59:48.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1172 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-13 09:17:17.000000 ewoksdata-0.3.0/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 09:18:32.000000 ewoksdata-0.3.0/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8552 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9870 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 09:18:32.000000 ewoksdata-0.3.0/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2023-07-13 07:11:55.000000 ewoksdata-0.3.0/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 09:18:38.000000 ewoksdata-0.3.0/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.7/LICENSE.md` & `ewoksdata-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/setup.cfg` & `ewoksdata-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 	hdf5plugin
 	blissdata
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
-bliss = 
-	blissdata
+online = 
+	blissdata[tango]
 test = 
-	%(bliss)s
+	%(online)s
 	pytest >=7
 dev = 
 	%(test)s
 	black >=22
 	flake8 >=4
 doc = 
 	%(test)s
```

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/bliss.py` & `ewoksdata-0.3.0/src/ewoksdata/data/bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.3.0/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.3.0/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.3.0/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/nexus.py` & `ewoksdata-0.3.0/src/ewoksdata/data/nexus.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         parent.attrs["default"] = name
         parent = parent.parent
 
 
 def create_url(url: str, **open_options) -> DataUrl:
     url = as_dataurl(url)
     filename = url.file_path()
-    os.makedirs(os.path.dirname(filename), exist_ok=True)
+    dirname = os.path.dirname(filename)
+    if dirname:
+        os.makedirs(dirname, exist_ok=True)
     open_options.setdefault("mode", "a")
     with h5py_utils.open_item(filename, "/", **open_options) as parent:
         h5item, _ = _create_h5group(parent, url.data_path())
         return as_dataurl(f"{filename}::{h5item.name}")
 
 
 def get_nxentry(h5item: Union[h5py.Dataset, h5py.Group]):
@@ -59,16 +61,17 @@
     :yields: (h5group, already_existed)
     """
     url = as_dataurl(url)
     filename = url.file_path()
     itemname = url.data_path()
     if not itemname:
         itemname = "/"
-    if os.path.dirname(filename):
-        os.makedirs(os.path.dirname(filename), exist_ok=True)
+    dirname = os.path.dirname(filename)
+    if dirname:
+        os.makedirs(dirname, exist_ok=True)
     open_options.setdefault("mode", "a")
     with h5py_utils.open_item(
         filename,
         "/",
         retry_timeout=retry_timeout,
         retry_period=retry_period,
         **open_options,
```

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/url.py` & `ewoksdata-0.3.0/src/ewoksdata/data/url.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/data/utils.py` & `ewoksdata-0.3.0/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.3.0/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     lima_dirname = tmpdir / f"scan{scannr:04d}"
     lima_dirname.mkdir()
     with h5py.File(str(dataset_filename), mode="w") as root:
         root.attrs["NX_class"] = "NXroot"
         root.attrs["creator"] = "bliss"
         scan = root.create_group(f"{scannr}.{subscannr}")
         scan.attrs["NX_class"] = "NXentry"
-        scan["end_time"] = datetime.now().astimezone().isoformat()
 
         instrument = scan.create_group("instrument")
         instrument.attrs["NX_class"] = "NXinstrument"
         measurement = scan.create_group("measurement")
         measurement.attrs["NX_class"] = "NXcollection"
 
         for name in counter_names:
@@ -44,14 +43,16 @@
                 image,
                 npoints,
                 npoints_per_file,
                 lima_dirname,
                 scannr,
                 sequence,
             )
+
+        scan["end_time"] = datetime.now().astimezone().isoformat()
     return dataset_filename
 
 
 def _save_counter(scan: h5py.Group, name: str, npoints: int) -> None:
     diode = _add_detector(scan, name)
     diode["data"] = numpy.arange(npoints)
```

### Comparing `ewoksdata-0.2.7/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.3.0/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.3.0/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.3.0/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.7/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.3.0/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

