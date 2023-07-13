# Comparing `tmp/surfify-0.1.0.tar.gz` & `tmp/surfify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/surfify-0.1.0.tar", last modified: Mon Oct 18 13:15:33 2021, max compression
+gzip compressed data, was "surfify-0.2.0.tar", last modified: Thu Jul 13 06:45:07 2023, max compression
```

## Comparing `surfify-0.1.0.tar` & `surfify-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:33.000000 surfify-0.1.0/
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify.egg-info/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1159 2021-10-18 13:15:29.000000 surfify-0.1.0/surfify.egg-info/SOURCES.txt
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)        8 2021-10-18 13:15:28.000000 surfify-0.1.0/surfify.egg-info/top_level.txt
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      145 2021-10-18 13:15:29.000000 surfify-0.1.0/surfify.egg-info/requires.txt
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      656 2021-10-18 13:15:29.000000 surfify-0.1.0/surfify.egg-info/PKG-INFO
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)        1 2021-10-18 13:15:28.000000 surfify-0.1.0/surfify.egg-info/dependency_links.txt
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      124 2021-10-18 13:15:33.000000 surfify-0.1.0/setup.cfg
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     1281 2021-10-15 13:34:46.000000 surfify-0.1.0/setup.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:33.000000 surfify-0.1.0/surfify/tests/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1539 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_utils_logging.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     2623 2021-10-18 13:02:52.000000 surfify-0.1.0/surfify/tests/test_utils_io.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     2922 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_models_vae.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3887 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_models_unet.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1092 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_plotting_surface.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3021 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_utils_coord.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     5452 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_utils_sampling.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1443 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_datasets.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     6353 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_nn_modules.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1755 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_augmentation.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3922 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/tests/test_models_vgg.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/resources/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)  7873790 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/resources/freesurfer_icos.npz
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:33.000000 surfify-0.1.0/surfify/utils/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    10994 2021-10-18 13:05:49.000000 surfify-0.1.0/surfify/utils/coord.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    41008 2021-10-15 13:34:47.000000 surfify-0.1.0/surfify/utils/sampling.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     7891 2021-10-15 13:34:47.000000 surfify-0.1.0/surfify/utils/io.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     2764 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/utils/__init__.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/models/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    18004 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/models/vgg.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    15284 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/models/vae.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     7749 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/models/base.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      914 2021-10-15 14:08:38.000000 surfify-0.1.0/surfify/models/__init__.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    20896 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/models/unet.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     2381 2021-10-15 13:35:53.000000 surfify-0.1.0/surfify/info.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/losses/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     2693 2021-09-17 10:00:18.000000 surfify-0.1.0/surfify/losses/vae.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      478 2021-09-15 12:38:37.000000 surfify-0.1.0/surfify/losses/__init__.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/datasets/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3496 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/datasets/_samples_generator.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      646 2021-07-08 12:07:04.000000 surfify-0.1.0/surfify/datasets/__init__.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/nn/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    31709 2021-09-17 09:53:43.000000 surfify-0.1.0/surfify/nn/modules.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1198 2021-09-15 08:43:54.000000 surfify-0.1.0/surfify/nn/functional.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      634 2021-09-17 09:37:58.000000 surfify-0.1.0/surfify/nn/__init__.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/augmentation/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      522 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/augmentation/__init__.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     7319 2021-10-18 13:12:47.000000 surfify-0.1.0/surfify/augmentation/augmentation.py
-drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2021-10-18 13:15:32.000000 surfify-0.1.0/surfify/plotting/
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3835 2021-10-15 13:34:46.000000 surfify-0.1.0/surfify/plotting/surface.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      494 2021-08-05 14:16:52.000000 surfify-0.1.0/surfify/plotting/__init__.py
--rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      509 2021-07-08 13:30:50.000000 surfify-0.1.0/surfify/__init__.py
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      656 2021-10-18 13:15:33.000000 surfify-0.1.0/PKG-INFO
--rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3902 2021-10-18 13:02:16.000000 surfify-0.1.0/README.rst
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:07.163433 surfify-0.2.0/
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      656 2023-07-13 06:45:07.164985 surfify-0.2.0/PKG-INFO
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3877 2023-07-13 06:41:33.000000 surfify-0.2.0/README.rst
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      124 2023-07-13 06:45:07.174740 surfify-0.2.0/setup.cfg
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     1281 2021-10-18 13:29:52.000000 surfify-0.2.0/setup.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.432351 surfify-0.2.0/surfify/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      509 2021-07-08 13:30:50.000000 surfify-0.2.0/surfify/__init__.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.540551 surfify-0.2.0/surfify/augmentation/
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      690 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/augmentation/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     9669 2023-07-12 15:28:51.000000 surfify-0.2.0/surfify/augmentation/base.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     5711 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/augmentation/mixup.py
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     7643 2023-07-12 11:56:20.000000 surfify-0.2.0/surfify/augmentation/utils.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.562676 surfify-0.2.0/surfify/datasets/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      646 2021-07-08 12:07:04.000000 surfify-0.2.0/surfify/datasets/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3496 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/datasets/_samples_generator.py
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     2381 2023-07-12 12:00:19.000000 surfify-0.2.0/surfify/info.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.585354 surfify-0.2.0/surfify/losses/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      478 2021-09-15 12:38:37.000000 surfify-0.2.0/surfify/losses/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3758 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/losses/vae.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.641555 surfify-0.2.0/surfify/models/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     1004 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/models/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     9055 2021-10-22 13:51:50.000000 surfify-0.2.0/surfify/models/base.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    26957 2023-03-15 07:09:53.000000 surfify-0.2.0/surfify/models/unet.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    31727 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/models/vae.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    20977 2021-10-22 14:01:43.000000 surfify-0.2.0/surfify/models/vgg.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.673555 surfify-0.2.0/surfify/nn/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      634 2021-09-17 09:37:58.000000 surfify-0.2.0/surfify/nn/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1198 2021-09-15 08:43:54.000000 surfify-0.2.0/surfify/nn/functional.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    31979 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/nn/modules.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.695967 surfify-0.2.0/surfify/plotting/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)      494 2021-08-05 14:16:52.000000 surfify-0.2.0/surfify/plotting/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     4139 2023-04-25 07:29:32.000000 surfify-0.2.0/surfify/plotting/surface.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.707174 surfify-0.2.0/surfify/resources/
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)  7873790 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/resources/freesurfer_icos.npz
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:07.108964 surfify-0.2.0/surfify/tests/
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     5154 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/tests/test_augmentation.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1443 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_datasets.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3887 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_models_unet.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3415 2023-07-12 11:52:36.000000 surfify-0.2.0/surfify/tests/test_models_vae.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3922 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_models_vgg.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     6353 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_nn_modules.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1092 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_plotting_surface.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     3021 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_utils_coord.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     2623 2021-10-18 13:02:52.000000 surfify-0.2.0/surfify/tests/test_utils_io.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1539 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_utils_logging.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     5452 2021-10-15 13:34:46.000000 surfify-0.2.0/surfify/tests/test_utils_sampling.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:07.154290 surfify-0.2.0/surfify/utils/
+-rwxrwxr-x   0 ag239446 (239446) ag239446 (239446)     2819 2023-04-25 07:22:50.000000 surfify-0.2.0/surfify/utils/__init__.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    10994 2021-10-18 13:05:49.000000 surfify-0.2.0/surfify/utils/coord.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     7891 2021-10-15 13:34:47.000000 surfify-0.2.0/surfify/utils/io.py
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)    42591 2023-04-25 06:54:58.000000 surfify-0.2.0/surfify/utils/sampling.py
+drwxrwxr-x   0 ag239446 (239446) ag239446 (239446)        0 2023-07-13 06:45:06.496087 surfify-0.2.0/surfify.egg-info/
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      656 2023-07-13 06:45:05.000000 surfify-0.2.0/surfify.egg-info/PKG-INFO
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)     1211 2023-07-13 06:45:06.000000 surfify-0.2.0/surfify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)        1 2023-07-13 06:45:05.000000 surfify-0.2.0/surfify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)      145 2023-07-13 06:45:05.000000 surfify-0.2.0/surfify.egg-info/requires.txt
+-rw-rw-r--   0 ag239446 (239446) ag239446 (239446)        8 2023-07-13 06:45:05.000000 surfify-0.2.0/surfify.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `surfify-0.1.0/surfify.egg-info/SOURCES.txt` & `surfify-0.2.0/surfify.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 surfify/info.py
 surfify.egg-info/PKG-INFO
 surfify.egg-info/SOURCES.txt
 surfify.egg-info/dependency_links.txt
 surfify.egg-info/requires.txt
 surfify.egg-info/top_level.txt
 surfify/augmentation/__init__.py
-surfify/augmentation/augmentation.py
+surfify/augmentation/base.py
+surfify/augmentation/mixup.py
+surfify/augmentation/utils.py
 surfify/datasets/__init__.py
 surfify/datasets/_samples_generator.py
 surfify/losses/__init__.py
 surfify/losses/vae.py
 surfify/models/__init__.py
 surfify/models/base.py
 surfify/models/unet.py
```

### Comparing `surfify-0.1.0/surfify.egg-info/PKG-INFO` & `surfify-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: surfify
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 PyTorch toolbox to work with spherical surfaces.
 
 Home-page: https://github.com/neurospin-deepinsight/surfify
 Author: 
 surfify developers
```

### Comparing `surfify-0.1.0/setup.py` & `surfify-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_utils_logging.py` & `surfify-0.2.0/surfify/tests/test_utils_logging.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_utils_io.py` & `surfify-0.2.0/surfify/tests/test_utils_io.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_models_vae.py` & `surfify-0.2.0/surfify/tests/test_models_vae.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch
 from surfify import models
 from surfify import utils
 from surfify import datasets
 
 
 class TestModelsVAE(unittest.TestCase):
-    """ Test the SphericalVAE.
+    """ Test the SphericalVAE with DiNe and RePa.
     """
     def setUp(self):
         """ Setup test.
         """
         self.order = 3
         self.n_classes = 2
         self.depth = 2
@@ -34,62 +34,71 @@
 
     def tearDown(self):
         """ Run after each test.
         """
         pass
 
     def test_forward(self):
-        """ Test SphericalVAE forward.
+        """ Test SphericalVAEs with DiNe and RePa forwards.
         """
         model = models.SphericalVAE(
             input_channels=self.n_classes, input_order=self.order,
-            latent_dim=32,  conv_mode="DiNe", dine_size=1,
+            latent_dim=32, conv_mode="DiNe", dine_size=1,
             conv_flts=[32, 64], standard_ico=True)
         out = model(self.X, self.X)
+        self.assertTrue(len(out) == 3)
+        self.assertTrue(out[0].shape == self.X.shape)
         model = models.SphericalVAE(
             input_channels=self.n_classes, input_order=self.order,
             latent_dim=32, conv_mode="RePa", repa_size=5, repa_zoom=5,
             conv_flts=[32, 64], standard_ico=True)
         out = model(self.X, self.X)
+        self.assertTrue(len(out) == 3)
+        self.assertTrue(out[0].shape == self.X.shape)
 
 
 class TestModelsGVAE(unittest.TestCase):
-    """ Test the SphericalGVAE.
+    """ Test the SphericalVAE with SpMa on regrided data.
     """
     def setUp(self):
         """ Setup test.
         """
         self.order = 3
         self.n_classes = 2
         self.depth = 2
         ico_vertices, _ = utils.icosahedron(
             order=self.order, standard_ico=True)
         X, _ = datasets.make_classification(
             ico_vertices, n_samples=40, n_classes=self.n_classes, scale=1,
             seed=42)
         self.X = []
+        self.input_dim = 193
         for sample_idx in range(X.shape[0]):
             _X = []
             for ch_idx in range(X.shape[1]):
-                _X.append(utils.text2grid(ico_vertices, X[sample_idx, ch_idx]))
+                _X.append(utils.text2grid(
+                    ico_vertices, X[sample_idx, ch_idx], resx=self.input_dim,
+                    resy=self.input_dim))
             self.X.append(_X)
         self.X = np.asarray(self.X)
         self.X = torch.from_numpy(self.X)
 
     def tearDown(self):
         """ Run after each test.
         """
         pass
 
     def test_forward(self):
-        """ Test SphericalGVAE forward.
+        """ Test SphericalVAE with SpMa forward.
         """
-        model = models.SphericalGVAE(
-            input_channels=self.n_classes, input_dim=194, latent_dim=32,
-            conv_flts=[64, 128, 128])
+        model = models.SphericalVAE(
+            input_channels=self.n_classes, input_dim=self.input_dim,
+            latent_dim=32, conv_flts=[64, 128, 128], conv_mode="SpMa")
         out = model(self.X, self.X)
+        self.assertTrue(len(out) == 3)
+        self.assertTrue(out[0].shape == self.X.shape)
 
 
 if __name__ == "__main__":
 
     utils.setup_logging(level="debug")
     unittest.main()
```

### Comparing `surfify-0.1.0/surfify/tests/test_models_unet.py` & `surfify-0.2.0/surfify/tests/test_models_unet.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_plotting_surface.py` & `surfify-0.2.0/surfify/tests/test_plotting_surface.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_utils_coord.py` & `surfify-0.2.0/surfify/tests/test_utils_coord.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_utils_sampling.py` & `surfify-0.2.0/surfify/tests/test_utils_sampling.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_datasets.py` & `surfify-0.2.0/surfify/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_nn_modules.py` & `surfify-0.2.0/surfify/tests/test_nn_modules.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/tests/test_models_vgg.py` & `surfify-0.2.0/surfify/tests/test_models_vgg.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/resources/freesurfer_icos.npz` & `surfify-0.2.0/surfify/resources/freesurfer_icos.npz`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/utils/coord.py` & `surfify-0.2.0/surfify/utils/coord.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/utils/sampling.py` & `surfify-0.2.0/surfify/utils/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 import tempfile
 import collections
 import numpy as np
 from time import time
 import networkx as nx
 from scipy.spatial import transform
 from sklearn.neighbors import BallTree
-from nilearn.surface import load_surf_mesh
-from nilearn.datasets import fetch_surf_fsaverage
 from .io import HidePrints
 
 
 def normalize(vertex):
     """ Return vertex coordinates fixed to the unit sphere.
     """
     x, y, z = vertex
@@ -125,58 +123,59 @@
     Returns
     --------
     neighs: dict
         a dictionary with vertices row index as keys and a dictionary of
         neighbors vertices row indexes organized by rings as values.
     """
     graph = vertex_adjacency_graph(vertices, triangles)
+    degrees = dict((node, val) for node, val in graph.degree())
     neighs = collections.OrderedDict()
     for node in sorted(graph.nodes):
         node_neighs = {}
         # node_neighs = [idx for idx in graph.neighbors(node)]
         for neigh, ring in nx.single_source_shortest_path_length(
                 graph, node, cutoff=depth).items():
             if ring == 0:
                 continue
             node_neighs.setdefault(ring, []).append(neigh)
         if direct_neighbor:
-            _node_neighs = []
-            if depth == 1:
-                delta = np.pi / 4
-            elif depth == 2:
-                delta = np.pi / 8
-            else:
-                raise ValueError("Direct neighbors implemented only for "
-                                 "depth <= 2.")
+            _node_neighs, _missing_neighs = [], {}
+            n_neighs, center_missing_neighs = 0, False
             for ring, ring_neighs in node_neighs.items():
                 angles = np.asarray([
                     get_angle_with_xaxis(vertices[node], vertices[node], vec)
                     for vec in vertices[ring_neighs]])
-                angles += delta
-                angles = np.degrees(np.mod(angles, 2 * np.pi))
+                angles = np.degrees(angles)
                 ring_neighs = [x for _, x in sorted(
                     zip(angles, ring_neighs), key=lambda pair: pair[0])]
-                if depth == 1 and ring == 1:
-                    if len(ring_neighs) == 5:
-                        ring_neighs.append(node)
-                    elif len(ring_neighs) != 6:
-                        raise ValueError("Mesh is not an icosahedron.")
-                if depth == 2 and ring == 2:
-                    ring_neighs = ring_neighs[1::2]
-                    if len(_node_neighs) + len(ring_neighs) == 10:
-                        ring_neighs.extend([node] * 2)
-                    elif len(_node_neighs) + len(ring_neighs) == 11:
-                        ring_neighs.append(node)
-                    elif len(_node_neighs) + len(ring_neighs) != 12:
-                        raise ValueError("Mesh is not an icosahedron.")
+                node_neighs[ring] = ring_neighs
+                n_neighs += 6 * ring
+                if ring > 1:
+                    _center_neighs = node_neighs[ring - 1]
+                else:
+                    _center_neighs = [node]
+                _node_missing_neighs = [
+                    _node for _node in _center_neighs if degrees[_node] == 5]
+                for _node, _counts in _missing_neighs.items():
+                    ring_neighs = [_node] * _counts[0] + ring_neighs
+                    _missing_neighs[_node] = _counts[1:]
+                for _node in _node_missing_neighs:
+                    _missing_neighs[_node] = list(range(2, depth + 2 - ring))
+                    if _node == node:
+                        center_missing_neighs = True
+                        continue
+                    _node_neighs.insert(_node_neighs.index(_node), _node)
                 _node_neighs.extend(ring_neighs)
-            _node_neighs.append(node)
+            _node_neighs.insert(0, node)
+            if center_missing_neighs:
+                _node_neighs.insert(0, node)
+            if len(_node_neighs) != n_neighs + 1:
+                raise ValueError("Mesh is not an icosahedron.")
             node_neighs = _node_neighs
         neighs[node] = node_neighs
-
     return neighs
 
 
 def vertex_adjacency_graph(vertices, triangles):
     """ Build a networkx graph representation of the vertices and
     their connections in the mesh.
 
@@ -286,15 +285,14 @@
     # Edges are in order of triangles due to reshape
     triangles_index = np.tile(
         np.arange(len(triangles)), (3, 1)).T.reshape(-1)
 
     return edges, triangles_index
 
 
-# TODO: normalize weights (see rotate_data).
 def neighbors_rec(vertices, triangles, size=5, zoom=5):
     """ Build rectangular grid neighbors and weights.
 
     This is the base function to build Rectangular Patch (RePa) kernels.
 
     See Also
     --------
@@ -347,14 +345,15 @@
         grid_in_sphere[idx1], _ = get_rectangular_projection(
             node, size=size, zoom=zoom)
         for idx2, point in enumerate(grid_in_sphere[idx1]):
             dist = np.linalg.norm(vertices - point, axis=1)
             ordered_neighs = np.argsort(dist)
             neighs[idx1, idx2] = ordered_neighs[:3]
             weights[idx1, idx2] = dist[neighs[idx1, idx2]]
+            weights[idx1, idx2] /= np.sum(dist[neighs[idx1, idx2]])
     return neighs, weights, grid_in_sphere
 
 
 def get_rectangular_projection(node, size=5, zoom=5):
     """ Project 2D rectangular grid defined in node tangent space into 3D
     spherical space.
 
@@ -473,14 +472,17 @@
     -1 and 1.
 
     Parameters
     ----------
     ico_file: str
         path to the generated FreeSurfer reference icosahedron topologies.
     """
+    from nilearn.surface import load_surf_mesh
+    from nilearn.datasets import fetch_surf_fsaverage
+
     data = {}
     for order in range(7, 2, -1):
         surf_name = "fsaverage{0}".format(order)
         with HidePrints(hide_err=True):
             with tempfile.TemporaryDirectory() as tmpdir:
                 fsaverage = fetch_surf_fsaverage(
                     mesh=surf_name, data_dir=tmpdir)
@@ -553,15 +555,15 @@
         icos = np.load(resource_file)
         surf_name = "fsaverage{0}".format(order)
         try:
             vertices = icos[surf_name + ".vertices"]
             triangles = icos[surf_name + ".triangles"]
         except Exception as err:
             print("-- available topologies:", icos.files)
-            raise(err)
+            raise err
 
     return vertices, triangles
 
 
 def middle_point(point_1, point_2, vertices, middle_point_cache):
     """ Find a middle point and project it to the unit sphere.
 
@@ -640,14 +642,77 @@
     if int(order) != order:
         raise ValueError(
             "This number of vertices does not correspond to those of a "
             "regular icosahedron.")
     return int(order)
 
 
+def number_of_neighbors(depth):
+    """ Get the number of neighbors up to a certain depth.
+
+    See Also
+    --------
+    min_order_to_get_n_neighbors
+
+    Examples
+    --------
+    >>> from surfify.utils import number_of_neighbors
+    >>> for depth in range(4):
+    >>>     n_neighs = number_of_neighbors(depth)
+    >>>     print(n_neighs)
+
+    Parameters
+    ----------
+    n_vertices: int
+        the number of vertices of an icosahedron.
+
+    Returns
+    -------
+    order: int
+        the order of the icosahedron.
+    """
+    n_neighs = 1
+    for order in range(1, depth + 1):
+        n_neighs += 6 * order
+    return n_neighs
+
+
+def min_depth_to_get_n_neighbors(n_neighs):
+    """ Get the minimal depth of neighborhood to get a desired number of
+    neighbors.
+
+    See Also
+    --------
+    number_of_neighbors
+
+    Examples
+    --------
+    >>> from surfify.utils import min_depth_to_get_n_neighbors, icosahedron
+    >>> ico3_verts, ico3_tris = icosahedron(order=3)
+    >>> depth = min_depth_to_get_n_neighbors(len(ico3_verts) / 2)
+    >>> print(depth)
+
+    Parameters
+    ----------
+    n_vertices: int
+        the number of vertices of an icosahedron.
+
+    Returns
+    -------
+    order: int
+        the order of the icosahedron.
+    """
+    cum_n_neighs = 1
+    depth = 1
+    while (cum_n_neighs < n_neighs):
+        cum_n_neighs += 6 * depth
+        depth += 1
+    return depth
+
+
 def interpolate(vertices, target_vertices, target_triangles):
     """ Interpolate icosahedron missing data by finding nearest neighbors.
 
     Interpolation weights are set to 1 for a regular icosahedron geometry.
 
     See Also
     --------
```

### Comparing `surfify-0.1.0/surfify/utils/io.py` & `surfify-0.2.0/surfify/utils/io.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/utils/__init__.py` & `surfify-0.2.0/surfify/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # Imports
 import logging
 import warnings
 from .sampling import (
     interpolate, interpolate_data, downsample, downsample_data, downsample_ico,
     neighbors, neighbors_rec, get_rectangular_projection, find_neighbors,
     icosahedron, number_of_ico_vertices, order_of_ico_from_vertices,
-    rotate_data, order_triangles, find_rotation_interpol_coefs)
+    rotate_data, order_triangles, find_rotation_interpol_coefs,
+    number_of_neighbors, min_depth_to_get_n_neighbors)
 from .coord import (
     cart2sph, sph2cart, text2grid, grid2text, ico2ico, text2ico)
 
 # Global parameters
 LEVELS = {
     "debug": logging.DEBUG,
     "info": logging.INFO,
```

### Comparing `surfify-0.1.0/surfify/models/vgg.py` & `surfify-0.2.0/surfify/models/vgg.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,35 @@
     -----
     Debuging messages can be displayed by changing the log level using
     ``setup_logging(level='debug')``.
 
     See Also
     --------
     SphericalGVGG
+
+    Examples
+    --------
+    >>> import torch
+    >>> from surfify.utils import icosahedron
+    >>> from surfify.models import SphericalVGG11
+    >>> verts, tris = icosahedron(order=6)
+    >>> x = torch.zeros((1, 2, len(verts)))
+    >>> model = SphericalVGG11(
+    >>>     input_channels=2, n_classes=10, input_order=6,
+    >>>     conv_mode="DiNe", dine_size=1, hidden_dim=512,
+    >>>     fusion_level=2, init_weights=True, standard_ico=False)
+    >>> print(model)
+    >>> out = model(x, x)
+    >>> print(out.shape)
     """
     def __init__(self, input_channels, cfg, n_classes, input_order=5,
                  conv_mode="DiNe", dine_size=1, repa_size=5, repa_zoom=5,
-                 hidden_dim=4096, batch_norm=False, init_weights=True,
-                 standard_ico=False, cachedir=None):
+                 dynamic_repa_zoom=False, hidden_dim=4096, batch_norm=False,
+                 fusion_level=1, init_weights=True, standard_ico=False,
+                 cachedir=None):
         """ Init class.
 
         Parameters
         ----------
         input_channels: int
             the number of input channels.
         cfg: list
@@ -56,41 +72,51 @@
             - 1 ring Direct Neighbor convolution method.
         dine_size: int, default 1
             the size of the spherical convolution filter, ie. the number of
             neighbor rings to be considered.
         repa_size: int, default 5
             the size of the rectangular grid in the tangent space.
         repa_zoom: int, default 5
-            a multiplicative factor applied to the rectangular grid in the
-            tangent space.
+            control the rectangular grid spacing in the tangent space by
+            applying a multiplicative factor of `1 / repa_zoom`.
+        dynamic_repa_zoom: bool, default False
+            dynamically adapt the RePa zoom by applying a multiplicative factor
+            of `log(order + 1) + 1`.
         hidden_dim: int, default 4096
             the 2-layer classification MLP number of hidden dims.
         batch_norm: bool, default False
             wether or not to use batch normalization after a convolution
             layer.
+        fusion_level: int, default 1
+            at which max pooling level left and right hemisphere data
+            are concatenated.
         init_weights: bool, default True
             initialize network weights.
         standard_ico: bool, default False
             optionaly use surfify tesselation.
         cachedir: str, default None
             set this folder to use smart caching speedup.
         """
         logger.debug("SphericalVGG init...")
-        cfg = cfg[:-1]
+        cfg = cfg
         super(SphericalVGG, self).__init__(
             input_order=input_order, n_layers=cfg.count("M"),
             conv_mode=conv_mode, dine_size=dine_size, repa_size=repa_size,
-            repa_zoom=repa_zoom, standard_ico=standard_ico,
-            cachedir=cachedir)
+            repa_zoom=repa_zoom, dynamic_repa_zoom=dynamic_repa_zoom,
+            standard_ico=standard_ico, cachedir=cachedir)
         self.input_channels = input_channels
         self.cfg = cfg
         self.n_classes = n_classes
         self.batch_norm = batch_norm
         self.n_modules = len(cfg)
-        self.final_flt = int(cfg[-1])
+        if fusion_level > self.n_layers or fusion_level <= 0:
+            raise ValueError("Impossible to use input fusion level with "
+                             "'{0}' layers.".format(self.n_layers))
+        self.fusion_level = fusion_level
+        self.final_flt = int(cfg[-2])
         self.top_flatten_dim = len(
             self.ico[self.input_order - self.n_layers + 1].vertices)
         self.top_final = self.final_flt * 7
         self._make_encoder()
         self.avgpool = nn.AdaptiveAvgPool1d((7))
         self.classifier = nn.Sequential(
             nn.Linear(self.top_final, hidden_dim),
@@ -113,26 +139,24 @@
             input left cortical texture.
         right_x: Tensor (samples, <input_channels>, azimuth, elevation)
             input right cortical texture.
 
         Returns
         -------
         out: torch.Tensor
+            the prediction.
         """
         logger.debug("SphericalVGG forward pass")
         logger.debug(debug_msg("left cortical", left_x))
         logger.debug(debug_msg("right cortical", right_x))
-        x = torch.cat(
-            (self.enc_left_conv(left_x), self.enc_right_conv(right_x)), dim=1)
+        left_x = self._safe_forward(self.enc_left_conv, left_x)
+        right_x = self._safe_forward(self.enc_right_conv, right_x)
+        x = torch.cat((left_x, right_x), dim=1)
         logger.debug(debug_msg("lh/rh path", x))
-        for mod in self.enc_w_conv.children():
-            if isinstance(mod, IcoPool):
-                x = mod(x)[0]
-            else:
-                x = mod(x)
+        x = self._safe_forward(self.enc_w_conv, x)
         logger.debug(debug_msg("features", x))
         x = self.avgpool(x)
         logger.debug(debug_msg("avg pooling", x))
         x = torch.flatten(x, 1)
         logger.debug(debug_msg("flat", x))
         x = self.classifier(x)
         logger.debug(debug_msg("classifier", x))
@@ -158,45 +182,54 @@
         """ Method to create the encoding layers.
         """
         input_channels = self.input_channels
         order = self.input_order
         self.enc_left_conv = nn.Sequential()
         self.enc_right_conv = nn.Sequential()
         self.enc_w_conv = nn.Sequential()
-        first_layer = True
+        multi_path = True
+        layer_idx = 0
         for idx in range(self.n_modules):
             if self.cfg[idx] == "M":
                 order -= 1
-                if first_layer:
-                    first_layer = False
+                layer_idx += 1
+                if layer_idx == self.fusion_level:
+                    multi_path = False
                     input_channels *= 2
                 pooling = IcoPool(
                     down_neigh_indices=self.ico[order + 1].neighbor_indices,
                     down_indices=self.ico[order + 1].down_indices,
                     pooling_type="max")
-                self.enc_w_conv.add_module("pooling_{0}".format(idx), pooling)
-            elif first_layer:
+                if multi_path:
+                    self.enc_left_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+                    self.enc_right_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+                else:
+                    self.enc_w_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+            elif multi_path:
                 lconv = self.sconv(
                     input_channels, (self.cfg[idx] // 2),
                     self.ico[order].conv_neighbor_indices)
-                self.enc_left_conv.add_module("lconv_{0}".format(idx), lconv)
+                self.enc_left_conv.add_module("l_conv_{0}".format(idx), lconv)
                 if self.batch_norm:
                     lbn = nn.BatchNorm1d(self.cfg[idx] // 2)
-                    self.enc_left_conv.add_module("lbn_{0}".format(idx), lbn)
+                    self.enc_left_conv.add_module("l_bn_{0}".format(idx), lbn)
                 lrelu = nn.ReLU(inplace=True)
-                self.enc_left_conv.add_module("lrelu_{0}".format(idx), lrelu)
+                self.enc_left_conv.add_module("l_relu_{0}".format(idx), lrelu)
                 rconv = self.sconv(
                     input_channels, (self.cfg[idx] // 2),
                     self.ico[order].conv_neighbor_indices)
-                self.enc_right_conv.add_module("rconv_{0}".format(idx), rconv)
+                self.enc_right_conv.add_module("r_conv_{0}".format(idx), rconv)
                 if self.batch_norm:
                     rbn = nn.BatchNorm1d(self.cfg[idx] // 2)
-                    self.enc_right_conv.add_module("rbn_{0}".format(idx), rbn)
+                    self.enc_right_conv.add_module("r_bn_{0}".format(idx), rbn)
                 rrelu = nn.ReLU(inplace=True)
-                self.enc_right_conv.add_module("rrelu_{0}".format(idx), rrelu)
+                self.enc_right_conv.add_module("r_relu_{0}".format(idx), rrelu)
                 input_channels = self.cfg[idx] // 2
             else:
                 conv = self.sconv(
                     input_channels, self.cfg[idx],
                     self.ico[order].conv_neighbor_indices)
                 self.enc_w_conv.add_module("conv_{0}".format(idx), conv)
                 if self.batch_norm:
@@ -214,17 +247,30 @@
     -----
     Debuging messages can be displayed by changing the log level using
     ``setup_logging(level='debug')``.
 
     See Also
     --------
     SphericalVGG
+
+    Examples
+    --------
+    >>> import torch
+    >>> from surfify.models import SphericalGVGG11
+    >>> x = torch.zeros((1, 2, 192, 192))
+    >>> model = SphericalGVGG11(
+    >>>     input_channels=2, n_classes=10, input_dim=194, hidden_dim=512,
+    >>>     fusion_level=2, init_weights=True)
+    >>> print(model)
+    >>> out = model(x, x)
+    >>> print(out.shape)
     """
     def __init__(self, input_channels, cfg, n_classes, input_dim=194,
-                 hidden_dim=4096, batch_norm=False, init_weights=True):
+                 hidden_dim=4096, batch_norm=False, fusion_level=1,
+                 init_weights=True):
         """ Init class.
 
         Parameters
         ----------
         input_channels: int
             the number of input channels.
         cfg: list
@@ -234,26 +280,33 @@
         input_dim: int, default 192
             the size of the converted 3-D surface to the 2-D grid.
         hidden_dim: int, default 4096
             the 2-layer classification MLP number of hidden dims.
         batch_norm: bool, default False
             wether or not to use batch normalization after a convolution
             layer.
+        fusion_level: int, default 1
+            at which max pooling level left and right hemisphere data
+            are concatenated.
         init_weights: bool, default True
             initialize network weights.
         """
         logger.debug("SphericalGVGG init...")
         super(SphericalGVGG, self).__init__()
         self.input_channels = input_channels
         self.cfg = cfg
         self.n_classes = n_classes
         self.input_dim = input_dim
         self.batch_norm = batch_norm
         self.n_modules = len(cfg)
         self.n_layers = cfg.count("M")
+        if fusion_level > self.n_layers or fusion_level <= 0:
+            raise ValueError("Impossible to use input fusion level with "
+                             "'{0}' layers.".format(self.n_layers))
+        self.fusion_level = fusion_level
         self.final_flt = int(cfg[-2])
         self.top_flatten_dim = int(self.input_dim / (2 ** self.n_layers))
         self.top_final = self.final_flt * 7 ** 2
         self._make_encoder()
         self.avgpool = nn.AdaptiveAvgPool2d((7, 7))
         self.classifier = nn.Sequential(
             nn.Linear(self.top_final, hidden_dim),
@@ -276,14 +329,15 @@
             input left cortical texture.
         right_x: Tensor (samples, <input_channels>, azimuth, elevation)
             input right cortical texture.
 
         Returns
         -------
         out: torch.Tensor
+            the prediction.
         """
         logger.debug("SphericalGVGG forward pass")
         logger.debug(debug_msg("left cortical", left_x))
         logger.debug(debug_msg("right cortical", right_x))
         x = torch.cat(
             (self.enc_left_conv(left_x), self.enc_right_conv(right_x)), dim=1)
         logger.debug(debug_msg("lh/rh path", x))
@@ -316,43 +370,52 @@
     def _make_encoder(self):
         """ Method to create the encoding layers.
         """
         input_channels = self.input_channels
         self.enc_left_conv = nn.Sequential()
         self.enc_right_conv = nn.Sequential()
         self.enc_w_conv = nn.Sequential()
-        first_layer = True
+        multi_path = True
+        layer_idx = 0
         for idx in range(self.n_modules):
             if self.cfg[idx] == "M":
-                if first_layer:
-                    first_layer = False
+                layer_idx += 1
+                if layer_idx == self.fusion_level:
+                    multi_path = False
                     input_channels *= 2
                 pooling = nn.MaxPool2d(kernel_size=2, stride=2)
-                self.enc_w_conv.add_module("pooling_{0}".format(idx), pooling)
-            elif first_layer:
+                if multi_path:
+                    self.enc_left_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+                    self.enc_right_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+                else:
+                    self.enc_w_conv.add_module(
+                        "pooling_{0}".format(idx), pooling)
+            elif multi_path:
                 lconv = IcoSpMaConv(
                     in_feats=input_channels,
                     out_feats=(self.cfg[idx] // 2),
                     kernel_size=3, pad=1)
-                self.enc_left_conv.add_module("lconv_{0}".format(idx), lconv)
+                self.enc_left_conv.add_module("l_conv_{0}".format(idx), lconv)
                 if self.batch_norm:
                     lbn = nn.BatchNorm2d(self.cfg[idx] // 2)
-                    self.enc_left_conv.add_module("lbn_{0}".format(idx), lbn)
+                    self.enc_left_conv.add_module("l_bn_{0}".format(idx), lbn)
                 lrelu = nn.ReLU(inplace=True)
-                self.enc_left_conv.add_module("lrelu_{0}".format(idx), lrelu)
+                self.enc_left_conv.add_module("l_relu_{0}".format(idx), lrelu)
                 rconv = IcoSpMaConv(
                     in_feats=input_channels,
                     out_feats=(self.cfg[idx] // 2),
                     kernel_size=3, pad=1)
-                self.enc_right_conv.add_module("rconv_{0}".format(idx), rconv)
+                self.enc_right_conv.add_module("r_conv_{0}".format(idx), rconv)
                 if self.batch_norm:
                     rbn = nn.BatchNorm2d(self.cfg[idx] // 2)
-                    self.enc_right_conv.add_module("rbn_{0}".format(idx), rbn)
+                    self.enc_right_conv.add_module("r_bn_{0}".format(idx), rbn)
                 rrelu = nn.ReLU(inplace=True)
-                self.enc_right_conv.add_module("rrelu_{0}".format(idx), rrelu)
+                self.enc_right_conv.add_module("r_relu_{0}".format(idx), rrelu)
                 input_channels = self.cfg[idx] // 2
             else:
                 conv = IcoSpMaConv(
                     in_feats=input_channels,
                     out_feats=self.cfg[idx],
                     kernel_size=3, pad=1)
                 self.enc_w_conv.add_module("conv_{0}".format(idx), conv)
@@ -379,50 +442,54 @@
     """
     class SphericalVGGBase(SphericalVGG):
         cfg = None
         batch_norm = False
 
         def __init__(self, input_channels, n_classes, input_order=5,
                      conv_mode="DiNe", dine_size=1, repa_size=5, repa_zoom=5,
-                     hidden_dim=4096, init_weights=True, standard_ico=False,
+                     dynamic_repa_zoom=False, hidden_dim=4096,
+                     fusion_level=1, init_weights=True, standard_ico=False,
                      cachedir=None):
             if self.cfg is None:
                 raise ValueError("Please specify a configuration first.")
             SphericalVGG.__init__(
                 self,
                 cfg=self.cfg,
                 batch_norm=self.batch_norm,
                 input_channels=input_channels,
                 n_classes=n_classes,
                 input_order=input_order,
                 conv_mode=conv_mode,
                 dine_size=dine_size,
                 repa_size=repa_size,
                 repa_zoom=repa_zoom,
+                dynamic_repa_zoom=dynamic_repa_zoom,
                 hidden_dim=hidden_dim,
+                fusion_level=fusion_level,
                 init_weights=init_weights,
                 standard_ico=standard_ico,
                 cachedir=cachedir)
 
     class SphericalGVGGBase(SphericalGVGG):
         cfg = None
         batch_norm = False
 
         def __init__(self, input_channels, n_classes, input_dim=194,
-                     hidden_dim=4096, init_weights=True):
+                     hidden_dim=4096, fusion_level=1, init_weights=True):
             if self.cfg is None:
                 raise ValueError("Please specify a configuration first.")
             SphericalGVGG.__init__(
                 self,
                 cfg=self.cfg,
                 batch_norm=self.batch_norm,
                 input_channels=input_channels,
                 n_classes=n_classes,
                 input_dim=input_dim,
                 hidden_dim=hidden_dim,
+                fusion_level=fusion_level,
                 init_weights=init_weights)
 
     klass_params.update({
         "__module__": destination_module_globals["__name__"],
         "_id":  destination_module_globals["__name__"] + "." + klass_name
     })
     _klass_name = "Spherical" + klass_name
```

### Comparing `surfify-0.1.0/surfify/models/base.py` & `surfify-0.2.0/surfify/models/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from collections import namedtuple
 import numpy as np
 from joblib import Memory
 import torch.nn as nn
 from ..utils import (
     icosahedron, neighbors, number_of_ico_vertices, downsample, interpolate,
     neighbors_rec, get_logger)
-from ..nn import IcoDiNeConv, IcoRePaConv
+from ..nn import IcoDiNeConv, IcoRePaConv, IcoPool
 
 # Global parameters
 logger = get_logger()
 
 
 class SphericalBase(nn.Module):
     """ Spherical network base information.
@@ -39,16 +39,16 @@
     >>> print(ico_info.keys())
     """
     Ico = namedtuple("Ico", ["order", "vertices", "triangles",
                              "neighbor_indices", "down_indices", "up_indices",
                              "conv_neighbor_indices"])
 
     def __init__(self, input_order, n_layers, conv_mode="DiNe",
-                 dine_size=1, repa_size=5, repa_zoom=5, standard_ico=False,
-                 cachedir=None):
+                 dine_size=1, repa_size=5, repa_zoom=5,
+                 dynamic_repa_zoom=False, standard_ico=False, cachedir=None):
         """ Init class.
 
         Parameters
         ----------
         input_order: int
             the input icosahedron order.
         n_layers: int
@@ -58,43 +58,63 @@
             - 1 ring Direct Neighbor convolution method.
         dine_size: int, default 1
             the size of the spherical convolution filter, ie. the number of
             neighbor rings to be considered.
         repa_size: int, default 5
             the size of the rectangular grid in the tangent space.
         repa_zoom: int, default 5
-            a multiplicative factor applied to the rectangular grid in the
-            tangent space.
+            control the rectangular grid spacing in the tangent space by
+            applying a multiplicative factor of `1 / repa_zoom`.
+        dynamic_repa_zoom: bool, default False
+            dynamically adapt the RePa zoom by applying a multiplicative factor
+            of `log(order + 1) + 1`.
         standard_ico: bool, default False
             optionally uses a standard icosahedron tessalation. FreeSurfer
             tesselation is used by default.
         cachedir: str, default None
             set this folder to use smart caching speedup.
         """
         super(SphericalBase, self).__init__()
         self.input_order = input_order
         self.n_layers = n_layers
         self.conv_mode = conv_mode
         self.dine_size = dine_size
         self.repa_size = repa_size
         self.repa_zoom = repa_zoom
+        self.dynamic_repa_zoom = dynamic_repa_zoom
         self.standard_ico = standard_ico
         self.cachedir = cachedir
         if conv_mode == "RePa":
             self.sconv = IcoRePaConv
         else:
             self.sconv = IcoDiNeConv
         self.ico = self.build_ico_info(
             input_order, n_layers, conv_mode, dine_size, repa_size, repa_zoom,
-            standard_ico, cachedir)
+            dynamic_repa_zoom, standard_ico, cachedir)
+
+    def _safe_forward(self, block, x, act=None, skip_last_act=False):
+        """ Perform a safe forward pass on a specific input block.
+        """
+        n_mods = len(list(block.children()))
+        for cnt, mod in enumerate(block.children()):
+            if isinstance(mod, IcoPool):
+                x = mod(x)[0]
+            else:
+                x = mod(x)
+                if skip_last_act and cnt == (n_mods - 1):
+                    continue
+                if act is not None:
+                    x = act(x)
+        return x
 
     @classmethod
     def build_ico_info(cls, input_order, n_layers, conv_mode="DiNe",
                        dine_size=1, repa_size=5, repa_zoom=5,
-                       standard_ico=False, cachedir=None):
+                       dynamic_repa_zoom=False, standard_ico=False,
+                       cachedir=None):
         """ Build an dictionnary containing icosehedron informations at
         each order of interest with the related upsampling and downsampling
         informations. This methods is useful to speed up processings
         by caching icosahedron onformations.
 
         Parameters
         ----------
@@ -107,16 +127,19 @@
             - 1 ring Direct Neighbor convolution method.
         dine_size: int, default 1
             the size of the spherical convolution filter, ie. the number of
             neighbor rings to be considered.
         repa_size: int, default 5
             the size of the rectangular grid in the tangent space.
         repa_zoom: int, default 5
-            a multiplicative factor applied to the rectangular grid in the
-            tangent space.
+            control the rectangular grid spacing in the tangent space by
+            applying a multiplicative factor of `1 / repa_zoom`.
+        dynamic_repa_zoom: bool, default False
+            dynamically adapt the RePa zoom by applying a multiplicative factor
+            of `log(order + 1) + 1`.
         standard_ico: bool, default False
             optionally uses a standard icosahedron tessalation. FreeSurfer
             tesselation is used by default.
         cachedir: str, default None
             set this folder to use smart caching speedup.
 
         Returns
@@ -146,19 +169,24 @@
                     conv_neighs = neighbors_cached(
                         vertices, triangles, depth=dine_size,
                         direct_neighbor=True)
                     conv_neighs = np.asarray(list(conv_neighs.values()))
                 logger.debug("- conv neighbors {0}: {1}".format(
                     order, conv_neighs.shape))
             elif conv_mode == "RePa":
+                if dynamic_repa_zoom:
+                    current_zoom = repa_zoom * (np.log(order + 1) + 1)
+                else:
+                    current_zoom = repa_zoom
                 conv_neighs, conv_weights, _ = neighbors_rec_cached(
                     vertices, triangles, size=repa_size,
-                    zoom=repa_zoom)
-                logger.debug("- conv neighbors {0}: {1} - {2}".format(
-                    order, conv_neighs.shape, conv_weights.shape))
+                    zoom=current_zoom)
+                logger.debug("- conv neighbors {0} - {1}: {2} - {3}".format(
+                    order, current_zoom, conv_neighs.shape,
+                    conv_weights.shape))
                 conv_neighs = (conv_neighs, conv_weights)
             else:
                 raise ValueError("Unexptected convolution mode.")
             ico[order] = cls.Ico(
                 order=order, vertices=vertices, triangles=triangles,
                 neighbor_indices=neighs, down_indices=None, up_indices=None,
                 conv_neighbor_indices=conv_neighs)
```

### Comparing `surfify-0.1.0/surfify/models/__init__.py` & `surfify-0.2.0/surfify/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 """
 Common architectures.
 """
 
 from .base import SphericalBase
 from .unet import SphericalUNet, SphericalGUNet
-from .vae import SphericalVAE, SphericalGVAE
+from .vae import (
+    SphericalVAE, HemiFusionEncoder, HemiFusionDecoder,
+    SphericalHemiFusionEncoder, SphericalHemiFusionDecoder)
 from .vgg import (
     SphericalVGG, SphericalGVGG,
     SphericalVGG11, SphericalVGG13, SphericalVGG16, SphericalVGG19,
     SphericalVGG11BN, SphericalVGG13BN, SphericalVGG16BN, SphericalVGG19BN,
     SphericalGVGG11, SphericalGVGG13, SphericalGVGG16, SphericalGVGG19,
     SphericalGVGG11BN, SphericalGVGG13BN, SphericalGVGG16BN, SphericalGVGG19BN)
```

### Comparing `surfify-0.1.0/surfify/models/unet.py` & `surfify-0.2.0/surfify/models/unet.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,177 @@
 The spherical UNet architecture.
 """
 
 # Imports
 import numpy as np
 import torch
 import torch.nn as nn
+import torch.nn.functional as func
 from joblib import Memory
 from ..utils import number_of_ico_vertices, get_logger, debug_msg
 from ..nn import (
     IcoUpConv, IcoMaxIndexUpSample, IcoFixIndexUpSample, IcoUpSample, IcoPool,
     IcoSpMaConv, IcoSpMaConvTranspose)
 from .base import SphericalBase
 
 
 # Global parameters
 logger = get_logger()
 
 
+class GraphicalUNet(nn.Module):
+    """ The Graph U-Net model: implements a U-Net like architecture with graph
+    pooling and unpooling operations.
+
+    Notes
+    -----
+    Debuging messages can be displayed by changing the log level using
+    ``setup_logging(level='debug')``.
+
+    See Also
+    --------
+    SphericalUNet, SphericalGUNet
+
+    References
+    ----------
+    Hongyang Gao, and Shuiwang Ji, Graph U-Nets, arXiv, 2019.
+    """
+    def __init__(self, in_channels, out_channels, depth=5, hidden_channels=32,
+                 pool_ratios=0.5, sum_res=False, act=func.relu):
+        """ Init GraphicalUNet.
+
+        Parameters
+        ----------
+        in_channels: int
+            input features/channels.
+        out_channels: int
+            output features/channels.
+        depth: int, default 5
+            number of layers in the UNet.
+        hidden_channels: int, default 32
+            number of convolutional filters for the convs.
+        pool_ratios: float or list of float, default 0.5
+            graph pooling ratio for each depth.
+        sum_res: bool,default True
+            if set to False, will use concatenation for integration of skip
+            connections instead summation.
+        act: torch.nn.functional, default relu
+            the nonlinearity to use.
+        """
+        from torch_sparse import spspmm
+        import torch_geometric.nn as gnn
+        from torch_geometric.utils import (
+            add_self_loops, sort_edge_index, remove_self_loops)
+        from torch_geometric.utils.repeat import repeat
+
+        super(GraphicalUNet, self).__init__()
+        assert depth >= 1
+        self.in_channels = in_channels
+        self.hidden_channels = hidden_channels
+        self.out_channels = out_channels
+        self.depth = depth
+        self.pool_ratios = repeat(pool_ratios, depth)
+        self.act = act
+        self.sum_res = sum_res
+
+        channels = hidden_channels
+        self.down_convs = torch.nn.ModuleList()
+        self.pools = torch.nn.ModuleList()
+        self.down_convs.append(gnn.GCNConv(in_channels, channels,
+                                           improved=True))
+        for i in range(depth):
+            new_channels = channels * 2
+            self.pools.append(gnn.TopKPooling(channels, self.pool_ratios[i]))
+            self.down_convs.append(gnn.GCNConv(channels, new_channels,
+                                               improved=True))
+            channels = new_channels
+
+        self.up_convs = torch.nn.ModuleList()
+        for i in range(depth - 1):
+            new_channels = channels // 2
+            in_channels = channels if sum_res else channels + new_channels
+            self.up_convs.append(gnn.GCNConv(in_channels, new_channels,
+                                             improved=True))
+            channels = new_channels
+        new_channels = channels // 2
+        in_channels = channels if sum_res else channels + new_channels
+        self.up_convs.append(gnn.GCNConv(in_channels, out_channels,
+                                         improved=True))
+
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        for conv in self.down_convs:
+            conv.reset_parameters()
+        for pool in self.pools:
+            pool.reset_parameters()
+        for conv in self.up_convs:
+            conv.reset_parameters()
+
+    def forward(self, x, edge_index, batch=None):
+        if batch is None:
+            batch = edge_index.new_zeros(x.size(0))
+        edge_weight = x.new_ones(edge_index.size(1))
+
+        # print("input", x.shape)
+        x = self.down_convs[0](x, edge_index, edge_weight)
+        x = self.act(x)
+        # print("down", x.shape)
+
+        xs = [x]
+        edge_indices = [edge_index]
+        edge_weights = [edge_weight]
+        perms = []
+
+        for i in range(1, self.depth + 1):
+            # edge_index, edge_weight = self.augment_adj(
+            #    edge_index, edge_weight, x.size(0))
+            x, edge_index, edge_weight, batch, perm, _ = self.pools[i - 1](
+                x, edge_index, edge_weight, batch)
+            x = self.down_convs[i](x, edge_index, edge_weight)
+            x = self.act(x)
+            if i < self.depth:
+                xs += [x]
+                edge_indices += [edge_index]
+                edge_weights += [edge_weight]
+            perms += [perm]
+
+        for i in range(self.depth):
+            j = self.depth - 1 - i
+
+            res = xs[j]
+            edge_index = edge_indices[j]
+            edge_weight = edge_weights[j]
+            perm = perms[j]
+
+            up = torch.zeros(res.size(dim=0), x.size(dim=1), dtype=x.dtype,
+                             device=x.device)
+            up[perm] = x
+            # print("zero-pad", x.shape, up.shape)
+            x = res + up if self.sum_res else torch.cat((res, up), dim=-1)
+            # print("cat", x.shape)
+            x = self.up_convs[i](x, edge_index, edge_weight)
+            x = self.act(x) if i < self.depth - 1 else x
+            # print("up", x.shape)
+
+        return x
+
+    def augment_adj(self, edge_index, edge_weight, num_nodes):
+        edge_index, edge_weight = remove_self_loops(edge_index, edge_weight)
+        edge_index, edge_weight = add_self_loops(edge_index, edge_weight,
+                                                 num_nodes=num_nodes)
+        edge_index, edge_weight = sort_edge_index(edge_index, edge_weight,
+                                                  num_nodes)
+        edge_index, edge_weight = spspmm(edge_index, edge_weight, edge_index,
+                                         edge_weight, num_nodes, num_nodes,
+                                         num_nodes)
+        edge_index, edge_weight = remove_self_loops(edge_index, edge_weight)
+        return edge_index, edge_weight
+
+
 class SphericalUNet(SphericalBase):
     """ The Spherical U-Net architecture.
 
     The architecture is built upon specific spherical surface convolution,
     pooling, and transposed convolution modules. It has an encoder path and
     a decoder path, with a user-defined resolution steps. Different from the
     standard U-Net, all 3×3 convolution are replaced with the RePa or DiNe
@@ -69,16 +220,16 @@
     References
     ----------
     Zhao F, et al., Spherical U-Net on Cortical Surfaces: Methods and
     Applications, IPMI, 2019.
     """
     def __init__(self, in_order, in_channels, out_channels, depth=5,
                  start_filts=32, conv_mode="DiNe", dine_size=1, repa_size=5,
-                 repa_zoom=5, up_mode="interp", standard_ico=False,
-                 cachedir=None):
+                 repa_zoom=5, dynamic_repa_zoom=False, up_mode="interp",
+                 standard_ico=False, cachedir=None):
         """ Init SphericalUNet.
 
         Parameters
         ----------
         in_order: int
             the input icosahedron order.
         in_channels: int
@@ -94,32 +245,35 @@
             - 1 ring Direct Neighbor convolution method..
         dine_size: int, default 1
             the size of the spherical convolution filter, ie. the number of
             neighbor rings to be considered.
         repa_size: int, default 5
             the size of the rectangular grid in the tangent space.
         repa_zoom: int, default 5
-            a multiplicative factor applied to the rectangular grid in the
-            tangent space.
+            control the rectangular grid spacing in the tangent space by
+            applying a multiplicative factor of `1 / repa_zoom`.
+        dynamic_repa_zoom: bool, default False
+            dynamically adapt the RePa zoom by applying a multiplicative factor
+            of `log(order + 1) + 1`.
         up_mode: str, default 'interp'
             type of upsampling: 'transpose' for transpose
             convolution (1 ring), 'interp' for nearest neighbor linear
             interpolation, 'maxpad' for max pooling shifted zero padding,
             and 'zeropad' for classical zero padding.
         standard_ico: bool, default False
             optionaly use surfify tesselation.
         cachedir: str, default None
             set this folder to use smart caching speedup.
         """
         logger.debug("SphericalUNet init...")
         super(SphericalUNet, self).__init__(
             input_order=in_order, n_layers=depth,
             conv_mode=conv_mode, dine_size=dine_size, repa_size=repa_size,
-            repa_zoom=repa_zoom, standard_ico=standard_ico,
-            cachedir=cachedir)
+            repa_zoom=repa_zoom, dynamic_repa_zoom=dynamic_repa_zoom,
+            standard_ico=standard_ico, cachedir=cachedir)
         self.memory = Memory(cachedir, verbose=0)
         self.in_order = in_order
         self.depth = depth
         self.in_vertices = number_of_ico_vertices(order=in_order)
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.up_mode = up_mode
```

### Comparing `surfify-0.1.0/surfify/info.py` & `surfify-0.2.0/surfify/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # http://www.cecill.info/licences/Licence_CeCILL-B_V1-en.html
 # for details.
 ##########################################################################
 
 
 # Module current version
 version_major = 0
-version_minor = 1
+version_minor = 2
 version_micro = 0
 
 # Expected by setup.py: string of form "X.Y.Z"
 __version__ = "{0}.{1}.{2}".format(version_major, version_minor, version_micro)
 
 # Expected by setup.py: the status of the project
 CLASSIFIERS = ["Development Status :: 5 - Production/Stable",
```

### Comparing `surfify-0.1.0/surfify/losses/vae.py` & `surfify-0.2.0/surfify/losses/vae.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,34 +13,57 @@
 
 # Imports
 import torch
 from torch.nn import functional as func
 from torch.distributions import Normal, kl_divergence
 
 
+def log_likelihood(recon, xs):
+    """ Computes the log likelihood of the input sample given the reconstructed
+    sample
+
+    Parameters
+    ----------
+    recon: Tensor (N, C, H, W)
+        reconstructed images
+    xs: Tensor (N, C, H, W)
+        original images
+
+    Returns
+    -------
+    log_likelihoods: Tensor (N)
+        log likelihood for each sample
+    """
+    return -Normal(recon, torch.ones_like(recon)).log_prob(xs).sum(
+        dim=tuple(range(1, recon.ndim)))
+
+
 class SphericalVAELoss(object):
     """ Spherical VAE Loss.
     """
-    def __init__(self, beta=9, left_mask=None, right_mask=None):
+    def __init__(self, beta=9, left_mask=None, right_mask=None, use_mse=True):
         """ Init class.
 
         Parameters
         ----------
         beta: float, default 9
             weight of the kl divergence.
         left_mask: Tensor (azimuth, elevation), default None
             left cortical binary mask.
         right_mask: Tensor (azimuth, elevation), default None
             right cortical binary mask.
+        use_mse: bool, default True
+            optionally uses the log likelihood.
         """
         super(SphericalVAELoss, self).__init__()
         self.beta = beta
         self.left_mask = left_mask
         self.right_mask = right_mask
         self.layer_outputs = None
+        self.use_mse = use_mse
 
     def __call__(self, left_recon_x, right_recon_x, left_x, right_x):
         """ Compute loss.
         """
         if self.layer_outputs is None:
             raise ValueError(
                 "This loss needs intermediate layers outputs. Please register "
@@ -50,23 +73,32 @@
         if self.left_mask is None:
             device = left_x.device
             self.left_mask = torch.ones(
                 (left_x.shape[-2], left_x.shape[-1]), dtype=int).to(device)
             self.right_mask = torch.ones(
                 (right_x.shape[-2], right_x.shape[-1]), dtype=int).to(device)
 
-        # Reconstruction loss term i.e. the mean squared error
-        left_mse = func.mse_loss(
-            left_recon_x * self.left_mask.detach(),
-            left_x * self.left_mask.detach(), reduction="mean")
-        right_mse = func.mse_loss(
-            right_recon_x * self.right_mask.detach(),
-            right_x * self.right_mask.detach(), reduction="mean")
+        # Reconstruction loss terms
+        if self.use_mse:
+            left_recon_loss = func.mse_loss(
+                left_recon_x * self.left_mask.detach(),
+                left_x * self.left_mask.detach(), reduction="mean")
+            right_recon_loss = func.mse_loss(
+                right_recon_x * self.right_mask.detach(),
+                right_x * self.right_mask.detach(), reduction="mean")
+        else:
+            left_recon_loss = log_likelihood(
+                left_recon_x * self.left_mask.detach(),
+                left_x * self.left_mask.detach()).mean()
+            right_recon_loss = log_likelihood(
+                right_recon_x * self.right_mask.detach(),
+                right_x * self.right_mask.detach()).mean()
 
         # Latent loss between approximate posterior and prior for z
         kl_div = kl_divergence(q, Normal(0, 1)).mean(dim=0).sum()
 
         # Need to maximise the ELBO with respect to these weights
-        loss = left_mse + right_mse + self.beta * kl_div
+        loss = left_recon_loss + right_recon_loss + self.beta * kl_div
 
-        return loss, {"left_mse": left_mse, "right_mse": right_mse,
-                      "kl_div": kl_div}
+        return loss, {"left_recon_loss": left_recon_loss,
+                      "right_recon_loss": right_recon_loss,
+                      "kl_div": kl_div, "beta": self.beta}
```

### Comparing `surfify-0.1.0/surfify/datasets/_samples_generator.py` & `surfify-0.2.0/surfify/datasets/_samples_generator.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/datasets/__init__.py` & `surfify-0.2.0/surfify/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/nn/modules.py` & `surfify-0.2.0/surfify/nn/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,50 +107,53 @@
             in_feats=16, out_feats=8, kernel_size=4, stride=2, zero_pad=3,
             pad=1)
     >>> proj_ico_x = torch.zeros((10, 16, 96, 96))
     >>> proj_ico_x = module(proj_ico_x)
     >>> proj_ico_x.shape
     """
     def __init__(self, in_feats, out_feats, kernel_size, stride=1, pad=0,
-                 zero_pad=0):
+                 zero_pad=0, output_shape=None):
         """ Init IcoSpMaConvTranspose.
 
         Parameters
         ----------
         in_feats: int
             input features/channels.
         out_feats: int
             output features/channels.
         kernel_size: int or tuple
             the convolutional kernel size.
         stride: int or tuple, default 1
             controls the stride for the cross-correlation.
         pad: int or tuple (pad_azimuth, pad_elevation), default 0
             the size of the padding.
-        zero_pad: int or tuple, deffault 0
-            add a zero padding in bith axis befor the transpose convolution.
+        zero_pad: int or tuple, default 0
+            add a zero padding in both axes before the transpose convolution.
         """
         super(IcoSpMaConvTranspose, self).__init__()
         self.in_feats = in_feats
         self.out_feats = out_feats
         self.kernel_size = kernel_size
         self.stride = stride
         self.pad = pad
         self.zero_pad = zero_pad
+        self.output_shape = output_shape
         self.tconv = nn.ConvTranspose2d(
             in_channels=in_feats,
             out_channels=out_feats,
             kernel_size=kernel_size, stride=stride, padding=zero_pad)
 
     def forward(self, x):
         logger.debug("IcoSpMaConvTranspose...")
         logger.debug(debug_msg("input", x))
         x = circular_pad(x, pad=self.pad)
         logger.debug(debug_msg("pad", x))
-        x = self.tconv(x)
+        output_size = ([len(x)] + self.output_shape if self.output_shape
+                       else None)
+        x = self.tconv(x, output_size=output_size)
         logger.debug(debug_msg("transpose conv", x))
         return x
 
 
 class IcoRePaConv(nn.Module):
     """ Define the convolutional layer on icosahedron discretized sphere using
     rectagular filter in tangent plane.
@@ -249,39 +252,42 @@
     >>> import torch
     >>> from surfify.nn import IcoDiNeConv
     >>> from surfify.utils import icosahedron, neighbors
     >>> ico2_vertices, ico2_triangles = icosahedron(order=2)
     >>> neighbor_indices = neighbors(
             ico2_vertices, ico2_triangles, depth=1, direct_neighbor=True)
     >>> neighbor_indices = np.asarray(list(neighbor_indices.values()))
-    >>> module = IcoUpConv(
+    >>> module = IcoDiNeConv(
             in_feats=8, out_feats=8, neigh_indices=neighbor_indices)
     >>> ico2_x = torch.zeros((10, 8, len(ico2_vertices)))
     >>> ico2_x = module(ico2_x)
     >>> ico2_x.shape
     """
-    def __init__(self, in_feats, out_feats, neigh_indices):
+    def __init__(self, in_feats, out_feats, neigh_indices, bias=True):
         """ Init IcoDiNeConv.
 
         Parameters
         ----------
         in_feats: int
             input features/channels.
         out_feats: int
             output features/channels.
         neigh_indices: array (N, k)
             conv layer's filters' neighborhood indices, where N is the ico
             number of vertices and k the considered nodes neighbors.
+        bias: bool, default True
+            the layer will learn / not learn an additive bias.
         """
         super(IcoDiNeConv, self).__init__()
         self.in_feats = in_feats
         self.out_feats = out_feats
         self.neigh_indices = neigh_indices
         self.n_vertices, self.neigh_size = neigh_indices.shape
-        self.weight = nn.Linear(self.neigh_size * in_feats, out_feats)
+        self.weight = nn.Linear(self.neigh_size * in_feats, out_feats,
+                                bias=bias)
 
     def forward(self, x):
         """ Forward method.
         """
         logger.debug("IcoDiNeConv...")
         logger.debug(debug_msg("input", x))
         logger.debug("  weight: {0}".format(self.weight))
@@ -320,15 +326,15 @@
     >>> down_neigh_indices = neighbors(
             ico2_vertices, ico2_triangles, depth=1, direct_neighbor=True)
     >>> down_neigh_indices = np.asarray(list(down_neigh_indices.values()))
     >>> down_indices = downsample(ico3_vertices, ico2_vertices)
     >>> module = IcoPool(
             down_neigh_indices=down_neigh_indices, down_indices=down_indices)
     >>> ico3_x = torch.zeros((10, 4, len(ico3_vertices)))
-    >>> ico2_x = module(ico3_x)
+    >>> ico2_x, _ = module(ico3_x)
     >>> ico2_x.shape, ico3_x.shape
     """
     def __init__(self, down_neigh_indices, down_indices, pooling_type="mean"):
         """ Init IcoPool.
 
         Parameters
         ----------
@@ -424,16 +430,16 @@
         self.down_indices = down_indices
         self.n_vertices, self.neigh_size = self.up_neigh_indices.shape
 
         self.flat_neigh_indices = self.neigh_indices.reshape(-1)
         self.argsort_neigh_indices = np.argsort(self.flat_neigh_indices)
         self.sorted_neigh_indices = self.flat_neigh_indices[
             self.argsort_neigh_indices]
-        assert(np.unique(self.sorted_neigh_indices).tolist() ==
-               list(range(self.n_vertices)))
+        assert (np.unique(self.sorted_neigh_indices).tolist() ==
+                list(range(self.n_vertices)))
 
         self.sorted_2occ_12neigh_indices = self.sorted_neigh_indices[:24]
         self._check_occurence(self.sorted_2occ_12neigh_indices, occ=2)
         self.sorted_1occ_neigh_indices = self.sorted_neigh_indices[
             24: len(down_indices) + 12]
         self._check_occurence(self.sorted_1occ_neigh_indices, occ=1)
         self.sorted_2occ_neigh_indices = self.sorted_neigh_indices[
@@ -539,16 +545,16 @@
         self.down_indices = down_indices
         self.n_vertices, self.neigh_size = self.up_neigh_indices.shape
 
         self.flat_neigh_indices = self.neigh_indices.reshape(-1)
         self.argsort_neigh_indices = np.argsort(self.flat_neigh_indices)
         self.sorted_neigh_indices = self.flat_neigh_indices[
             self.argsort_neigh_indices]
-        assert(np.unique(self.sorted_neigh_indices).tolist() ==
-               list(range(self.n_vertices)))
+        assert (np.unique(self.sorted_neigh_indices).tolist() ==
+                list(range(self.n_vertices)))
         count = collections.Counter(self.sorted_neigh_indices)
         self.count = sorted(count.items(), key=lambda item: item[0])
 
         self.weight = nn.Linear(in_feats, self.neigh_size * out_feats)
 
     def _check_occurence(self, data, occ):
         count = collections.Counter(data)
@@ -573,15 +579,15 @@
         x = x.view(n_samples, n_vertices, self.neigh_size, self.out_feats)
         logger.debug(debug_msg("weighted input", x))
         x = x.view(n_samples, n_vertices * self.neigh_size, self.out_feats)
         out = torch.zeros(n_samples, self.out_feats, self.n_vertices)
         start = 0
         for idx in range(self.n_vertices):
             _idx, _count = self.count[idx]
-            assert(_idx == idx)
+            assert _idx == idx
             stop = start + _count
             _x = x[:, self.argsort_neigh_indices[start: stop]]
             out[..., idx] = torch.mean(_x, dim=1)
             start = stop
         logger.debug(debug_msg("output", out))
         return out
 
@@ -606,17 +612,16 @@
     >>> from surfify.nn import IcoUpSample
     >>> from surfify.utils import interpolate, icosahedron
     >>> ico2_vertices, ico2_triangles = icosahedron(order=2)
     >>> ico3_vertices, ico3_triangles = icosahedron(order=3)
     >>> up_indices = interpolate(
             ico2_vertices, ico3_vertices, ico3_triangles)
     >>> up_indices = np.asarray(list(up_indices.values()))
-    >>> module = IcoGenericUpConv(
-            in_feats=8, out_feats=4, up_neigh_indices=up_indices,
-            down_indices=down_indices)
+    >>> module = IcoUpSample(
+            in_feats=8, out_feats=4, up_neigh_indices=up_indices)
     >>> ico2_x = torch.zeros((10, 8, len(ico2_vertices)))
     >>> ico3_x = module(ico2_x)
     >>> ico2_x.shape, ico3_x.shape
     """
     def __init__(self, in_feats, out_feats, up_neigh_indices):
         """ Init IcoUpSample.
 
@@ -681,17 +686,16 @@
     >>> from surfify.nn import IcoFixIndexUpSample
     >>> from surfify.utils import interpolate, icosahedron
     >>> ico2_vertices, ico2_triangles = icosahedron(order=2)
     >>> ico3_vertices, ico3_triangles = icosahedron(order=3)
     >>> up_indices = interpolate(
             ico2_vertices, ico3_vertices, ico3_triangles)
     >>> up_indices = np.asarray(list(up_indices.values()))
-    >>> module = IcoGenericUpConv(
-            in_feats=8, out_feats=4, up_neigh_indices=up_indices,
-            down_indices=down_indices)
+    >>> module = IcoFixIndexUpSample(
+            in_feats=8, out_feats=4, up_neigh_indices=up_indices)
     >>> ico2_x = torch.zeros((10, 8, len(ico2_vertices)))
     >>> ico3_x = module(ico2_x)
     >>> ico2_x.shape, ico3_x.shape
     """
     def __init__(self, in_feats, out_feats, up_neigh_indices):
         """ Init IcoFixIndexUpSample.
```

### Comparing `surfify-0.1.0/surfify/nn/functional.py` & `surfify-0.2.0/surfify/nn/functional.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/nn/__init__.py` & `surfify-0.2.0/surfify/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `surfify-0.1.0/surfify/augmentation/augmentation.py` & `surfify-0.2.0/surfify/augmentation/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,209 +4,273 @@
 # Distributed under the terms of the CeCILL-B license, as published by
 # the CEA-CNRS-INRIA. Refer to the LICENSE file or to
 # http://www.cecill.info/licences/Licence_CeCILL-B_V1-en.html
 # for details.
 ##########################################################################
 
 """
-Surface augmentation tools.
+Augmentations are directly inspired by natural image transformations used to
+train CNNs.
 """
 
 # Imports
-import numbers
-import datetime
+from joblib import Memory
+import itertools
 import numpy as np
+import torch
 from surfify.utils import (
-    neighbors, rotate_data, find_neighbors, find_rotation_interpol_coefs)
+    neighbors, rotate_data, find_rotation_interpol_coefs)
+from surfify.nn import IcoDiNeConv
 from surfify.utils.io import compute_and_store
+from .utils import RandomAugmentation
 
 
-class SphericalRandomRotation(object):
-    """ Rotation of the icosahedron's vertices.
+class SurfCutOut(RandomAugmentation):
+    """ Starting from random vertices, the SurfCutOut sets an adaptive connex
+    neighborhood to zero.
 
     See Also
     --------
-    surfify.utils.rotate_data
-
-    Examples
-    --------
-    >>> from surfify.utils import icosahedron
-    >>> from surfify.datasets import make_classification
-    >>> from surfify.augmentation import SphericalRandomRotation
-    >>> import matplotlib.pyplot as plt
-    >>> from surfify.plotting import plot_trisurf
-    >>> ico3_verts, ico3_tris = icosahedron(order=3)
-    >>> X, y = make_classification(ico3_verts, n_samples=1, n_classes=3,
-                                   scale=1, seed=42)
-    >>> processor = SphericalRandomRotation(
-            ico3_verts, ico3_tris, angles=(45, 0, 0))
-    >>> y_rot = processor(y)
-    >>> plot_trisurf(ico3_verts, triangles=ico3_tris, texture=y_rot,
-                     is_label=False)
-    >>> plt.show()
+    surfify.utils.neighbors
     """
-    def __init__(self, vertices, triangles, angles=(5, 0, 0), fixed_angle=True,
-                 interpolation="barycentric", cachedir=None):
+    def __init__(self, vertices, triangles, neighs=None, patch_size=3,
+                 n_patches=1, sigma=0, replacement_value=0, cachedir=None):
         """ Init class.
 
         Parameters
         ----------
         vertices: array (N, 3)
             icosahedron's vertices.
         triangles: array (M, 3)
             icosahdron's triangles.
-        angles: 3-uplet, default (5, 0, 0)
-            the rotation angles intervals in degrees for each axis (Euler
-            representation).
-        fixed_angle: bool, default True
-            if True changes the angle of the rotation at each call. This option
-            slows down the training as the rotation needs to be initialiazed at
-            each call
-        interpolation: str, default 'barycentric'
-            type of interpolation to use by the rotate_data function, see
-            `rotate_data`.
+        neighs: dict, default None
+            optionnaly specify the DiNe neighboors of each vertex as build
+            with `sufify.utils.neighbors`, ie. a dictionary with vertices row
+            index as keys and a dictionary of neighbors vertices row indexes
+            organized by rings as values.
+        patch_size: int, default 3
+            the number of neighboring rings from one node to be considered
+            during the ablation.
+        n_patches: int, default 1
+            the number of patches to be considered.
+        sigma: int, default 0
+            use different patch size in [patch_size-sigma, patch_size+sigma]
+            for each cutout.
+        replacement_value: float, default 0
+            the replacement patch value.
         cachedir: str, default None
-            set this folder to use smart caching speedup.
+            the optional path to cache the neighbors function output.
         """
+        super().__init__()
+        memory = Memory(cachedir, verbose=0)
+        neighbors_cached = memory.cache(neighbors)
         self.vertices = vertices
         self.triangles = triangles
-        self.angles = [interval(val) for val in angles]
-        self.fixed_angle = fixed_angle
-        if fixed_angle:
-            self.angles = [
-                np.random.uniform(val[0], val[1]) for val in self.angles]
-        self.interpolation = interpolation
-        self.rotate_data_cached = compute_and_store(
-            find_rotation_interpol_coefs, cachedir)(rotate_data)
+        max_depth = patch_size
+        if isinstance(patch_size, RandomAugmentation.Interval):
+            max_depth = patch_size.high
+        if neighs is None or type(neighs[0]) is not dict:
+            self.neighs = neighbors_cached(
+                vertices, triangles, depth=max_depth)
+        else:
+            self.neighs = neighs
+        self.patch_size = patch_size
+        self.n_patches = n_patches
+        self.sigma = sigma
+        self.replacement_value = replacement_value
 
-    def __call__(self, data):
-        """ Rotates the provided vertices and projects the input data
-        accordingly.
+    def run(self, data):
+        """ Applies the cut out (ablation) augmentation to the data.
 
         Parameters
         ----------
         data: array (N, )
             input data/texture.
 
         Returns
         -------
-        rot_data: arr (N, )
-            rotated input data.
+        data: arr (N, )
+            ablated input data.
         """
-        np.random.seed(datetime.datetime.now().second +
-                       datetime.datetime.now().microsecond)
-        angles = self.angles
-        if not self.fixed_angle:
-            angles = [np.random.uniform(val[0], val[1]) for val in self.angles]
-        return self.rotate_data_cached(
-            data[np.newaxis, :], self.vertices, self.triangles,
-            angles).squeeze()
+        for _ in range(self.n_patches):
+            random_node = np.random.randint(len(self.vertices))
+            # If sigma is not null, patch size can vary around its current
+            # value by +- sigma for each patch, but staying in
+            # [0, max_patch_size]
+            max_patch_size = self.patch_size
+            if "patch_size" in self.intervals.keys():
+                max_patch_size = self.intervals["patch_size"].high
+            random_size = np.random.randint(
+                max(self.patch_size - self.sigma, 0),
+                min(self.patch_size + self.sigma + 1, max_patch_size + 1))
+            # for each neighbor, so in each direction, we seek neighbors
+            # up to a different random order, creating irregular patches
+            # in different directions
+            patch_indices = []
+            for neigh in self.neighs[random_node][1]:
+                _size = np.random.randint(random_size)
+                for ring in range(1, _size + 1):
+                    patch_indices += self.neighs[neigh][ring]
+            patch_indices = list(set(patch_indices))
+            data[patch_indices] = self.replacement_value
+        return data
+
+
+class SurfNoise(RandomAugmentation):
+    """ The SurfNoise adds a Gaussian white noise with standard deviation
+    sigma.
+    """
+    def __init__(self, sigma):
+        """ Init class.
 
+        Parameters
+        ----------
+        sigma: float
+            the noise standard deviation.
+        """
+        super().__init__()
+        self.sigma = sigma
 
-class SphericalRandomCut(object):
-    """ Random cut of patches on the icosahedron: use Direct Neighbors (DiNe)
-    to build patches.
+    def run(self, data):
+        """ Applies the noising augmentation to the data.
 
-    See Also
-    --------
-    surfify.utils.neighbors
+        Parameters
+        ----------
+        data: array (N, )
+            input data/texture.
 
-    Examples
+        Returns
+        -------
+        data: arr (N, )
+            noised input data.
+        """
+        data += np.random.normal(0, self.sigma, len(data))
+        return data
+
+
+class SurfBlur(RandomAugmentation):
+    """ An icosahedron texture Gaussian blur implementation. It uses the DiNe
+    convolution filter for speed. The receptive field is controlled by sigma,
+    the standard deviation of the kernel.
+
+    See Also
     --------
-    >>> from surfify.utils import icosahedron
-    >>> from surfify.datasets import make_classification
-    >>> from surfify.augmentation import SphericalRandomCut
-    >>> import matplotlib.pyplot as plt
-    >>> from surfify.plotting import plot_trisurf
-    >>> ico3_verts, ico3_tris = icosahedron(order=3)
-    >>> X, y = make_classification(ico3_verts, n_samples=1, n_classes=3,
-                                   scale=1, seed=42)
-    >>> processor = SphericalRandomCut(
-            ico3_verts, ico3_tris, replacement_value=5)
-    >>> y_cut = processor(y)
-    >>> plot_trisurf(ico3_verts, triangles=ico3_tris, texture=y_cut,
-                     is_label=True)
-    >>> plt.show()
+    surfify.utils.neighbors, surfify.nn.modules.IcoDiNeConv
     """
-    def __init__(self, vertices, triangles, neighs=None, patch_size=3,
-                 n_patches=1, replacement_value=0):
+    def __init__(self, vertices, triangles, sigma, neighs=None, cachedir=None):
         """ Init class.
 
         Parameters
         ----------
         vertices: array (N, 3)
             icosahedron's vertices.
         triangles: array (M, 3)
             icosahdron's triangles.
+        sigma: float
+            sigma parameter of the gaussian filter.
         neighs: dict, default None
             optionnaly specify the DiNe neighboors of each vertex as build
             with `sufify.utils.neighbors`, ie. a dictionary with vertices row
             index as keys and a dictionary of neighbors vertices row indexes
             organized by rings as values.
-        n_rings: int, default 3
-            the number of neighboring rings from one node to be considered
-            during the ablation.
-        n_patches: int, default 1
-            the number of patches to be considered.
-        replacement_value: float, default 0
-            the replacement patch value.
+        cachedir: str, default None
+            the optional path to cache the neighbors function output.
         """
+        super().__init__()
+        memory = Memory(cachedir, verbose=0)
+        neighbors_cached = memory.cache(neighbors)
         self.vertices = vertices
         self.triangles = triangles
+        self.sigma = sigma
+        max_sigma = sigma
+        if isinstance(sigma, RandomAugmentation.Interval):
+            max_sigma = sigma.high
+        depth = max(1, int(2 * max_sigma + 0.5))
         if neighs is None:
-            self.neighs = neighbors(vertices, triangles, direct_neighbor=True)
+            self.neighs = neighbors_cached(vertices, triangles, depth=depth,
+                                           direct_neighbor=True)
         else:
             self.neighs = neighs
-        self.patch_size = patch_size
-        self.n_patches = n_patches
-        self.replacement_value = replacement_value
+        self.neighs = np.asarray(list(self.neighs.values()))
+        self.positions = np.array([0] + list(itertools.chain(*[
+            [ring] * (6 * ring) for ring in range(1, depth + 1)])))
+        assert len(self.positions) == len(self.neighs[0])
+        self.conv = IcoDiNeConv(1, 1, self.neighs, bias=False)
 
-    def __call__(self, data):
-        """ Applies the cut out (ablation) augmentation to the data.
+    def run(self, data):
+        """ Applies the augmentation to the data.
 
         Parameters
         ----------
         data: array (N, )
             input data/texture.
 
         Returns
         -------
-        cut_data: arr (N, )
-            ablated input data.
+        data: array (N, )
+            blurred output data.
         """
-        data_cut = data.copy()
-        for idx in range(self.n_patches):
-            random_node = np.random.randint(0, len(self.vertices))
-            patch_indices = find_neighbors(
-                random_node, self.patch_size, self.neighs)
-            data_cut[patch_indices] = self.replacement_value
-        return data_cut
-
-
-def interval(bound, lower=None):
-    """ Create an interval.
-
-    Parameters
-    ----------
-    bound: 2-uplet or number
-        the object used to build the interval.
-    lower: number, default None
-        the lower bound of the interval. If not specified, a symetric
-        interval is generated.
-
-    Returns
-    -------
-    interval: 2-uplet
-        an interval.
+        gaussian_kernel = np.exp(-0.5 * (self.positions / self.sigma) ** 2)
+        gaussian_kernel = gaussian_kernel / gaussian_kernel.sum()
+        with torch.no_grad():
+            self.conv.weight.weight = torch.nn.Parameter(
+                torch.Tensor(gaussian_kernel), False)
+        data = self.conv(torch.from_numpy(data[None, None]).float())
+        return data.numpy().squeeze()
+
+
+class SurfRotation(RandomAugmentation):
+    """ The SurfRotation rotate the cortical measures.
+
+    See Also
+    --------
+    surfify.utils.rotate_data
     """
-    if isinstance(bound, numbers.Number):
-        if bound < 0:
-            raise ValueError("Specified interval value must be positive.")
-        if lower is None:
-            lower = -bound
-        return (lower, bound)
-    if len(bound) != 2:
-        raise ValueError("Interval must be specified with 2 values.")
-    min_val, max_val = bound
-    if min_val > max_val:
-        raise ValueError("Wrong interval boundaries.")
-    return tuple(bound)
+    def __init__(self, vertices, triangles, phi=5, theta=0, psi=0,
+                 interpolation="barycentric", cachedir=None):
+        """ Init class.
+
+        Parameters
+        ----------
+        vertices: array (N, 3)
+            icosahedron's vertices.
+        triangles: array (M, 3)
+            icosahdron's triangles.
+        phi: float, default 5
+            the rotation phi angle in degrees: Euler representation.
+        theta: float, default 0
+            the rotation theta angle in degrees: Euler representation.
+        psi: float, default 0
+            the rotation psi angle in degrees: Euler representation.
+        interpolation: str, default 'barycentric'
+            type of interpolation to use by the rotate_data function, see
+            `rotate_data`.
+        cachedir: str, default None
+            set this folder to use smart caching speedup.
+        """
+        super().__init__()
+        self.vertices = vertices
+        self.triangles = triangles
+        self.phi = phi
+        self.theta = theta
+        self.psi = psi
+        self.interpolation = interpolation
+        self.rotate_data_cached = compute_and_store(
+            find_rotation_interpol_coefs, cachedir)(rotate_data)
+
+    def run(self, data):
+        """ Rotates the provided vertices and projects the input data
+        accordingly.
+
+        Parameters
+        ----------
+        data: array (N, )
+            input data/texture.
+
+        Returns
+        -------
+        data: arr (N, )
+            rotated input data.
+        """
+        return self.rotate_data_cached(
+            data[np.newaxis, :, np.newaxis], self.vertices, self.triangles,
+            [self.phi, self.theta, self.psi], self.interpolation).squeeze()
```

### Comparing `surfify-0.1.0/surfify/plotting/surface.py` & `surfify-0.2.0/surfify/plotting/surface.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d import axes3d
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 
 def plot_trisurf(vertices, triangles, texture=None, vmin=None,
                  vmax=None, colorbar=True, fig=None, ax=None,
-                 is_label=False, alpha=1, edgecolors="black"):
+                 is_label=False, alpha=1, edgecolors="black",
+                 linewidths=1, color_map=cm.coolwarm):
     """ Display a triangular surface.
 
     Parameters
     ----------
     vertices: array (N, 3)
         the surface vertices.
     triangles: array (M, 3)
@@ -47,14 +48,18 @@
         optionally specify that the texture contains labels in order to
         use most representative neighboor interpolation.
     alpha: float, default 1
         number between 0 and 1 defining the opacity of the faces. Not use
         when texture is None, where alpha is fixed at 0.1
     edgecolors: string, default 'black'
         name of the matplotlib color to use for the edges
+    linewidths: float, default 1
+        edge line width.
+    color_map: Mapping, default cm.coolwarm
+        container for colormaps.
     """
 
     # Parameters
     if texture is not None and vmin is None:
         vmin = texture.min()
     if texture is not None and vmax is None:
         vmax = texture.max()
@@ -68,29 +73,31 @@
         else:
             texture = np.asarray([np.mean(texture[tri]) for tri in triangles])
 
     # Display tri surface
     x, y, z = vertices[:, 0], vertices[:, 1], vertices[:, 2]
     triangle_vertices = np.array([vertices[tri] for tri in triangles])
     if texture is not None:
-        norm = colors.Normalize(vmin=0, vmax=vmax, clip=False)
-        facecolors = cm.coolwarm(norm(texture))
+        norm = colors.Normalize(vmin=vmin, vmax=vmax, clip=False)
+        facecolors = color_map(norm(texture))
         polygon = Poly3DCollection(triangle_vertices, facecolors=facecolors,
-                                   edgecolors=edgecolors, alpha=alpha)
+                                   edgecolors=edgecolors, alpha=alpha,
+                                   linewidths=linewidths)
     else:
         polygon = Poly3DCollection(triangle_vertices, facecolors="white",
-                                   edgecolors=edgecolors, alpha=0.1)
+                                   edgecolors=edgecolors, alpha=0.1,
+                                   linewidths=linewidths)
     ax.add_collection3d(polygon)
     ax.set_xlim(-1, 1)
     ax.set_ylim(-1, 1)
     ax.set_zlim(-1, 1)
 
     # Add colorbar
     if texture is not None:
-        m = cm.ScalarMappable(cmap=cm.coolwarm, norm=norm)
+        m = cm.ScalarMappable(cmap=color_map, norm=norm)
         m.set_array(texture)
         if colorbar:
             fig.colorbar(m, ax=ax, fraction=0.046, pad=0.04)
 
     # Get rid of the panes
     ax.xaxis.set_pane_color((1.0, 1.0, 1.0, 0.0))
     ax.yaxis.set_pane_color((1.0, 1.0, 1.0, 0.0))
```

### Comparing `surfify-0.1.0/PKG-INFO` & `surfify-0.2.0/surfify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: surfify
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 PyTorch toolbox to work with spherical surfaces.
 
 Home-page: https://github.com/neurospin-deepinsight/surfify
 Author: 
 surfify developers
```

### Comparing `surfify-0.1.0/README.rst` & `surfify-0.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. -*- mode: rst -*-
 
 |PythonVersion|_ |Coveralls|_ |Testing|_ |Pep8|_ |PyPi|_ |Doc|_
 
-.. |PythonVersion| image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-.. _PythonVersion: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
+.. |PythonVersion| image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue
+.. _PythonVersion: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue
 
 .. |Coveralls| image:: https://coveralls.io/repos/neurospin-deepinsight/surfify/badge.svg?branch=master&service=github
 .. _Coveralls: https://coveralls.io/github/neurospin-deepinsight/surfify
 
 .. |Testing| image:: https://github.com/neurospin-deepinsight/surfify/actions/workflows/testing.yml/badge.svg
 .. _Testing: https://github.com/neurospin-deepinsight/surfify/actions
 
@@ -70,15 +70,15 @@
     :width: 400px
     :align: center
     
 Important links
 ===============
 
 - `Official source code repo <https://github.com/neurospin-deepinsight/surfify>`_
-- `HTML stable documentation: <https://surfify.readthedocs.io/en/v0.1.0>`_
+- `HTML stable documentation <https://surfify.readthedocs.io/en/v0.2.0>`_
 - `HTML documentation <https://surfify.readthedocs.io/en/latest>`_
 - `Release notes <https://github.com/neurospin-deepinsight/surfify/blob/master/CHANGELOG.rst>`_
 
 Where to start
 ==============
 
 Examples are available in the
```

