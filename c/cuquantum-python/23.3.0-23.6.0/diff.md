# Comparing `tmp/cuquantum-python-23.3.0.tar.gz` & `tmp/cuquantum-python-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuquantum-python-23.3.0.tar", last modified: Thu Mar 30 06:35:15 2023, max compression
+gzip compressed data, was "cuquantum-python-23.6.0.tar", last modified: Tue Jul 11 03:51:23 2023, max compression
```

## Comparing `cuquantum-python-23.3.0.tar` & `cuquantum-python-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:35:15.091996 cuquantum-python-23.3.0/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-03-30 06:20:23.000000 cuquantum-python-23.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2016 2023-03-30 06:35:15.087996 cuquantum-python-23.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-03-30 06:20:23.000000 cuquantum-python-23.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     8862 2023-03-30 06:20:23.000000 cuquantum-python-23.3.0/cuda_autodetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:35:15.087996 cuquantum-python-23.3.0/cuquantum_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2016 2023-03-30 06:35:15.000000 cuquantum-python-23.3.0/cuquantum_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-03-30 06:35:15.000000 cuquantum-python-23.3.0/cuquantum_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 06:35:15.000000 cuquantum-python-23.3.0/cuquantum_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 06:35:15.000000 cuquantum-python-23.3.0/cuquantum_python.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-30 06:35:15.000000 cuquantum-python-23.3.0/cuquantum_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 06:35:15.091996 cuquantum-python-23.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2600 2023-03-30 06:20:23.000000 cuquantum-python-23.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     8953 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/cuda_autodetect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/cuquantum_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 03:51:23.000000 cuquantum-python-23.6.0/cuquantum_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:51:23.900126 cuquantum-python-23.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-07-11 03:36:36.000000 cuquantum-python-23.6.0/setup.py
```

### Comparing `cuquantum-python-23.3.0/LICENSE` & `cuquantum-python-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuquantum-python-23.3.0/PKG-INFO` & `cuquantum-python-23.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum-python
-Version: 23.3.0
+Version: 23.6.0
 Summary: NVIDIA cuQuantum Python
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
@@ -25,26 +25,29 @@
 NVIDIA cuQuantum Python provides Python bindings and high-level object-oriented models for accessing the full functionalities of NVIDIA cuQuantum SDK from Python.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum-python
+   pip install -v --no-cache-dir cuquantum-python
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-python-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-python-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 Citing cuQuantum
 ================
 
 Pleae click this Zenodo badge to see the citation format: |DOI|
 
 .. |DOI| image:: https://zenodo.org/badge/435003852.svg
     :target: https://zenodo.org/badge/latestdoi/435003852
```

### Comparing `cuquantum-python-23.3.0/README.rst` & `cuquantum-python-23.6.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 NVIDIA cuQuantum Python provides Python bindings and high-level object-oriented models for accessing the full functionalities of NVIDIA cuQuantum SDK from Python.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum-python
+   pip install -v --no-cache-dir cuquantum-python
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-python-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-python-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 Citing cuQuantum
 ================
 
 Pleae click this Zenodo badge to see the citation format: |DOI|
 
 .. |DOI| image:: https://zenodo.org/badge/435003852.svg
     :target: https://zenodo.org/badge/latestdoi/435003852
```

### Comparing `cuquantum-python-23.3.0/cuda_autodetect.py` & `cuquantum-python-23.6.0/cuda_autodetect.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 # the caller
 PACKAGE_NAME = ''
 PACKAGE_SUPPORTED_CUDA_VER = []
 
 # ========================================================================
 
 PACKAGE_RESOLUTION = None
+CUDA_RESOLUTION = None
 
 
 class AutoDetectionFailed(Exception):
     def __str__(self) -> str:
         return f'''
 \n\n============================================================
 {super().__str__()}
@@ -210,26 +211,28 @@
              "WARNING: Unable to detect NVIDIA CUDA Toolkit installation, assuming\n"
              "WARNING: CUDA 11 is in use... This behavior is subject to future change.\n"
              f"WARNING: To be explicit, instead of \"pip install {PACKAGE_NAME}\" run\n"
              f"WARNING: \"pip install {PACKAGE_NAME}-cuXX\", with XX being the major\n"
              "WARNING: version of your CUDA Toolkit installation.\n"
              "************************************************************************\n\n")
         to_install = _cuda_version_to_package(11080)
+        version = -1
 
     # Disallow -cu11 & -cu12 wheels from coexisting
     if len(installed) > 1 or (len(installed) == 1 and installed[0] != to_install):
         raise AutoDetectionFailed(
             f'You already have the {PACKAGE_NAME} package(s) installed: \n'
             f'  {installed}\n'
             'while you attempt to install:\n'
             f'  {to_install}\n'
             'Please uninstall all of them first, then try reinstalling.')
 
-    global PACKAGE_RESOLUTION
+    global PACKAGE_RESOLUTION, CUDA_RESOLUTION
     PACKAGE_RESOLUTION = to_install
+    CUDA_RESOLUTION = version
     _log(f"Installing {to_install}...")
     return to_install
 
 
 # "Public" API to the caller
 if _bdist_wheel is not None:
```

### Comparing `cuquantum-python-23.3.0/cuquantum_python.egg-info/PKG-INFO` & `cuquantum-python-23.6.0/cuquantum_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum-python
-Version: 23.3.0
+Version: 23.6.0
 Summary: NVIDIA cuQuantum Python
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
@@ -25,26 +25,29 @@
 NVIDIA cuQuantum Python provides Python bindings and high-level object-oriented models for accessing the full functionalities of NVIDIA cuQuantum SDK from Python.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum-python
+   pip install -v --no-cache-dir cuquantum-python
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-python-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-python-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 Citing cuQuantum
 ================
 
 Pleae click this Zenodo badge to see the citation format: |DOI|
 
 .. |DOI| image:: https://zenodo.org/badge/435003852.svg
     :target: https://zenodo.org/badge/latestdoi/435003852
```

### Comparing `cuquantum-python-23.3.0/setup.py` & `cuquantum-python-23.6.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import shutil
 import site
 import subprocess
 import sys
 
 from setuptools import setup
 
+import cuda_autodetect
 from cuda_autodetect import infer_best_package, bdist_wheel
 
 
 # Update this for every release
 # Must pin to the cuquantum-python-cuXX version
-package_ver = "23.03.0"
+package_ver = "23.06.0"
 package_name = "cuquantum-python"
 
 
 # get project long description
 with open("README.rst") as f:
     long_description = f.read()
 
@@ -34,14 +35,26 @@
     # Case 1: generate sdist
     install_requires = []
     data_files = [('', ['cuda_autodetect.py',])]  # extra files to be copied into sdist
     cmdclass = {}
 else:
     # Case 2: install sdist
     install_requires = [f"{infer_best_package(package_name)}=={package_ver}",]
+    if 11000 <= cuda_autodetect.CUDA_RESOLUTION < 11010:
+        install_requires.append('cupy-cuda110')
+    elif 11010 <= cuda_autodetect.CUDA_RESOLUTION < 11020:
+        install_requires.append('cupy-cuda111')
+    elif 11020 <= cuda_autodetect.CUDA_RESOLUTION < 12000:
+        install_requires.append('cupy-cuda11x')
+    elif 12000 <= cuda_autodetect.CUDA_RESOLUTION < 13000:
+        # no ambiguity for CUDA 12, cuquantum-python-cu12 would do the right thing
+        pass
+    else:
+        # most likely we failed to detect the CUDA version, assume CUDA 11.2+
+        install_requires.append('cupy-cuda11x')
     data_files = []
     cmdclass = {'bdist_wheel': bdist_wheel} if bdist_wheel is not None else {}
 
 
 setup(
     name=package_name,
     version=package_ver,
```

