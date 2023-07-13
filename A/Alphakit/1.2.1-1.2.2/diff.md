# Comparing `tmp/Alphakit-1.2.1.tar.gz` & `tmp/Alphakit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Alphakit-1.2.1.tar", last modified: Thu Jul 13 06:29:33 2023, max compression
+gzip compressed data, was "dist/Alphakit-1.2.2.tar", last modified: Thu Jul 13 08:25:12 2023, max compression
```

## Comparing `Alphakit-1.2.1.tar` & `Alphakit-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      764 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 06:29:33.000000 Alphakit-1.2.1/Alphakit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-13 05:13:18.000000 Alphakit-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      215 2023-07-13 06:29:33.000000 Alphakit-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-05 02:25:31.000000 Alphakit-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-13 06:28:35.000000 Alphakit-1.2.1/alphakit/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117998 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/const.c
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/const.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/data/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)   774588 2023-07-13 06:26:18.000000 Alphakit-1.2.1/alphakit/data/calculator.c
--rw-r--r--   0 root         (0) root         (0)     7937 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/data/calculator.pyx
--rw-r--r--   0 root         (0) root         (0)   162253 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/data/processing.c
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/data/processing.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/factor/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/factor/__init__.py
--rw-r--r--   0 root         (0) root         (0)   287606 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/analysis.c
--rw-r--r--   0 root         (0) root         (0)     3799 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/analysis.pyx
--rw-r--r--   0 root         (0) root         (0)   361294 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/metrics.c
--rw-r--r--   0 root         (0) root         (0)     4267 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/metrics.pyx
--rw-r--r--   0 root         (0) root         (0)   299502 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/processing.c
--rw-r--r--   0 root         (0) root         (0)     4718 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/processing.pyx
--rw-r--r--   0 root         (0) root         (0)   212245 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/factor/transform.c
--rw-r--r--   0 root         (0) root         (0)     1504 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/factor/transform.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/alphakit/portfolio/
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 02:26:44.000000 Alphakit-1.2.1/alphakit/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)   147280 2023-07-13 06:26:17.000000 Alphakit-1.2.1/alphakit/portfolio/combine.c
--rw-r--r--   0 root         (0) root         (0)      480 2023-07-13 05:13:18.000000 Alphakit-1.2.1/alphakit/portfolio/combine.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:29:33.000000 Alphakit-1.2.1/requirements/
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-05 02:25:31.000000 Alphakit-1.2.1/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 06:29:33.000000 Alphakit-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3356 2023-07-13 05:13:18.000000 Alphakit-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-13 08:25:12.000000 Alphakit-1.2.2/Alphakit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-05 02:25:31.000000 Alphakit-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-13 05:13:18.000000 Alphakit-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-13 08:25:12.000000 Alphakit-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-05 02:25:31.000000 Alphakit-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/alphakit/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-13 07:49:01.000000 Alphakit-1.2.2/alphakit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117998 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/const.c
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/const.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/alphakit/data/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-13 08:23:58.000000 Alphakit-1.2.2/alphakit/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   774588 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/data/calculator.c
+-rw-r--r--   0 root         (0) root         (0)     7937 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/data/calculator.pyx
+-rw-r--r--   0 root         (0) root         (0)   162253 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/data/processing.c
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/data/processing.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/alphakit/factor/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-13 08:24:38.000000 Alphakit-1.2.2/alphakit/factor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   287606 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/factor/analysis.c
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/factor/analysis.pyx
+-rw-r--r--   0 root         (0) root         (0)   361294 2023-07-13 07:49:55.000000 Alphakit-1.2.2/alphakit/factor/metrics.c
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/factor/metrics.pyx
+-rw-r--r--   0 root         (0) root         (0)   299502 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/factor/processing.c
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/factor/processing.pyx
+-rw-r--r--   0 root         (0) root         (0)   212245 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/factor/transform.c
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/factor/transform.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/alphakit/portfolio/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-13 08:24:57.000000 Alphakit-1.2.2/alphakit/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   147280 2023-07-13 08:21:32.000000 Alphakit-1.2.2/alphakit/portfolio/combine.c
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-13 05:13:18.000000 Alphakit-1.2.2/alphakit/portfolio/combine.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 08:25:12.000000 Alphakit-1.2.2/requirements/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-05 02:25:31.000000 Alphakit-1.2.2/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 08:25:12.000000 Alphakit-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-07-13 08:20:57.000000 Alphakit-1.2.2/setup.py
```

### Comparing `Alphakit-1.2.1/Alphakit.egg-info/SOURCES.txt` & `Alphakit-1.2.2/Alphakit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./README.md
 Alphakit.egg-info/PKG-INFO
 Alphakit.egg-info/SOURCES.txt
 Alphakit.egg-info/dependency_links.txt
```

### Comparing `Alphakit-1.2.1/alphakit/const.c` & `Alphakit-1.2.2/alphakit/const.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/const.pyx` & `Alphakit-1.2.2/alphakit/const.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/data/calculator.c` & `Alphakit-1.2.2/alphakit/data/calculator.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/data/calculator.pyx` & `Alphakit-1.2.2/alphakit/data/calculator.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/data/processing.c` & `Alphakit-1.2.2/alphakit/data/processing.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/data/processing.pyx` & `Alphakit-1.2.2/alphakit/data/processing.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/analysis.c` & `Alphakit-1.2.2/alphakit/factor/analysis.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/analysis.pyx` & `Alphakit-1.2.2/alphakit/factor/analysis.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/metrics.c` & `Alphakit-1.2.2/alphakit/factor/metrics.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/metrics.pyx` & `Alphakit-1.2.2/alphakit/factor/metrics.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/processing.c` & `Alphakit-1.2.2/alphakit/factor/processing.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/processing.pyx` & `Alphakit-1.2.2/alphakit/factor/processing.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/transform.c` & `Alphakit-1.2.2/alphakit/factor/transform.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/factor/transform.pyx` & `Alphakit-1.2.2/alphakit/factor/transform.pyx`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/alphakit/portfolio/combine.c` & `Alphakit-1.2.2/alphakit/portfolio/combine.c`

 * *Files identical despite different names*

### Comparing `Alphakit-1.2.1/setup.py` & `Alphakit-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+
 from Cython.Build import cythonize
 from setuptools import setup
 from setuptools import find_packages
 from distutils.cmd import Command
 from distutils.extension import Extension
 import os, sys, io, subprocess, platform
 from alphakit import __version__
@@ -26,14 +27,15 @@
 if "--line_trace" in sys.argv:
     line_trace = True
     print("Build with line trace enabled ...")
     sys.argv.remove("--line_trace")
 else:
     line_trace = False
 
+
 class version_build(Command):
 
     description = "test the distribution prior to install"
 
     user_options = [
         ('test-dir=', None, "directory that contains the test definitions"),
     ]
@@ -42,15 +44,15 @@
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         git_ver = git_version()[:10]
-        configFile = 'alphakit/__init__.py'
+        configFile = 'hermes/__init__.py'
 
         file_handle = open(configFile, 'r')
         lines = file_handle.readlines()
         newFiles = []
         for line in lines:
             if line.startswith('__version__'):
                 line = line.split('+')[0].rstrip()
@@ -67,18 +69,21 @@
 
 if platform.system() != "Windows":
     import multiprocessing
     n_cpu = multiprocessing.cpu_count()
 else:
     n_cpu = 0
 
-ext_modules = ['alphakit/data/calculator.pyx','alphakit/data/processing.pyx',
-               'alphakit/factor/analysis.pyx','alphakit/factor/metrics.pyx',
-               'alphakit/factor/processing.pyx','alphakit/factor/transform.pyx',
-               'alphakit/portfolio/combine.pyx','alphakit/const.pyx']
+ext_modules = [
+    'alphakit/factor/metrics.pyx', 'alphakit/factor/analysis.pyx',
+    'alphakit/factor/processing.pyx', 'alphakit/factor/transform.pyx',
+    'alphakit/data/calculator.pyx', 'alphakit/data/processing.pyx',
+    'alphakit/portfolio/combine.pyx', 'alphakit/const.pyx'
+]
+
 
 def generate_extensions(ext_modules, line_trace=True):
 
     extensions = []
 
     if line_trace:
         print("define cython trace to True ...")
@@ -97,19 +102,18 @@
 ext_modules_settings = cythonize(generate_extensions(ext_modules, line_trace),
                                  compiler_directives={
                                      'embedsignature': True,
                                      'linetrace': line_trace
                                  },
                                  nthreads=n_cpu)
 
-
 setup(name=NAME,
       version=VERSION,
       description=DESCRIPTION,
       author=AUTHOR,
       author_email=AUTHOR_EMAIL,
       url=URL,
       ext_modules=ext_modules_settings,
       packages=find_packages(),
       include_package_data=False,
       install_requires=io.open(requirements, encoding='utf8').read(),
-      classifiers=[])
+      classifiers=[])
```

