# Comparing `tmp/tiskitpy-0.4.tar.gz` & `tmp/tiskitpy-0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiskitpy-0.4.tar", last modified: Thu Jul 13 07:14:13 2023, max compression
+gzip compressed data, was "tiskitpy-0.4.post1.tar", last modified: Thu Jul 13 09:39:30 2023, max compression
```

## Comparing `tiskitpy-0.4.tar` & `tiskitpy-0.4.post1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.149482 tiskitpy-0.4/
--rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskitpy-0.4/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)       83 2023-07-13 06:27:46.000000 tiskitpy-0.4/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     2837 2023-07-13 07:14:13.149203 tiskitpy-0.4/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     2029 2023-07-13 06:27:17.000000 tiskitpy-0.4/README.md
--rw-r--r--   0 crawford   (501) admin       (80)       38 2023-07-13 07:14:13.149549 tiskitpy-0.4/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     1402 2023-07-13 06:26:59.000000 tiskitpy-0.4/setup.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.127877 tiskitpy-0.4/tiskitpy/
--rw-r--r--   0 crawford   (501) admin       (80)     1800 2023-07-13 06:17:33.000000 tiskitpy-0.4/tiskitpy/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-10-11 14:36:20.000000 tiskitpy-0.4/tiskitpy/clean_rotator.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.132210 tiskitpy-0.4/tiskitpy/data_cleaner/
--rw-r--r--   0 crawford   (501) admin       (80)      212 2023-07-13 06:11:49.000000 tiskitpy-0.4/tiskitpy/data_cleaner/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     4196 2023-07-13 06:12:41.000000 tiskitpy-0.4/tiskitpy/data_cleaner/cleaner_string.py
--rw-r--r--   0 crawford   (501) admin       (80)    19092 2023-07-13 06:50:24.000000 tiskitpy-0.4/tiskitpy/data_cleaner/data_cleaner_tf.py
--rw-r--r--   0 crawford   (501) admin       (80)     6169 2023-07-13 06:16:45.000000 tiskitpy-0.4/tiskitpy/data_cleaner/dcrfs.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.135456 tiskitpy-0.4/tiskitpy/decimate/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskitpy-0.4/tiskitpy/decimate/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      184 2021-06-11 13:44:08.000000 tiskitpy-0.4/tiskitpy/decimate/ToDo.md
--rw-r--r--   0 crawford   (501) admin       (80)     1678 2021-06-24 09:28:18.000000 tiskitpy-0.4/tiskitpy/decimate/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.141139 tiskitpy-0.4/tiskitpy/decimate/__pycache__/
--rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     1871 2023-07-11 20:46:27.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4980 2022-12-16 15:51:31.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)    13928 2022-12-14 10:39:43.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)    13946 2023-07-13 06:38:30.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     7514 2023-07-11 20:46:27.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskitpy-0.4/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     5760 2023-07-12 22:13:55.000000 tiskitpy-0.4/tiskitpy/decimate/decimate_SDS.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    18945 2023-07-13 05:48:23.000000 tiskitpy-0.4/tiskitpy/decimate/decimator.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     7672 2022-07-12 10:18:50.000000 tiskitpy-0.4/tiskitpy/decimate/fir_filter.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.142905 tiskitpy-0.4/tiskitpy/decimate/sac_fir/
--rw-r--r--   0 crawford   (501) admin       (80)      845 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec2
--rw-r--r--   0 crawford   (501) admin       (80)     1218 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec3
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec4
--rw-r--r--   0 crawford   (501) admin       (80)     1866 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec5
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec6
--rw-r--r--   0 crawford   (501) admin       (80)     1898 2012-02-01 20:07:02.000000 tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec7
--rw-r--r--   0 crawford   (501) admin       (80)       18 2021-06-07 17:29:05.000000 tiskitpy-0.4/tiskitpy/decimate/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.143670 tiskitpy-0.4/tiskitpy/fir_corr/
--rw-r--r--   0 crawford   (501) admin       (80)       39 2022-07-06 10:50:29.000000 tiskitpy-0.4/tiskitpy/fir_corr/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    12282 2022-07-12 10:17:27.000000 tiskitpy-0.4/tiskitpy/fir_corr/fir2caus.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2231 2022-07-23 07:09:08.000000 tiskitpy-0.4/tiskitpy/read_mseed.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.144345 tiskitpy-0.4/tiskitpy/response_functions/
--rw-r--r--   0 crawford   (501) admin       (80)      133 2023-07-13 06:37:56.000000 tiskitpy-0.4/tiskitpy/response_functions/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    26617 2023-07-13 07:06:35.000000 tiskitpy-0.4/tiskitpy/response_functions/response_functions.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.146699 tiskitpy-0.4/tiskitpy/rptransient/
--rw-r--r--   0 crawford   (501) admin       (80)       85 2022-05-04 22:13:23.000000 tiskitpy-0.4/tiskitpy/rptransient/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    23821 2022-10-11 14:36:20.000000 tiskitpy-0.4/tiskitpy/rptransient/dirac_comb.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    10734 2022-07-12 10:07:11.000000 tiskitpy-0.4/tiskitpy/rptransient/periodic_transient.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3099 2022-01-31 13:45:08.000000 tiskitpy-0.4/tiskitpy/rptransient/transients.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3201 2022-07-23 07:22:23.000000 tiskitpy-0.4/tiskitpy/rptransient/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       21 2021-12-09 22:15:36.000000 tiskitpy-0.4/tiskitpy/rptransient/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.148344 tiskitpy-0.4/tiskitpy/spectral_density/
--rw-r--r--   0 crawford   (501) admin       (80)     2781 2022-05-04 22:20:44.000000 tiskitpy-0.4/tiskitpy/spectral_density/Peterson_noise_model.py
--rw-r--r--   0 crawford   (501) admin       (80)      125 2022-05-04 22:25:27.000000 tiskitpy-0.4/tiskitpy/spectral_density/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    56471 2023-07-13 06:53:58.000000 tiskitpy-0.4/tiskitpy/spectral_density/spectral_density.py
--rw-r--r--   0 crawford   (501) admin       (80)     4116 2022-03-28 12:36:00.000000 tiskitpy-0.4/tiskitpy/spectral_density/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       18 2022-01-06 11:06:02.000000 tiskitpy-0.4/tiskitpy/spectral_density/version.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    19847 2022-12-14 10:25:03.000000 tiskitpy-0.4/tiskitpy/time_spans.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.148755 tiskitpy-0.4/tiskitpy/utils/
--rw-r--r--   0 crawford   (501) admin       (80)       61 2022-05-05 11:42:52.000000 tiskitpy-0.4/tiskitpy/utils/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    11844 2022-10-11 14:36:20.000000 tiskitpy-0.4/tiskitpy/utils/seis_rotate.py
--rw-r--r--   0 crawford   (501) admin       (80)       20 2023-07-13 06:21:06.000000 tiskitpy-0.4/tiskitpy/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 07:14:13.130465 tiskitpy-0.4/tiskitpy.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     2837 2023-07-13 07:14:12.000000 tiskitpy-0.4/tiskitpy.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     2238 2023-07-13 07:14:13.000000 tiskitpy-0.4/tiskitpy.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2023-07-13 07:14:12.000000 tiskitpy-0.4/tiskitpy.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)       78 2023-07-13 07:14:12.000000 tiskitpy-0.4/tiskitpy.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       50 2023-07-13 07:14:12.000000 tiskitpy-0.4/tiskitpy.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        9 2023-07-13 07:14:12.000000 tiskitpy-0.4/tiskitpy.egg-info/top_level.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.201572 tiskitpy-0.4.post1/
+-rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskitpy-0.4.post1/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       83 2023-07-13 06:27:46.000000 tiskitpy-0.4.post1/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     2477 2023-07-13 09:39:30.201291 tiskitpy-0.4.post1/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1661 2023-07-13 07:39:52.000000 tiskitpy-0.4.post1/README.md
+-rw-r--r--   0 crawford   (501) admin       (80)       38 2023-07-13 09:39:30.201642 tiskitpy-0.4.post1/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     1404 2023-07-13 08:51:24.000000 tiskitpy-0.4.post1/setup.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.165737 tiskitpy-0.4.post1/tiskitpy/
+-rw-r--r--   0 crawford   (501) admin       (80)     1800 2023-07-13 06:17:33.000000 tiskitpy-0.4.post1/tiskitpy/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-10-11 14:36:20.000000 tiskitpy-0.4.post1/tiskitpy/clean_rotator.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.169881 tiskitpy-0.4.post1/tiskitpy/data_cleaner/
+-rw-r--r--   0 crawford   (501) admin       (80)      212 2023-07-13 06:11:49.000000 tiskitpy-0.4.post1/tiskitpy/data_cleaner/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4196 2023-07-13 06:12:41.000000 tiskitpy-0.4.post1/tiskitpy/data_cleaner/cleaner_string.py
+-rw-r--r--   0 crawford   (501) admin       (80)    19078 2023-07-13 09:29:05.000000 tiskitpy-0.4.post1/tiskitpy/data_cleaner/data_cleaner_tf.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6169 2023-07-13 06:16:45.000000 tiskitpy-0.4.post1/tiskitpy/data_cleaner/dcrfs.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.174511 tiskitpy-0.4.post1/tiskitpy/decimate/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskitpy-0.4.post1/tiskitpy/decimate/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      184 2021-06-11 13:44:08.000000 tiskitpy-0.4.post1/tiskitpy/decimate/ToDo.md
+-rw-r--r--   0 crawford   (501) admin       (80)     1678 2021-06-24 09:28:18.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.184546 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/
+-rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1871 2023-07-11 20:46:27.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4980 2022-12-16 15:51:31.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13928 2022-12-14 10:39:43.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13946 2023-07-13 06:38:30.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     7514 2023-07-11 20:46:27.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     5760 2023-07-12 22:13:55.000000 tiskitpy-0.4.post1/tiskitpy/decimate/decimate_SDS.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    18945 2023-07-13 05:48:23.000000 tiskitpy-0.4.post1/tiskitpy/decimate/decimator.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     7672 2022-07-12 10:18:50.000000 tiskitpy-0.4.post1/tiskitpy/decimate/fir_filter.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.188615 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/
+-rw-r--r--   0 crawford   (501) admin       (80)      845 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec2
+-rw-r--r--   0 crawford   (501) admin       (80)     1218 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec3
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec4
+-rw-r--r--   0 crawford   (501) admin       (80)     1866 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec5
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec6
+-rw-r--r--   0 crawford   (501) admin       (80)     1898 2012-02-01 20:07:02.000000 tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec7
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2021-06-07 17:29:05.000000 tiskitpy-0.4.post1/tiskitpy/decimate/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.189623 tiskitpy-0.4.post1/tiskitpy/fir_corr/
+-rw-r--r--   0 crawford   (501) admin       (80)       39 2022-07-06 10:50:29.000000 tiskitpy-0.4.post1/tiskitpy/fir_corr/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    12282 2022-07-12 10:17:27.000000 tiskitpy-0.4.post1/tiskitpy/fir_corr/fir2caus.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2231 2022-07-23 07:09:08.000000 tiskitpy-0.4.post1/tiskitpy/read_mseed.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.191240 tiskitpy-0.4.post1/tiskitpy/response_functions/
+-rw-r--r--   0 crawford   (501) admin       (80)      133 2023-07-13 06:37:56.000000 tiskitpy-0.4.post1/tiskitpy/response_functions/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    26700 2023-07-13 09:33:40.000000 tiskitpy-0.4.post1/tiskitpy/response_functions/response_functions.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.196288 tiskitpy-0.4.post1/tiskitpy/rptransient/
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2022-05-04 22:13:23.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    23821 2022-10-11 14:36:20.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/dirac_comb.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    10734 2022-07-12 10:07:11.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/periodic_transient.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3099 2022-01-31 13:45:08.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/transients.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3201 2022-07-23 07:22:23.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       21 2021-12-09 22:15:36.000000 tiskitpy-0.4.post1/tiskitpy/rptransient/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.200003 tiskitpy-0.4.post1/tiskitpy/spectral_density/
+-rw-r--r--   0 crawford   (501) admin       (80)     2781 2022-05-04 22:20:44.000000 tiskitpy-0.4.post1/tiskitpy/spectral_density/Peterson_noise_model.py
+-rw-r--r--   0 crawford   (501) admin       (80)      125 2022-05-04 22:25:27.000000 tiskitpy-0.4.post1/tiskitpy/spectral_density/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    56485 2023-07-13 09:35:54.000000 tiskitpy-0.4.post1/tiskitpy/spectral_density/spectral_density.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4116 2022-03-28 12:36:00.000000 tiskitpy-0.4.post1/tiskitpy/spectral_density/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2022-01-06 11:06:02.000000 tiskitpy-0.4.post1/tiskitpy/spectral_density/version.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    19851 2023-07-13 09:21:16.000000 tiskitpy-0.4.post1/tiskitpy/time_spans.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.200970 tiskitpy-0.4.post1/tiskitpy/utils/
+-rw-r--r--   0 crawford   (501) admin       (80)       61 2022-05-05 11:42:52.000000 tiskitpy-0.4.post1/tiskitpy/utils/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11844 2022-10-11 14:36:20.000000 tiskitpy-0.4.post1/tiskitpy/utils/seis_rotate.py
+-rw-r--r--   0 crawford   (501) admin       (80)       26 2023-07-13 07:16:40.000000 tiskitpy-0.4.post1/tiskitpy/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-13 09:39:30.168233 tiskitpy-0.4.post1/tiskitpy.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     2477 2023-07-13 09:39:29.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     2238 2023-07-13 09:39:30.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-07-13 09:39:29.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       78 2023-07-13 09:39:29.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       50 2023-07-13 09:39:29.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        9 2023-07-13 09:39:29.000000 tiskitpy-0.4.post1/tiskitpy.egg-info/top_level.txt
```

### Comparing `tiskitpy-0.4/LICENSE.txt` & `tiskitpy-0.4.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/PKG-INFO` & `tiskitpy-0.4.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tiskitpy
-Version: 0.4
+Version: 0.4.post1
 Summary: TIme Series toolKIT
-Home-page: https://github.com/WayneCrawford/tiskit
+Home-page: https://github.com/WayneCrawford/tiskitpy
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -24,26 +24,26 @@
 
 Routines for time series data processing
 
 Uses the obspy seismological Trace, Stream (data) and Inventory (metadata)
 classes, but should work for non-seismology datasets as well
 
 
-[Documentation](https://tiskit.readthedocs.io/en/latest/index.html)
+[Documentation](https://tiskitpy.readthedocs.io/en/latest/index.html)
 
 
 ## Classes
 
 - `CleanRotator`: rotate data to minimize noise on vertical channel
 - `DataCleaner`: Transfer_Function-based data cleaning
 - `Decimator`: Decimate time series and update metadata with the decimator's
   response
 - `SpectralDensity`: Calculate and manipulate spectral density functions.
 - `TimeSpans`: Specify time spans to be removed, kept, zeroed, etc.
-- `TransferFunctions`: Transfer functions for a given input channel.
+- `ResponseFunctions`: Frequency response functions for a given input channel.
             
                
 ## Functions
 
 - `FIR_corr`: transform zero-phase data to minimum phase (only works for
               LCHEAPO loggers, need to update to calculate/work for any
               zero-phase filter)
@@ -51,20 +51,14 @@
                for obspy's read() function
 - `rptransient`: calculate and remove periodic transient (VERY manual!).  
  	Based on Matlab code by E Wielandt, used in Deen et al., 2017
 
 - `PetersonNoiseModel`: return the Peterson High and Low Noise Models
 
 
-## `seismo_tools` submodule: seismology-specific functions
-
-- `plot_response`: plot instrument response (command line?)
-- `plot_sensitivity`: plot instrument sensitivity (command line?)
-
-
 ## Installation
 
 First, install `obspy` using the instructions on their webpage.
 Then, in the pip/conda environment that contains obspy...
 
 ### From this repository
 
@@ -74,12 +68,8 @@
 
 You can also install in editable mode (for developers), with:
 
 `pip install -e .`
 
 ### Using `pip`
 
-Type `pip install tiskit-py`
-
-Note that I had to call this module `tiskit-py` on PyPI, rather than `tiskit`,
-so you may have to change the `import` calls in your code from `import tiskit`
-to `import tiskit-py as tiskit`
+Type `pip install tiskitpy`
```

### Comparing `tiskitpy-0.4/README.md` & `tiskitpy-0.4.post1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 Routines for time series data processing
 
 Uses the obspy seismological Trace, Stream (data) and Inventory (metadata)
 classes, but should work for non-seismology datasets as well
 
 
-[Documentation](https://tiskit.readthedocs.io/en/latest/index.html)
+[Documentation](https://tiskitpy.readthedocs.io/en/latest/index.html)
 
 
 ## Classes
 
 - `CleanRotator`: rotate data to minimize noise on vertical channel
 - `DataCleaner`: Transfer_Function-based data cleaning
 - `Decimator`: Decimate time series and update metadata with the decimator's
   response
 - `SpectralDensity`: Calculate and manipulate spectral density functions.
 - `TimeSpans`: Specify time spans to be removed, kept, zeroed, etc.
-- `TransferFunctions`: Transfer functions for a given input channel.
+- `ResponseFunctions`: Frequency response functions for a given input channel.
             
                
 ## Functions
 
 - `FIR_corr`: transform zero-phase data to minimum phase (only works for
               LCHEAPO loggers, need to update to calculate/work for any
               zero-phase filter)
@@ -29,20 +29,14 @@
                for obspy's read() function
 - `rptransient`: calculate and remove periodic transient (VERY manual!).  
  	Based on Matlab code by E Wielandt, used in Deen et al., 2017
 
 - `PetersonNoiseModel`: return the Peterson High and Low Noise Models
 
 
-## `seismo_tools` submodule: seismology-specific functions
-
-- `plot_response`: plot instrument response (command line?)
-- `plot_sensitivity`: plot instrument sensitivity (command line?)
-
-
 ## Installation
 
 First, install `obspy` using the instructions on their webpage.
 Then, in the pip/conda environment that contains obspy...
 
 ### From this repository
 
@@ -52,12 +46,8 @@
 
 You can also install in editable mode (for developers), with:
 
 `pip install -e .`
 
 ### Using `pip`
 
-Type `pip install tiskit-py`
-
-Note that I had to call this module `tiskit-py` on PyPI, rather than `tiskit`,
-so you may have to change the `import` calls in your code from `import tiskit`
-to `import tiskit-py as tiskit`
+Type `pip install tiskitpy`
```

### Comparing `tiskitpy-0.4/setup.py` & `tiskitpy-0.4.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     name="tiskitpy",
     version=version['__version__'],
     author="Wayne Crawford",
     author_email="crawford@ipgp.fr",
     description="TIme Series toolKIT",
     long_description=long_description,
     long_description_content_type="text/markdown; charset=UTF-8",
-    url="https://github.com/WayneCrawford/tiskit",
+    url="https://github.com/WayneCrawford/tiskitpy",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=['obspy>=1.3.0','PyYAML', 'numpy', 'scipy', 'matplotlib',
                       'xarray'],
     entry_points={
          'console_scripts': [
             'tiskitpy_decimate_SDS=tiskitpy.decimate.decimate_SDS:main'
```

### Comparing `tiskitpy-0.4/tiskitpy/__init__.py` & `tiskitpy-0.4.post1/tiskitpy/__init__.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/clean_rotator.py` & `tiskitpy-0.4.post1/tiskitpy/clean_rotator.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/data_cleaner/cleaner_string.py` & `tiskitpy-0.4.post1/tiskitpy/data_cleaner/cleaner_string.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/data_cleaner/data_cleaner_tf.py` & `tiskitpy-0.4.post1/tiskitpy/data_cleaner/data_cleaner_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Clean data using frequency response functions between channels
 
 Test using spectra (ATACR-style) and time-series (TisKit style):  is there a
 difference?  If not, will be a lot faster to remove noise after calculating
 spectra!
 """
+
 import fnmatch
 from copy import deepcopy
 import logging
 
 import numpy as np
 from scipy import signal
 from obspy.core.stream import Stream
@@ -145,20 +146,20 @@
         return sdf
 
     def clean_stream_to_sdf(self, stream, fast_calc=False, **kwargs):
         """
         Calculate corrected spectral density functions from an input stream
 
         Applys the DataCleaner values to each FFT
+
         Args:
             stream (:class:`obspy.core.stream.Stream`): data to apply to
             fast_calc (bool): Calculate corrected spectra directly from
                 previous spectra.
-            **kwargs (dict): keyword arguments for
-                SpectralDensity.from_stream()
+            kwargs (dict): keyword arguments for `SpectralDensity.from_stream()`
         Return:
             sdf (:class:`.SpectralDensity`): corrected spectral density
                 functions
         """
         assert isinstance(stream, Stream)
         if fast_calc:
             sdf = SpectralDensity.from_stream(stream, **kwargs)
```

### Comparing `tiskitpy-0.4/tiskitpy/data_cleaner/dcrfs.py` & `tiskitpy-0.4.post1/tiskitpy/data_cleaner/dcrfs.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/.DS_Store` & `tiskitpy-0.4.post1/tiskitpy/decimate/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__init__.py` & `tiskitpy-0.4.post1/tiskitpy/decimate/__init__.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/FIR_filter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/PSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/coherence.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimate.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimate_SDS.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/decimator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/fir_filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/transfer_function.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc` & `tiskitpy-0.4.post1/tiskitpy/decimate/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/decimate_SDS.py` & `tiskitpy-0.4.post1/tiskitpy/decimate/decimate_SDS.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/decimator.py` & `tiskitpy-0.4.post1/tiskitpy/decimate/decimator.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/fir_filter.py` & `tiskitpy-0.4.post1/tiskitpy/decimate/fir_filter.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec2` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec2`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec3` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec3`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec4` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec4`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec5` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec5`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec6` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec6`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/decimate/sac_fir/dec7` & `tiskitpy-0.4.post1/tiskitpy/decimate/sac_fir/dec7`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/fir_corr/fir2caus.py` & `tiskitpy-0.4.post1/tiskitpy/fir_corr/fir2caus.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/read_mseed.py` & `tiskitpy-0.4.post1/tiskitpy/read_mseed.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/response_functions/response_functions.py` & `tiskitpy-0.4.post1/tiskitpy/response_functions/response_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 
 class ResponseFunctions(object):
     """
     Class of Frequency Response Functions for a given input channel.
 
     From Bendat & Piersol, chapter 6.  The frequency response function is
     the relation between coherent parts of the signal: if the measured
-    input x(t) = u(t) + m(t) and the measured output y(t) = v(t) + n(t),
-    where u(t) and v(t) are coherent and m(t) and n(t) are not, then the
-    frequency response function H(f) is such that v(t) = H(f)*u(t).  As
-    to spectra, G_vv(f) = abs(H(f))^2 * G_uu(f)
+    input :math:`x(t) = u(t) + m(t)` and the measured output
+    :math:`y(t) = v(t) + n(t)`, where :math:`u(t)` and :math:`v(t)` are
+    coherent and :math:`m(t)` and :math:`n(t)` are not, then the
+    frequency response function :math:`H(f)` is such that
+    :math:`v(t) = H(f)*u(t)`.
+    As to spectra, :math:`G_vv(f) = abs(H(f))^2 * G_uu(f)`
 
     Args:
         sdm (:class:`.SpectralDensity`): Spectral density matrix objet
-        in_chan (str): input channel.  Can use Unix wildcards (*, ?) but
+        in_chan (str): input channel.  Can use Unix wildcards ('*', '?') but
             will return error if more than one string matches
         out_chans (list of str): output channels  (None => all but
             in_chan))
         noise_chan (str): 'input', 'output', 'equal', 'unknown'
         n_to_reject (int): number of neighboring frequencies for which the
             coherence must be above the 95% significance level in order
             to calculate frequency response function (other values are set to 0,
```

### Comparing `tiskitpy-0.4/tiskitpy/rptransient/dirac_comb.py` & `tiskitpy-0.4.post1/tiskitpy/rptransient/dirac_comb.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/rptransient/periodic_transient.py` & `tiskitpy-0.4.post1/tiskitpy/rptransient/periodic_transient.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/rptransient/transients.py` & `tiskitpy-0.4.post1/tiskitpy/rptransient/transients.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/rptransient/utils.py` & `tiskitpy-0.4.post1/tiskitpy/rptransient/utils.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/spectral_density/Peterson_noise_model.py` & `tiskitpy-0.4.post1/tiskitpy/spectral_density/Peterson_noise_model.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/spectral_density/spectral_density.py` & `tiskitpy-0.4.post1/tiskitpy/spectral_density/spectral_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,19 +660,19 @@
         """
         Plot autospectra
 
         Args:
             x (list of str): limit to the listed channels
             overlay (bool): put all spect on one axis
             plot_peterson(bool): plot Peterson Noise model if any channel has
-                units of (m/s^2)^2/Hz
+                units of :math:`(m/s^2)^2/Hz`
             show (bool): show on desktop
             outfile (str): save figure to this filename
             title (str): custom plot title
-            **fig_kw (**dict): all additional keyword arguments (such as `figsize`
+            fig_kw (dict): all additional keyword arguments (such as `figsize`
                 and `dpi`) are passed to the `pyplot.figure` call
         Returns:
             (:class:`numpy.ndarray`): array of axis pairs (amplitude, phase)
         """
         x = self._get_validate_channel_names(x)
         if not overlay:
             rows, cols = _squarish_grid(len(x))
@@ -734,17 +734,17 @@
         """
         Plot cross (and auto) spectra
 
         Args:
             x (list of str): limit to the listed channels
             show (bool): show on desktop
             plot_peterson(bool): plot Peterson Noise model if any channel has
-                units of (m/s^2)^2/Hz
+                units of :math:`(m/s^2)^2/Hz`
             show_coherence (bool): show coherence as well
-            fig_kw (**dict): all additional keyword arguments (such as `figsize`
+            fig_kw (dict): all additional keyword arguments (such as `figsize`
                 and `dpi`) are passed to the `pyplot.figure` call
         Returns:
             :class:`numpy.ndarray`: array of axis pairs (amplitude, phase)
         """
         x = self._get_validate_channel_names(x)
         n_subkeys = len(x)
         rows, cols = n_subkeys, n_subkeys
@@ -823,15 +823,15 @@
             label (str): 'units': print units without channel name in legend
             ax_a (Axis): use an existing axis for the amplitude plot
             ax_p (Axis): use this existing axis for the phase plot
             title (str): title to put on this subplot
             show_coherence (bool): draw coherence on the same plot
             show_phase (bool): show phase as well as amplitude
             plot_peterson(bool): plot Peterson Noise model if channel has
-                units of (m/s^2)^2/Hz
+                units of :math:`(m/s^2)^2/Hz`
             outfile (str): save figure to this filename
 
         Returns:
             (tuple): tuple containing
                 - :class:`matplotlib.axes.axis`: amplitude plot axis
                 - :class:`matplotlib.axes.axis`: phase plot axis
         """
@@ -971,15 +971,15 @@
             overlay (bool): put all coherences on one plot
             show (bool): show on desktop
             outfile (str): save to the named file
             labels (str): labels to put on x and y axes ('full', 'chan' or
                 'loc-chan')
             sort_by (str): how to sort x and y axes ('full', 'chan' or
                 'loc-chan')
-            fig_kw (**dict): all additional keyword arguments (such as `figsize`
+            fig_kw (dict): all additional keyword arguments (such as `figsize`
                 and `dpi`) are passed to the `pyplot.figure` call
 
         Returns:
             (:class:`numpy.ndarray`): array of axis pairs (amplitude, phase)
         """
         strfun = self._seedid_strfun(sort_by)
         x = sorted(self._get_validate_channel_names(x), key=strfun)
@@ -1074,15 +1074,15 @@
             ylabel (str): label to put on y axis (if show_label).  If not
                 speficied, will use 'dB ref UNITS/Hz'
             label (str): text to put in legend
             ax_a (Axis): use an existing axis for the amplitude plot
             ax_p (Axis): use this existing axis for the phase plot
             title (str): title to put on this subplot
             show_phase (bool): show phase as well as amplitude
-            kwargs (**dict): values to pass on to plotting routines
+            kwargs (dict): values to pass on to plotting routines
 
         Returns:
             (tuple): tuple containing:
                 - (:class:`matplotlib.axes.axis`): amplitude plot axis
                 - (:class:`matplotlib.axes.axis`): phase plot axis
         """
         in_chan = self.channel_name(in_chan,'in_chan')
```

### Comparing `tiskitpy-0.4/tiskitpy/spectral_density/utils.py` & `tiskitpy-0.4.post1/tiskitpy/spectral_density/utils.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy/time_spans.py` & `tiskitpy-0.4.post1/tiskitpy/time_spans.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 If a str, must by ISO8601 compatible
             minmag (float): EQ Magnitude above which to cut out times
             days_per_magnitude (float): days to cut per magnitude above
                 min_magnitude
             eq_file (str): the eq filename (otherwise, generates it)
             save_eq_file (bool): save the catalog file for future use
         Returns:
-            eq_spans (TimeSpans_): time spans covering EQ signal
+            eq_spans (:class:`TimeSpans`): time spans covering EQ signal
         """
         if isinstance(starttime, str):
             try:
                 starttime = UTCDateTime(starttime)
             except Exception:
                 raise ValueError(f"UTCDateTime() could not read {starttime=}")
         if isinstance(endtime, str):
@@ -460,15 +460,15 @@
         Args:
             stream (:class:`obspy.core.trace.Stream` or
                 :class:`obspy.core.trace.Trace`): obspy stream/trace to plot
             color (str): highlight color
             alpha (float): highlight transparency alpha (1=opaque, 0 =
                 invisible)
             title (str): figure title
-            **kwargs (**dict): arguments to stream/trace plot program
+            kwargs (dict): arguments to stream/trace plot program
         Returns:
             (tuple):
                 fig (matplotlib Figure):
                 ax (list): list of axes
         """
         if alpha < 0:
             raise ValueError("alpha < 0")
```

### Comparing `tiskitpy-0.4/tiskitpy/utils/seis_rotate.py` & `tiskitpy-0.4.post1/tiskitpy/utils/seis_rotate.py`

 * *Files identical despite different names*

### Comparing `tiskitpy-0.4/tiskitpy.egg-info/PKG-INFO` & `tiskitpy-0.4.post1/tiskitpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tiskitpy
-Version: 0.4
+Version: 0.4.post1
 Summary: TIme Series toolKIT
-Home-page: https://github.com/WayneCrawford/tiskit
+Home-page: https://github.com/WayneCrawford/tiskitpy
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -24,26 +24,26 @@
 
 Routines for time series data processing
 
 Uses the obspy seismological Trace, Stream (data) and Inventory (metadata)
 classes, but should work for non-seismology datasets as well
 
 
-[Documentation](https://tiskit.readthedocs.io/en/latest/index.html)
+[Documentation](https://tiskitpy.readthedocs.io/en/latest/index.html)
 
 
 ## Classes
 
 - `CleanRotator`: rotate data to minimize noise on vertical channel
 - `DataCleaner`: Transfer_Function-based data cleaning
 - `Decimator`: Decimate time series and update metadata with the decimator's
   response
 - `SpectralDensity`: Calculate and manipulate spectral density functions.
 - `TimeSpans`: Specify time spans to be removed, kept, zeroed, etc.
-- `TransferFunctions`: Transfer functions for a given input channel.
+- `ResponseFunctions`: Frequency response functions for a given input channel.
             
                
 ## Functions
 
 - `FIR_corr`: transform zero-phase data to minimum phase (only works for
               LCHEAPO loggers, need to update to calculate/work for any
               zero-phase filter)
@@ -51,20 +51,14 @@
                for obspy's read() function
 - `rptransient`: calculate and remove periodic transient (VERY manual!).  
  	Based on Matlab code by E Wielandt, used in Deen et al., 2017
 
 - `PetersonNoiseModel`: return the Peterson High and Low Noise Models
 
 
-## `seismo_tools` submodule: seismology-specific functions
-
-- `plot_response`: plot instrument response (command line?)
-- `plot_sensitivity`: plot instrument sensitivity (command line?)
-
-
 ## Installation
 
 First, install `obspy` using the instructions on their webpage.
 Then, in the pip/conda environment that contains obspy...
 
 ### From this repository
 
@@ -74,12 +68,8 @@
 
 You can also install in editable mode (for developers), with:
 
 `pip install -e .`
 
 ### Using `pip`
 
-Type `pip install tiskit-py`
-
-Note that I had to call this module `tiskit-py` on PyPI, rather than `tiskit`,
-so you may have to change the `import` calls in your code from `import tiskit`
-to `import tiskit-py as tiskit`
+Type `pip install tiskitpy`
```

### Comparing `tiskitpy-0.4/tiskitpy.egg-info/SOURCES.txt` & `tiskitpy-0.4.post1/tiskitpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

