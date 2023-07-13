# Comparing `tmp/IS2view-0.0.3.tar.gz` & `tmp/IS2view-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IS2view-0.0.3.tar", last modified: Thu Jul  6 19:35:59 2023, max compression
+gzip compressed data, was "IS2view-0.0.4.tar", last modified: Thu Jul 13 05:14:58 2023, max compression
```

## Comparing `IS2view-0.0.3.tar` & `IS2view-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 19:35:49.000000 IS2view-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-06 19:35:49.000000 IS2view-0.0.3/CONTRIBUTORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/IS2view/
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    66749 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    14581 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    46061 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/IS2view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-06 19:35:49.000000 IS2view-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-06 19:35:49.000000 IS2view-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-06 19:35:59.993704 IS2view-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-06 19:35:49.000000 IS2view-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-06 19:35:49.000000 IS2view-0.0.3/postBuild
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-06 19:35:49.000000 IS2view-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-06 19:35:49.000000 IS2view-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 19:35:59.993704 IS2view-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-07-06 19:35:49.000000 IS2view-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-06 19:35:49.000000 IS2view-0.0.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 05:14:58.881585 IS2view-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-13 05:14:46.000000 IS2view-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     5545 2023-07-13 05:14:46.000000 IS2view-0.0.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-13 05:14:46.000000 IS2view-0.0.4/CONTRIBUTORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 05:14:58.877585 IS2view-0.0.4/IS2view/
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66157 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14370 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45866 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-13 05:14:46.000000 IS2view-0.0.4/IS2view/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-13 05:14:58.881585 IS2view-0.0.4/IS2view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-13 05:14:58.000000 IS2view-0.0.4/IS2view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-13 05:14:58.000000 IS2view-0.0.4/IS2view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-13 05:14:58.000000 IS2view-0.0.4/IS2view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-13 05:14:58.000000 IS2view-0.0.4/IS2view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-13 05:14:58.000000 IS2view-0.0.4/IS2view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-13 05:14:46.000000 IS2view-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-13 05:14:46.000000 IS2view-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-13 05:14:58.881585 IS2view-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-13 05:14:46.000000 IS2view-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-13 05:14:46.000000 IS2view-0.0.4/postBuild
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-13 05:14:46.000000 IS2view-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-13 05:14:46.000000 IS2view-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-13 05:14:58.881585 IS2view-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-07-13 05:14:46.000000 IS2view-0.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-13 05:14:46.000000 IS2view-0.0.4/version.txt
```

### Comparing `IS2view-0.0.3/.gitignore` & `IS2view-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.3/IS2view/__init__.py` & `IS2view-0.0.4/IS2view/__init__.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.3/IS2view/api.py` & `IS2view-0.0.4/IS2view/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,82 +25,66 @@
     xarray: N-D labeled arrays and datasets in Python
         https://docs.xarray.dev/en/stable/
 
 UPDATE HISTORY:
     Updated 07/2023: renamed module from IS2view.py to api.py
         add plot functions for map basemaps and added geometries
         add imshow function for visualizing current leaflet map
+        use logging instead of warnings for import attempts
     Updated 06/2023: moved widgets functions to separate moddule
     Updated 12/2022: added case for warping input image
     Updated 11/2022: modifications for dask-chunked rasters
     Written 07/2022
 """
 import io
 import os
 import copy
 import json
 import base64
 import asyncio
 import logging
-import warnings
 import numpy as np
 import collections.abc
 from traitlets import HasTraits, Float, Tuple, observe
 from traitlets.utils.bunch import Bunch
 
 # attempt imports
 try:
     import geopandas as gpd
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("geopandas not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("geopandas not available")
 try:
     import ipywidgets
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("ipywidgets not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("ipywidgets not available")
 try:
     import ipyleaflet
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("ipyleaflet not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("ipyleaflet not available")
 try:
     import matplotlib
     import matplotlib.cm as cm
     import matplotlib.colorbar
     import matplotlib.pyplot as plt
     import matplotlib.colors as colors
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("matplotlib not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.critical("matplotlib not available")
 try:
     import owslib.wms
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("owslib not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("owslib not available")
 try:
     import rasterio.transform
     import rasterio.warp
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("rasterio not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.critical("rasterio not available")
 try:
     import xarray as xr
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("xarray not available")
-    warnings.warn("Some functions will throw an exception if called")
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("xarray not available")
 
 # set environmental variable for anonymous s3 access
 os.environ['AWS_NO_SIGN_REQUEST'] = 'YES'
 
 # map projections
 projections = {}
 projections['EPSG:3857'] = dict(name='EPSG3857', custom=False),
@@ -450,14 +434,17 @@
         bbox[0] = self.map.crs['origin'][0] + left*resolution
         bbox[1] = self.map.crs['origin'][1] - bottom*resolution
         bbox[2] = self.map.crs['origin'][0] + right*resolution
         bbox[3] = self.map.crs['origin'][1] - top*resolution
         kwargs.setdefault('bbox', bbox)
         # create WMS request for basemap image at bounds and resolution
         srs = kwargs['srs'].replace(':', '').lower()
+        # url of NASA Global Imagery Browse Services (GIBS)
+        # https://wiki.earthdata.nasa.gov/display/GIBS
+        # https://worldview.earthdata.nasa.gov/
         url = f'https://gibs.earthdata.nasa.gov/wms/{srs}/best/wms.cgi?'
         wms = owslib.wms.WebMapService(url=url, version='1.1.1')
         basemap = wms.getmap(**kwargs)
         # read WMS layer and plot
         img = plt.imread(io.BytesIO(basemap.read()))
         ax.imshow(img, extent=[bbox[0],bbox[2],bbox[1],bbox[3]])
```

### Comparing `IS2view-0.0.3/IS2view/convert.py` & `IS2view-0.0.4/IS2view/convert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 """
 convert.py
-Written by Tyler Sutterley (06/2023)
+Written by Tyler Sutterley (07/2023)
 Utilities for converting gridded ICESat-2 files from native netCDF4
 
 PYTHON DEPENDENCIES:
     netCDF4: Python interface to the netCDF C library
         https://unidata.github.io/netcdf4-python/netCDF4/index.html
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     xarray: N-D labeled arrays and datasets in Python
         https://docs.xarray.dev/en/stable/
 
 UPDATE HISTORY:
+    Updated 07/2023: use logging instead of warnings for import attempts
     Updated 06/2023: using pathlib to define and expand paths
     Updated 11/2022: output variables and attributes in top-level group
         use netCDF4 directly due to changes in xarray backends
     Written 07/2022
 """
 import logging
 import pathlib
-import warnings
 import numpy as np
 
 # attempt imports
 try:
     import netCDF4
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("netCDF4 not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.critical("netCDF4 not available")
 try:
     import xarray as xr
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("xarray not available")
-    warnings.warn("Some functions will throw an exception if called")
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("xarray not available")
 
 class convert():
     np.seterr(invalid='ignore')
     def __init__(self, filename=None, output=None):
         """Utilities for converting gridded ICESat-2 files from native netCDF4
 
         Parameters
```

### Comparing `IS2view-0.0.3/IS2view/io.py` & `IS2view-0.0.4/IS2view/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 io.py
-Written by Tyler Sutterley (11/2022)
+Written by Tyler Sutterley (07/2023)
 Utilities for reading gridded ICESat-2 files using rasterio and xarray
 
 PYTHON DEPENDENCIES:
     netCDF4: Python interface to the netCDF C library
         https://unidata.github.io/netcdf4-python/netCDF4/index.html
     numpy: Scientific Computing Tools For Python
         https://numpy.org
@@ -14,36 +14,30 @@
         https://rasterio.readthedocs.io
     rioxarray: geospatial xarray extension powered by rasterio
         https://github.com/corteva/rioxarray
     xarray: N-D labeled arrays and datasets in Python
         https://docs.xarray.dev/en/stable/
 
 UPDATE HISTORY:
+    Updated 07/2023: use logging instead of warnings for import attempts
     Written 11/2022
 """
 import os
 import logging
-import warnings
 import numpy as np
 
 # attempt imports
 try:
     import rioxarray
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("rioxarray not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.critical("rioxarray not available")
 try:
     import xarray as xr
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("xarray not available")
-    warnings.warn("Some functions will throw an exception if called")
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.critical("xarray not available")
 
 # set environmental variable for anonymous s3 access
 os.environ['AWS_NO_SIGN_REQUEST'] = 'YES'
 
 def from_file(granule, group=None, format='nc', **kwargs):
     """
     Wrapper function for reading gridded ICESat-2 files
```

### Comparing `IS2view-0.0.3/IS2view/tools.py` & `IS2view-0.0.4/IS2view/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 #!/usr/bin/env python
 u"""
 tools.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (07/2023)
 User interface tools for Jupyter Notebooks
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython
         https://ipywidgets.readthedocs.io/en/latest/
     matplotlib: Python 2D plotting library
         http://matplotlib.org/
         https://github.com/matplotlib/matplotlib
 
 UPDATE HISTORY:
+    Updated 07/2023: use logging instead of warnings for import attempts
     Updated 06/2023: moved widgets functions to separate module
     Updated 12/2022: added case for warping input image
     Updated 11/2022: modifications for dask-chunked rasters
     Written 07/2022
 """
 import os
 import copy
 import logging
-import warnings
 import numpy as np
 
 # attempt imports
 try:
     import ipywidgets
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("ipywidgets not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("ipywidgets not available")
 try:
     import matplotlib.cm as cm
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("matplotlib not available")
-    warnings.warn("Some functions will throw an exception if called")
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("matplotlib not available")
 
 # set environmental variable for anonymous s3 access
 os.environ['AWS_NO_SIGN_REQUEST'] = 'YES'
 
 class widgets:
     def __init__(self, **kwargs):
         # set default keyword options
```

### Comparing `IS2view-0.0.3/IS2view/utilities.py` & `IS2view-0.0.4/IS2view/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (06/2023)
+Written by Tyler Sutterley (07/2023)
 Download and management utilities
 
 UPDATE HISTORY:
+    Updated 07/2023: use logging instead of warnings for import attempts
     Updated 06/2023: using pathlib to define and expand paths
         add functions to retrieve and revoke NASA Earthdata User tokens
         updated netCDF4 request type for NSIDC s3 bucket CMR queries
     Updated 12/2022: functions for managing and maintaining git repositories
     Updated 11/2022: can query for zarr datasets
     Updated 10/2022: public release of NSIDC s3 access
     Written 07/2022
@@ -43,25 +44,19 @@
     from urllib.parse import urlencode
     import urllib.request as urllib2
 
 # attempt imports
 try:
     import boto3
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("boto3 not available")
-    warnings.warn("Some functions will throw an exception if called")
+    logging.debug("boto3 not available")
 try:
     import s3fs
 except (ImportError, ModuleNotFoundError) as exc:
-    warnings.filterwarnings("module")
-    warnings.warn("s3fs not available")
-    warnings.warn("Some functions will throw an exception if called")
-# ignore warnings
-warnings.filterwarnings("ignore")
+    logging.debug("s3fs not available")
 
 # PURPOSE: get absolute path within a package from a relative path
 def get_data_path(relpath: list | str | pathlib.Path):
     """
     Get the absolute path within a package from a relative path
 
     Parameters
```

### Comparing `IS2view-0.0.3/IS2view.egg-info/PKG-INFO` & `IS2view-0.0.4/IS2view.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.3
+Version: 0.0.4
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.3/LICENSE` & `IS2view-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.3/PKG-INFO` & `IS2view-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.3
+Version: 0.0.4
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `IS2view-0.0.3/README.rst` & `IS2view-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.3/setup.py` & `IS2view-0.0.4/setup.py`

 * *Files identical despite different names*

