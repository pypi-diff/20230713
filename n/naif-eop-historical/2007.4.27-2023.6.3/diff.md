# Comparing `tmp/naif_eop_historical-2007.4.27.tar.gz` & `tmp/naif_eop_historical-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naif_eop_historical-2007.4.27.tar", last modified: Thu Jun  1 17:30:58 2023, max compression
+gzip compressed data, was "naif_eop_historical-2023.6.3.tar", last modified: Thu Jul 13 15:10:41 2023, max compression
```

## Comparing `naif_eop_historical-2007.4.27.tar` & `naif_eop_historical-2023.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:58.931476 naif_eop_historical-2007.4.27/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-01 17:30:58.931476 naif_eop_historical-2007.4.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:58.927476 naif_eop_historical-2007.4.27/naif_eop_historical/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/naif_eop_historical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  8603648 2023-06-01 17:30:39.000000 naif_eop_historical-2007.4.27/naif_eop_historical/earth_720101_070426.bpc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 17:30:39.000000 naif_eop_historical-2007.4.27/naif_eop_historical/earth_720101_070426.md5
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/naif_eop_historical/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:58.931476 naif_eop_historical-2007.4.27/naif_eop_historical/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/naif_eop_historical/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/naif_eop_historical/tests/test_naif_historical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:30:58.931476 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-01 17:30:58.000000 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-01 17:30:58.000000 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:30:58.000000 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 17:30:58.000000 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 17:30:58.000000 naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-01 17:30:35.000000 naif_eop_historical-2007.4.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:30:58.931476 naif_eop_historical-2007.4.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/naif_eop_historical/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/naif_eop_historical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9780224 2023-07-13 15:10:21.000000 naif_eop_historical-2023.6.3/naif_eop_historical/earth_720101_230601.bpc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 15:10:21.000000 naif_eop_historical-2023.6.3/naif_eop_historical/earth_720101_230601.md5
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/naif_eop_historical/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/naif_eop_historical/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/naif_eop_historical/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/naif_eop_historical/tests/test_naif_historical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-13 15:10:41.000000 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-13 15:10:41.000000 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:10:41.000000 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 15:10:41.000000 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 15:10:41.000000 naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-13 15:10:15.000000 naif_eop_historical-2023.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:10:41.792824 naif_eop_historical-2023.6.3/setup.cfg
```

### Comparing `naif_eop_historical-2007.4.27/PKG-INFO` & `naif_eop_historical-2023.6.3/naif_eop_historical.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: naif_eop_historical
-Version: 2007.4.27
+Name: naif-eop-historical
+Version: 2023.6.3
 Summary: NAIF Historical Earth Orientation Parameters (EOP) Kernel for SPICE
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # naif_eop_historical: NAIF Historical Earth Orientation Parameters Kernel for SPICE
@@ -12,24 +12,24 @@
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/naif-eop-historical)](https://img.shields.io/pypi/v/naif-eop-historical)
 [![PyPi downloads](https://img.shields.io/pypi/dm/naif-eop-historical)](https://img.shields.io/pypi/dm/naif-eop-historical)  
 [![Build and Test](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml)
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml)  
 
-This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_070426_historical.bpc).
+This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_230601.bpc).
 
 **This is not an official NAIF package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`. 
 
-The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2007 APR 26 00:01:05.185
+The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2023 JUN 01 00:01:09.184
 
 ## Installation
 
-The latest version of the file can be install via pip:  
+The latest version of the file can be installed via pip:  
 `pip install naif-eop-historical`
 
 ## Usage
 ```python
 import spiceypy as sp
 from naif_eop_historical import eop_historical
```

### Comparing `naif_eop_historical-2007.4.27/README.md` & `naif_eop_historical-2023.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/naif-eop-historical)](https://img.shields.io/pypi/v/naif-eop-historical)
 [![PyPi downloads](https://img.shields.io/pypi/dm/naif-eop-historical)](https://img.shields.io/pypi/dm/naif-eop-historical)  
 [![Build and Test](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml)
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml)  
 
-This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_070426_historical.bpc).
+This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_230601.bpc).
 
 **This is not an official NAIF package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`. 
 
-The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2007 APR 26 00:01:05.185
+The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2023 JUN 01 00:01:09.184
 
 ## Installation
 
-The latest version of the file can be install via pip:  
+The latest version of the file can be installed via pip:  
 `pip install naif-eop-historical`
 
 ## Usage
 ```python
 import spiceypy as sp
 from naif_eop_historical import eop_historical
```

### Comparing `naif_eop_historical-2007.4.27/naif_eop_historical/fetch.py` & `naif_eop_historical-2023.6.3/naif_eop_historical/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import hashlib
 import os
 
 import requests
 
-URL = "https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_070426.bpc"
-FILE = os.path.join(os.path.dirname(__file__), "earth_720101_070426.bpc")
-MD5_FILE = os.path.join(os.path.dirname(__file__), "earth_720101_070426.md5")
+URL = "https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_230601.bpc"
+FILE = os.path.join(os.path.dirname(__file__), "earth_720101_230601.bpc")
+MD5_FILE = os.path.join(os.path.dirname(__file__), "earth_720101_230601.md5")
 
 
 def fetch_file(url: str, output_file: str):
     """
     Fetches the file from the given URL and saves it to the output file.
 
     Parameters
```

### Comparing `naif_eop_historical-2007.4.27/naif_eop_historical.egg-info/PKG-INFO` & `naif_eop_historical-2023.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: naif-eop-historical
-Version: 2007.4.27
+Name: naif_eop_historical
+Version: 2023.6.3
 Summary: NAIF Historical Earth Orientation Parameters (EOP) Kernel for SPICE
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # naif_eop_historical: NAIF Historical Earth Orientation Parameters Kernel for SPICE
@@ -12,24 +12,24 @@
 
 [![Python 3.7+](https://img.shields.io/badge/Python-3.7%2B-blue)](https://img.shields.io/badge/Python-3.7%2B-blue)
 [![PyPI version](https://img.shields.io/pypi/v/naif-eop-historical)](https://img.shields.io/pypi/v/naif-eop-historical)
 [![PyPi downloads](https://img.shields.io/pypi/dm/naif-eop-historical)](https://img.shields.io/pypi/dm/naif-eop-historical)  
 [![Build and Test](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test.yml)
 [![Build, Test, & Publish](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml/badge.svg)](https://github.com/B612-Asteroid-Institute/naif_eop_historical/actions/workflows/build_test_publish.yml)  
 
-This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_070426_historical.bpc).
+This package ships the Navigation and Ancillary Information Facility's high accuracy, historical Earth orientation parameters (EOP) [kernel](https://naif.jpl.nasa.gov/pub/naif/generic_kernels/pck/earth_720101_230601.bpc).
 
 **This is not an official NAIF package**. It is an automatically generated mirror of the file so that it is
 installable via `pip`. 
 
-The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2007 APR 26 00:01:05.185
+The current version of the file released on 2007 APR 27 spans the following times: 1972 JAN 01 00:00:42.183 - 2023 JUN 01 00:01:09.184
 
 ## Installation
 
-The latest version of the file can be install via pip:  
+The latest version of the file can be installed via pip:  
 `pip install naif-eop-historical`
 
 ## Usage
 ```python
 import spiceypy as sp
 from naif_eop_historical import eop_historical
```

### Comparing `naif_eop_historical-2007.4.27/pyproject.toml` & `naif_eop_historical-2023.6.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naif_eop_historical"
-version = "2007.04.27" 
+version = "2023.06.03" 
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "NAIF Historical Earth Orientation Parameters (EOP) Kernel for SPICE"
 readme = "README.md"
 requires-python = ">=3.7"
 
@@ -18,8 +18,8 @@
     "spiceypy"
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
-naif_eop_historical = ["naif_eop_historical/earth_720101_070426.bpc", "naif_eop_historical/earth_720101_070426.md5"]
+naif_eop_historical = ["naif_eop_historical/earth_720101_230601.bpc", "naif_eop_historical/earth_720101_230601.md5"]
```

