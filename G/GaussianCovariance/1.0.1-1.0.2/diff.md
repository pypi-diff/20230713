# Comparing `tmp/GaussianCovariance-1.0.1.tar.gz` & `tmp/GaussianCovariance-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GaussianCovariance-1.0.1.tar", last modified: Thu Jul 13 18:13:59 2023, max compression
+gzip compressed data, was "GaussianCovariance-1.0.2.tar", last modified: Thu Jul 13 18:47:47 2023, max compression
```

## Comparing `GaussianCovariance-1.0.1.tar` & `GaussianCovariance-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:13:59.425599 GaussianCovariance-1.0.1/
-drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:13:59.410663 GaussianCovariance-1.0.1/GaussianCovariance/
--rw-r--r--   0 alfonso    (502) staff       (20)       34 2022-10-07 09:25:24.000000 GaussianCovariance-1.0.1/GaussianCovariance/__init__.py
--rw-r--r--   0 alfonso    (502) staff       (20)     9460 2022-10-27 12:00:21.000000 GaussianCovariance-1.0.1/GaussianCovariance/gaussian_covariance.py
-drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:13:59.418925 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/
--rw-r--r--   0 alfonso    (502) staff       (20)     1407 2023-07-13 18:13:59.000000 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/PKG-INFO
--rw-r--r--   0 alfonso    (502) staff       (20)      327 2023-07-13 18:13:59.000000 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/SOURCES.txt
--rw-r--r--   0 alfonso    (502) staff       (20)        1 2023-07-13 18:13:59.000000 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/dependency_links.txt
--rw-r--r--   0 alfonso    (502) staff       (20)       12 2023-07-13 18:13:59.000000 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/requires.txt
--rw-r--r--   0 alfonso    (502) staff       (20)       19 2023-07-13 18:13:59.000000 GaussianCovariance-1.0.1/GaussianCovariance.egg-info/top_level.txt
--rw-r--r--   0 alfonso    (502) staff       (20)    35098 2023-07-13 17:55:33.000000 GaussianCovariance-1.0.1/LICENSE
--rw-r--r--   0 alfonso    (502) staff       (20)     1407 2023-07-13 18:13:59.422353 GaussianCovariance-1.0.1/PKG-INFO
--rw-r--r--   0 alfonso    (502) staff       (20)      624 2023-07-13 17:55:33.000000 GaussianCovariance-1.0.1/README.md
--rw-r--r--   0 alfonso    (502) staff       (20)      779 2023-07-13 18:13:39.000000 GaussianCovariance-1.0.1/pyproject.toml
--rw-r--r--   0 alfonso    (502) staff       (20)       38 2023-07-13 18:13:59.426015 GaussianCovariance-1.0.1/setup.cfg
--rw-r--r--   0 alfonso    (502) staff       (20)      627 2023-07-13 18:13:41.000000 GaussianCovariance-1.0.1/setup.py
+drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:47:47.223763 GaussianCovariance-1.0.2/
+drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:47:47.220701 GaussianCovariance-1.0.2/GaussianCovariance/
+-rw-r--r--   0 alfonso    (502) staff       (20)       34 2022-10-07 09:25:24.000000 GaussianCovariance-1.0.2/GaussianCovariance/__init__.py
+-rw-r--r--   0 alfonso    (502) staff       (20)     9460 2022-10-27 12:00:21.000000 GaussianCovariance-1.0.2/GaussianCovariance/gaussian_covariance.py
+drwxr-xr-x   0 alfonso    (502) staff       (20)        0 2023-07-13 18:47:47.222995 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/
+-rw-r--r--   0 alfonso    (502) staff       (20)     1407 2023-07-13 18:47:47.000000 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/PKG-INFO
+-rw-r--r--   0 alfonso    (502) staff       (20)      327 2023-07-13 18:47:47.000000 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/SOURCES.txt
+-rw-r--r--   0 alfonso    (502) staff       (20)        1 2023-07-13 18:47:47.000000 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/dependency_links.txt
+-rw-r--r--   0 alfonso    (502) staff       (20)       12 2023-07-13 18:47:47.000000 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/requires.txt
+-rw-r--r--   0 alfonso    (502) staff       (20)       19 2023-07-13 18:47:47.000000 GaussianCovariance-1.0.2/GaussianCovariance.egg-info/top_level.txt
+-rw-r--r--   0 alfonso    (502) staff       (20)    35098 2023-07-13 17:55:33.000000 GaussianCovariance-1.0.2/LICENSE
+-rw-r--r--   0 alfonso    (502) staff       (20)     1407 2023-07-13 18:47:47.223421 GaussianCovariance-1.0.2/PKG-INFO
+-rw-r--r--   0 alfonso    (502) staff       (20)      624 2023-07-13 17:55:33.000000 GaussianCovariance-1.0.2/README.md
+-rw-r--r--   0 alfonso    (502) staff       (20)      780 2023-07-13 18:45:10.000000 GaussianCovariance-1.0.2/pyproject.toml
+-rw-r--r--   0 alfonso    (502) staff       (20)       38 2023-07-13 18:47:47.223886 GaussianCovariance-1.0.2/setup.cfg
+-rw-r--r--   0 alfonso    (502) staff       (20)      628 2023-07-13 18:45:00.000000 GaussianCovariance-1.0.2/setup.py
```

### Comparing `GaussianCovariance-1.0.1/GaussianCovariance/gaussian_covariance.py` & `GaussianCovariance-1.0.2/GaussianCovariance/gaussian_covariance.py`

 * *Files identical despite different names*

### Comparing `GaussianCovariance-1.0.1/GaussianCovariance.egg-info/PKG-INFO` & `GaussianCovariance-1.0.2/GaussianCovariance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GaussianCovariance
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Module to compute the covariance of two-point clustering statistics
 Home-page: https://gitlab.com/veropalumbo.alfonso/gaussiancovariance
 Author: Alfonso Veropalumbo
 Author-email: Alfonso Veropalumbo <alfonso.veropalumbo@inaf.it>, Elena Sarpa <sarpa@cppm.in2p3.fr>
 Project-URL: Homepage, https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/
 Project-URL: Bug Tracker, https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GaussianCovariance-1.0.1/LICENSE` & `GaussianCovariance-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GaussianCovariance-1.0.1/PKG-INFO` & `GaussianCovariance-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GaussianCovariance
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Module to compute the covariance of two-point clustering statistics
 Home-page: https://gitlab.com/veropalumbo.alfonso/gaussiancovariance
 Author: Alfonso Veropalumbo
 Author-email: Alfonso Veropalumbo <alfonso.veropalumbo@inaf.it>, Elena Sarpa <sarpa@cppm.in2p3.fr>
 Project-URL: Homepage, https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/
 Project-URL: Bug Tracker, https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GaussianCovariance-1.0.1/README.md` & `GaussianCovariance-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `GaussianCovariance-1.0.1/pyproject.toml` & `GaussianCovariance-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GaussianCovariance"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Alfonso Veropalumbo", email="alfonso.veropalumbo@inaf.it" },
   { name="Elena Sarpa", email="sarpa@cppm.in2p3.fr" },
 ]
 description = "Python Module to compute the covariance of two-point clustering statistics"
 readme = "README.md"
 requires-python = ">=3.6"
@@ -16,8 +16,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/"
-"Bug Tracker" = "https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/issues"
+"Bug Tracker" = "https://gitlab.com/veropalumbo.alfonso/gaussiancovariance/issues"
```

### Comparing `GaussianCovariance-1.0.1/setup.py` & `GaussianCovariance-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="GaussianCovariances",
-    version="1.0.1",
+    version="1.0.2",
     author="Alfonso Veropalumbo",
     author_email="alfonso.veropalumbo@inaf.it",
     description="Python Module to compute the gaussian covariance of two-point clustering probes.",
     long_description_content_type="text/markdown",
     url="https://gitlab.com/veropalumbo.alfonso/gaussiancovariance",
     package_dir={"": "."},
     packages=['GaussianCovariance'],
     python_requires=">=3.6",
     install_requires=["numpy", "scipy"]
-)
+)
```

