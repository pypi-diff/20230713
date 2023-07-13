# Comparing `tmp/icecube-skyreader-1.2.1.tar.gz` & `tmp/icecube-skyreader-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skyreader-1.2.1.tar", last modified: Thu Jul 13 19:21:25 2023, max compression
+gzip compressed data, was "icecube-skyreader-1.2.2.tar", last modified: Thu Jul 13 21:16:51 2023, max compression
```

## Comparing `icecube-skyreader-1.2.1.tar` & `icecube-skyreader-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 19:21:25.000000 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-13 19:21:25.000000 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 19:21:25.000000 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-13 19:21:25.000000 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 19:21:25.000000 icecube-skyreader-1.2.1/icecube_skyreader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/skyreader/
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 19:21:22.000000 icecube-skyreader-1.2.1/skyreader/__init__.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/skyreader/event_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 19:21:25.501441 icecube-skyreader-1.2.1/skyreader/plot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/skyreader/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9057 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/skyreader/plot/plotting_tools.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/skyreader/py.typed
--rw-r--r--   0 root         (0) root         (0)    47000 2023-07-13 19:21:21.000000 icecube-skyreader-1.2.1/skyreader/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.305630 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-13 21:16:51.000000 icecube-skyreader-1.2.2/icecube_skyreader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.305630 icecube-skyreader-1.2.2/skyreader/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-13 21:16:48.000000 icecube-skyreader-1.2.2/skyreader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/event_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 21:16:51.309630 icecube-skyreader-1.2.2/skyreader/plot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9057 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/plot/plotting_tools.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/py.typed
+-rw-r--r--   0 root         (0) root         (0)    47135 2023-07-13 21:16:47.000000 icecube-skyreader-1.2.2/skyreader/result.py
```

### Comparing `icecube-skyreader-1.2.1/LICENSE` & `icecube-skyreader-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.1/PKG-INFO` & `icecube-skyreader-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.1
+Version: 1.2.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.1/README.md` & `icecube-skyreader-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.1/icecube_skyreader.egg-info/PKG-INFO` & `icecube-skyreader-1.2.2/icecube_skyreader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skyreader
-Version: 1.2.1
+Version: 1.2.2
 Summary: An API for Results Produced by SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skyreader
 Download-URL: https://pypi.org/project/icecube-skyreader/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skyreader/issues
```

### Comparing `icecube-skyreader-1.2.1/setup.cfg` & `icecube-skyreader-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.1/skyreader/__init__.py` & `icecube-skyreader-1.2.2/skyreader/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skyreader-1.2.1/skyreader/event_metadata.py` & `icecube-skyreader-1.2.2/skyreader/event_metadata.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.1/skyreader/plot/plotting_tools.py` & `icecube-skyreader-1.2.2/skyreader/plot/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `icecube-skyreader-1.2.1/skyreader/result.py` & `icecube-skyreader-1.2.2/skyreader/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,19 @@
         extension: str,
         output_dir: Union[str, Path, None] = None
     ) -> Path:
         """Make a filepath for writing representations of `self` to disk."""
         if not extension.startswith('.'):
             extension = '.' + extension
 
-        filename = Path(f"{str(event_metadata)}_{self.get_nside_string()}{extension}")
+        if nside_string := self.get_nside_string():
+            filename = Path(f"{str(event_metadata)}_{nside_string}{extension}")
+        else:
+            raise ValueError("cannot create filename for an empty result")
+
         if output_dir is not None:
             filename = output_dir / Path(filename)
         return filename
 
     """
     NPZ input / output
     """
```

