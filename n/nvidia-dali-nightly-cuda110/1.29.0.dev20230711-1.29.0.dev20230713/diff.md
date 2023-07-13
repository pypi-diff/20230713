# Comparing `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230711.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230711.tar", last modified: Tue Jul 11 18:44:42 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230713.tar", last modified: Thu Jul 13 17:25:10 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230711.tar` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230713.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-11 18:44:42.071864 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-11 18:44:42.071864 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-11 18:44:42.071864 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-11 18:44:42.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-11 18:44:42.071864 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230711/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-13 17:25:10.367864 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-13 17:25:10.367864 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-13 17:25:10.367864 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-13 17:25:10.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-13 17:25:10.367864 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230713/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230711/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230713/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230711/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230713/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230711
+Version: 1.29.0.dev20230713
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230711/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230713/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230711
+Version: 1.29.0.dev20230713
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230711/setup.py` & `nvidia-dali-nightly-cuda110-1.29.0.dev20230713/setup.py`

 * *Files identical despite different names*

