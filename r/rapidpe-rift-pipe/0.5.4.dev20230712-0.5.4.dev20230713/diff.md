# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230712.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.4.dev20230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230712.tar", last modified: Wed Jul 12 05:15:41 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230713.tar", last modified: Thu Jul 13 05:15:59 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230712.tar` & `rapidpe_rift_pipe-0.5.4.dev20230713.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.189999 rapidpe_rift_pipe-0.5.4.dev20230712/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-12 05:15:41.189999 rapidpe_rift_pipe-0.5.4.dev20230712/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.184999 rapidpe_rift_pipe-0.5.4.dev20230712/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.186999 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-12 05:15:41.190999 rapidpe_rift_pipe-0.5.4.dev20230712/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.184999 rapidpe_rift_pipe-0.5.4.dev20230712/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.187999 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.188999 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.189999 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.189999 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-12 05:15:30.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:15:41.188999 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-12 05:15:41.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 05:15:40.000000 rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.761347 rapidpe_rift_pipe-0.5.4.dev20230713/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-13 05:15:59.761347 rapidpe_rift_pipe-0.5.4.dev20230713/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.752347 rapidpe_rift_pipe-0.5.4.dev20230713/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.755347 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-13 05:15:59.762348 rapidpe_rift_pipe-0.5.4.dev20230713/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.753347 rapidpe_rift_pipe-0.5.4.dev20230713/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.758347 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-10 17:53:47.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.760347 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 05:15:42.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.761347 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 05:15:42.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-07 05:15:05.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.761347 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-13 05:15:42.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-06 05:13:38.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 05:15:59.760347 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 05:15:59.000000 rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/COPYING` & `rapidpe_rift_pipe-0.5.4.dev20230713/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230712
+Name: rapidpe-rift-pipe
+Version: 0.5.4.dev20230713
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/setup.cfg` & `rapidpe_rift_pipe-0.5.4.dev20230713/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 	= src
 install_requires = 
 	numpy
 	matplotlib
 	h5py
 	tabulate
 	astropy
-	lalsuite
+	lalsuite!=7.15
 	gwpy>=3.0.4
 	rift==0.0.15.9
 	rapid_pe>=0.1.0,<0.2.0
 scripts = 
 	bin/postscripts/convert_result_to_txt.py
 	bin/postscripts/create_summarypage.py
 	bin/postscripts/compute_posterior.py
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230712
+tag_build = dev.20230713
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230713/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230712
+Name: rapidpe_rift_pipe
+Version: 0.5.4.dev20230713
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230712/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.4.dev20230713/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

