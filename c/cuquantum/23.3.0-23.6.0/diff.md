# Comparing `tmp/cuquantum-23.3.0.tar.gz` & `tmp/cuquantum-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuquantum-23.3.0.tar", last modified: Thu Mar 30 06:22:05 2023, max compression
+gzip compressed data, was "cuquantum-23.6.0.tar", last modified: Tue Jul 11 03:38:41 2023, max compression
```

## Comparing `cuquantum-23.3.0.tar` & `cuquantum-23.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:22:05.620751 cuquantum-23.3.0/
--rw-r--r--   0 root         (0) root         (0)    11004 2023-03-30 06:20:23.000000 cuquantum-23.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2721 2023-03-30 06:22:05.620751 cuquantum-23.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1920 2023-03-30 06:20:23.000000 cuquantum-23.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     8862 2023-03-30 06:20:23.000000 cuquantum-23.3.0/cuda_autodetect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 06:22:05.620751 cuquantum-23.3.0/cuquantum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2721 2023-03-30 06:22:05.000000 cuquantum-23.3.0/cuquantum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-03-30 06:22:05.000000 cuquantum-23.3.0/cuquantum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 06:22:05.000000 cuquantum-23.3.0/cuquantum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 06:22:05.000000 cuquantum-23.3.0/cuquantum.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-30 06:22:05.000000 cuquantum-23.3.0/cuquantum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 06:22:05.620751 cuquantum-23.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2525 2023-03-30 06:20:23.000000 cuquantum-23.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:38:41.020473 cuquantum-23.6.0/
+-rw-r--r--   0 root         (0) root         (0)    11004 2023-07-11 03:36:36.000000 cuquantum-23.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-11 03:38:41.020473 cuquantum-23.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-07-11 03:36:36.000000 cuquantum-23.6.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     8953 2023-07-11 03:36:36.000000 cuquantum-23.6.0/cuda_autodetect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 03:38:41.016473 cuquantum-23.6.0/cuquantum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 03:38:40.000000 cuquantum-23.6.0/cuquantum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 03:38:41.020473 cuquantum-23.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-11 03:36:36.000000 cuquantum-23.6.0/setup.py
```

### Comparing `cuquantum-23.3.0/LICENSE` & `cuquantum-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuquantum-23.3.0/PKG-INFO` & `cuquantum-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.3.0
+Version: 23.6.0
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
@@ -37,26 +37,29 @@
 Please refer to https://docs.nvidia.com/cuda/cuquantum/index.html for the cuQuantum documentation.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum
+   pip install -v --no-cache-dir cuquantum
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 .. note::
 
    To use cuQuantum's Python APIs, please directly install `cuQuantum Python`_.
 
 Citing cuQuantum
 ================
```

### Comparing `cuquantum-23.3.0/README.rst` & `cuquantum-23.6.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -18,26 +18,29 @@
 Please refer to https://docs.nvidia.com/cuda/cuquantum/index.html for the cuQuantum documentation.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum
+   pip install -v --no-cache-dir cuquantum
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 .. note::
 
    To use cuQuantum's Python APIs, please directly install `cuQuantum Python`_.
 
 Citing cuQuantum
 ================
```

### Comparing `cuquantum-23.3.0/cuda_autodetect.py` & `cuquantum-23.6.0/cuda_autodetect.py`

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

### Comparing `cuquantum-23.3.0/cuquantum.egg-info/PKG-INFO` & `cuquantum-23.6.0/cuquantum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuquantum
-Version: 23.3.0
+Version: 23.6.0
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
@@ -37,26 +37,29 @@
 Please refer to https://docs.nvidia.com/cuda/cuquantum/index.html for the cuQuantum documentation.
 
 Installation
 ============
 
 .. code-block:: bash
 
-   pip install -v cuquantum
+   pip install -v --no-cache-dir cuquantum
 
 .. note::
 
    Starting cuQuantum 22.11, this package is a meta package pointing to ``cuquantum-cuXX``,
    where XX is the CUDA major version (currently CUDA 11 & 12 are supported).
    The meta package will attempt to infer and install the correct ``-cuXX`` wheel. However,
    in situations where the auto-detection fails, this package currently points to ``cuquantum-cu11``
    with a warning raised (if the verbosity flag ``-v`` is set, as shown above). This behavior
    is subject to change in the future, and users are encouraged to install the new wheels that
    come *with* the ``-cuXX`` suffix.
 
+   The argument ``--no-cache-dir`` is required for pip 23.1+. It forces pip to execute the
+   auto-detection logic.
+
 .. note::
 
    To use cuQuantum's Python APIs, please directly install `cuQuantum Python`_.
 
 Citing cuQuantum
 ================
```

### Comparing `cuquantum-23.3.0/setup.py` & `cuquantum-23.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup
 
 from cuda_autodetect import infer_best_package, bdist_wheel
 
 
 # Update this for every release
-package_ver = '23.03.0'
+package_ver = '23.06.0'
 package_name = "cuquantum"
 
 
 # get project long description
 with open("README.rst") as f:
     long_description = f.read()
```

