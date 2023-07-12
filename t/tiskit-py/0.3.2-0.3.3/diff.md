# Comparing `tmp/tiskit-py-0.3.2.tar.gz` & `tmp/tiskit-py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiskit-py-0.3.2.tar", last modified: Wed Dec 14 09:18:55 2022, max compression
+gzip compressed data, was "tiskit-py-0.3.3.tar", last modified: Wed Jul 12 22:08:34 2023, max compression
```

## Comparing `tiskit-py-0.3.2.tar` & `tiskit-py-0.3.3.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.155263 tiskit-py-0.3.2/
--rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskit-py-0.3.2/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)       81 2022-12-14 09:13:54.000000 tiskit-py-0.3.2/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     2839 2022-12-14 09:18:55.154855 tiskit-py-0.3.2/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     2027 2022-12-14 09:08:40.000000 tiskit-py-0.3.2/README.md
--rw-r--r--   0 crawford   (501) admin       (80)       38 2022-12-14 09:18:55.155419 tiskit-py-0.3.2/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     1398 2022-12-14 09:08:40.000000 tiskit-py-0.3.2/setup.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.110010 tiskit-py-0.3.2/tiskit/
--rw-r--r--   0 crawford   (501) admin       (80)     1790 2022-12-14 09:08:40.000000 tiskit-py-0.3.2/tiskit/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/clean_rotator.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.113139 tiskit-py-0.3.2/tiskit/data_cleaner/
--rw-r--r--   0 crawford   (501) admin       (80)      151 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/data_cleaner/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     4176 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/data_cleaner/cleaner_string.py
--rw-r--r--   0 crawford   (501) admin       (80)    18935 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/data_cleaner/data_cleaner_tf.py
--rw-r--r--   0 crawford   (501) admin       (80)     6139 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/data_cleaner/dctfs.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.120626 tiskit-py-0.3.2/tiskit/decimate/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskit-py-0.3.2/tiskit/decimate/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      184 2021-06-11 13:44:08.000000 tiskit-py-0.3.2/tiskit/decimate/ToDo.md
--rw-r--r--   0 crawford   (501) admin       (80)     1678 2021-06-24 09:28:18.000000 tiskit-py-0.3.2/tiskit/decimate/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.130190 tiskit-py-0.3.2/tiskit/decimate/__pycache__/
--rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/FIR_filter.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/PSD.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/coherence.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimate.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     5000 2022-07-27 13:51:48.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimate_SDS.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)    13726 2022-10-11 15:26:31.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimator.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/transfer_function.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskit-py-0.3.2/tiskit/decimate/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 crawford   (501) admin       (80)     5833 2022-07-27 14:05:27.000000 tiskit-py-0.3.2/tiskit/decimate/decimate_SDS.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    18622 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/decimate/decimator.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     7672 2022-07-12 10:18:50.000000 tiskit-py-0.3.2/tiskit/decimate/fir_filter.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.133561 tiskit-py-0.3.2/tiskit/decimate/sac_fir/
--rw-r--r--   0 crawford   (501) admin       (80)      845 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec2
--rw-r--r--   0 crawford   (501) admin       (80)     1218 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec3
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec4
--rw-r--r--   0 crawford   (501) admin       (80)     1866 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec5
--rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec6
--rw-r--r--   0 crawford   (501) admin       (80)     1898 2012-02-01 20:07:02.000000 tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec7
--rw-r--r--   0 crawford   (501) admin       (80)       18 2021-06-07 17:29:05.000000 tiskit-py-0.3.2/tiskit/decimate/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.134884 tiskit-py-0.3.2/tiskit/fir_corr/
--rw-r--r--   0 crawford   (501) admin       (80)       39 2022-07-06 10:50:29.000000 tiskit-py-0.3.2/tiskit/fir_corr/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    12282 2022-07-12 10:17:27.000000 tiskit-py-0.3.2/tiskit/fir_corr/fir2caus.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2231 2022-07-23 07:09:08.000000 tiskit-py-0.3.2/tiskit/read_mseed.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.142190 tiskit-py-0.3.2/tiskit/rptransient/
--rw-r--r--   0 crawford   (501) admin       (80)       85 2022-05-04 22:13:23.000000 tiskit-py-0.3.2/tiskit/rptransient/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    23821 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/rptransient/dirac_comb.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    10734 2022-07-12 10:07:11.000000 tiskit-py-0.3.2/tiskit/rptransient/periodic_transient.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3099 2022-01-31 13:45:08.000000 tiskit-py-0.3.2/tiskit/rptransient/transients.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3201 2022-07-23 07:22:23.000000 tiskit-py-0.3.2/tiskit/rptransient/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       21 2021-12-09 22:15:36.000000 tiskit-py-0.3.2/tiskit/rptransient/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.149008 tiskit-py-0.3.2/tiskit/spectral_density/
--rw-r--r--   0 crawford   (501) admin       (80)     2781 2022-05-04 22:20:44.000000 tiskit-py-0.3.2/tiskit/spectral_density/Peterson_noise_model.py
--rw-r--r--   0 crawford   (501) admin       (80)      125 2022-05-04 22:25:27.000000 tiskit-py-0.3.2/tiskit/spectral_density/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    55979 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/spectral_density/spectral_density.py
--rw-r--r--   0 crawford   (501) admin       (80)     4116 2022-03-28 12:36:00.000000 tiskit-py-0.3.2/tiskit/spectral_density/utils.py
--rw-r--r--   0 crawford   (501) admin       (80)       18 2022-01-06 11:06:02.000000 tiskit-py-0.3.2/tiskit/spectral_density/version.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    19847 2022-12-14 09:08:40.000000 tiskit-py-0.3.2/tiskit/time_spans.py
--rw-r--r--   0 crawford   (501) admin       (80)    23502 2022-12-14 09:08:40.000000 tiskit-py-0.3.2/tiskit/transfer_functions.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.151231 tiskit-py-0.3.2/tiskit/utils/
--rw-r--r--   0 crawford   (501) admin       (80)       61 2022-05-05 11:42:52.000000 tiskit-py-0.3.2/tiskit/utils/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    11844 2022-10-11 14:36:20.000000 tiskit-py-0.3.2/tiskit/utils/seis_rotate.py
--rw-r--r--   0 crawford   (501) admin       (80)       22 2022-12-14 09:14:18.000000 tiskit-py-0.3.2/tiskit/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2022-12-14 09:18:55.154318 tiskit-py-0.3.2/tiskit_py.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     2839 2022-12-14 09:18:54.000000 tiskit-py-0.3.2/tiskit_py.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1924 2022-12-14 09:18:55.000000 tiskit-py-0.3.2/tiskit_py.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2022-12-14 09:18:54.000000 tiskit-py-0.3.2/tiskit_py.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)       74 2022-12-14 09:18:54.000000 tiskit-py-0.3.2/tiskit_py.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       50 2022-12-14 09:18:54.000000 tiskit-py-0.3.2/tiskit_py.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        7 2022-12-14 09:18:54.000000 tiskit-py-0.3.2/tiskit_py.egg-info/top_level.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.476759 tiskit-py-0.3.3/
+-rw-r--r--   0 crawford   (501) admin       (80)    35150 2019-02-11 14:51:26.000000 tiskit-py-0.3.3/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       81 2022-12-14 10:25:03.000000 tiskit-py-0.3.3/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     2838 2023-07-12 22:08:34.475958 tiskit-py-0.3.3/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     2027 2022-12-14 10:25:03.000000 tiskit-py-0.3.3/README.md
+-rw-r--r--   0 crawford   (501) admin       (80)       38 2023-07-12 22:08:34.476949 tiskit-py-0.3.3/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     1397 2023-07-11 20:32:01.000000 tiskit-py-0.3.3/setup.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.427735 tiskit-py-0.3.3/tiskit/
+-rw-r--r--   0 crawford   (501) admin       (80)     1790 2022-12-14 10:25:03.000000 tiskit-py-0.3.3/tiskit/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7091 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/clean_rotator.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.430469 tiskit-py-0.3.3/tiskit/data_cleaner/
+-rw-r--r--   0 crawford   (501) admin       (80)      151 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/data_cleaner/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4176 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/data_cleaner/cleaner_string.py
+-rw-r--r--   0 crawford   (501) admin       (80)    18935 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/data_cleaner/data_cleaner_tf.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6139 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/data_cleaner/dctfs.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.437914 tiskit-py-0.3.3/tiskit/decimate/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-07-06 10:22:56.000000 tiskit-py-0.3.3/tiskit/decimate/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      184 2021-06-11 13:44:08.000000 tiskit-py-0.3.3/tiskit/decimate/ToDo.md
+-rw-r--r--   0 crawford   (501) admin       (80)     1678 2021-06-24 09:28:18.000000 tiskit-py-0.3.3/tiskit/decimate/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.450693 tiskit-py-0.3.3/tiskit/decimate/__pycache__/
+-rw-r--r--   0 crawford   (501) admin       (80)     7539 2022-07-12 10:22:39.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/FIR_filter.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     6045 2021-05-10 08:50:39.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/PSD.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3012 2021-05-10 08:47:59.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1877 2021-06-24 12:32:02.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     1871 2023-07-11 20:46:27.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4165 2021-05-10 08:50:39.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/coherence.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     9716 2021-06-20 21:41:01.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimate.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4980 2022-12-16 15:51:31.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimate_SDS.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13928 2022-12-14 10:39:43.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimator.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)    13909 2023-07-11 20:46:27.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimator.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     7514 2023-07-11 20:46:27.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/fir_filter.cpython-39.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     4430 2021-05-10 08:49:04.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/transfer_function.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     3397 2021-05-10 08:55:09.000000 tiskit-py-0.3.3/tiskit/decimate/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 crawford   (501) admin       (80)     5760 2022-12-16 16:23:47.000000 tiskit-py-0.3.3/tiskit/decimate/decimate_SDS.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    18912 2022-12-14 10:39:35.000000 tiskit-py-0.3.3/tiskit/decimate/decimator.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     7672 2022-07-12 10:18:50.000000 tiskit-py-0.3.3/tiskit/decimate/fir_filter.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.454095 tiskit-py-0.3.3/tiskit/decimate/sac_fir/
+-rw-r--r--   0 crawford   (501) admin       (80)      845 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec2
+-rw-r--r--   0 crawford   (501) admin       (80)     1218 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec3
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec4
+-rw-r--r--   0 crawford   (501) admin       (80)     1866 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec5
+-rw-r--r--   0 crawford   (501) admin       (80)     1542 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec6
+-rw-r--r--   0 crawford   (501) admin       (80)     1898 2012-02-01 20:07:02.000000 tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec7
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2021-06-07 17:29:05.000000 tiskit-py-0.3.3/tiskit/decimate/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.455351 tiskit-py-0.3.3/tiskit/fir_corr/
+-rw-r--r--   0 crawford   (501) admin       (80)       39 2022-07-06 10:50:29.000000 tiskit-py-0.3.3/tiskit/fir_corr/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    12282 2022-07-12 10:17:27.000000 tiskit-py-0.3.3/tiskit/fir_corr/fir2caus.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2231 2022-07-23 07:09:08.000000 tiskit-py-0.3.3/tiskit/read_mseed.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.462390 tiskit-py-0.3.3/tiskit/rptransient/
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2022-05-04 22:13:23.000000 tiskit-py-0.3.3/tiskit/rptransient/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    23821 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/rptransient/dirac_comb.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    10734 2022-07-12 10:07:11.000000 tiskit-py-0.3.3/tiskit/rptransient/periodic_transient.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3099 2022-01-31 13:45:08.000000 tiskit-py-0.3.3/tiskit/rptransient/transients.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     3201 2022-07-23 07:22:23.000000 tiskit-py-0.3.3/tiskit/rptransient/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       21 2021-12-09 22:15:36.000000 tiskit-py-0.3.3/tiskit/rptransient/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.467994 tiskit-py-0.3.3/tiskit/spectral_density/
+-rw-r--r--   0 crawford   (501) admin       (80)     2781 2022-05-04 22:20:44.000000 tiskit-py-0.3.3/tiskit/spectral_density/Peterson_noise_model.py
+-rw-r--r--   0 crawford   (501) admin       (80)      125 2022-05-04 22:25:27.000000 tiskit-py-0.3.3/tiskit/spectral_density/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    56063 2023-07-12 22:07:23.000000 tiskit-py-0.3.3/tiskit/spectral_density/spectral_density.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4116 2022-03-28 12:36:00.000000 tiskit-py-0.3.3/tiskit/spectral_density/utils.py
+-rw-r--r--   0 crawford   (501) admin       (80)       18 2022-01-06 11:06:02.000000 tiskit-py-0.3.3/tiskit/spectral_density/version.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    19847 2022-12-14 10:25:03.000000 tiskit-py-0.3.3/tiskit/time_spans.py
+-rw-r--r--   0 crawford   (501) admin       (80)    26151 2023-07-12 21:38:15.000000 tiskit-py-0.3.3/tiskit/transfer_functions.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.471413 tiskit-py-0.3.3/tiskit/utils/
+-rw-r--r--   0 crawford   (501) admin       (80)       61 2022-05-05 11:42:52.000000 tiskit-py-0.3.3/tiskit/utils/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11844 2022-10-11 14:36:20.000000 tiskit-py-0.3.3/tiskit/utils/seis_rotate.py
+-rw-r--r--   0 crawford   (501) admin       (80)       22 2022-12-14 10:42:26.000000 tiskit-py-0.3.3/tiskit/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-07-12 22:08:34.475010 tiskit-py-0.3.3/tiskit_py.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     2838 2023-07-12 22:08:33.000000 tiskit-py-0.3.3/tiskit_py.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     2083 2023-07-12 22:08:34.000000 tiskit-py-0.3.3/tiskit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-07-12 22:08:33.000000 tiskit-py-0.3.3/tiskit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       74 2023-07-12 22:08:34.000000 tiskit-py-0.3.3/tiskit_py.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       50 2023-07-12 22:08:34.000000 tiskit-py-0.3.3/tiskit_py.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        7 2023-07-12 22:08:34.000000 tiskit-py-0.3.3/tiskit_py.egg-info/top_level.txt
```

### Comparing `tiskit-py-0.3.2/LICENSE.txt` & `tiskit-py-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/PKG-INFO` & `tiskit-py-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tiskit-py
-Version: 0.3.2
-Summary: TIme Series  toolKIT
+Version: 0.3.3
+Summary: TIme Series toolKIT
 Home-page: https://github.com/WayneCrawford/tiskit
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tiskit-py-0.3.2/README.md` & `tiskit-py-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/setup.py` & `tiskit-py-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     exec(fp.read(),version)
 
 setuptools.setup(
     name="tiskit-py",
     version=version['__version__'],
     author="Wayne Crawford",
     author_email="crawford@ipgp.fr",
-    description="TIme Series  toolKIT",
+    description="TIme Series toolKIT",
     long_description=long_description,
     long_description_content_type="text/markdown; charset=UTF-8",
     url="https://github.com/WayneCrawford/tiskit",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=['obspy>=1.3.0','PyYAML', 'numpy', 'scipy', 'matplotlib',
                       'xarray'],
```

### Comparing `tiskit-py-0.3.2/tiskit/__init__.py` & `tiskit-py-0.3.3/tiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/clean_rotator.py` & `tiskit-py-0.3.3/tiskit/clean_rotator.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/data_cleaner/cleaner_string.py` & `tiskit-py-0.3.3/tiskit/data_cleaner/cleaner_string.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/data_cleaner/data_cleaner_tf.py` & `tiskit-py-0.3.3/tiskit/data_cleaner/data_cleaner_tf.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/data_cleaner/dctfs.py` & `tiskit-py-0.3.3/tiskit/data_cleaner/dctfs.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/.DS_Store` & `tiskit-py-0.3.3/tiskit/decimate/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__init__.py` & `tiskit-py-0.3.3/tiskit/decimate/__init__.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/FIR_filter.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/FIR_filter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/PSD.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/PSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/__init__.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/coherence.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/coherence.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimate.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimate.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimate_SDS.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimate_SDS.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jul 27 13:51:44 2022 UTC, .py size: 5828 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 f042 e162 c416 0000  U........B.b....
+00000000: 550d 0d0a 0000 0000 0292 9c63 ab16 0000  U..........c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6401 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6401 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6407 6408 8400 5a0b 640d 6409 640a  ..d.d...Z.d.d.d.
@@ -14,300 +14,299 @@
 000000d0: 5320 7374 7275 6374 7572 650a 616e 6420  S structure.and 
 000000e0: 7265 7475 726e 2074 6865 206d 6f64 6966  return the modif
 000000f0: 6965 6420 696e 7665 6e74 6f72 790a e900  ied inventory...
 00000100: 0000 004e 2901 da04 5061 7468 2901 da04  ...N)...Path)...
 00000110: 7265 6164 2901 da0e 7265 6164 5f69 6e76  read)...read_inv
 00000120: 656e 746f 7279 2901 da09 4465 6369 6d61  entory)...Decima
 00000130: 746f 7263 0400 0000 0000 0000 0000 0000  torc............
-00000140: 1b00 0000 1200 0000 4300 0000 734a 0200  ........C...sJ..
+00000140: 1b00 0000 1200 0000 4300 0000 738e 0200  ........C...s...
 00000150: 0074 007c 0083 017d 0074 017c 0383 017d  .t.|...}.t.|...}
 00000160: 047c 027c 046a 021b 007d 0574 01a0 0364  .|.|.j...}.t...d
 00000170: 017c 02a1 027d 0674 01a0 0364 017c 05a1  .|...}.t...d.|..
 00000180: 027d 0774 04a0 0564 02a0 067c 057c 07a1  .}.t...d...|.|..
-00000190: 02a1 0101 007c 067c 076b 0272 5474 0764  .....|.|.k.rTt.d
-000001a0: 0383 0182 0164 0464 0584 007c 00a0 08a1  .....d.d...|....
-000001b0: 0044 0083 0144 0090 015d dc7d 0874 04a0  .D...D...].}.t..
-000001c0: 0564 06a1 0101 0064 0764 0584 007c 08a0  .d.....d.d...|..
-000001d0: 08a1 0044 0083 0144 0090 015d b87d 0974  ...D...D...].}.t
-000001e0: 04a0 0564 08a1 0101 0064 0964 0584 007c  ...d.....d.d...|
-000001f0: 09a0 08a1 0044 0083 0144 0090 015d 947d  .....D...D...].}
-00000200: 0a74 04a0 0564 0aa1 0101 0064 0b64 0584  .t...d.....d.d..
-00000210: 007c 0aa0 08a1 0044 0083 0144 0090 015d  .|.....D...D...]
-00000220: 707d 0b74 04a0 0564 0ca0 0674 097c 0a6a  p}.t...d...t.|.j
-00000230: 0a83 01a1 01a1 0101 007c 0b6a 0a7d 0c7c  .........|.j.}.|
-00000240: 0c64 0d19 007c 066b 0273 fc71 cc7c 0a7c  .d...|.k.s.q.|.|
-00000250: 077c 0c64 0e64 0f85 0219 0017 001b 007d  .|.d.d.........}
-00000260: 0d7c 0da0 0ba1 0001 0074 04a0 0564 10a0  .|.......t...d..
-00000270: 067c 0d6a 0aa1 01a1 0101 007c 0ba0 0c64  .|.j.......|...d
-00000280: 117c 0c9b 0064 129d 03a1 017d 0e74 04a0  .|...d.....}.t..
-00000290: 0564 13a1 0101 007c 0e44 005d e67d 0f74  .d.....|.D.].}.t
-000002a0: 0d74 097c 0f83 0164 1483 027d 107c 1064  .t.|...d...}.|.d
-000002b0: 0d19 006a 0e6a 0f7c 046a 0216 0064 0d6b  ...j.j.|.j...d.k
-000002c0: 0290 0172 9474 0764 157c 1064 0d19 006a  ...r.t.d.|.d...j
-000002d0: 0e6a 0f9b 0064 167c 046a 029b 0064 179d  .j...d.|.j...d..
-000002e0: 0583 0101 007c 1064 0d19 006a 0e6a 107c  .....|.d...j.j.|
-000002f0: 026b 0390 0172 ba74 04a0 1174 097c 0f83  .k...r.t...t.|..
-00000300: 019b 0064 189d 02a1 0101 0074 097c 0f6a  ...d.......t.|.j
-00000310: 0a83 01a0 1264 19a1 015c 077d 117d 127d  .....d...\.}.}.}
-00000320: 137d 147d 157d 167d 177c 04a0 137c 10a1  .}.}.}.}.|...|..
-00000330: 017d 187c 077c 1464 0e64 0f85 0219 0017  .}.|.|.d.d......
-00000340: 007d 197c 119b 0064 197c 129b 0064 197c  .}.|...d.|...d.|
-00000350: 139b 0064 197c 199b 0064 197c 159b 0064  ...d.|...d.|...d
-00000360: 197c 169b 0064 197c 179b 009d 0d7d 1a7c  .|...d.|.....}.|
-00000370: 18a0 147c 0d7c 1a1b 0064 14a1 0201 0090  ...|.|...d......
-00000380: 0171 4a7c 04a0 157c 017c 10a1 027d 0171  .qJ|...|.|...}.q
-00000390: cc71 aa71 8871 667c 0153 0029 1a61 3002  .q.q.qf|.S.).a0.
-000003a0: 0000 0a20 2020 2054 6865 206d 6169 6e20  ...    The main 
-000003b0: 6675 6e63 7469 6f6e 0a0a 2020 2020 5368  function..    Sh
-000003c0: 6f75 6c64 2065 6e73 7572 6520 636f 6e74  ould ensure cont
-000003d0: 696e 7569 7479 2061 6372 6f73 7320 6461  inuity across da
-000003e0: 7920 616e 6420 7965 6172 2062 6f75 6e64  y and year bound
-000003f0: 6172 6965 732e 0a20 2020 2043 7572 7265  aries..    Curre
-00000400: 6e74 6c79 206a 7573 7420 6368 6563 6b73  ntly just checks
-00000410: 2069 6620 7468 6520 7265 7175 6573 7465   if the requeste
-00000420: 6420 6465 6369 6d61 7469 6f6e 2069 7320  d decimation is 
-00000430: 616e 2069 6e74 6567 7261 6c20 6469 7669  an integral divi
-00000440: 736f 720a 2020 2020 6f66 2074 6865 2063  sor.    of the c
-00000450: 7572 7265 6e74 2064 6179 2773 2073 616d  urrent day's sam
-00000460: 706c 6573 2061 6e64 2072 6574 7572 6e73  ples and returns
-00000470: 2061 6e20 6572 726f 7220 6966 206e 6f74   an error if not
-00000480: 0a20 2020 204f 6e6c 7920 776f 726b 7320  .    Only works 
-00000490: 666f 7220 6272 6f61 642d 6261 6e64 2063  for broad-band c
-000004a0: 6861 6e6e 656c 730a 0a20 2020 2041 7267  hannels..    Arg
-000004b0: 733a 0a20 2020 2020 2020 2053 4453 5f72  s:.        SDS_r
-000004c0: 6f6f 7420 2873 7472 206f 7220 5061 7468  oot (str or Path
-000004d0: 293a 2053 4453 2072 6f6f 7420 6469 7265  ): SDS root dire
-000004e0: 6374 6f72 790a 2020 2020 2020 2020 696e  ctory.        in
-000004f0: 7620 283a 636c 6173 733a 606f 6273 7079  v (:class:`obspy
-00000500: 2e63 6f72 652e 696e 7665 6e74 6f72 792e  .core.inventory.
-00000510: 496e 7665 6e74 6f72 7960 293a 2073 7461  Inventory`): sta
-00000520: 7469 6f6e 2069 6e76 656e 746f 7279 0a20  tion inventory. 
-00000530: 2020 2020 2020 2069 6e70 7574 5f73 616d         input_sam
-00000540: 706c 655f 7261 7465 2028 666c 6f61 7429  ple_rate (float)
-00000550: 3a20 7361 6d70 6c65 2072 6174 6520 6f66  : sample rate of
-00000560: 2064 6174 6120 746f 2070 726f 6365 7373   data to process
-00000570: 0a20 2020 2020 2020 2064 6563 696d 5f6c  .        decim_l
-00000580: 6973 7420 286c 6973 7429 3a20 6c69 7374  ist (list): list
-00000590: 206f 6620 6465 6369 6d61 7469 6f6e 2066   of decimation f
-000005a0: 6163 746f 7273 2028 696e 7465 6765 7273  actors (integers
-000005b0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
-000005c0: 2020 2020 2032 2061 6e64 2037 290a 2020       2 and 7).  
-000005d0: 2020 da01 427a 3b6f 7574 7075 7420 7361    ..Bz;output sa
-000005e0: 6d70 6c69 6e67 2072 6174 6520 7769 6c6c  mpling rate will
-000005f0: 2062 6520 7b3a 677d 2073 7073 2c20 6261   be {:g} sps, ba
-00000600: 6e64 2063 6f64 6520 7769 6c6c 2062 6520  nd code will be 
-00000610: 7b7d 7a33 6964 656e 7469 6361 6c20 696e  {}z3identical in
-00000620: 7075 7420 2620 6f75 7470 7574 2062 616e  put & output ban
-00000630: 6420 636f 6465 733a 207b 696e 5f62 616e  d codes: {in_ban
-00000640: 645f 636f 6465 7d63 0100 0000 0000 0000  d_code}c........
-00000650: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00000660: 7318 0000 0067 007c 005d 107d 017c 01a0  s....g.|.].}.|..
-00000670: 00a1 0072 047c 0191 0271 0453 00a9 00a9  ...r.|...q.S....
-00000680: 01da 0669 735f 6469 72a9 02da 022e 30da  ...is_dir.....0.
-00000690: 0178 7207 0000 0072 0700 0000 fa48 2f55  .xr....r.....H/U
-000006a0: 7365 7273 2f63 7261 7766 6f72 642f 5f57  sers/crawford/_W
-000006b0: 6f72 6b2f 5072 6f67 7261 6d6d 696e 672f  ork/Programming/
-000006c0: 7469 736b 6974 2f74 6973 6b69 742f 6465  tiskit/tiskit/de
-000006d0: 6369 6d61 7465 2f64 6563 696d 6174 655f  cimate/decimate_
-000006e0: 5344 532e 7079 da0a 3c6c 6973 7463 6f6d  SDS.py..<listcom
-000006f0: 703e 2900 0000 7306 0000 0006 0002 0008  p>)...s.........
-00000700: 007a 2064 6563 696d 6174 655f 5344 532e  .z decimate_SDS.
-00000710: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000720: 6d70 3e7a 2457 6f72 6b69 6e67 206f 6e20  mp>z$Working on 
-00000730: 7965 6172 207b 7374 7228 7965 6172 5f64  year {str(year_d
-00000740: 6972 2e6e 616d 6529 7d63 0100 0000 0000  ir.name)}c......
-00000750: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00000760: 0000 7318 0000 0067 007c 005d 107d 017c  ..s....g.|.].}.|
-00000770: 01a0 00a1 0072 047c 0191 0271 0453 0072  .....r.|...q.S.r
-00000780: 0700 0000 7208 0000 0072 0a00 0000 7207  ....r....r....r.
-00000790: 0000 0072 0700 0000 720d 0000 0072 0e00  ...r....r....r..
-000007a0: 0000 2b00 0000 7306 0000 0006 0002 0008  ..+...s.........
-000007b0: 007a 2309 576f 726b 696e 6720 6f6e 206e  .z#.Working on n
-000007c0: 6574 207b 7374 7228 6e65 745f 6469 722e  et {str(net_dir.
-000007d0: 6e61 6d65 297d 6301 0000 0000 0000 0000  name)}c.........
-000007e0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-000007f0: 1800 0000 6700 7c00 5d10 7d01 7c01 a000  ....g.|.].}.|...
-00000800: a100 7204 7c01 9102 7104 5300 7207 0000  ..r.|...q.S.r...
-00000810: 0072 0800 0000 720a 0000 0072 0700 0000  .r....r....r....
-00000820: 7207 0000 0072 0d00 0000 720e 0000 002d  r....r....r....-
-00000830: 0000 0073 0600 0000 0600 0200 0800 7a28  ...s..........z(
-00000840: 0909 576f 726b 696e 6720 6f6e 2073 7461  ..Working on sta
-00000850: 7469 6f6e 207b 7374 7228 7374 615f 6469  tion {str(sta_di
-00000860: 722e 6e61 6d65 297d 6301 0000 0000 0000  r.name)}c.......
-00000870: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00000880: 0073 1800 0000 6700 7c00 5d10 7d01 7c01  .s....g.|.].}.|.
-00000890: a000 a100 7204 7c01 9102 7104 5300 7207  ....r.|...q.S.r.
-000008a0: 0000 0072 0800 0000 720a 0000 0072 0700  ...r....r....r..
-000008b0: 0000 7207 0000 0072 0d00 0000 720e 0000  ..r....r....r...
-000008c0: 002f 0000 0073 0600 0000 0600 0200 0800  ./...s..........
-000008d0: 7a18 0909 0957 6f72 6b69 6e67 206f 6e20  z....Working on 
-000008e0: 6368 616e 6e65 6c20 7b7d 7201 0000 00e9  channel {}r.....
-000008f0: 0100 0000 4e7a 2409 0909 0943 7265 6174  ....Nz$....Creat
-00000900: 696e 6720 6f75 7470 7574 2063 6861 6e6e  ing output chann
-00000910: 656c 2064 6972 2022 7b7d 227a 022a 2e7a  el dir "{}"z.*.z
-00000920: 022e 2a7a 2309 0909 097b 6c65 6e28 6669  ..*z#....{len(fi
-00000930: 6c65 7329 3a64 7d20 6669 6c65 7320 746f  les):d} files to
-00000940: 2070 726f 6365 7373 da05 4d53 4545 447a   process..MSEEDz
-00000950: 1564 6179 2773 2073 7472 6561 6d20 6c65  .day's stream le
-00000960: 6e67 7468 2028 7a21 2920 6973 206e 6f74  ngth (z!) is not
-00000970: 2064 6976 6973 6962 6c65 2062 7920 6465   divisible by de
-00000980: 6369 6d61 746f 7220 28fa 0129 7a40 2066  cimator (..)z@ f
-00000990: 6972 7374 2062 6c6f 636b 2773 2073 616d  irst block's sam
-000009a0: 706c 696e 6720 7261 7465 2021 3d20 7b69  pling rate != {i
-000009b0: 6e70 7574 5f73 616d 706c 655f 7261 7465  nput_sample_rate
-000009c0: 7d2c 2073 6b69 7070 696e 672e 2e2e da01  }, skipping.....
-000009d0: 2e29 1672 0200 0000 7205 0000 00da 1164  .).r....r......d
-000009e0: 6563 696d 6174 696f 6e5f 6661 6374 6f72  ecimation_factor
-000009f0: da0d 6765 745f 6261 6e64 5f63 6f64 65da  ..get_band_code.
-00000a00: 076c 6f67 6769 6e67 da04 696e 666f da06  .logging..info..
-00000a10: 666f 726d 6174 da0a 5661 6c75 6545 7272  format..ValueErr
-00000a20: 6f72 da07 6974 6572 6469 72da 0373 7472  or..iterdir..str
-00000a30: da04 6e61 6d65 da05 6d6b 6469 72da 0467  ..name..mkdir..g
-00000a40: 6c6f 6272 0300 0000 da05 7374 6174 73da  lobr......stats.
-00000a50: 046e 7074 73da 0d73 616d 706c 696e 675f  .npts..sampling_
-00000a60: 7261 7465 da07 7761 726e 696e 67da 0573  rate..warning..s
-00000a70: 706c 6974 da03 7275 6eda 0577 7269 7465  plit..run..write
-00000a80: da10 7570 6461 7465 5f69 6e76 656e 746f  ..update_invento
-00000a90: 7279 291b da08 5344 535f 726f 6f74 da03  ry)...SDS_root..
-00000aa0: 696e 76da 1169 6e70 7574 5f73 616d 706c  inv..input_sampl
-00000ab0: 655f 7261 7465 da0a 6465 6369 6d5f 6c69  e_rate..decim_li
-00000ac0: 7374 da09 6465 6369 6d61 746f 725a 126f  st..decimatorZ.o
-00000ad0: 7574 7075 745f 7361 6d70 6c65 5f72 6174  utput_sample_rat
-00000ae0: 65da 0c69 6e5f 6261 6e64 5f63 6f64 655a  e..in_band_codeZ
-00000af0: 0d6f 7574 5f62 616e 645f 636f 6465 5a08  .out_band_codeZ.
-00000b00: 7965 6172 5f64 6972 5a07 6e65 745f 6469  year_dirZ.net_di
-00000b10: 725a 0773 7461 5f64 6972 5a07 6368 615f  rZ.sta_dirZ.cha_
-00000b20: 6469 725a 0863 6861 5f6e 616d 655a 0b6f  dirZ.cha_nameZ.o
-00000b30: 7574 5f63 6861 5f64 6972 da05 6669 6c65  ut_cha_dir..file
-00000b40: 73da 0166 da06 7374 7265 616d da03 6e65  s..f..stream..ne
-00000b50: 74da 0373 7461 da03 6c6f 635a 0369 6368  t..sta..locZ.ich
-00000b60: da03 7479 70da 0279 72da 0264 795a 0864  ..typ..yr..dyZ.d
-00000b70: 5f73 7472 6561 6d5a 036f 6368 5a08 6f75  _streamZ.ochZ.ou
-00000b80: 7466 6e61 6d65 7207 0000 0072 0700 0000  tfnamer....r....
-00000b90: 720d 0000 00da 0c64 6563 696d 6174 655f  r......decimate_
-00000ba0: 5344 530f 0000 0073 6000 0000 0010 0801  SDS....s`.......
-00000bb0: 0801 0a01 0c01 0c01 0801 0200 02ff 0602  ................
-00000bc0: 0801 0802 1801 0a01 1801 0a01 1801 0a01  ................
-00000bd0: 1801 0801 08ff 0602 0601 0c01 0201 1401  ................
-00000be0: 0801 0801 04ff 0602 1201 0a01 0801 0e01  ................
-00000bf0: 1801 0201 1aff 0404 1201 0401 0cff 0403  ................
-00000c00: 1e01 0a01 1001 2c01 1401 1401 7235 0000  ......,.....r5..
-00000c10: 0063 0500 0000 0000 0000 0000 0000 0600  .c..............
-00000c20: 0000 0500 0000 4300 0000 733e 0000 0074  ......C...s>...t
-00000c30: 007c 0164 0183 027d 0574 017c 007c 057c  .|.d...}.t.|.|.|
-00000c40: 027c 0383 047d 057c 0464 026b 0872 2c7c  .|...}.|.d.k.r,|
-00000c50: 01a0 0264 0364 04a1 027d 047c 056a 037c  ...d.d...}.|.j.|
-00000c60: 0464 0164 058d 0201 0064 0253 0029 0661  .d.d.....d.S.).a
-00000c70: 1302 0000 0a20 2020 2041 7070 6c69 6573  .....    Applies
-00000c80: 2064 6563 696d 6174 655f 5344 5320 7768   decimate_SDS wh
-00000c90: 656e 2074 6865 2069 6e76 656e 746f 7279  en the inventory
-00000ca0: 2069 7320 696e 2061 2053 7461 7469 6f6e   is in a Station
-00000cb0: 584d 4c20 6669 6c65 0a0a 2020 2020 4172  XML file..    Ar
-00000cc0: 6773 3a0a 2020 2020 2020 2020 5344 535f  gs:.        SDS_
-00000cd0: 726f 6f74 2028 7374 7220 6f72 2050 6174  root (str or Pat
-00000ce0: 6829 3a20 5344 5320 726f 6f74 2064 6972  h): SDS root dir
-00000cf0: 6563 746f 7279 0a20 2020 2020 2020 2069  ectory.        i
-00000d00: 6e76 5f66 696c 6520 2873 7472 206f 7220  nv_file (str or 
-00000d10: 5061 7468 293a 2050 6174 6820 746f 2053  Path): Path to S
-00000d20: 7461 7469 6f6e 584d 4c20 6669 6c65 0a20  tationXML file. 
-00000d30: 2020 2020 2020 2069 6e70 7574 5f73 616d         input_sam
-00000d40: 706c 655f 7261 7465 2028 666c 6f61 7429  ple_rate (float)
-00000d50: 3a20 7361 6d70 6c65 2072 6174 6520 6f66  : sample rate of
-00000d60: 2064 6174 6120 746f 2070 726f 6365 7373   data to process
-00000d70: 0a20 2020 2020 2020 2064 6563 696d 5f6c  .        decim_l
-00000d80: 6973 7420 286c 6973 7429 3a20 6c69 7374  ist (list): list
-00000d90: 206f 6620 6465 6369 6d61 7469 6f6e 2066   of decimation f
-00000da0: 6163 746f 7273 2028 696e 7465 6765 7273  actors (integers
-00000db0: 2062 6574 7765 656e 0a20 2020 2020 2020   between.       
-00000dc0: 2020 2020 2032 2061 6e64 2037 290a 2020       2 and 7).  
-00000dd0: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
-00000de0: 6520 2873 7472 293a 206f 7574 7075 7420  e (str): output 
-00000df0: 5374 6174 696f 6e58 4d4c 2066 696c 656e  StationXML filen
-00000e00: 616d 6520 284e 6f6e 6520 3d3e 200a 2020  ame (None => .  
-00000e10: 2020 2020 2020 2020 2020 696e 6669 6c65            infile
-00000e20: 2e72 6570 6c61 6365 2827 2e78 6d6c 272c  .replace('.xml',
-00000e30: 2027 5f64 6563 696d 2e78 6d6c 2729 290a   '_decim.xml')).
-00000e40: 0a20 2020 2054 6865 206f 7574 7075 7420  .    The output 
-00000e50: 5374 6174 696f 6e58 4d4c 2066 696c 6520  StationXML file 
-00000e60: 7769 6c6c 2068 6176 6520 7468 6520 7375  will have the su
-00000e70: 6666 6978 2020 605f 6465 6369 6d2e 786d  ffix  `_decim.xm
-00000e80: 6c60 0a20 2020 20da 0a53 5441 5449 4f4e  l`.    ..STATION
-00000e90: 584d 4c4e 7a04 2e78 6d6c 7a0a 5f64 6563  XMLNz..xmlz._dec
-00000ea0: 696d 2e78 6d6c 2901 7217 0000 0029 0472  im.xml).r....).r
-00000eb0: 0400 0000 7235 0000 00da 0772 6570 6c61  ....r5.....repla
-00000ec0: 6365 7224 0000 0029 0672 2600 0000 da08  cer$...).r&.....
-00000ed0: 696e 765f 6669 6c65 7228 0000 0072 2900  inv_filer(...r).
-00000ee0: 0000 da0b 6f75 7470 7574 5f66 696c 6572  ....output_filer
-00000ef0: 2700 0000 7207 0000 0072 0700 0000 720d  '...r....r....r.
-00000f00: 0000 00da 1764 6563 696d 6174 655f 5344  .....decimate_SD
-00000f10: 535f 5374 6174 696f 6e58 4d4c 4f00 0000  S_StationXMLO...
-00000f20: 730a 0000 0000 100a 010e 0108 010c 0172  s..............r
-00000f30: 3a00 0000 6300 0000 0000 0000 0000 0000  :...c...........
-00000f40: 0002 0000 000a 0000 0043 0000 0073 b400  .........C...s..
-00000f50: 0000 7400 6a01 6401 6402 8d01 7d00 7c00  ..t.j.d.d...}.|.
-00000f60: 6a02 6403 6404 6405 8d02 0100 7c00 6a02  j.d.d.d.....|.j.
-00000f70: 6406 6407 6405 8d02 0100 7c00 6a02 6408  d.d.d.....|.j.d.
-00000f80: 7403 6409 640a 8d03 0100 7c00 6a02 640b  t.d.d.....|.j.d.
-00000f90: 7404 640c 640d 640e 640f 6410 6411 6412  t.d.d.d.d.d.d.d.
-00000fa0: 6706 6413 6414 8d05 0100 7c00 6a02 6415  g.d.d.....|.j.d.
-00000fb0: 6416 6400 6417 6418 8d04 0100 7c00 6a02  d.d.d.d.....|.j.
-00000fc0: 6419 641a 641b 641c 641d 8d04 0100 7c00  d.d.d.d.d.....|.
-00000fd0: a005 a100 7d01 7c01 6a06 7396 7407 a008  ....}.|.j.s.t...
-00000fe0: 7407 6a09 a101 0100 740a 7c01 6a0b 7c01  t.j.....t.|.j.|.
-00000ff0: 6a0c 7c01 6a0d 7c01 6a0e 7c01 6a0f 8305  j.|.j.|.j.|.j...
-00001000: 0100 6400 5300 291e 4e7a 3849 6e73 6572  ..d.S.).Nz8Inser
-00001010: 7420 6465 6369 6d61 7465 6420 6368 616e  t decimated chan
-00001020: 6e65 6c73 2061 6e64 2063 7265 6174 6520  nels and create 
-00001030: 6e65 7720 5374 6174 696f 6e58 4d4c 2066  new StationXML f
-00001040: 696c 6529 01da 0b64 6573 6372 6970 7469  ile)...descripti
-00001050: 6f6e 7226 0000 007a 1253 4453 2072 6f6f  onr&...z.SDS roo
-00001060: 7420 6469 7265 6374 6f72 7929 01da 0468  t directory)...h
-00001070: 656c 7072 3800 0000 7a0f 5374 6174 696f  elpr8...z.Statio
-00001080: 6e58 4d4c 2066 696c 6572 2800 0000 7a2d  nXML filer(...z-
-00001090: 5072 6f63 6573 7320 6f6e 6c79 2063 6861  Process only cha
-000010a0: 6e6e 656c 7320 6861 7669 6e67 2074 6869  nnels having thi
-000010b0: 7320 7361 6d70 6c65 2072 6174 6529 02da  s sample rate)..
-000010c0: 0474 7970 6572 3c00 0000 da0c 6465 6369  .typer<.....deci
-000010d0: 6d5f 6661 6374 6f72 fa01 2be9 0200 0000  m_factor..+.....
-000010e0: e903 0000 00e9 0400 0000 e905 0000 00e9  ................
-000010f0: 0600 0000 e907 0000 007a 2653 6571 7565  .........z&Seque
-00001100: 6e63 6520 6f66 2064 6563 696d 6174 696f  nce of decimatio
-00001110: 6e20 6661 6374 6f72 7320 746f 2075 7365  n factors to use
-00001120: 2929 0472 3d00 0000 da05 6e61 7267 73da  )).r=.....nargs.
-00001130: 0763 686f 6963 6573 723c 0000 007a 042d  .choicesr<...z.-
-00001140: 2d6f 6672 3900 0000 7a4a 4f75 7470 7574  -ofr9...zJOutput
-00001150: 2053 7461 7469 6f6e 584d 4c20 6669 6c65   StationXML file
-00001160: 6e61 6d65 2028 6465 6661 756c 7420 3d20  name (default = 
-00001170: 696e 6669 6c65 2e72 6570 6c61 6365 2827  infile.replace('
-00001180: 2e78 6d6c 272c 2027 5f64 6563 696d 2e78  .xml', '_decim.x
-00001190: 6d6c 2729 2903 da04 6465 7374 da07 6465  ml'))...dest..de
-000011a0: 6661 756c 7472 3c00 0000 7a02 2d71 7a07  faultr<...z.-qz.
-000011b0: 2d2d 7175 6965 74da 0a73 746f 7265 5f74  --quiet..store_t
-000011c0: 7275 657a 1d53 7570 7072 6573 7320 696e  ruez.Suppress in
-000011d0: 666f 726d 6174 696f 6e20 6d65 7373 6167  formation messag
-000011e0: 6573 2902 da06 6163 7469 6f6e 723c 0000  es)...actionr<..
-000011f0: 0029 10da 0861 7267 7061 7273 65da 0e41  .)...argparse..A
-00001200: 7267 756d 656e 7450 6172 7365 72da 0c61  rgumentParser..a
-00001210: 6464 5f61 7267 756d 656e 74da 0566 6c6f  dd_argument..flo
-00001220: 6174 da03 696e 74da 0a70 6172 7365 5f61  at..int..parse_a
-00001230: 7267 73da 0571 7569 6574 7215 0000 00da  rgs..quietr.....
-00001240: 0764 6973 6162 6c65 da05 4445 4255 4772  .disable..DEBUGr
-00001250: 3a00 0000 7226 0000 0072 3800 0000 7228  :...r&...r8...r(
-00001260: 0000 0072 3e00 0000 7239 0000 0029 02da  ...r>...r9...)..
-00001270: 0670 6172 7365 72da 0461 7267 7372 0700  .parser..argsr..
-00001280: 0000 7207 0000 0072 0d00 0000 da04 6d61  ..r....r......ma
-00001290: 696e 6600 0000 7338 0000 0000 0104 0102  inf...s8........
-000012a0: ff06 030e 0106 0102 ff06 0208 0102 ff06  ................
-000012b0: 020a 010e 0102 fe06 030a 0102 ff06 030a  ................
-000012c0: 0102 ff06 0208 0106 010c 010a 0104 0004  ................
-000012d0: 0104 fe72 5700 0000 2901 4e29 0eda 075f  ...rW...).N)..._
-000012e0: 5f64 6f63 5f5f 7215 0000 0072 4c00 0000  _doc__r....rL...
-000012f0: da07 7061 7468 6c69 6272 0200 0000 da11  ..pathlibr......
-00001300: 6f62 7370 792e 636f 7265 2e73 7472 6561  obspy.core.strea
-00001310: 6d72 0300 0000 da14 6f62 7370 792e 636f  mr......obspy.co
-00001320: 7265 2e69 6e76 656e 746f 7279 7204 0000  re.inventoryr...
-00001330: 00da 0674 6973 6b69 7472 0500 0000 7235  ...tiskitr....r5
-00001340: 0000 0072 3a00 0000 7257 0000 0072 0700  ...r:...rW...r..
-00001350: 0000 7207 0000 0072 0700 0000 720d 0000  ..r....r....r...
-00001360: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001370: 1400 0000 0404 0801 0801 0c02 0c01 0c02  ................
-00001380: 0c03 0841 00ff 0a17                      ...A....
+00000190: 02a1 0101 007c 067c 076b 0272 5a74 0764  .....|.|.k.rZt.d
+000001a0: 037c 069b 009d 0283 0182 0164 0464 0584  .|.........d.d..
+000001b0: 007c 00a0 08a1 0044 0083 0144 0090 025d  .|.....D...D...]
+000001c0: 1a7d 0874 04a0 0564 0674 097c 086a 0a83  .}.t...d.t.|.j..
+000001d0: 019b 009d 02a1 0101 0064 0764 0584 007c  .........d.d...|
+000001e0: 08a0 08a1 0044 0083 0144 0090 015d ea7d  .....D...D...].}
+000001f0: 0974 04a0 0564 0874 097c 096a 0a83 019b  .t...d.t.|.j....
+00000200: 009d 02a1 0101 0064 0964 0584 007c 09a0  .......d.d...|..
+00000210: 08a1 0044 0083 0144 0090 015d ba7d 0a74  ...D...D...].}.t
+00000220: 04a0 0564 0a74 097c 0a6a 0a83 019b 009d  ...d.t.|.j......
+00000230: 02a1 0101 0064 0b64 0584 007c 0aa0 08a1  .....d.d...|....
+00000240: 0044 0083 0144 0090 015d 8a7d 0b74 04a0  .D...D...].}.t..
+00000250: 0564 0c74 097c 0b6a 0a83 019b 009d 02a1  .d.t.|.j........
+00000260: 0101 007c 0b6a 0a7d 0c7c 0c64 0d19 007c  ...|.j.}.|.d...|
+00000270: 066b 0290 0173 2871 f67c 0a7c 077c 0c64  .k...s(q.|.|.|.d
+00000280: 0e64 0f85 0219 0017 001b 007d 0d7c 0da0  .d.........}.|..
+00000290: 0ba1 0001 0074 04a0 0564 10a0 067c 0d6a  .....t...d...|.j
+000002a0: 0aa1 01a1 0101 0074 0c7c 0ba0 0d64 117c  .......t.|...d.|
+000002b0: 0c9b 0064 129d 03a1 0183 017d 0e74 04a0  ...d.......}.t..
+000002c0: 0564 1374 0e7c 0e83 0164 149b 0464 159d  .d.t.|...d...d..
+000002d0: 03a1 0101 007c 0e44 005d ec7d 0f74 0f74  .....|.D.].}.t.t
+000002e0: 097c 0f83 0164 1683 027d 107c 1064 0d19  .|...d...}.|.d..
+000002f0: 006a 106a 117c 046a 0216 0064 0d6b 0290  .j.j.|.j...d.k..
+00000300: 0172 d274 0764 177c 1064 0d19 006a 106a  .r.t.d.|.d...j.j
+00000310: 119b 0064 187c 046a 029b 0064 199d 0583  ...d.|.j...d....
+00000320: 0101 007c 1064 0d19 006a 106a 127c 026b  ...|.d...j.j.|.k
+00000330: 0390 0172 fe74 04a0 1374 097c 0f83 019b  ...r.t...t.|....
+00000340: 0064 1a7c 029b 0064 1b9d 04a1 0101 0074  .d.|...d.......t
+00000350: 097c 0f6a 0a83 01a0 1464 1ca1 015c 077d  .|.j.....d...\.}
+00000360: 117d 127d 137d 147d 157d 167d 177c 04a0  .}.}.}.}.}.}.|..
+00000370: 157c 10a1 017d 187c 077c 1464 0e64 0f85  .|...}.|.|.d.d..
+00000380: 0219 0017 007d 197c 119b 0064 1c7c 129b  .....}.|...d.|..
+00000390: 0064 1c7c 139b 0064 1c7c 199b 0064 1c7c  .d.|...d.|...d.|
+000003a0: 159b 0064 1c7c 169b 0064 1c7c 179b 009d  ...d.|...d.|....
+000003b0: 0d7d 1a7c 18a0 167c 0d7c 1a1b 0064 16a1  .}.|...|.|...d..
+000003c0: 0201 0090 0171 887c 04a0 177c 017c 10a1  .....q.|...|.|..
+000003d0: 027d 0171 f671 c871 9a71 6c7c 0153 0029  .}.q.q.q.ql|.S.)
+000003e0: 1d61 3002 0000 0a20 2020 2054 6865 206d  .a0....    The m
+000003f0: 6169 6e20 6675 6e63 7469 6f6e 0a0a 2020  ain function..  
+00000400: 2020 5368 6f75 6c64 2065 6e73 7572 6520    Should ensure 
+00000410: 636f 6e74 696e 7569 7479 2061 6372 6f73  continuity acros
+00000420: 7320 6461 7920 616e 6420 7965 6172 2062  s day and year b
+00000430: 6f75 6e64 6172 6965 732e 0a20 2020 2043  oundaries..    C
+00000440: 7572 7265 6e74 6c79 206a 7573 7420 6368  urrently just ch
+00000450: 6563 6b73 2069 6620 7468 6520 7265 7175  ecks if the requ
+00000460: 6573 7465 6420 6465 6369 6d61 7469 6f6e  ested decimation
+00000470: 2069 7320 616e 2069 6e74 6567 7261 6c20   is an integral 
+00000480: 6469 7669 736f 720a 2020 2020 6f66 2074  divisor.    of t
+00000490: 6865 2063 7572 7265 6e74 2064 6179 2773  he current day's
+000004a0: 2073 616d 706c 6573 2061 6e64 2072 6574   samples and ret
+000004b0: 7572 6e73 2061 6e20 6572 726f 7220 6966  urns an error if
+000004c0: 206e 6f74 0a20 2020 204f 6e6c 7920 776f   not.    Only wo
+000004d0: 726b 7320 666f 7220 6272 6f61 642d 6261  rks for broad-ba
+000004e0: 6e64 2063 6861 6e6e 656c 730a 0a20 2020  nd channels..   
+000004f0: 2041 7267 733a 0a20 2020 2020 2020 2053   Args:.        S
+00000500: 4453 5f72 6f6f 7420 2873 7472 206f 7220  DS_root (str or 
+00000510: 5061 7468 293a 2053 4453 2072 6f6f 7420  Path): SDS root 
+00000520: 6469 7265 6374 6f72 790a 2020 2020 2020  directory.      
+00000530: 2020 696e 7620 283a 636c 6173 733a 606f    inv (:class:`o
+00000540: 6273 7079 2e63 6f72 652e 696e 7665 6e74  bspy.core.invent
+00000550: 6f72 792e 496e 7665 6e74 6f72 7960 293a  ory.Inventory`):
+00000560: 2073 7461 7469 6f6e 2069 6e76 656e 746f   station invento
+00000570: 7279 0a20 2020 2020 2020 2069 6e70 7574  ry.        input
+00000580: 5f73 616d 706c 655f 7261 7465 2028 666c  _sample_rate (fl
+00000590: 6f61 7429 3a20 7361 6d70 6c65 2072 6174  oat): sample rat
+000005a0: 6520 6f66 2064 6174 6120 746f 2070 726f  e of data to pro
+000005b0: 6365 7373 0a20 2020 2020 2020 2064 6563  cess.        dec
+000005c0: 696d 5f6c 6973 7420 286c 6973 7429 3a20  im_list (list): 
+000005d0: 6c69 7374 206f 6620 6465 6369 6d61 7469  list of decimati
+000005e0: 6f6e 2066 6163 746f 7273 2028 696e 7465  on factors (inte
+000005f0: 6765 7273 2062 6574 7765 656e 0a20 2020  gers between.   
+00000600: 2020 2020 2020 2020 2032 2061 6e64 2037           2 and 7
+00000610: 290a 2020 2020 da01 427a 3b6f 7574 7075  ).    ..Bz;outpu
+00000620: 7420 7361 6d70 6c69 6e67 2072 6174 6520  t sampling rate 
+00000630: 7769 6c6c 2062 6520 7b3a 677d 2073 7073  will be {:g} sps
+00000640: 2c20 6261 6e64 2063 6f64 6520 7769 6c6c  , band code will
+00000650: 2062 6520 7b7d 7a25 6964 656e 7469 6361   be {}z%identica
+00000660: 6c20 696e 7075 7420 2620 6f75 7470 7574  l input & output
+00000670: 2062 616e 6420 636f 6465 733a 2063 0100   band codes: c..
+00000680: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000690: 0000 5300 0000 7318 0000 0067 007c 005d  ..S...s....g.|.]
+000006a0: 107d 017c 01a0 00a1 0072 047c 0191 0271  .}.|.....r.|...q
+000006b0: 0453 00a9 00a9 01da 0669 735f 6469 72a9  .S.......is_dir.
+000006c0: 02da 022e 30da 0178 7207 0000 0072 0700  ....0..xr....r..
+000006d0: 0000 fa48 2f55 7365 7273 2f63 7261 7766  ...H/Users/crawf
+000006e0: 6f72 642f 5f57 6f72 6b2f 5072 6f67 7261  ord/_Work/Progra
+000006f0: 6d6d 696e 672f 7469 736b 6974 2f74 6973  mming/tiskit/tis
+00000700: 6b69 742f 6465 6369 6d61 7465 2f64 6563  kit/decimate/dec
+00000710: 696d 6174 655f 5344 532e 7079 da0a 3c6c  imate_SDS.py..<l
+00000720: 6973 7463 6f6d 703e 2900 0000 7306 0000  istcomp>)...s...
+00000730: 0006 0002 0008 007a 2064 6563 696d 6174  .......z decimat
+00000740: 655f 5344 532e 3c6c 6f63 616c 733e 2e3c  e_SDS.<locals>.<
+00000750: 6c69 7374 636f 6d70 3e7a 1057 6f72 6b69  listcomp>z.Worki
+00000760: 6e67 206f 6e20 7965 6172 2063 0100 0000  ng on year c....
+00000770: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000780: 5300 0000 7318 0000 0067 007c 005d 107d  S...s....g.|.].}
+00000790: 017c 01a0 00a1 0072 047c 0191 0271 0453  .|.....r.|...q.S
+000007a0: 0072 0700 0000 7208 0000 0072 0a00 0000  .r....r....r....
+000007b0: 7207 0000 0072 0700 0000 720d 0000 0072  r....r....r....r
+000007c0: 0e00 0000 2b00 0000 7306 0000 0006 0002  ....+...s.......
+000007d0: 0008 007a 1009 576f 726b 696e 6720 6f6e  ...z..Working on
+000007e0: 206e 6574 2063 0100 0000 0000 0000 0000   net c..........
+000007f0: 0000 0200 0000 0400 0000 5300 0000 7318  ..........S...s.
+00000800: 0000 0067 007c 005d 107d 017c 01a0 00a1  ...g.|.].}.|....
+00000810: 0072 047c 0191 0271 0453 0072 0700 0000  .r.|...q.S.r....
+00000820: 7208 0000 0072 0a00 0000 7207 0000 0072  r....r....r....r
+00000830: 0700 0000 720d 0000 0072 0e00 0000 2d00  ....r....r....-.
+00000840: 0000 7306 0000 0006 0002 0008 007a 1509  ..s..........z..
+00000850: 0957 6f72 6b69 6e67 206f 6e20 7374 6174  .Working on stat
+00000860: 696f 6e20 6301 0000 0000 0000 0000 0000  ion c...........
+00000870: 0002 0000 0004 0000 0053 0000 0073 1800  .........S...s..
+00000880: 0000 6700 7c00 5d10 7d01 7c01 a000 a100  ..g.|.].}.|.....
+00000890: 7204 7c01 9102 7104 5300 7207 0000 0072  r.|...q.S.r....r
+000008a0: 0800 0000 720a 0000 0072 0700 0000 7207  ....r....r....r.
+000008b0: 0000 0072 0d00 0000 720e 0000 002f 0000  ...r....r..../..
+000008c0: 0073 0600 0000 0600 0200 0800 7a16 0909  .s..........z...
+000008d0: 0957 6f72 6b69 6e67 206f 6e20 6368 616e  .Working on chan
+000008e0: 6e65 6c20 7201 0000 00e9 0100 0000 4e7a  nel r.........Nz
+000008f0: 2409 0909 0943 7265 6174 696e 6720 6f75  $....Creating ou
+00000900: 7470 7574 2063 6861 6e6e 656c 2064 6972  tput channel dir
+00000910: 2022 7b7d 227a 022a 2e7a 022e 2a7a 0409   "{}"z.*.z..*z..
+00000920: 0909 09da 0164 7a11 2066 696c 6573 2074  .....dz. files t
+00000930: 6f20 7072 6f63 6573 73da 054d 5345 4544  o process..MSEED
+00000940: 7a15 6461 7927 7320 7374 7265 616d 206c  z.day's stream l
+00000950: 656e 6774 6820 287a 2129 2069 7320 6e6f  ength (z!) is no
+00000960: 7420 6469 7669 7369 626c 6520 6279 2064  t divisible by d
+00000970: 6563 696d 6174 6f72 2028 fa01 297a 2020  ecimator (..)z  
+00000980: 6669 7273 7420 626c 6f63 6b27 7320 7361  first block's sa
+00000990: 6d70 6c69 6e67 2072 6174 6520 213d 207a  mpling rate != z
+000009a0: 0d2c 2073 6b69 7070 696e 672e 2e2e da01  ., skipping.....
+000009b0: 2e29 1872 0200 0000 7205 0000 00da 1164  .).r....r......d
+000009c0: 6563 696d 6174 696f 6e5f 6661 6374 6f72  ecimation_factor
+000009d0: da0d 6765 745f 6261 6e64 5f63 6f64 65da  ..get_band_code.
+000009e0: 076c 6f67 6769 6e67 da04 696e 666f da06  .logging..info..
+000009f0: 666f 726d 6174 da0a 5661 6c75 6545 7272  format..ValueErr
+00000a00: 6f72 da07 6974 6572 6469 72da 0373 7472  or..iterdir..str
+00000a10: da04 6e61 6d65 da05 6d6b 6469 72da 046c  ..name..mkdir..l
+00000a20: 6973 74da 0467 6c6f 62da 036c 656e 7203  ist..glob..lenr.
+00000a30: 0000 00da 0573 7461 7473 da04 6e70 7473  .....stats..npts
+00000a40: da0d 7361 6d70 6c69 6e67 5f72 6174 65da  ..sampling_rate.
+00000a50: 0777 6172 6e69 6e67 da05 7370 6c69 74da  .warning..split.
+00000a60: 0864 6563 696d 6174 65da 0577 7269 7465  .decimate..write
+00000a70: da10 7570 6461 7465 5f69 6e76 656e 746f  ..update_invento
+00000a80: 7279 291b da08 5344 535f 726f 6f74 da03  ry)...SDS_root..
+00000a90: 696e 76da 1169 6e70 7574 5f73 616d 706c  inv..input_sampl
+00000aa0: 655f 7261 7465 da0a 6465 6369 6d5f 6c69  e_rate..decim_li
+00000ab0: 7374 da09 6465 6369 6d61 746f 725a 126f  st..decimatorZ.o
+00000ac0: 7574 7075 745f 7361 6d70 6c65 5f72 6174  utput_sample_rat
+00000ad0: 65da 0c69 6e5f 6261 6e64 5f63 6f64 655a  e..in_band_codeZ
+00000ae0: 0d6f 7574 5f62 616e 645f 636f 6465 5a08  .out_band_codeZ.
+00000af0: 7965 6172 5f64 6972 5a07 6e65 745f 6469  year_dirZ.net_di
+00000b00: 725a 0773 7461 5f64 6972 5a07 6368 615f  rZ.sta_dirZ.cha_
+00000b10: 6469 725a 0863 6861 5f6e 616d 655a 0b6f  dirZ.cha_nameZ.o
+00000b20: 7574 5f63 6861 5f64 6972 da05 6669 6c65  ut_cha_dir..file
+00000b30: 73da 0166 da06 7374 7265 616d da03 6e65  s..f..stream..ne
+00000b40: 74da 0373 7461 da03 6c6f 635a 0369 6368  t..sta..locZ.ich
+00000b50: da03 7479 70da 0279 72da 0264 795a 0864  ..typ..yr..dyZ.d
+00000b60: 5f73 7472 6561 6d5a 036f 6368 5a08 6f75  _streamZ.ochZ.ou
+00000b70: 7466 6e61 6d65 7207 0000 0072 0700 0000  tfnamer....r....
+00000b80: 720d 0000 00da 0c64 6563 696d 6174 655f  r......decimate_
+00000b90: 5344 530f 0000 0073 5c00 0000 0010 0801  SDS....s\.......
+00000ba0: 0801 0a01 0c01 0c01 0801 0200 02ff 0602  ................
+00000bb0: 0801 0e02 1801 1601 1801 1601 1801 1601  ................
+00000bc0: 1801 1601 0601 0e01 0201 1401 0801 0801  ................
+00000bd0: 04ff 0602 1601 1801 0801 0e01 1801 0201  ................
+00000be0: 1aff 0404 1201 0401 12ff 0403 1e01 0a01  ................
+00000bf0: 1001 2c01 1401 1401 7238 0000 0063 0500  ..,.....r8...c..
+00000c00: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+00000c10: 0000 4300 0000 733e 0000 0074 007c 0164  ..C...s>...t.|.d
+00000c20: 0183 027d 0574 017c 007c 057c 027c 0383  ...}.t.|.|.|.|..
+00000c30: 047d 057c 0464 026b 0872 2c7c 01a0 0264  .}.|.d.k.r,|...d
+00000c40: 0364 04a1 027d 047c 056a 037c 0464 0164  .d...}.|.j.|.d.d
+00000c50: 058d 0201 0064 0253 0029 0661 1302 0000  .....d.S.).a....
+00000c60: 0a20 2020 2041 7070 6c69 6573 2064 6563  .    Applies dec
+00000c70: 696d 6174 655f 5344 5320 7768 656e 2074  imate_SDS when t
+00000c80: 6865 2069 6e76 656e 746f 7279 2069 7320  he inventory is 
+00000c90: 696e 2061 2053 7461 7469 6f6e 584d 4c20  in a StationXML 
+00000ca0: 6669 6c65 0a0a 2020 2020 4172 6773 3a0a  file..    Args:.
+00000cb0: 2020 2020 2020 2020 5344 535f 726f 6f74          SDS_root
+00000cc0: 2028 7374 7220 6f72 2050 6174 6829 3a20   (str or Path): 
+00000cd0: 5344 5320 726f 6f74 2064 6972 6563 746f  SDS root directo
+00000ce0: 7279 0a20 2020 2020 2020 2069 6e76 5f66  ry.        inv_f
+00000cf0: 696c 6520 2873 7472 206f 7220 5061 7468  ile (str or Path
+00000d00: 293a 2050 6174 6820 746f 2053 7461 7469  ): Path to Stati
+00000d10: 6f6e 584d 4c20 6669 6c65 0a20 2020 2020  onXML file.     
+00000d20: 2020 2069 6e70 7574 5f73 616d 706c 655f     input_sample_
+00000d30: 7261 7465 2028 666c 6f61 7429 3a20 7361  rate (float): sa
+00000d40: 6d70 6c65 2072 6174 6520 6f66 2064 6174  mple rate of dat
+00000d50: 6120 746f 2070 726f 6365 7373 0a20 2020  a to process.   
+00000d60: 2020 2020 2064 6563 696d 5f6c 6973 7420       decim_list 
+00000d70: 286c 6973 7429 3a20 6c69 7374 206f 6620  (list): list of 
+00000d80: 6465 6369 6d61 7469 6f6e 2066 6163 746f  decimation facto
+00000d90: 7273 2028 696e 7465 6765 7273 2062 6574  rs (integers bet
+00000da0: 7765 656e 0a20 2020 2020 2020 2020 2020  ween.           
+00000db0: 2032 2061 6e64 2037 290a 2020 2020 2020   2 and 7).      
+00000dc0: 2020 6f75 7470 7574 5f66 696c 6520 2873    output_file (s
+00000dd0: 7472 293a 206f 7574 7075 7420 5374 6174  tr): output Stat
+00000de0: 696f 6e58 4d4c 2066 696c 656e 616d 6520  ionXML filename 
+00000df0: 284e 6f6e 6520 3d3e 200a 2020 2020 2020  (None => .      
+00000e00: 2020 2020 2020 696e 6669 6c65 2e72 6570        infile.rep
+00000e10: 6c61 6365 2827 2e78 6d6c 272c 2027 5f64  lace('.xml', '_d
+00000e20: 6563 696d 2e78 6d6c 2729 290a 0a20 2020  ecim.xml'))..   
+00000e30: 2054 6865 206f 7574 7075 7420 5374 6174   The output Stat
+00000e40: 696f 6e58 4d4c 2066 696c 6520 7769 6c6c  ionXML file will
+00000e50: 2068 6176 6520 7468 6520 7375 6666 6978   have the suffix
+00000e60: 2020 605f 6465 6369 6d2e 786d 6c60 0a20    `_decim.xml`. 
+00000e70: 2020 20da 0a53 5441 5449 4f4e 584d 4c4e     ..STATIONXMLN
+00000e80: 7a04 2e78 6d6c 7a0a 5f64 6563 696d 2e78  z..xmlz._decim.x
+00000e90: 6d6c 2901 7218 0000 0029 0472 0400 0000  ml).r....).r....
+00000ea0: 7238 0000 00da 0772 6570 6c61 6365 7227  r8.....replacer'
+00000eb0: 0000 0029 0672 2900 0000 da08 696e 765f  ...).r).....inv_
+00000ec0: 6669 6c65 722b 0000 0072 2c00 0000 da0b  filer+...r,.....
+00000ed0: 6f75 7470 7574 5f66 696c 6572 2a00 0000  output_filer*...
+00000ee0: 7207 0000 0072 0700 0000 720d 0000 00da  r....r....r.....
+00000ef0: 1764 6563 696d 6174 655f 5344 535f 5374  .decimate_SDS_St
+00000f00: 6174 696f 6e58 4d4c 4e00 0000 730a 0000  ationXMLN...s...
+00000f10: 0000 100a 010e 0108 010c 0172 3d00 0000  ...........r=...
+00000f20: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
+00000f30: 000a 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
+00000f40: 6a01 6401 6402 8d01 7d00 7c00 6a02 6403  j.d.d...}.|.j.d.
+00000f50: 6404 6405 8d02 0100 7c00 6a02 6406 6407  d.d.....|.j.d.d.
+00000f60: 6405 8d02 0100 7c00 6a02 6408 7403 6409  d.....|.j.d.t.d.
+00000f70: 640a 8d03 0100 7c00 6a02 640b 7404 640c  d.....|.j.d.t.d.
+00000f80: 640d 640e 640f 6410 6411 6412 6706 6413  d.d.d.d.d.d.g.d.
+00000f90: 6414 8d05 0100 7c00 6a02 6415 6416 6400  d.....|.j.d.d.d.
+00000fa0: 6417 6418 8d04 0100 7c00 6a02 6419 641a  d.d.....|.j.d.d.
+00000fb0: 641b 641c 641d 8d04 0100 7c00 a005 a100  d.d.d.....|.....
+00000fc0: 7d01 7c01 6a06 7396 7407 a008 7407 6a09  }.|.j.s.t...t.j.
+00000fd0: a101 0100 740a 7c01 6a0b 7c01 6a0c 7c01  ....t.|.j.|.j.|.
+00000fe0: 6a0d 7c01 6a0e 7c01 6a0f 8305 0100 6400  j.|.j.|.j.....d.
+00000ff0: 5300 291e 4e7a 3849 6e73 6572 7420 6465  S.).Nz8Insert de
+00001000: 6369 6d61 7465 6420 6368 616e 6e65 6c73  cimated channels
+00001010: 2061 6e64 2063 7265 6174 6520 6e65 7720   and create new 
+00001020: 5374 6174 696f 6e58 4d4c 2066 696c 6529  StationXML file)
+00001030: 01da 0b64 6573 6372 6970 7469 6f6e 7229  ...descriptionr)
+00001040: 0000 007a 1253 4453 2072 6f6f 7420 6469  ...z.SDS root di
+00001050: 7265 6374 6f72 7929 01da 0468 656c 7072  rectory)...helpr
+00001060: 3b00 0000 7a0f 5374 6174 696f 6e58 4d4c  ;...z.StationXML
+00001070: 2066 696c 6572 2b00 0000 7a2d 5072 6f63   filer+...z-Proc
+00001080: 6573 7320 6f6e 6c79 2063 6861 6e6e 656c  ess only channel
+00001090: 7320 6861 7669 6e67 2074 6869 7320 7361  s having this sa
+000010a0: 6d70 6c65 2072 6174 6529 02da 0474 7970  mple rate)...typ
+000010b0: 6572 3f00 0000 da0c 6465 6369 6d5f 6661  er?.....decim_fa
+000010c0: 6374 6f72 fa01 2be9 0200 0000 e903 0000  ctor..+.........
+000010d0: 00e9 0400 0000 e905 0000 00e9 0600 0000  ................
+000010e0: e907 0000 007a 2653 6571 7565 6e63 6520  .....z&Sequence 
+000010f0: 6f66 2064 6563 696d 6174 696f 6e20 6661  of decimation fa
+00001100: 6374 6f72 7320 746f 2075 7365 2929 0472  ctors to use)).r
+00001110: 4000 0000 da05 6e61 7267 73da 0763 686f  @.....nargs..cho
+00001120: 6963 6573 723f 0000 007a 042d 2d6f 6672  icesr?...z.--ofr
+00001130: 3c00 0000 7a4a 4f75 7470 7574 2053 7461  <...zJOutput Sta
+00001140: 7469 6f6e 584d 4c20 6669 6c65 6e61 6d65  tionXML filename
+00001150: 2028 6465 6661 756c 7420 3d20 696e 6669   (default = infi
+00001160: 6c65 2e72 6570 6c61 6365 2827 2e78 6d6c  le.replace('.xml
+00001170: 272c 2027 5f64 6563 696d 2e78 6d6c 2729  ', '_decim.xml')
+00001180: 2903 da04 6465 7374 da07 6465 6661 756c  )...dest..defaul
+00001190: 7472 3f00 0000 7a02 2d71 7a07 2d2d 7175  tr?...z.-qz.--qu
+000011a0: 6965 74da 0a73 746f 7265 5f74 7275 657a  iet..store_truez
+000011b0: 1d53 7570 7072 6573 7320 696e 666f 726d  .Suppress inform
+000011c0: 6174 696f 6e20 6d65 7373 6167 6573 2902  ation messages).
+000011d0: da06 6163 7469 6f6e 723f 0000 0029 10da  ..actionr?...)..
+000011e0: 0861 7267 7061 7273 65da 0e41 7267 756d  .argparse..Argum
+000011f0: 656e 7450 6172 7365 72da 0c61 6464 5f61  entParser..add_a
+00001200: 7267 756d 656e 74da 0566 6c6f 6174 da03  rgument..float..
+00001210: 696e 74da 0a70 6172 7365 5f61 7267 73da  int..parse_args.
+00001220: 0571 7569 6574 7216 0000 00da 0764 6973  .quietr......dis
+00001230: 6162 6c65 da05 4445 4255 4772 3d00 0000  able..DEBUGr=...
+00001240: 7229 0000 0072 3b00 0000 722b 0000 0072  r)...r;...r+...r
+00001250: 4100 0000 723c 0000 0029 02da 0670 6172  A...r<...)...par
+00001260: 7365 72da 0461 7267 7372 0700 0000 7207  ser..argsr....r.
+00001270: 0000 0072 0d00 0000 da04 6d61 696e 6500  ...r......maine.
+00001280: 0000 7338 0000 0000 0104 0102 ff06 030e  ..s8............
+00001290: 0106 0102 ff06 0208 0102 ff06 020a 010e  ................
+000012a0: 0102 fe06 030a 0102 ff06 030a 0102 ff06  ................
+000012b0: 0208 0106 010c 010a 0104 0004 0104 fe72  ...............r
+000012c0: 5a00 0000 2901 4e29 0eda 075f 5f64 6f63  Z...).N)...__doc
+000012d0: 5f5f 7216 0000 0072 4f00 0000 da07 7061  __r....rO.....pa
+000012e0: 7468 6c69 6272 0200 0000 da11 6f62 7370  thlibr......obsp
+000012f0: 792e 636f 7265 2e73 7472 6561 6d72 0300  y.core.streamr..
+00001300: 0000 da14 6f62 7370 792e 636f 7265 2e69  ....obspy.core.i
+00001310: 6e76 656e 746f 7279 7204 0000 005a 0674  nventoryr....Z.t
+00001320: 6973 6b69 7472 0500 0000 7238 0000 0072  iskitr....r8...r
+00001330: 3d00 0000 725a 0000 0072 0700 0000 7207  =...rZ...r....r.
+00001340: 0000 0072 0700 0000 720d 0000 00da 083c  ...r....r......<
+00001350: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00001360: 0404 0801 0801 0c02 0c01 0c02 0c03 0840  ...............@
+00001370: 00ff 0a17                                ....
```

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/decimator.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/decimator.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Oct 11 14:36:20 2022 UTC, .py size: 18622 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 647f 4563 be48 0000  U.......d.Ec.H..
+00000000: 550d 0d0a 0000 0000 e7a7 9963 e049 0000  U..........c.I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6402 6c09 5a09 6401 6402 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6401 6402 6c0b 5a0b 6401 6406 6c0c  Z.d.d.l.Z.d.d.l.
@@ -20,839 +20,852 @@
 00000130: 6f64 2902 da06 5374 7265 616d da05 5472  od)...Stream..Tr
 00000140: 6163 6529 01da 0553 7461 7473 2902 da10  ace)...Stats)...
 00000150: 4649 5252 6573 706f 6e73 6553 7461 6765  FIRResponseStage
 00000160: da1d 436f 6566 6669 6369 656e 7473 5479  ..CoefficientsTy
 00000170: 7065 5265 7370 6f6e 7365 5374 6167 65e9  peResponseStage.
 00000180: 0100 0000 2901 da09 4649 5246 696c 7465  ....)...FIRFilte
 00000190: 7263 0000 0000 0000 0000 0000 0000 0000  rc..............
-000001a0: 0000 0600 0000 4000 0000 73ba 0000 0065  ......@...s....e
+000001a0: 0000 0600 0000 4000 0000 73bc 0000 0065  ......@...s....e
 000001b0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
 000001c0: 0564 023c 0064 035a 0665 0765 0564 043c  .d.<.d.Z.e.e.d.<
-000001d0: 0065 0864 0564 0684 0083 015a 0964 0764  .e.d.d.....Z.d.d
-000001e0: 0884 005a 0a64 2664 0a64 0b84 015a 0b64  ...Z.d&d.d...Z.d
-000001f0: 2764 0d64 0e84 015a 0c65 0d64 0f64 1084  'd.d...Z.e.d.d..
-00000200: 0083 015a 0e64 1164 1284 005a 0f64 2864  ...Z.d.d...Z.d(d
-00000210: 1464 1584 015a 1065 0d64 1664 1784 0083  .d...Z.e.d.d....
-00000220: 015a 1167 0066 0164 1864 1984 015a 1267  .Z.g.f.d.d...Z.g
-00000230: 0066 0164 1a64 1b84 015a 1364 1c64 1d84  .f.d.d...Z.d.d..
-00000240: 005a 1464 1e64 1f84 005a 1564 2064 2184  .Z.d.d...Z.d d!.
-00000250: 005a 1664 2264 2384 005a 1764 2964 2464  .Z.d"d#..Z.d)d$d
-00000260: 2584 015a 1864 0953 0029 2ada 0944 6563  %..Z.d.S.)*..Dec
-00000270: 696d 6174 6f72 6136 0100 000a 2020 2020  imatora6....    
-00000280: 436c 6173 7320 746f 2064 6563 696d 6174  Class to decimat
-00000290: 6520 6f62 7370 7920 7374 7265 616d 2069  e obspy stream i
-000002a0: 6e74 656c 6c69 6765 6e74 790a 0a20 2020  ntelligenty..   
-000002b0: 2043 616e 2061 6c73 6f20 7570 6461 7465   Can also update
-000002c0: 2074 6865 2073 7461 7469 6f6e 2069 6e76   the station inv
-000002d0: 656e 746f 7279 2077 6974 6820 7468 6520  entory with the 
-000002e0: 7573 6564 2066 696c 7465 7220 7265 7370  used filter resp
-000002f0: 6f6e 7365 730a 0a20 2020 2041 7267 733a  onses..    Args:
-00000300: 0a20 2020 2020 2020 2064 6563 696d 6174  .        decimat
-00000310: 6573 2028 6c69 7374 293a 206c 6973 7420  es (list): list 
-00000320: 6f66 2064 6563 696d 6174 696f 6e20 6661  of decimation fa
-00000330: 6374 6f72 7374 2074 6f20 7573 6520 2869  ctorst to use (i
-00000340: 6e74 6567 6572 7320 6265 7477 6565 6e0a  ntegers between.
-00000350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000360: 2020 2020 2020 2020 3220 616e 6420 372c          2 and 7,
-00000370: 2077 696c 6c20 6265 2061 7070 6c69 6564   will be applied
-00000380: 2069 6e20 6f72 6465 7229 0a20 2020 2020   in order).     
-00000390: 2020 2076 6572 626f 7365 2028 626f 6f6c     verbose (bool
-000003a0: 293a 2042 6520 6368 6174 7479 0a20 2020  ): Be chatty.   
-000003b0: 20da 0964 6563 696d 6174 6573 46da 0776   ..decimatesF..v
-000003c0: 6572 626f 7365 6301 0000 0000 0000 0000  erbosec.........
-000003d0: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-000003e0: 0a00 0000 7400 7c00 6a01 8301 5300 2901  ....t.|.j...S.).
-000003f0: 7a29 546f 7461 6c20 6465 6369 6d61 7469  z)Total decimati
-00000400: 6f6e 2028 7072 6f64 7563 7420 6f66 2060  on (product of `
-00000410: 6465 6369 6d61 7465 7360 2929 0272 0600  decimates`)).r..
-00000420: 0000 720f 0000 0029 01da 0473 656c 66a9  ..r....)...self.
-00000430: 0072 1200 0000 fa45 2f55 7365 7273 2f63  .r.....E/Users/c
-00000440: 7261 7766 6f72 642f 5f57 6f72 6b2f 5072  rawford/_Work/Pr
-00000450: 6f67 7261 6d6d 696e 672f 7469 736b 6974  ogramming/tiskit
-00000460: 2f74 6973 6b69 742f 6465 6369 6d61 7465  /tiskit/decimate
-00000470: 2f64 6563 696d 6174 6f72 2e70 79da 1164  /decimator.py..d
-00000480: 6563 696d 6174 696f 6e5f 6661 6374 6f72  ecimation_factor
-00000490: 3200 0000 7302 0000 0000 037a 1b44 6563  2...s......z.Dec
-000004a0: 696d 6174 6f72 2e64 6563 696d 6174 696f  imator.decimatio
-000004b0: 6e5f 6661 6374 6f72 6302 0000 0000 0000  n_factorc.......
-000004c0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000004d0: 0073 3e00 0000 7400 7c01 7401 8302 7214  .s>...t.|.t...r.
-000004e0: 7c00 a002 7c01 a101 5300 7400 7c01 7403  |...|...S.t.|.t.
-000004f0: 8302 7232 7c00 a002 7401 7c01 6701 8301  ..r2|...t.|.g...
-00000500: a101 6401 1900 5300 7404 6402 8301 8201  ..d...S.t.d.....
-00000510: 6403 5300 2904 7a88 0a20 2020 2020 2020  d.S.).z..       
-00000520: 2041 7070 6c79 2064 6563 696d 6174 6f72   Apply decimator
-00000530: 2074 6f20 6461 7461 0a0a 2020 2020 2020   to data..      
-00000540: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00000550: 2020 2020 6461 7461 2028 3a63 6c61 7373      data (:class
-00000560: 3a60 6f62 7370 792e 5374 7265 616d 6020  :`obspy.Stream` 
-00000570: 6f72 203a 636c 6173 733a 606f 6273 7079  or :class:`obspy
-00000580: 2e54 7261 6365 6029 3a20 7761 7665 666f  .Trace`): wavefo
-00000590: 726d 2064 6174 610a 2020 2020 2020 2020  rm data.        
-000005a0: 7201 0000 007a 1d64 6174 6120 6973 206e  r....z.data is n
-000005b0: 6f74 2061 2053 7472 6561 6d20 6f72 2054  ot a Stream or T
-000005c0: 7261 6365 4e29 05da 0a69 7369 6e73 7461  raceN)...isinsta
-000005d0: 6e63 6572 0700 0000 da0b 5f72 756e 5f73  ncer......_run_s
-000005e0: 7472 6561 6d72 0800 0000 da09 5479 7065  treamr......Type
-000005f0: 4572 726f 7229 0272 1100 0000 da04 6461  Error).r......da
-00000600: 7461 7212 0000 0072 1200 0000 7213 0000  tar....r....r...
-00000610: 00da 0864 6563 696d 6174 6537 0000 0073  ...decimate7...s
-00000620: 0a00 0000 0007 0a01 0a01 0a01 1402 7a12  ..............z.
-00000630: 4465 6369 6d61 746f 722e 6465 6369 6d61  Decimator.decima
-00000640: 7465 4e63 0500 0000 0000 0000 0000 0000  teNc............
-00000650: 0800 0000 0900 0000 4300 0000 7384 0000  ........C...s...
-00000660: 007c 01a0 00a1 007d 017c 0264 016b 0972  .|.....}.|.d.k.r
-00000670: 2064 0264 0384 007c 0244 0083 017d 056e   d.d...|.D...}.n
-00000680: 0e64 0464 0384 007c 0144 0083 017d 057c  .d.d...|.D...}.|
-00000690: 0544 005d 4c7d 067c 006a 017c 017c 066a  .D.]L}.|.j.|.|.j
-000006a0: 027c 066a 037c 066a 047c 066a 057c 0364  .|.j.|.j.|.j.|.d
-000006b0: 058d 067d 077c 076a 067c 066a 076b 0273  ...}.|.j.|.j.k.s
-000006c0: 6874 0864 0683 0182 017c 006a 097c 077c  ht.d.....|.j.|.|
-000006d0: 066a 027c 066a 037c 0464 078d 0401 0071  .j.|.j.|.d.....q
-000006e0: 327c 0153 0029 0861 ce01 0000 0a20 2020  2|.S.).a.....   
-000006f0: 2020 2020 2055 7064 6174 6520 696e 7665       Update inve
-00000700: 6e74 6f72 7920 666f 7220 6368 616e 6e65  ntory for channe
-00000710: 6c73 2066 6f75 6e64 2069 6e20 7374 7265  ls found in stre
-00000720: 616d 0a0a 2020 2020 2020 2020 4172 6773  am..        Args
-00000730: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-00000740: 7620 283a 636c 6173 733a 606f 6273 7079  v (:class:`obspy
-00000750: 2e63 6f72 652e 6576 656e 7473 2e69 6e76  .core.events.inv
-00000760: 656e 746f 7279 2e49 6e76 656e 746f 7279  entory.Inventory
-00000770: 6029 3a20 696e 7665 6e74 6f72 790a 2020  `): inventory.  
-00000780: 2020 2020 2020 2020 2020 7374 2028 3a63            st (:c
-00000790: 6c61 7373 3a60 6f62 7370 792e 636f 7265  lass:`obspy.core
-000007a0: 2e73 7472 6561 6d2e 5374 7265 616d 6029  .stream.Stream`)
-000007b0: 3a20 6461 7461 2073 7472 6561 6d20 2875  : data stream (u
-000007c0: 7365 6420 746f 0a20 2020 2020 2020 2020  sed to.         
-000007d0: 2020 2020 2020 2064 6574 6572 6d69 6e65         determine
-000007e0: 206e 6574 2f73 7461 2f63 6861 6e2f 6c6f   net/sta/chan/lo
-000007f0: 6320 636f 6465 7329 2e20 2049 6620 4e6f  c codes).  If No
-00000800: 6e65 2c20 7769 6c6c 2075 7064 6174 650a  ne, will update.
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 6576 6572 7920 6368 616e 6e65 6c0a 2020  every channel.  
-00000830: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
-00000840: 697a 655f 6669 7273 2028 626f 6f6c 293a  ize_firs (bool):
-00000850: 206e 6f72 6d61 6c69 7a65 2046 4952 2063   normalize FIR c
-00000860: 6861 6e6e 656c 7320 7468 6174 2061 7265  hannels that are
-00000870: 6e27 7420 616c 7265 6164 790a 0a20 2020  n't already..   
-00000880: 2020 2020 203a 2072 6574 7572 6e73 3a20       : returns: 
-00000890: 6f62 7370 7920 696e 7665 6e74 6f72 7920  obspy inventory 
-000008a0: 7769 7468 206e 6577 2063 6861 6e6e 656c  with new channel
-000008b0: 730a 2020 2020 2020 2020 4e63 0100 0000  s.        Nc....
-000008c0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000008d0: 5300 0000 7312 0000 0067 007c 005d 0a7d  S...s....g.|.].}
-000008e0: 017c 016a 0091 0271 0453 0072 1200 0000  .|.j...q.S.r....
-000008f0: 2901 da05 7374 6174 73a9 02da 022e 30da  )...stats.....0.
-00000900: 0274 7272 1200 0000 7212 0000 0072 1300  .trr....r....r..
-00000910: 0000 da0a 3c6c 6973 7463 6f6d 703e 5600  ....<listcomp>V.
-00000920: 0000 7304 0000 0006 0002 007a 2e44 6563  ..s........z.Dec
-00000930: 696d 6174 6f72 2e75 7064 6174 655f 696e  imator.update_in
-00000940: 7665 6e74 6f72 792e 3c6c 6f63 616c 733e  ventory.<locals>
-00000950: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
-00000960: 0000 0000 0000 0000 0400 0000 0c00 0000  ................
-00000970: 5300 0000 7342 0000 0067 007c 005d 3a7d  S...sB...g.|.]:}
-00000980: 017c 0144 005d 307d 027c 0244 005d 267d  .|.D.]0}.|.D.]&}
-00000990: 0374 0074 017c 016a 027c 026a 027c 036a  .t.t.|.j.|.j.|.j
-000009a0: 037c 036a 027c 036a 0464 008d 0564 018d  .|.j.|.j.d...d..
-000009b0: 0191 0471 1471 0c71 0453 0029 0229 05da  ...q.q.q.S.).)..
-000009c0: 076e 6574 776f 726b da07 7374 6174 696f  .network..statio
-000009d0: 6eda 086c 6f63 6174 696f 6eda 0763 6861  n..location..cha
-000009e0: 6e6e 656c da0d 7361 6d70 6c69 6e67 5f72  nnel..sampling_r
-000009f0: 6174 6529 01da 0668 6561 6465 7229 0572  ate)...header).r
-00000a00: 0900 0000 da04 6469 6374 da04 636f 6465  ......dict..code
-00000a10: da0d 6c6f 6361 7469 6f6e 5f63 6f64 65da  ..location_code.
-00000a20: 0b73 616d 706c 655f 7261 7465 2904 721c  .sample_rate).r.
-00000a30: 0000 00da 036e 6574 da03 7374 61da 0263  .....net..sta..c
-00000a40: 6872 1200 0000 7212 0000 0072 1300 0000  hr....r....r....
-00000a50: 721e 0000 0058 0000 0073 1c00 0000 060a  r....X...s......
-00000a60: 0201 0600 0201 0600 02f5 0201 0201 0401  ................
-00000a70: 0401 0401 0401 04fb 04ff 2905 721f 0000  ..........).r...
-00000a80: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000a90: da0e 6e6f 726d 616c 697a 655f 6669 7273  ..normalize_firs
-00000aa0: 7a2f 6461 7461 2061 6e64 206d 6574 6164  z/data and metad
-00000ab0: 6174 6120 7361 6d70 6c69 6e67 2072 6174  ata sampling rat
-00000ac0: 6573 2061 7265 2064 6966 6665 7265 6e74  es are different
-00000ad0: 21a9 0372 2900 0000 722a 0000 00da 0571  !..r)...r*.....q
-00000ae0: 7569 6574 290a da04 636f 7079 da12 5f64  uiet)...copy.._d
-00000af0: 7570 6c69 6361 7465 5f63 6861 6e6e 656c  uplicate_channel
-00000b00: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00000b10: 2200 0000 7228 0000 0072 2300 0000 da0a  "...r(...r#.....
-00000b20: 5661 6c75 6545 7272 6f72 da0c 5f6d 6f64  ValueError.._mod
-00000b30: 6966 795f 6368 616e 2908 7211 0000 00da  ify_chan).r.....
-00000b40: 0369 6e76 da02 7374 722c 0000 0072 2e00  .inv..str,...r..
-00000b50: 0000 5a0a 7374 6174 735f 6c69 7374 721a  ..Z.stats_listr.
-00000b60: 0000 00da 076e 6577 5f63 6861 7212 0000  .....new_char...
-00000b70: 0072 1200 0000 7213 0000 00da 1075 7064  .r....r......upd
-00000b80: 6174 655f 696e 7665 6e74 6f72 7945 0000  ate_inventoryE..
-00000b90: 0073 3400 0000 000f 0801 0801 1002 060a  .s4.............
-00000ba0: 02f6 060e 0801 0401 0201 0401 0401 0401  ................
-00000bb0: 0401 02fa 0608 0c01 0201 02ff 0403 0401  ................
-00000bc0: 0200 0400 0400 02ff 0803 7a1a 4465 6369  ..........z.Deci
-00000bd0: 6d61 746f 722e 7570 6461 7465 5f69 6e76  mator.update_inv
-00000be0: 656e 746f 7279 da01 2a63 0800 0000 0000  entory..*c......
-00000bf0: 0000 0000 0000 0e00 0000 0b00 0000 4300  ..............C.
-00000c00: 0000 7374 0000 007c 01a0 00a1 007d 017c  ..st...|.....}.|
-00000c10: 016a 017c 027c 037c 057c 0464 018d 047d  .j.|.|.|.|.d...}
-00000c20: 087c 0844 005d 507d 097c 0944 005d 467d  .|.D.]P}.|.D.]F}
-00000c30: 0a7c 0aa0 00a1 007d 0b7c 0b44 005d 347d  .|.....}.|.D.]4}
-00000c40: 0c7c 006a 027c 017c 096a 037c 0a6a 037c  .|.j.|.|.j.|.j.|
-00000c50: 0c6a 047c 0c6a 037c 0764 028d 067d 0d7c  .j.|.j.|.d...}.|
-00000c60: 006a 057c 0d7c 027c 037c 0664 038d 0401  .j.|.|.|.|.d....
-00000c70: 0071 3671 2671 1e7c 0153 0029 0461 0403  .q6q&q.|.S.).a..
-00000c80: 0000 0a20 2020 2020 2020 2055 7064 6174  ...        Updat
-00000c90: 6520 696e 7665 6e74 6f72 7920 6261 7365  e inventory base
-00000ca0: 6420 6f6e 206e 6574 776f 726b 2c20 7374  d on network, st
-00000cb0: 6174 696f 6e2c 2063 6861 6e6e 656c 2061  ation, channel a
-00000cc0: 6e64 206c 6f63 6174 696f 6e20 636f 6465  nd location code
-00000cd0: 730a 0a20 2020 2020 2020 2041 7267 733a  s..        Args:
-00000ce0: 0a20 2020 2020 2020 2020 2020 2069 6e76  .            inv
-00000cf0: 2028 3a63 6c61 7373 3a60 6f62 7370 792e   (:class:`obspy.
-00000d00: 636f 7265 2e65 7665 6e74 732e 696e 7665  core.events.inve
-00000d10: 6e74 6f72 792e 496e 7665 6e74 6f72 7960  ntory.Inventory`
-00000d20: 293a 2069 6e76 656e 746f 7279 0a20 2020  ): inventory.   
-00000d30: 2020 2020 2020 2020 206e 6574 776f 726b           network
-00000d40: 2028 7374 7229 3a20 4644 534e 206e 6574   (str): FDSN net
-00000d50: 776f 726b 2063 6f64 650a 2020 2020 2020  work code.      
-00000d60: 2020 2020 2020 7374 6174 696f 6e20 2873        station (s
-00000d70: 7472 293a 2073 7461 7469 6f6e 2063 6f64  tr): station cod
-00000d80: 650a 2020 2020 2020 2020 2020 2020 6368  e.            ch
-00000d90: 616e 6e65 6c20 2873 7472 293a 2063 6861  annel (str): cha
-00000da0: 6e6e 656c 2063 6f64 650a 2020 2020 2020  nnel code.      
-00000db0: 2020 2020 2020 6c6f 6361 7469 6f6e 2028        location (
-00000dc0: 7374 7229 3a20 4644 534e 206c 6f63 6174  str): FDSN locat
-00000dd0: 696f 6e20 636f 6465 0a20 2020 2020 2020  ion code.       
-00000de0: 2020 2020 2071 7569 6574 2028 626f 6f6c       quiet (bool
-00000df0: 293a 2044 6f20 6e6f 7420 7361 7920 7768  ): Do not say wh
-00000e00: 6174 2063 6861 6e6e 656c 2873 2920 7761  at channel(s) wa
-00000e10: 7320 6368 616e 6765 640a 2020 2020 2020  s changed.      
-00000e20: 2020 2020 2020 6e6f 726d 616c 697a 655f        normalize_
-00000e30: 6669 7273 2028 626f 6f6c 293a 206e 6f72  firs (bool): nor
-00000e40: 6d61 6c69 7a65 2046 4952 2063 6861 6e6e  malize FIR chann
-00000e50: 6573 6c20 7468 6174 2061 7265 6e27 7420  esl that aren't 
-00000e60: 616c 7265 6164 790a 0a20 2020 2020 2020  already..       
-00000e70: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000e80: 2020 2020 2020 6e65 7769 6e76 3a20 696e        newinv: in
-00000e90: 7620 283a 636c 6173 733a 606f 6273 7079  v (:class:`obspy
-00000ea0: 2e63 6f72 652e 6576 656e 7473 2e69 6e76  .core.events.inv
-00000eb0: 656e 746f 7279 2e49 6e76 656e 746f 7279  entory.Inventory
-00000ec0: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-00000ed0: 2020 2020 7570 6461 7465 6420 696e 7665      updated inve
-00000ee0: 6e74 6f72 790a 0a20 2020 2020 2020 206e  ntory..        n
-00000ef0: 6574 776f 726b 2c20 7374 6174 696f 6e2c  etwork, station,
-00000f00: 2063 6861 6e6e 656c 2061 6e64 206c 6f63   channel and loc
-00000f10: 6174 696f 6e20 636f 6465 7320 6172 6520  ation codes are 
-00000f20: 272a 2720 6279 2064 6566 6175 6c74 2c0a  '*' by default,.
-00000f30: 2020 2020 2020 2020 6d61 7920 696e 636c          may incl
-00000f40: 7564 6520 7769 6c64 6361 7264 7320 6173  ude wildcards as
-00000f50: 2073 7065 6369 6669 6564 2069 6e20 6f62   specified in ob
-00000f60: 7370 792e 636f 7265 2e73 7472 6561 6d2e  spy.core.stream.
-00000f70: 5374 7265 616d 2e73 656c 6563 740a 2020  Stream.select.  
-00000f80: 2020 2020 2020 2904 721f 0000 0072 2000        ).r....r .
-00000f90: 0000 7221 0000 0072 2200 0000 2901 722c  ..r!...r"...).r,
-00000fa0: 0000 0072 2d00 0000 2906 722f 0000 00da  ...r-...).r/....
-00000fb0: 0673 656c 6563 7472 3000 0000 7226 0000  .selectr0...r&..
-00000fc0: 0072 2700 0000 7232 0000 0029 0e72 1100  .r'...r2...).r..
-00000fd0: 0000 7233 0000 0072 1f00 0000 7220 0000  ..r3...r....r ..
-00000fe0: 0072 2200 0000 7221 0000 0072 2e00 0000  .r"...r!...r....
-00000ff0: 722c 0000 005a 0c69 6e76 5f73 656c 6563  r,...Z.inv_selec
-00001000: 7465 6472 2900 0000 722a 0000 005a 076f  tedr)...r*...Z.o
-00001010: 6c64 5f73 7461 da03 6368 6172 3500 0000  ld_sta..char5...
-00001020: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00001030: 1a75 7064 6174 655f 696e 7665 6e74 6f72  .update_inventor
-00001040: 795f 6672 6f6d 5f6e 736c 6378 0000 0073  y_from_nslcx...s
-00001050: 3400 0000 0016 0801 0401 0201 0201 0201  4...............
-00001060: 02fc 0606 0801 0801 0801 0801 0401 0201  ................
-00001070: 0401 0401 0401 0401 02fa 0608 0401 0200  ................
-00001080: 0200 0200 02ff 0c03 7a24 4465 6369 6d61  ........z$Decima
-00001090: 746f 722e 7570 6461 7465 5f69 6e76 656e  tor.update_inven
-000010a0: 746f 7279 5f66 726f 6d5f 6e73 6c63 6302  tory_from_nslcc.
-000010b0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000010c0: 0000 0043 0000 0073 0e01 0000 7400 7c00  ...C...s....t.|.
-000010d0: 8301 6401 6b03 721c 7401 6402 7c00 9b02  ..d.k.r.t.d.|...
-000010e0: 6403 9d03 8301 8201 7c00 6404 6b06 72ae  d.......|.d.k.r.
-000010f0: 7c01 6405 6b05 7230 6406 5300 7c01 6407  |.d.k.r0d.S.|.d.
-00001100: 6b05 723c 6408 5300 7c01 6409 6b05 7248  k.r<d.S.|.d.k.rH
-00001110: 640a 5300 7c01 640b 6b05 7254 640c 5300  d.S.|.d.k.rTd.S.
-00001120: 7c01 6401 6b04 7260 640d 5300 7c01 640e  |.d.k.r`d.S.|.d.
-00001130: 6b04 726c 640f 5300 7c01 6410 6b04 7278  k.rld.S.|.d.k.rx
-00001140: 6411 5300 7c01 6412 6b04 7284 6413 5300  d.S.|.d.k.r.d.S.
-00001150: 7c01 6414 6b05 7290 6415 5300 7c01 6416  |.d.k.r.d.S.|.d.
-00001160: 6b05 729c 6417 5300 7c01 6418 6b05 72a8  k.r.d.S.|.d.k.r.
-00001170: 6419 5300 641a 5300 6e5c 7c00 641b 6b06  d.S.d.S.n\|.d.k.
-00001180: 9000 72fa 7c01 6405 6b05 72c4 641c 5300  ..r.|.d.k.r.d.S.
-00001190: 7c01 6407 6b05 72d0 641d 5300 7c01 6409  |.d.k.r.d.S.|.d.
-000011a0: 6b05 72dc 641e 5300 7c01 640b 6b05 9000  k.r.d.S.|.d.k...
-000011b0: 72ea 641f 5300 7402 a003 6420 a101 0100  r.d.S.t...d ....
-000011c0: 6421 5300 6e10 7404 6422 7c00 9b00 6423  d!S.n.t.d"|...d#
-000011d0: 9d03 8301 8201 6424 5300 2925 7add 0a20  ......d$S.)%z.. 
-000011e0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
-000011f0: 6520 6368 616e 6e65 6c20 6261 6e64 2063  e channel band c
-00001200: 6f64 6520 6261 7365 6420 6f6e 2061 6e20  ode based on an 
-00001210: 696e 7075 7420 6261 6e64 5f63 6f64 650a  input band_code.
-00001220: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001230: 696e 5f62 616e 645f 636f 6465 3a20 696e  in_band_code: in
-00001240: 7075 7420 6261 6e64 2063 6f64 6520 2827  put band code ('
-00001250: 4227 2069 6620 6375 746f 6666 203e 2031  B' if cutoff > 1
-00001260: 3073 2c0a 2020 2020 2020 2020 2020 2020  0s,.            
-00001270: 2753 2720 6f74 6865 7277 6973 6529 0a20  'S' otherwise). 
-00001280: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
-00001290: 6d70 6c65 5f72 6174 653a 2069 6e70 7574  mple_rate: input
-000012a0: 2073 616d 706c 6520 7261 7465 2028 7370   sample rate (sp
-000012b0: 7329 0a20 2020 2020 2020 2072 0c00 0000  s).        r....
-000012c0: 7a0e 2269 6e5f 6261 6e64 5f63 6f64 653d  z."in_band_code=
-000012d0: 7a1c 2220 6973 206d 6f72 6520 7468 616e  z." is more than
-000012e0: 206f 6e65 2063 6861 7261 6374 6572 5a0c   one characterZ.
-000012f0: 4643 4842 4d4c 5655 5250 5451 69e8 0300  FCHBMLVURPTQi...
-00001300: 00da 0146 e9fa 0000 00da 0143 e950 0000  ...F.......C.P..
-00001310: 00da 0148 e90a 0000 00da 0142 da01 4d67  ...H.......B..Mg
-00001320: 3333 3333 3333 d33f da01 4c67 b81e 85eb  333333.?..Lg....
-00001330: 51b8 9e3f da01 5667 fa7e 6abc 7493 683f  Q..?..Vg.~j.t.h?
-00001340: da01 5567 2d43 1ceb e236 1a3f da01 5267  ..Ug-C...6.?..Rg
-00001350: f168 e388 b5f8 e43e da01 5067 8ded b5a0  .h.....>..Pg....
-00001360: f7c6 b03e da01 54da 0151 5a04 4744 4553  ...>..T..QZ.GDES
-00001370: da01 47da 0144 da01 45da 0153 7a28 5368  ..G..D..E..Sz(Sh
-00001380: 6f72 7420 7065 7269 6f64 2073 656e 736f  ort period senso
-00001390: 7220 7361 6d70 6c65 2072 6174 6520 3c20  r sample rate < 
-000013a0: 3130 2073 7073 da01 587a 1955 6e6b 6e6f  10 sps..Xz.Unkno
-000013b0: 776e 2062 616e 6420 6261 7365 2063 6f64  wn band base cod
-000013c0: 653a 2022 fa01 224e 2905 da03 6c65 6e72  e: ".."N)...lenr
-000013d0: 3100 0000 da08 7761 726e 696e 6773 da04  1.....warnings..
-000013e0: 7761 726e 7217 0000 0029 02da 0c69 6e5f  warnr....)...in_
-000013f0: 6261 6e64 5f63 6f64 6572 2800 0000 7212  band_coder(...r.
-00001400: 0000 0072 1200 0000 7213 0000 00da 0d67  ...r....r......g
-00001410: 6574 5f62 616e 645f 636f 6465 a600 0000  et_band_code....
-00001420: 734c 0000 0000 090c 0110 0108 0108 0104  sL..............
-00001430: 0108 0104 0108 0104 0108 0104 0108 0104  ................
-00001440: 0108 0104 0108 0104 0108 0104 0108 0104  ................
-00001450: 0108 0104 0108 0104 0206 010a 0108 0104  ................
-00001460: 0108 0104 0108 0104 010a 0104 020a 0106  ................
-00001470: 027a 1744 6563 696d 6174 6f72 2e67 6574  .z.Decimator.get
-00001480: 5f62 616e 645f 636f 6465 6304 0000 0000  _band_codec.....
-00001490: 0000 0000 0000 0004 0000 0007 0000 0043  ...............C
-000014a0: 0000 0073 3400 0000 7c01 7c00 a000 7c01  ...s4...|.|...|.
-000014b0: 7c02 a102 6b03 7228 7401 a002 6401 7c01  |...k.r(t...d.|.
-000014c0: 9b00 6402 7c02 9b00 6403 9d05 a101 0100  ..d.|...d.......
-000014d0: 7c00 a000 7c01 7c03 a102 5300 2904 7acc  |...|.|...S.).z.
-000014e0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-000014f0: 7468 6520 6368 616e 6e65 6c20 6261 6e64  the channel band
-00001500: 2063 6f64 650a 0a20 2020 2020 2020 203a   code..        :
-00001510: 7061 7261 6d20 696e 5f62 616e 645f 636f  param in_band_co
-00001520: 6465 3a20 696e 7075 7420 6261 6e64 2063  de: input band c
-00001530: 6f64 650a 2020 2020 2020 2020 3a70 6172  ode.        :par
-00001540: 616d 2069 6e5f 7361 6d70 6c65 5f72 6174  am in_sample_rat
-00001550: 653a 2069 6e70 7574 2073 616d 706c 6520  e: input sample 
-00001560: 7261 7465 2028 7370 7329 0a20 2020 2020  rate (sps).     
-00001570: 2020 203a 7061 7261 6d20 6f75 745f 7361     :param out_sa
-00001580: 6d70 6c65 5f72 6174 653a 206f 7574 7075  mple_rate: outpu
-00001590: 7420 7361 6d70 6c65 2072 6174 6520 2873  t sample rate (s
-000015a0: 7073 290a 2020 2020 2020 2020 7a11 496e  ps).        z.In
-000015b0: 7075 7420 6261 6e64 2063 6f64 6520 287a  put band code (z
-000015c0: 2729 2064 6f65 7320 6e6f 7420 6d61 7463  ') does not matc
-000015d0: 6820 2069 6e70 7574 2073 616d 706c 696e  h  input samplin
-000015e0: 6720 7261 7465 2028 fa01 2929 0372 5400  g rate (..)).rT.
-000015f0: 0000 7251 0000 0072 5200 0000 2904 7211  ..rQ...rR...).r.
-00001600: 0000 0072 5300 0000 5a0e 696e 5f73 616d  ...rS...Z.in_sam
-00001610: 706c 655f 7261 7465 5a0f 6f75 745f 7361  ple_rateZ.out_sa
-00001620: 6d70 6c65 5f72 6174 6572 1200 0000 7212  mple_rater....r.
-00001630: 0000 0072 1300 0000 da12 5f67 6574 5f6e  ...r......_get_n
-00001640: 6577 5f62 616e 645f 636f 6465 d900 0000  ew_band_code....
-00001650: 730a 0000 0000 0910 0104 0110 ff04 047a  s..............z
-00001660: 1c44 6563 696d 6174 6f72 2e5f 6765 745f  .Decimator._get_
-00001670: 6e65 775f 6261 6e64 5f63 6f64 65da 0063  new_band_code..c
-00001680: 0600 0000 0000 0000 0000 0000 0700 0000  ................
-00001690: 0900 0000 4300 0000 738e 0000 007c 0564  ....C...s....|.d
-000016a0: 016b 0972 3074 0064 02a0 0164 03a0 027c  .k.r0t.d...d...|
-000016b0: 027c 037c 016a 037c 016a 0467 04a1 017c  .|.|.j.|.j.g...|
-000016c0: 016a 05a1 0264 0464 058d 0201 007c 016a  .j...d.d.....|.j
-000016d0: 057d 067c 00a0 067c 017c 06a1 0201 007c  .}.|...|.|.....|
-000016e0: 00a0 077c 017c 06a1 0201 007c 0104 006a  ...|.|.....|...j
-000016f0: 057c 006a 081d 0002 005f 057c 0564 016b  .|.j....._.|.d.k
-00001700: 0972 8a74 0064 06a0 0164 03a0 027c 027c  .r.t.d...d...|.|
-00001710: 037c 016a 037c 016a 0467 04a1 017c 016a  .|.j.|.j.g...|.j
-00001720: 05a1 0283 0101 0064 0753 0029 0861 9e01  .......d.S.).a..
-00001730: 0000 0a20 2020 2020 2020 206d 6f64 6966  ...        modif
-00001740: 7920 7265 706f 6e73 6520 616e 6420 6e61  y reponse and na
-00001750: 6d65 206f 6620 6120 6368 616e 6e65 6c20  me of a channel 
-00001760: 746f 2063 6f72 7265 7370 6f6e 6420 746f  to correspond to
-00001770: 2064 6563 696d 6174 696f 6e0a 0a20 2020   decimation..   
-00001780: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00001790: 2020 2020 2020 2063 6861 2028 3a63 6c61         cha (:cla
-000017a0: 7373 3a60 6f62 7370 792e 636f 7265 2e69  ss:`obspy.core.i
-000017b0: 6e76 656e 746f 7279 2e63 6861 6e6e 656c  nventory.channel
-000017c0: 6029 3a20 6f72 6967 696e 616c 2063 6861  `): original cha
-000017d0: 6e6e 656c 0a20 2020 2020 2020 2020 2020  nnel.           
-000017e0: 206e 6574 2028 7374 7229 3a20 6e65 7477   net (str): netw
-000017f0: 6f72 6b20 636f 6465 2028 6a75 7374 2066  ork code (just f
-00001800: 6f72 2063 6c65 6172 6572 2070 726f 6772  or clearer progr
-00001810: 6573 7320 7072 696e 746f 7574 290a 2020  ess printout).  
-00001820: 2020 2020 2020 2020 2020 7374 6120 2873            sta (s
-00001830: 7472 293a 2073 7461 7469 6f6e 2063 6f64  tr): station cod
-00001840: 6520 286a 7573 7420 666f 7220 636c 6561  e (just for clea
-00001850: 7265 7220 7072 6f67 7265 7373 2070 7269  rer progress pri
-00001860: 6e74 6f75 7429 0a20 2020 2020 2020 2020  ntout).         
-00001870: 2020 206e 6f72 6d61 6c69 7a65 5f66 6972     normalize_fir
-00001880: 7320 2862 6f6f 6c29 3a20 6e6f 726d 616c  s (bool): normal
-00001890: 697a 6573 2061 6e79 2046 4952 2063 6861  izes any FIR cha
-000018a0: 6e6e 656c 2074 6861 7420 6973 6e27 740a  nnel that isn't.
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 616c 7265 6164 790a 2020 2020 2020 2020  already.        
-000018d0: 547a 2163 6861 6e6e 656c 206d 6f64 6966  Tz!channel modif
-000018e0: 6965 6420 6672 6f6d 207b 7d20 287b 7d20  ied from {} ({} 
-000018f0: 7370 7329 da01 2efa 0120 2901 da03 656e  sps)..... )...en
-00001900: 647a 1074 6f20 7b7d 2028 7b3a 677d 2073  dz.to {} ({:g} s
-00001910: 7073 294e 2909 da05 7072 696e 74da 0666  ps)N)...print..f
-00001920: 6f72 6d61 74da 046a 6f69 6e72 2700 0000  ormat..joinr'...
-00001930: 7226 0000 0072 2800 0000 da0d 5f61 6464  r&...r(....._add
-00001940: 5f72 6573 706f 6e73 65da 105f 6368 616e  _response.._chan
-00001950: 6765 5f63 6861 6e5f 6c6f 6372 1400 0000  ge_chan_locr....
-00001960: 2907 7211 0000 0072 3900 0000 7229 0000  ).r....r9...r)..
-00001970: 0072 2a00 0000 722c 0000 0072 2e00 0000  .r*...r,...r....
-00001980: da11 696e 7075 745f 7361 6d70 6c65 5f72  ..input_sample_r
-00001990: 6174 6572 1200 0000 7212 0000 0072 1300  ater....r....r..
-000019a0: 0000 7232 0000 00e9 0000 0073 2000 0000  ..r2.......s ...
-000019b0: 000c 0801 0601 1401 04fe 0202 02fe 0603  ................
-000019c0: 0601 0c01 0c01 1001 0801 0601 1401 04fe  ................
-000019d0: 7a16 4465 6369 6d61 746f 722e 5f6d 6f64  z.Decimator._mod
-000019e0: 6966 795f 6368 616e 6301 0000 0000 0000  ify_chanc.......
-000019f0: 0000 0000 0002 0000 0006 0000 0003 0000  ................
-00001a00: 0073 3e01 0000 7c00 6a00 6a01 4400 9001  .s>...|.j.j.D...
-00001a10: 5d2e 7d01 7402 7c01 7403 8302 72be 7c01  ].}.t.|.t...r.|.
-00001a20: 6a04 6401 6b02 722e 7405 7c01 6a06 8301  j.d.k.r.t.|.j...
-00001a30: 8900 6e56 7c01 6a04 6402 6b02 7248 6403  ..nV|.j.d.k.rHd.
-00001a40: 7405 7c01 6a06 8301 1400 8900 6e3c 7c01  t.|.j.......n<|.
-00001a50: 6a04 6404 6b02 7274 6403 7405 7c01 6a06  j.d.k.rtd.t.|.j.
-00001a60: 6405 6406 8502 1900 8301 1400 7c01 6a06  d.d.........|.j.
-00001a70: 6406 1900 1700 8900 6e10 7407 6407 7c01  d.......n.t.d.|.
-00001a80: 6a04 9b00 9d02 8301 8201 7408 8800 6408  j.........t...d.
-00001a90: 1800 8301 6409 6b04 72bc 7409 a00a 640a  ....d.k.r.t...d.
-00001aa0: 8800 9b00 640b 9d03 a101 0100 8700 6601  ....d.........f.
-00001ab0: 640c 640d 8408 7c01 6a06 4400 8301 7c01  d.d...|.j.D...|.
-00001ac0: 5f06 7108 7402 7c01 740b 8302 7208 7405  _.q.t.|.t...r.t.
-00001ad0: 7c01 6a0c 8301 640e 6b02 72ec 7405 7c01  |.j...d.k.r.t.|.
-00001ae0: 6a0d 8301 8900 8800 640e 6b02 72ea 7108  j.......d.k.r.q.
-00001af0: 6e14 7405 7c01 6a0d 8301 7405 7c01 6a0c  n.t.|.j...t.|.j.
-00001b00: 8301 1b00 8900 7408 8800 6408 1800 8301  ......t...d.....
-00001b10: 6409 6b04 7208 7409 a00a 640f 8800 9b00  d.k.r.t...d.....
-00001b20: 640b 9d03 a101 0100 8700 6601 6410 640d  d.........f.d.d.
-00001b30: 8408 7c01 6a0d 4400 8301 7c01 5f0d 7108  ..|.j.D...|._.q.
-00001b40: 6405 5300 2911 7aa8 0a20 2020 2020 2020  d.S.).z..       
-00001b50: 2056 6572 6966 6965 7320 262c 2069 6620   Verifies &, if 
-00001b60: 6e65 6564 6564 2c20 6e6f 726d 616c 697a  needed, normaliz
-00001b70: 6573 2063 6861 6e6e 656c 2773 2046 4952  es channel's FIR
-00001b80: 206f 7220 436f 6566 6669 6369 656e 7473   or Coefficients
-00001b90: 2063 6f65 6666 730a 0a20 2020 2020 2020   coeffs..       
-00001ba0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00001bb0: 2020 2063 6861 2028 3a63 6c61 7373 3a60     cha (:class:`
-00001bc0: 6f62 7370 792e 636f 7265 2e69 6e76 656e  obspy.core.inven
-00001bd0: 746f 7279 2e63 6861 6e6e 656c 6029 3a20  tory.channel`): 
-00001be0: 6368 616e 6e65 6c0a 2020 2020 2020 2020  channel.        
-00001bf0: da04 4e4f 4e45 da04 4556 454e e902 0000  ..NONE..EVEN....
-00001c00: 00da 034f 4444 4ee9 ffff ffff 7a22 556e  ...ODDN.....z"Un
-00001c10: 6b6e 6f77 6e20 4649 5220 636f 6566 6669  known FIR coeffi
-00001c20: 6369 656e 7420 7379 6d6d 6574 7279 3a20  cient symmetry: 
-00001c30: 720c 0000 0067 7b14 ae47 e17a 843f 7a1f  r....g{..G.z.?z.
-00001c40: 4445 4349 4d41 544f 523a 2053 756d 206f  DECIMATOR: Sum o
-00001c50: 6620 4649 5220 636f 6566 6673 203d 207a  f FIR coeffs = z
-00001c60: 0d2c 206e 6f72 6d61 6c69 7a69 6e67 6301  ., normalizingc.
-00001c70: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001c80: 0000 0013 0000 0073 1400 0000 6700 7c00  .......s....g.|.
-00001c90: 5d0c 7d01 7c01 8800 1b00 9102 7104 5300  ].}.|.......q.S.
-00001ca0: 7212 0000 0072 1200 0000 a902 721c 0000  r....r......r...
-00001cb0: 00da 0178 a901 5a09 636f 6566 665f 7375  ...x..Z.coeff_su
-00001cc0: 6d72 1200 0000 7213 0000 0072 1e00 0000  mr....r....r....
-00001cd0: 1b01 0000 7304 0000 0006 0102 ff7a 2d44  ....s........z-D
-00001ce0: 6563 696d 6174 6f72 2e5f 6e6f 726d 616c  ecimator._normal
-00001cf0: 697a 655f 6669 7273 2e3c 6c6f 6361 6c73  ize_firs.<locals
-00001d00: 3e2e 3c6c 6973 7463 6f6d 703e 7201 0000  >.<listcomp>r...
-00001d10: 007a 3544 4543 494d 4154 4f52 3a20 7375  .z5DECIMATOR: su
-00001d20: 6d28 6e75 6d65 7261 746f 7220 636f 6566  m(numerator coef
-00001d30: 6673 292f 7375 6d28 6465 6e6f 6d20 636f  fs)/sum(denom co
-00001d40: 6566 6673 2920 3d20 6301 0000 0000 0000  effs) = c.......
-00001d50: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00001d60: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
-00001d70: 8800 1b00 9102 7104 5300 7212 0000 0072  ......q.S.r....r
-00001d80: 1200 0000 7266 0000 0072 6800 0000 7212  ....rf...rh...r.
-00001d90: 0000 0072 1300 0000 721e 0000 0029 0100  ...r....r....)..
-00001da0: 0073 0400 0000 0600 0200 290e da08 7265  .s........)...re
-00001db0: 7370 6f6e 7365 da0f 7265 7370 6f6e 7365  sponse..response
-00001dc0: 5f73 7461 6765 7372 1500 0000 720a 0000  _stagesr....r...
-00001dd0: 00da 0873 796d 6d65 7472 79da 0373 756d  ...symmetry..sum
-00001de0: da0c 636f 6566 6669 6369 656e 7473 7231  ..coefficientsr1
-00001df0: 0000 00da 0361 6273 da07 6c6f 6767 696e  .....abs..loggin
-00001e00: 67da 0469 6e66 6f72 0b00 0000 da0b 6465  g..infor......de
-00001e10: 6e6f 6d69 6e61 746f 72da 096e 756d 6572  nominator..numer
-00001e20: 6174 6f72 2902 7239 0000 005a 0373 7467  ator).r9...Z.stg
-00001e30: 7212 0000 0072 6800 0000 7213 0000 00da  r....rh...r.....
-00001e40: 0f5f 6e6f 726d 616c 697a 655f 6669 7273  ._normalize_firs
-00001e50: 0201 0000 7338 0000 0000 080e 010a 010a  ....s8..........
-00001e60: 010c 010a 0110 010a 021e ff04 0402 010a  ................
-00001e70: ff04 0310 0112 020a 0104 ff0a 020a 010e  ................
-00001e80: 010a 0108 0104 0214 0210 0104 010a ff04  ................
-00001e90: 037a 1944 6563 696d 6174 6f72 2e5f 6e6f  .z.Decimator._no
-00001ea0: 726d 616c 697a 655f 6669 7273 6304 0000  rmalize_firsc...
-00001eb0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00001ec0: 0043 0000 0073 2000 0000 7c00 a000 7c01  .C...s ...|...|.
-00001ed0: 6a01 7c01 6a02 7c02 7c03 a104 5c02 7c01  j.|.j.|.|...\.|.
-00001ee0: 5f01 7c01 5f02 6401 5300 2902 611c 0100  _.|._.d.S.).a...
-00001ef0: 000a 2020 2020 2020 2020 4368 616e 6765  ..        Change
-00001f00: 2063 6861 6e6e 656c 2028 6f72 206c 6f63   channel (or loc
-00001f10: 6174 696f 6e29 2063 6f64 6520 696e 2070  ation) code in p
-00001f20: 6c61 6365 2c20 6163 636f 7264 696e 6720  lace, according 
-00001f30: 746f 2064 6563 696d 6174 696f 6e0a 0a20  to decimation.. 
-00001f40: 2020 2020 2020 2041 7267 756d 656e 7473         Arguments
-00001f50: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-00001f60: 6120 2849 6e76 656e 746f 7279 2e43 6861  a (Inventory.Cha
-00001f70: 6e6e 656c 2920 6368 616e 6e65 6c20 746f  nnel) channel to
-00001f80: 2062 6520 6d6f 6469 6669 6564 2028 696e   be modified (in
-00001f90: 2070 6c61 6365 290a 2020 2020 2020 2020   place).        
-00001fa0: 2020 2020 696e 5f73 7220 2866 6c6f 6174      in_sr (float
-00001fb0: 293a 2069 6e70 7574 2073 616d 706c 6520  ): input sample 
-00001fc0: 7261 7465 0a20 2020 2020 2020 2020 2020  rate.           
-00001fd0: 2061 766f 6964 5f63 6f64 6573 2028 6c69   avoid_codes (li
-00001fe0: 7374 293a 2063 6861 6e6e 656c 3a6c 6f63  st): channel:loc
-00001ff0: 6174 696f 6e20 636f 6465 7320 746f 2061  ation codes to a
-00002000: 766f 6964 0a20 2020 2020 2020 204e 2903  void.        N).
-00002010: da0d 5f67 6574 5f63 6861 6e5f 6c6f 6372  .._get_chan_locr
-00002020: 2600 0000 7227 0000 0029 0472 1100 0000  &...r'...).r....
-00002030: 7239 0000 00da 0569 6e5f 7372 da0b 6176  r9.....in_sr..av
-00002040: 6f69 645f 636f 6465 7372 1200 0000 7212  oid_codesr....r.
-00002050: 0000 0072 1300 0000 725f 0000 002b 0100  ...r....r_...+..
-00002060: 0073 0c00 0000 0009 0401 0400 0400 0200  .s..............
-00002070: 02ff 7a1a 4465 6369 6d61 746f 722e 5f63  ..z.Decimator._c
-00002080: 6861 6e67 655f 6368 616e 5f6c 6f63 6305  hange_chan_locc.
-00002090: 0000 0000 0000 0000 0000 000a 0000 0008  ................
-000020a0: 0000 0043 0000 0073 c600 0000 7c00 6a00  ...C...s....|.j.
-000020b0: 6401 6b02 7212 7401 6402 8301 8201 7c03  d.k.r.t.d.....|.
-000020c0: 7c00 6a00 1b00 7d05 7c00 a002 7c01 6403  |.j...}.|...|.d.
-000020d0: 1900 7c03 7c05 a103 7d06 7c06 7c01 6401  ..|.|...}.|.|.d.
-000020e0: 6404 8502 1900 1700 7d07 7c07 7c01 6b02  d.......}.|.|.k.
-000020f0: 7276 7a14 7403 7c02 8301 6401 1700 6405  rvz.t.|...d...d.
-00002100: 9b04 7d08 5700 717a 0400 7404 6b0a 7272  ..}.W.qz..t.k.rr
-00002110: 0100 0100 0100 6406 7d08 5900 717a 5800  ......d.}.Y.qzX.
-00002120: 6e04 7c02 7d08 7c04 4400 5d3a 7d09 7c07  n.|.}.|.D.]:}.|.
-00002130: 7c09 a005 6407 a101 6403 1900 6b02 727e  |...d...d...k.r~
-00002140: 7c08 7c09 a005 6407 a101 6401 1900 6b02  |.|...d...d...k.
-00002150: 727e 7403 7c08 8301 6401 1700 6405 9b04  r~t.|...d...d...
-00002160: 7d08 717e 717e 71be 717a 7c07 7c08 6602  }.q~q~q.qz|.|.f.
-00002170: 5300 2908 618f 0100 000a 2020 2020 2020  S.).a.....      
-00002180: 2020 4765 7420 6e65 7720 6368 616e 6e65    Get new channe
-00002190: 6c20 286f 7220 6c6f 6329 2063 6f64 6573  l (or loc) codes
-000021a0: 2066 726f 6d20 6f6c 6420 636f 6465 7320   from old codes 
-000021b0: 616e 6420 6465 6369 6d61 7469 6f6e 2066  and decimation f
-000021c0: 6163 746f 720a 0a20 2020 2020 2020 2041  actor..        A
-000021d0: 7267 756d 656e 7473 3a0a 2020 2020 2020  rguments:.      
-000021e0: 2020 2020 2020 6368 615f 636f 6465 3a20        cha_code: 
-000021f0: 696e 7075 7420 6368 616e 6e65 6c20 636f  input channel co
-00002200: 6465 0a20 2020 2020 2020 2020 2020 206c  de.            l
-00002210: 6f63 5f63 6f64 653a 2069 6e70 7574 206c  oc_code: input l
-00002220: 6f63 6174 696f 6e20 636f 6465 0a20 2020  ocation code.   
-00002230: 2020 2020 2020 2020 2069 6e5f 7372 3a20           in_sr: 
-00002240: 696e 7075 7420 7361 6d70 6c69 6e67 2072  input sampling r
-00002250: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-00002260: 6176 6f69 645f 636f 6465 7320 286c 6973  avoid_codes (lis
-00002270: 7429 3a20 6368 616e 6e65 6c3a 6c6f 6361  t): channel:loca
-00002280: 7469 6f6e 2063 6f64 6573 2074 6f20 6176  tion codes to av
-00002290: 6f69 640a 0a20 2020 2020 2020 2052 6574  oid..        Ret
-000022a0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000022b0: 2020 7475 706c 653a 0a20 2020 2020 2020    tuple:.       
-000022c0: 2020 2020 2020 2020 206e 6577 5f63 6861           new_cha
-000022d0: 6e5f 636f 6465 2028 7374 7229 0a20 2020  n_code (str).   
-000022e0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-000022f0: 5f6c 6f63 5f63 6f64 6520 2873 7472 290a  _loc_code (str).
-00002300: 2020 2020 2020 2020 720c 0000 007a 1044          r....z.D
-00002310: 6563 696d 6174 696f 6e20 3d3d 2031 2172  ecimation == 1!r
-00002320: 0100 0000 4eda 0330 3264 5a02 3031 fa01  ....N..02dZ.01..
-00002330: 3a29 0672 1400 0000 7231 0000 0072 5600  :).r....r1...rV.
-00002340: 0000 da03 696e 74da 0945 7863 6570 7469  ....int..Excepti
-00002350: 6f6e da05 7370 6c69 7429 0a72 1100 0000  on..split).r....
-00002360: 5a08 6368 615f 636f 6465 5a08 6c6f 635f  Z.cha_codeZ.loc_
-00002370: 636f 6465 7275 0000 0072 7600 0000 5a06  coderu...rv...Z.
-00002380: 6f75 745f 7372 5a0d 6e65 775f 6261 6e64  out_srZ.new_band
-00002390: 5f63 6f64 655a 0c6e 6577 5f63 6861 5f63  _codeZ.new_cha_c
-000023a0: 6f64 655a 0c6e 6577 5f6c 6f63 5f63 6f64  odeZ.new_loc_cod
-000023b0: 65da 0163 7212 0000 0072 1200 0000 7213  e..cr....r....r.
-000023c0: 0000 0072 7400 0000 3801 0000 7328 0000  ...rt...8...s(..
-000023d0: 0000 0f0a 0108 010a 0112 0110 0108 0202  ................
-000023e0: 0114 010e 010c 0204 0308 0210 ff02 0210  ................
-000023f0: fe02 0410 0104 0104 017a 1744 6563 696d  .........z.Decim
-00002400: 6174 6f72 2e5f 6765 745f 6368 616e 5f6c  ator._get_chan_l
-00002410: 6f63 6303 0000 0000 0000 0000 0000 0007  occ.............
-00002420: 0000 0008 0000 0043 0000 0073 a600 0000  .......C...s....
-00002430: 7c01 6a00 6a01 6401 1900 6a02 7d03 7c00  |.j.j.d...j.}.|.
-00002440: 6a03 4400 5d34 7d04 7404 a005 7c04 a101  j.D.]4}.t...|...
-00002450: 7d05 7c03 6402 3700 7d03 7c01 6a00 6a01  }.|.d.7.}.|.j.j.
-00002460: a006 7c05 a007 7c02 7c03 a102 a101 0100  ..|...|.|.......
-00002470: 7c02 7c04 1d00 7d02 7114 7a0e 7c01 6a00  |.|...}.q.z.|.j.
-00002480: a008 a100 0100 5700 6e48 0400 7409 6b0a  ......W.nH..t.k.
-00002490: 72a0 0100 0100 0100 7c01 6a00 6a0a 6a0b  r.......|.j.j.j.
-000024a0: 7d06 7c06 a00c a100 6403 6b02 729c 6404  }.|.....d.k.r.d.
-000024b0: 7c01 6a00 6a0a 5f0b 7c01 6a00 a008 a100  |.j.j._.|.j.....
-000024c0: 0100 7c06 7c01 6a00 6a0a 5f0b 5900 6e02  ..|.|.j.j._.Y.n.
-000024d0: 5800 6405 5300 2906 7a58 0a20 2020 2020  X.d.S.).zX.     
-000024e0: 2020 2041 7070 656e 6420 2064 6563 696d     Append  decim
-000024f0: 6174 696f 6e20 6f62 6a65 6374 2773 2072  ation object's r
-00002500: 6573 706f 6e73 6520 746f 2061 6e20 6578  esponse to an ex
-00002510: 6973 7469 6e67 2063 6861 6e6e 656c 2773  isting channel's
-00002520: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-00002530: 2020 7265 0000 0072 0c00 0000 da02 5041    re...r......PA
-00002540: 7a03 4d2f 534e 290d 7269 0000 0072 6a00  z.M/SN).ri...rj.
-00002550: 0000 da15 7374 6167 655f 7365 7175 656e  ....stage_sequen
-00002560: 6365 5f6e 756d 6265 7272 0f00 0000 720d  ce_numberr....r.
-00002570: 0000 00da 0866 726f 6d5f 5341 43da 0661  .....from_SAC..a
-00002580: 7070 656e 645a 0874 6f5f 6f62 7370 79da  ppendZ.to_obspy.
-00002590: 1f72 6563 616c 6375 6c61 7465 5f6f 7665  .recalculate_ove
-000025a0: 7261 6c6c 5f73 656e 7369 7469 7669 7479  rall_sensitivity
-000025b0: 727a 0000 00da 1669 6e73 7472 756d 656e  rz.....instrumen
-000025c0: 745f 7365 6e73 6974 6976 6974 79da 0b69  t_sensitivity..i
-000025d0: 6e70 7574 5f75 6e69 7473 da05 7570 7065  nput_units..uppe
-000025e0: 7229 0772 1100 0000 7239 0000 0072 6000  r).r....r9...r`.
-000025f0: 0000 da0c 7374 6167 655f 6e75 6d62 6572  ....stage_number
-00002600: da01 64da 0a66 6972 5f66 696c 7465 72da  ..d..fir_filter.
-00002610: 0369 5f75 7212 0000 0072 1200 0000 7213  .i_ur....r....r.
-00002620: 0000 0072 5e00 0000 6001 0000 7320 0000  ...r^...`...s ..
-00002630: 0000 040e 010a 010a 0108 0108 010a ff04  ................
-00002640: 030a 0102 010e 010e 010a 010c 010a 010a  ................
-00002650: 017a 1744 6563 696d 6174 6f72 2e5f 6164  .z.Decimator._ad
-00002660: 645f 7265 7370 6f6e 7365 6302 0000 0000  d_responsec.....
-00002670: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
-00002680: 0000 0073 6a00 0000 7400 7c01 7401 8302  ...sj...t.|.t...
-00002690: 7312 7402 6401 8301 8201 7c01 a003 a100  s.t.d.....|.....
-000026a0: 7d02 6700 7d03 7c02 6a04 4400 5d14 7d04  }.g.}.|.j.D.].}.
-000026b0: 7c03 a005 7c00 a006 7c04 a101 a101 0100  |...|...|.......
-000026c0: 7124 7c03 7c02 5f04 7c00 6a07 725e 7408  q$|.|._.|.j.r^t.
-000026d0: 6402 a009 6403 6404 8400 7c02 4400 8301  d...d.d...|.D...
-000026e0: a101 8301 0100 7c02 a00a a100 0100 7c02  ......|.......|.
-000026f0: 5300 2905 7a2f 0a20 2020 2020 2020 2052  S.).z/.        R
-00002700: 6574 7572 6e20 6465 6369 6d61 7465 6420  eturn decimated 
-00002710: 6f62 7370 7920 7374 7265 616d 0a20 2020  obspy stream.   
-00002720: 2020 2020 207a 2469 6e70 7574 2073 7472       z$input str
-00002730: 6561 6d20 6973 206e 6f74 2061 6e20 6f62  eam is not an ob
-00002740: 7370 7920 5374 7265 616d 217a 174e 6577  spy Stream!z.New
-00002750: 2064 6174 6120 6861 7320 7b7d 2073 616d   data has {} sam
-00002760: 706c 6573 6301 0000 0000 0000 0000 0000  plesc...........
-00002770: 0002 0000 0003 0000 0053 0000 0073 1400  .........S...s..
-00002780: 0000 6700 7c00 5d0c 7d01 7c01 6a00 6a01  ..g.|.].}.|.j.j.
-00002790: 9102 7104 5300 7212 0000 0029 0272 1800  ..q.S.r....).r..
-000027a0: 0000 da04 7369 7a65 721b 0000 0072 1200  ....sizer....r..
-000027b0: 0000 7212 0000 0072 1300 0000 721e 0000  ..r....r....r...
-000027c0: 0081 0100 0073 0400 0000 0601 02ff 7a29  .....s........z)
-000027d0: 4465 6369 6d61 746f 722e 5f72 756e 5f73  Decimator._run_s
-000027e0: 7472 6561 6d2e 3c6c 6f63 616c 733e 2e3c  tream.<locals>.<
-000027f0: 6c69 7374 636f 6d70 3e29 0b72 1500 0000  listcomp>).r....
-00002800: 7207 0000 0072 3100 0000 722f 0000 00da  r....r1...r/....
-00002810: 0674 7261 6365 7372 8000 0000 da0a 5f72  .tracesr......_r
-00002820: 756e 5f74 7261 6365 7210 0000 0072 5b00  un_tracer....r[.
-00002830: 0000 725c 0000 00da 0676 6572 6966 7929  ..r\.....verify)
-00002840: 0572 1100 0000 da06 7374 7265 616d 7234  .r......streamr4
-00002850: 0000 005a 056e 6577 7472 721d 0000 0072  ...Z.newtrr....r
-00002860: 1200 0000 7212 0000 0072 1300 0000 7216  ....r....r....r.
-00002870: 0000 0075 0100 0073 1a00 0000 0004 0a01  ...u...s........
-00002880: 0801 0801 0401 0a01 1201 0601 0601 0c01  ................
-00002890: 02ff 0a02 0801 7a15 4465 6369 6d61 746f  ......z.Decimato
-000028a0: 722e 5f72 756e 5f73 7472 6561 6d63 0200  r._run_streamc..
-000028b0: 0000 0000 0000 0000 0000 0700 0000 0600  ................
-000028c0: 0000 4300 0000 73c8 0000 0074 007c 0174  ..C...s....t.|.t
-000028d0: 0183 0273 1274 0264 0183 0182 017c 01a0  ...s.t.d.....|..
-000028e0: 03a1 007d 027c 026a 046a 057d 037c 006a  ...}.|.j.j.}.|.j
-000028f0: 0672 4274 0764 02a0 087c 037c 037c 006a  .rBt.d...|.|.|.j
-00002900: 091b 007c 006a 09a1 0383 0101 0074 0aa0  ...|.j.......t..
-00002910: 0aa1 007d 047c 006a 0b44 005d 2a7d 0574  ...}.|.j.D.]*}.t
-00002920: 0ca0 0d7c 05a1 017d 067c 06a0 0e7c 026a  ...|...}.|...|.j
-00002930: 0fa1 017c 025f 0f7c 026a 107c 0564 0364  ...|._.|.j.|.d.d
-00002940: 048d 0201 0071 507c 00a0 117c 026a 046a  .....qP|...|.j.j
-00002950: 127c 026a 046a 137c 026a 046a 057c 006a  .|.j.j.|.j.j.|.j
-00002960: 0914 00a1 035c 027c 026a 045f 127c 026a  .....\.|.j._.|.j
-00002970: 045f 137c 006a 0672 c474 0764 05a0 0874  ._.|.j.r.t.d...t
-00002980: 0aa0 0aa1 007c 0418 00a1 0183 0101 007c  .....|.........|
-00002990: 0253 0029 067a 260a 2020 2020 2020 2020  .S.).z&.        
-000029a0: 4465 6369 6d61 7465 206f 6273 7079 2074  Decimate obspy t
-000029b0: 7261 6365 0a20 2020 2020 2020 207a 2269  race.        z"i
-000029c0: 6e70 7574 2074 7261 6365 2069 7320 6e6f  nput trace is no
-000029d0: 7420 616e 206f 6273 7079 2054 7261 6365  t an obspy Trace
-000029e0: 217a 3044 6563 696d 6174 696e 6720 6461  !z0Decimating da
-000029f0: 7461 2066 726f 6d20 7b3a 677d 2074 6f20  ta from {:g} to 
-00002a00: 7b3a 677d 2048 7a20 287b 3a64 7d78 292e  {:g} Hz ({:d}x).
-00002a10: 2e2e 2054 2901 da09 6e6f 5f66 696c 7465  .. T)...no_filte
-00002a20: 727a 1354 6f6f 6b20 7b3a 2e31 667d 2073  rz.Took {:.1f} s
-00002a30: 6563 6f6e 6473 2914 7215 0000 0072 0800  econds).r....r..
-00002a40: 0000 7231 0000 0072 2f00 0000 721a 0000  ..r1...r/...r...
-00002a50: 0072 2300 0000 7210 0000 0072 5b00 0000  .r#...r....r[...
-00002a60: 725c 0000 0072 1400 0000 da04 7469 6d65  r\...r......time
-00002a70: 720f 0000 0072 0d00 0000 727f 0000 00da  r....r....r.....
-00002a80: 0863 6f6e 766f 6c76 6572 1800 0000 7219  .convolver....r.
-00002a90: 0000 0072 7400 0000 7222 0000 0072 2100  ...rt...r"...r!.
-00002aa0: 0000 2907 7211 0000 00da 0574 7261 6365  ..).r......trace
-00002ab0: 721d 0000 00da 0273 72da 0374 6963 7286  r......sr..ticr.
-00002ac0: 0000 0072 8700 0000 7212 0000 0072 1200  ...r....r....r..
-00002ad0: 0000 7213 0000 0072 8b00 0000 8601 0000  ..r....r........
-00002ae0: 732e 0000 0000 040a 0108 0108 0108 0106  s...............
-00002af0: 0106 0102 0008 0104 fe06 0308 010a 010a  ................
-00002b00: 010e 0110 0104 0106 0106 010c fd10 0406  ................
-00002b10: 0116 017a 1444 6563 696d 6174 6f72 2e5f  ...z.Decimator._
-00002b20: 7275 6e5f 7472 6163 6563 0100 0000 0000  run_tracec......
-00002b30: 0000 0000 0000 0a00 0000 0900 0000 0300  ................
-00002b40: 0000 73f6 0000 0074 0074 0174 0283 0083  ..s....t.t.t....
-00002b50: 0183 01a0 03a1 006a 047d 0164 017c 0064  .......j.}.d.|.d
-00002b60: 029b 049d 027d 027c 01a0 057c 02a1 017d  .....}.|...|...}
-00002b70: 0374 067c 0383 0164 036b 0273 3e74 0764  .t.|...d.k.s>t.d
-00002b80: 0483 0182 0174 087c 0383 018f 5e7d 047c  .....t.|....^}.|
-00002b90: 04a0 09a1 0001 007c 04a0 09a1 00a0 0aa1  .......|........
-00002ba0: 007d 0574 0b7c 0564 0519 0083 0189 0074  .}.t.|.d.......t
-00002bb0: 0c7c 0564 0319 0083 017d 0667 007d 077c  .|.d.....}.g.}.|
-00002bc0: 04a0 0da1 0044 005d 1e7d 087c 0787 0066  .....D.].}.|...f
-00002bd0: 0164 0664 0784 087c 08a0 0aa1 0044 0083  .d.d...|.....D..
-00002be0: 0117 007d 0771 8057 0035 0051 0052 0058  ...}.q.W.5.Q.R.X
-00002bf0: 0074 067c 0783 017c 066b 0273 ca74 0e64  .t.|...|.k.s.t.d
-00002c00: 08a0 0f74 067c 0783 017c 06a1 0283 0182  ...t.|...|......
-00002c10: 0174 067c 0783 0164 0318 007d 097c 0764  .t.|...d...}.|.d
-00002c20: 0964 0564 0985 0319 007c 0717 007d 0774  .d.d.....|...}.t
-00002c30: 107c 077c 0964 0364 0a83 0453 0029 0b7a  .|.|.d.d...S.).z
-00002c40: 2a0a 2020 2020 2020 2020 5265 7475 726e  *.        Return
-00002c50: 7320 6120 5341 4320 4649 5220 6669 6c74  s a SAC FIR filt
-00002c60: 6572 0a20 2020 2020 2020 20da 0364 6563  er.        ..dec
-00002c70: 7286 0000 0072 0c00 0000 7a23 5341 4320  r....r....z#SAC 
-00002c80: 6669 6c74 6572 2066 696c 6520 227b 6662  filter file "{fb
-00002c90: 6173 657d 2220 6e6f 7420 666f 756e 6472  ase}" not foundr
-00002ca0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00002cb0: 0002 0000 0004 0000 0013 0000 0073 1800  .............s..
-00002cc0: 0000 6700 7c00 5d10 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-00002cd0: 8800 1b00 9102 7104 5300 7212 0000 0029  ......q.S.r....)
-00002ce0: 01da 0566 6c6f 6174 7266 0000 00a9 01da  ...floatrf......
-00002cf0: 0764 6976 6973 6f72 7212 0000 0072 1300  .divisorr....r..
-00002d00: 0000 721e 0000 00af 0100 0073 0400 0000  ..r........s....
-00002d10: 0600 0200 7a2b 4465 6369 6d61 746f 722e  ....z+Decimator.
-00002d20: 5f72 6561 645f 4649 525f 5341 432e 3c6c  _read_FIR_SAC.<l
-00002d30: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00002d40: 3e7a 3246 4952 206c 656e 6774 6820 6973  >z2FIR length is
-00002d50: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
-00002d60: 7468 6174 2073 7461 7465 643a 207b 7d20  that stated: {} 
-00002d70: 213d 207b 7d72 6500 0000 7257 0000 0029  != {}re...rW...)
-00002d80: 1172 0500 0000 7203 0000 0072 0400 0000  .r....r....r....
-00002d90: da07 7265 736f 6c76 65da 0670 6172 656e  ..resolve..paren
-00002da0: 74da 0467 6c6f 6272 5000 0000 da09 4e61  t..globrP.....Na
-00002db0: 6d65 4572 726f 72da 046f 7065 6eda 0872  meError..open..r
-00002dc0: 6561 646c 696e 6572 7b00 0000 7295 0000  eadliner{...r...
-00002dd0: 0072 7900 0000 da09 7265 6164 6c69 6e65  .ry.....readline
-00002de0: 73da 0c52 756e 7469 6d65 4572 726f 7272  s..RuntimeErrorr
-00002df0: 5c00 0000 720d 0000 0029 0ada 0a64 6563  \...r....)...dec
-00002e00: 696d 6174 696f 6eda 0862 6173 655f 6469  imation..base_di
-00002e10: 725a 0566 6261 7365 da08 6669 6c65 6e61  rZ.fbase..filena
-00002e20: 6d65 da01 66da 0141 5a07 6e43 6f65 6666  me..f..AZ.nCoeff
-00002e30: 73da 0663 6f65 6666 73da 046c 696e 65da  s..coeffs..line.
-00002e40: 0564 656c 6179 7212 0000 0072 9600 0000  .delayr....r....
-00002e50: 7213 0000 00da 0d5f 7265 6164 5f46 4952  r......_read_FIR
-00002e60: 5f53 4143 9f01 0000 732e 0000 0000 0414  _SAC....s.......
-00002e70: 010c 010a 010c 0108 010a 0108 010c 010c  ................
-00002e80: 010c 0104 010c 0126 010c 0102 0104 0106  .......&........
-00002e90: 0002 ff02 ff04 050c 0112 017a 1744 6563  ...........z.Dec
-00002ea0: 696d 6174 6f72 2e5f 7265 6164 5f46 4952  imator._read_FIR
-00002eb0: 5f53 4143 6307 0000 0000 0000 0000 0000  _SACc...........
-00002ec0: 000d 0000 000a 0000 0043 0000 0073 3001  .........C...s0.
-00002ed0: 0000 6700 7d07 6700 7d08 7c01 6a00 4400  ..g.}.g.}.|.j.D.
-00002ee0: 5d90 7d09 7401 a001 7c09 6a02 a003 a100  ].}.t...|.j.....
-00002ef0: 7c02 a003 a100 a102 732a 710e 7c09 6a04  |.......s*q.|.j.
-00002f00: 4400 5d6c 7d0a 7401 a001 7c0a 6a02 a003  D.]l}.t...|.j...
-00002f10: a100 7c03 a003 a100 a102 734c 7130 7c0a  ..|.......sLq0|.
-00002f20: 6a05 4400 5d48 7d0b 7401 a001 7c0b 6a06  j.D.]H}.t...|.j.
-00002f30: a003 a100 7c04 a003 a100 a102 736e 7152  ....|.......snqR
-00002f40: 7401 a001 7c0b 6a02 a003 a100 7c05 a003  t...|.j.....|...
-00002f50: a100 a102 7386 7152 7c07 a007 7c0a a101  ....s.qR|...|...
-00002f60: 0100 7c08 a007 7c0b a101 0100 7152 7130  ..|...|.....qRq0
-00002f70: 710e 7408 7c07 8301 6401 6b02 72d2 7409  q.t.|...d.k.r.t.
-00002f80: 6402 7c02 9b00 6403 7c03 9b00 6403 7c04  d.|...d.|...d.|.
-00002f90: 9b00 6403 7c05 9b00 6404 9d09 8301 8201  ..d.|...d.......
-00002fa0: 6405 5300 7408 7c07 8301 6406 6b04 72f8  d.S.t.|...d.k.r.
-00002fb0: 7409 6407 a00a 7408 7c07 8301 7c02 7c03  t.d...t.|...|.|.
-00002fc0: 7c04 7c05 a105 8301 8201 7c06 6408 6b08  |.|.......|.d.k.
-00002fd0: 9001 7210 7c00 a00b 7c08 6401 1900 a101  ..r.|...|.d.....
-00002fe0: 0100 7c08 6401 1900 a00c a100 7d0c 7c07  ..|.d.......}.|.
-00002ff0: 6401 1900 6a05 a007 7c0c a101 0100 7c0c  d...j...|.....|.
-00003000: 5300 2909 61c3 0100 000a 2020 2020 2020  S.).a.....      
-00003010: 2020 5265 7475 726e 2053 7461 7469 6f6e    Return Station
-00003020: 2026 2043 6861 6e6e 656c 206d 6174 6368   & Channel match
-00003030: 696e 6720 6e65 7477 6f72 6b2c 2073 7461  ing network, sta
-00003040: 7469 6f6e 2c20 6c6f 6361 7469 6f6e 2c20  tion, location, 
-00003050: 6368 616e 6e65 6c0a 0a20 2020 2020 2020  channel..       
-00003060: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
-00003070: 2020 2020 2020 2020 6e65 7477 6f72 6b20          network 
-00003080: 2873 7472 293a 206e 6574 776f 726b 2063  (str): network c
-00003090: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
-000030a0: 7374 6174 696f 6e20 2873 7472 293a 2073  station (str): s
-000030b0: 7461 7469 6f6e 2063 6f64 650a 2020 2020  tation code.    
-000030c0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-000030d0: 2028 7374 7229 3a20 6c6f 6361 7469 6f6e   (str): location
-000030e0: 2063 6f64 650a 2020 2020 2020 2020 2020   code.          
-000030f0: 2020 6368 616e 6e65 6c20 2873 7472 293a    channel (str):
-00003100: 2063 6861 6e6e 656c 2063 6f64 650a 2020   channel code.  
-00003110: 2020 2020 2020 2020 2020 6e6f 726d 616c            normal
-00003120: 697a 655f 6669 7273 2028 626f 6f6c 293a  ize_firs (bool):
-00003130: 206e 6f72 6d61 6c69 7a65 7320 616e 7920   normalizes any 
-00003140: 4649 5220 6368 616e 6e65 6c20 7468 6174  FIR channel that
-00003150: 2069 736e 2774 0a20 2020 2020 2020 2020   isn't.         
-00003160: 2020 2020 2020 2061 6c72 6561 6479 0a0a         already..
-00003170: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00003180: 0a20 2020 2020 2020 2020 2020 2028 4368  .            (Ch
-00003190: 616e 6e65 6c29 3a20 6475 706c 6963 6174  annel): duplicat
-000031a0: 6520 6f66 2066 6f75 6e64 2063 6861 6e6e  e of found chann
-000031b0: 656c 2c20 7265 6164 7920 746f 206d 6f64  el, ready to mod
-000031c0: 6966 790a 2020 2020 2020 2020 7201 0000  ify.        r...
-000031d0: 007a 1274 7261 6365 2077 6176 6566 6f72  .z.trace wavefor
-000031e0: 6d69 6420 2272 5800 0000 7a18 2220 6e6f  mid "rX...z." no
-000031f0: 7420 666f 756e 6420 696e 2069 6e76 656e  t found in inven
-00003200: 746f 7279 2902 4e4e 720c 0000 007a 297b  tory).NNr....z){
-00003210: 3a64 7d20 7374 6174 696f 6e2d 6368 616e  :d} station-chan
-00003220: 6e65 6c73 206d 6174 6368 6564 207b 7d2e  nels matched {}.
-00003230: 7b7d 2e7b 7d2e 7b7d 5429 0dda 086e 6574  {}.{}.{}T)...net
-00003240: 776f 726b 73da 0766 6e6d 6174 6368 7226  works..fnmatchr&
-00003250: 0000 0072 8400 0000 da08 7374 6174 696f  ...r......statio
-00003260: 6e73 da08 6368 616e 6e65 6c73 7227 0000  ns..channelsr'..
-00003270: 0072 8000 0000 7250 0000 0072 3100 0000  .r....rP...r1...
-00003280: 725c 0000 0072 7300 0000 722f 0000 0029  r\...rs...r/...)
-00003290: 0d72 1100 0000 7233 0000 0072 1f00 0000  .r....r3...r....
-000032a0: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-000032b0: 2c00 0000 72ab 0000 0072 ac00 0000 7229  ,...r....r....r)
-000032c0: 0000 0072 2a00 0000 7239 0000 0072 3500  ...r*...r9...r5.
-000032d0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000032e0: 0072 3000 0000 bc01 0000 7348 0000 0000  .r0.......sH....
-000032f0: 1104 0104 010a 0216 0102 010a 0116 0102  ................
-00003300: 010a 0104 0108 0006 ff04 0302 0116 0102  ................
-00003310: 010a 0110 010c 0122 0204 010c 0102 0104  ......."........
-00003320: 0106 0002 0002 0002 0002 ff02 ff04 050a  ................
-00003330: 010e 010c 0110 017a 1c44 6563 696d 6174  .......z.Decimat
-00003340: 6f72 2e5f 6475 706c 6963 6174 655f 6368  or._duplicate_ch
-00003350: 616e 6e65 6c29 034e 4646 2906 7237 0000  annel).NFF).r7..
-00003360: 0072 3700 0000 7237 0000 0072 3700 0000  .r7...r7...r7...
-00003370: 4646 2904 7257 0000 0072 5700 0000 4646  FF).rW...rW...FF
-00003380: 2901 4629 19da 085f 5f6e 616d 655f 5fda  ).F)...__name__.
-00003390: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000033a0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
-000033b0: 5f5f da04 6c69 7374 da0f 5f5f 616e 6e6f  __..list..__anno
-000033c0: 7461 7469 6f6e 735f 5f72 1000 0000 da04  tations__r......
-000033d0: 626f 6f6c da08 7072 6f70 6572 7479 7214  bool..propertyr.
-000033e0: 0000 0072 1900 0000 7236 0000 0072 3a00  ...r....r6...r:.
-000033f0: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-00003400: 7254 0000 0072 5600 0000 7232 0000 0072  rT...rV...r2...r
-00003410: 7300 0000 725f 0000 0072 7400 0000 725e  s...r_...rt...r^
-00003420: 0000 0072 1600 0000 728b 0000 0072 a800  ...r....r....r..
-00003430: 0000 7230 0000 0072 1200 0000 7212 0000  ..r0...r....r...
-00003440: 0072 1200 0000 7213 0000 0072 0e00 0000  .r....r....r....
-00003450: 2300 0000 7340 0000 000a 0204 0a08 010c  #...s@..........
-00003460: 0202 010a 0408 0f00 0000 0000 ff0a 3300  ..............3.
-00003470: 0100 0000 0000 0100 fe0a 2e02 010a 3208  ..............2.
-00003480: 1000 0100 ff0a 1902 010a 280c 0d0c 2808  ..........(...(.
-00003490: 1508 1108 1908 1e00 ff72 0e00 0000 2919  .........r....).
-000034a0: 72b0 0000 0072 8f00 0000 da0b 6461 7461  r....r......data
-000034b0: 636c 6173 7365 7372 0200 0000 da07 696e  classesr......in
-000034c0: 7370 6563 7472 0300 0000 7204 0000 00da  spectr....r.....
-000034d0: 0770 6174 686c 6962 7205 0000 0072 5100  .pathlibr....rQ.
-000034e0: 0000 72aa 0000 0072 6f00 0000 da05 6e75  ..r....ro.....nu
-000034f0: 6d70 7972 0600 0000 da11 6f62 7370 792e  mpyr......obspy.
-00003500: 636f 7265 2e73 7472 6561 6d72 0700 0000  core.streamr....
-00003510: 7208 0000 00da 106f 6273 7079 2e63 6f72  r......obspy.cor
-00003520: 652e 7472 6163 6572 0900 0000 da14 6f62  e.tracer......ob
-00003530: 7370 792e 636f 7265 2e69 6e76 656e 746f  spy.core.invento
-00003540: 7279 720a 0000 0072 0b00 0000 7287 0000  ryr....r....r...
-00003550: 0072 0d00 0000 720e 0000 0072 1200 0000  .r....r....r....
-00003560: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00003570: 083c 6d6f 6475 6c65 3e02 0000 0073 1c00  .<module>....s..
-00003580: 0000 0410 0801 0c01 1001 0c01 0801 0801  ................
-00003590: 0802 0c01 1001 0c01 1003 0c03 0201       ..............
+000001d0: 0065 0864 0564 0684 0083 015a 0964 2764  .e.d.d.....Z.d'd
+000001e0: 0864 0984 015a 0a64 2864 0b64 0c84 015a  .d...Z.d(d.d...Z
+000001f0: 0b64 2964 0e64 0f84 015a 0c65 0d64 1064  .d)d.d...Z.e.d.d
+00000200: 1184 0083 015a 0e64 1264 1384 005a 0f64  .....Z.d.d...Z.d
+00000210: 2a64 1564 1684 015a 1065 0d64 1764 1884  *d.d...Z.e.d.d..
+00000220: 0083 015a 1167 0066 0164 1964 1a84 015a  ...Z.g.f.d.d...Z
+00000230: 1267 0066 0164 1b64 1c84 015a 1364 1d64  .g.f.d.d...Z.d.d
+00000240: 1e84 005a 1464 1f64 2084 005a 1564 2164  ...Z.d.d ..Z.d!d
+00000250: 2284 005a 1664 2364 2484 005a 1764 2b64  "..Z.d#d$..Z.d+d
+00000260: 2564 2684 015a 1864 0a53 0029 2cda 0944  %d&..Z.d.S.),..D
+00000270: 6563 696d 6174 6f72 6136 0100 000a 2020  ecimatora6....  
+00000280: 2020 436c 6173 7320 746f 2064 6563 696d    Class to decim
+00000290: 6174 6520 6f62 7370 7920 7374 7265 616d  ate obspy stream
+000002a0: 2069 6e74 656c 6c69 6765 6e74 790a 0a20   intelligenty.. 
+000002b0: 2020 2043 616e 2061 6c73 6f20 7570 6461     Can also upda
+000002c0: 7465 2074 6865 2073 7461 7469 6f6e 2069  te the station i
+000002d0: 6e76 656e 746f 7279 2077 6974 6820 7468  nventory with th
+000002e0: 6520 7573 6564 2066 696c 7465 7220 7265  e used filter re
+000002f0: 7370 6f6e 7365 730a 0a20 2020 2041 7267  sponses..    Arg
+00000300: 733a 0a20 2020 2020 2020 2064 6563 696d  s:.        decim
+00000310: 6174 6573 2028 6c69 7374 293a 206c 6973  ates (list): lis
+00000320: 7420 6f66 2064 6563 696d 6174 696f 6e20  t of decimation 
+00000330: 6661 6374 6f72 7374 2074 6f20 7573 6520  factorst to use 
+00000340: 2869 6e74 6567 6572 7320 6265 7477 6565  (integers betwee
+00000350: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00000360: 2020 2020 2020 2020 2020 3220 616e 6420            2 and 
+00000370: 372c 2077 696c 6c20 6265 2061 7070 6c69  7, will be appli
+00000380: 6564 2069 6e20 6f72 6465 7229 0a20 2020  ed in order).   
+00000390: 2020 2020 2076 6572 626f 7365 2028 626f       verbose (bo
+000003a0: 6f6c 293a 2042 6520 6368 6174 7479 0a20  ol): Be chatty. 
+000003b0: 2020 20da 0964 6563 696d 6174 6573 46da     ..decimatesF.
+000003c0: 0776 6572 626f 7365 6301 0000 0000 0000  .verbosec.......
+000003d0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+000003e0: 0073 0a00 0000 7400 7c00 6a01 8301 5300  .s....t.|.j...S.
+000003f0: 2901 7a29 546f 7461 6c20 6465 6369 6d61  ).z)Total decima
+00000400: 7469 6f6e 2028 7072 6f64 7563 7420 6f66  tion (product of
+00000410: 2060 6465 6369 6d61 7465 7360 2929 0272   `decimates`)).r
+00000420: 0600 0000 720f 0000 0029 01da 0473 656c  ....r....)...sel
+00000430: 66a9 0072 1200 0000 fa45 2f55 7365 7273  f..r.....E/Users
+00000440: 2f63 7261 7766 6f72 642f 5f57 6f72 6b2f  /crawford/_Work/
+00000450: 5072 6f67 7261 6d6d 696e 672f 7469 736b  Programming/tisk
+00000460: 6974 2f74 6973 6b69 742f 6465 6369 6d61  it/tiskit/decima
+00000470: 7465 2f64 6563 696d 6174 6f72 2e70 79da  te/decimator.py.
+00000480: 1164 6563 696d 6174 696f 6e5f 6661 6374  .decimation_fact
+00000490: 6f72 3200 0000 7302 0000 0000 037a 1b44  or2...s......z.D
+000004a0: 6563 696d 6174 6f72 2e64 6563 696d 6174  ecimator.decimat
+000004b0: 696f 6e5f 6661 6374 6f72 5463 0300 0000  ion_factorTc....
+000004c0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+000004d0: 4300 0000 733a 0000 007c 027c 005f 0074  C...s:...|.|._.t
+000004e0: 017c 0174 0283 0272 1a7c 00a0 037c 01a1  .|.t...r.|...|..
+000004f0: 0153 0074 017c 0174 0483 0272 2e7c 00a0  .S.t.|.t...r.|..
+00000500: 057c 01a1 0153 0074 0664 0183 0182 0164  .|...S.t.d.....d
+00000510: 0253 0029 037a fa0a 2020 2020 2020 2020  .S.).z..        
+00000520: 4170 706c 7920 6465 6369 6d61 746f 7220  Apply decimator 
+00000530: 746f 2064 6174 610a 0a20 2020 2020 2020  to data..       
+00000540: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000550: 2020 2064 6174 6120 283a 636c 6173 733a     data (:class:
+00000560: 606f 6273 7079 2e53 7472 6561 6d60 206f  `obspy.Stream` o
+00000570: 7220 3a63 6c61 7373 3a60 6f62 7370 792e  r :class:`obspy.
+00000580: 5472 6163 6560 293a 2077 6176 6566 6f72  Trace`): wavefor
+00000590: 6d20 6461 7461 0a20 2020 2020 2020 2020  m data.         
+000005a0: 2020 206b 6565 705f 6466 6f72 6d61 7420     keep_dformat 
+000005b0: 2862 6f6f 6c29 3a20 666f 7263 6520 6f75  (bool): force ou
+000005c0: 7470 7574 2064 6174 6120 666f 726d 6174  tput data format
+000005d0: 2074 6f20 6265 2074 6865 2073 616d 6520   to be the same 
+000005e0: 6173 0a20 2020 2020 2020 2020 2020 2020  as.             
+000005f0: 2020 2074 6865 2069 6e70 7574 2064 6174     the input dat
+00000600: 615f 666f 726d 6174 0a20 2020 2020 2020  a_format.       
+00000610: 207a 1d64 6174 6120 6973 206e 6f74 2061   z.data is not a
+00000620: 2053 7472 6561 6d20 6f72 2054 7261 6365   Stream or Trace
+00000630: 4e29 07da 0a6b 6565 705f 6474 7970 65da  N)...keep_dtype.
+00000640: 0a69 7369 6e73 7461 6e63 6572 0700 0000  .isinstancer....
+00000650: da0b 5f72 756e 5f73 7472 6561 6d72 0800  .._run_streamr..
+00000660: 0000 da0a 5f72 756e 5f74 7261 6365 da09  ...._run_trace..
+00000670: 5479 7065 4572 726f 7229 0372 1100 0000  TypeError).r....
+00000680: da04 6461 7461 7215 0000 0072 1200 0000  ..datar....r....
+00000690: 7212 0000 0072 1300 0000 da08 6465 6369  r....r......deci
+000006a0: 6d61 7465 3700 0000 730c 0000 0000 0906  mate7...s.......
+000006b0: 010a 010a 010a 010a 027a 1244 6563 696d  .........z.Decim
+000006c0: 6174 6f72 2e64 6563 696d 6174 654e 6305  ator.decimateNc.
+000006d0: 0000 0000 0000 0000 0000 0008 0000 0009  ................
+000006e0: 0000 0043 0000 0073 8400 0000 7c01 a000  ...C...s....|...
+000006f0: a100 7d01 7c02 6401 6b09 7220 6402 6403  ..}.|.d.k.r d.d.
+00000700: 8400 7c02 4400 8301 7d05 6e0e 6404 6403  ..|.D...}.n.d.d.
+00000710: 8400 7c01 4400 8301 7d05 7c05 4400 5d4c  ..|.D...}.|.D.]L
+00000720: 7d06 7c00 6a01 7c01 7c06 6a02 7c06 6a03  }.|.j.|.|.j.|.j.
+00000730: 7c06 6a04 7c06 6a05 7c03 6405 8d06 7d07  |.j.|.j.|.d...}.
+00000740: 7c07 6a06 7c06 6a07 6b02 7368 7408 6406  |.j.|.j.k.sht.d.
+00000750: 8301 8201 7c00 6a09 7c07 7c06 6a02 7c06  ....|.j.|.|.j.|.
+00000760: 6a03 7c04 6407 8d04 0100 7132 7c01 5300  j.|.d.....q2|.S.
+00000770: 2908 61ce 0100 000a 2020 2020 2020 2020  ).a.....        
+00000780: 5570 6461 7465 2069 6e76 656e 746f 7279  Update inventory
+00000790: 2066 6f72 2063 6861 6e6e 656c 7320 666f   for channels fo
+000007a0: 756e 6420 696e 2073 7472 6561 6d0a 0a20  und in stream.. 
+000007b0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000007c0: 2020 2020 2020 2020 2069 6e76 2028 3a63           inv (:c
+000007d0: 6c61 7373 3a60 6f62 7370 792e 636f 7265  lass:`obspy.core
+000007e0: 2e65 7665 6e74 732e 696e 7665 6e74 6f72  .events.inventor
+000007f0: 792e 496e 7665 6e74 6f72 7960 293a 2069  y.Inventory`): i
+00000800: 6e76 656e 746f 7279 0a20 2020 2020 2020  nventory.       
+00000810: 2020 2020 2073 7420 283a 636c 6173 733a       st (:class:
+00000820: 606f 6273 7079 2e63 6f72 652e 7374 7265  `obspy.core.stre
+00000830: 616d 2e53 7472 6561 6d60 293a 2064 6174  am.Stream`): dat
+00000840: 6120 7374 7265 616d 2028 7573 6564 2074  a stream (used t
+00000850: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+00000860: 2020 6465 7465 726d 696e 6520 6e65 742f    determine net/
+00000870: 7374 612f 6368 616e 2f6c 6f63 2063 6f64  sta/chan/loc cod
+00000880: 6573 292e 2020 4966 204e 6f6e 652c 2077  es).  If None, w
+00000890: 696c 6c20 7570 6461 7465 0a20 2020 2020  ill update.     
+000008a0: 2020 2020 2020 2020 2020 2065 7665 7279             every
+000008b0: 2063 6861 6e6e 656c 0a20 2020 2020 2020   channel.       
+000008c0: 2020 2020 206e 6f72 6d61 6c69 7a65 5f66       normalize_f
+000008d0: 6972 7320 2862 6f6f 6c29 3a20 6e6f 726d  irs (bool): norm
+000008e0: 616c 697a 6520 4649 5220 6368 616e 6e65  alize FIR channe
+000008f0: 6c73 2074 6861 7420 6172 656e 2774 2061  ls that aren't a
+00000900: 6c72 6561 6479 0a0a 2020 2020 2020 2020  lready..        
+00000910: 3a20 7265 7475 726e 733a 206f 6273 7079  : returns: obspy
+00000920: 2069 6e76 656e 746f 7279 2077 6974 6820   inventory with 
+00000930: 6e65 7720 6368 616e 6e65 6c73 0a20 2020  new channels.   
+00000940: 2020 2020 204e 6301 0000 0000 0000 0000       Nc.........
+00000950: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00000960: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
+00000970: 9102 7104 5300 7212 0000 0029 01da 0573  ..q.S.r....)...s
+00000980: 7461 7473 a902 da02 2e30 da02 7472 7212  tats.....0..trr.
+00000990: 0000 0072 1200 0000 7213 0000 00da 0a3c  ...r....r......<
+000009a0: 6c69 7374 636f 6d70 3e59 0000 0073 0400  listcomp>Y...s..
+000009b0: 0000 0600 0200 7a2e 4465 6369 6d61 746f  ......z.Decimato
+000009c0: 722e 7570 6461 7465 5f69 6e76 656e 746f  r.update_invento
+000009d0: 7279 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ry.<locals>.<lis
+000009e0: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
+000009f0: 0000 0004 0000 000c 0000 0053 0000 0073  ...........S...s
+00000a00: 4200 0000 6700 7c00 5d3a 7d01 7c01 4400  B...g.|.]:}.|.D.
+00000a10: 5d30 7d02 7c02 4400 5d26 7d03 7400 7401  ]0}.|.D.]&}.t.t.
+00000a20: 7c01 6a02 7c02 6a02 7c03 6a03 7c03 6a02  |.j.|.j.|.j.|.j.
+00000a30: 7c03 6a04 6400 8d05 6401 8d01 9104 7114  |.j.d...d.....q.
+00000a40: 710c 7104 5300 2902 2905 da07 6e65 7477  q.q.S.).)...netw
+00000a50: 6f72 6bda 0773 7461 7469 6f6e da08 6c6f  ork..station..lo
+00000a60: 6361 7469 6f6e da07 6368 616e 6e65 6cda  cation..channel.
+00000a70: 0d73 616d 706c 696e 675f 7261 7465 2901  .sampling_rate).
+00000a80: da06 6865 6164 6572 2905 7209 0000 00da  ..header).r.....
+00000a90: 0464 6963 74da 0463 6f64 65da 0d6c 6f63  .dict..code..loc
+00000aa0: 6174 696f 6e5f 636f 6465 da0b 7361 6d70  ation_code..samp
+00000ab0: 6c65 5f72 6174 6529 0472 1e00 0000 da03  le_rate).r......
+00000ac0: 6e65 74da 0373 7461 da02 6368 7212 0000  net..sta..chr...
+00000ad0: 0072 1200 0000 7213 0000 0072 2000 0000  .r....r....r ...
+00000ae0: 5b00 0000 731c 0000 0006 0a02 0106 0002  [...s...........
+00000af0: 0106 0002 f502 0102 0104 0104 0104 0104  ................
+00000b00: 0104 fb04 ff29 0572 2100 0000 7222 0000  .....).r!...r"..
+00000b10: 0072 2300 0000 7224 0000 00da 0e6e 6f72  .r#...r$.....nor
+00000b20: 6d61 6c69 7a65 5f66 6972 737a 2f64 6174  malize_firsz/dat
+00000b30: 6120 616e 6420 6d65 7461 6461 7461 2073  a and metadata s
+00000b40: 616d 706c 696e 6720 7261 7465 7320 6172  ampling rates ar
+00000b50: 6520 6469 6666 6572 656e 7421 a903 722b  e different!..r+
+00000b60: 0000 0072 2c00 0000 da05 7175 6965 7429  ...r,.....quiet)
+00000b70: 0ada 0463 6f70 79da 125f 6475 706c 6963  ...copy.._duplic
+00000b80: 6174 655f 6368 616e 6e65 6c72 2100 0000  ate_channelr!...
+00000b90: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00000ba0: 2a00 0000 7225 0000 00da 0a56 616c 7565  *...r%.....Value
+00000bb0: 4572 726f 72da 0c5f 6d6f 6469 6679 5f63  Error.._modify_c
+00000bc0: 6861 6e29 0872 1100 0000 da03 696e 76da  han).r......inv.
+00000bd0: 0273 7472 2e00 0000 7230 0000 005a 0a73  .str....r0...Z.s
+00000be0: 7461 7473 5f6c 6973 7472 1c00 0000 da07  tats_listr......
+00000bf0: 6e65 775f 6368 6172 1200 0000 7212 0000  new_char....r...
+00000c00: 0072 1300 0000 da10 7570 6461 7465 5f69  .r......update_i
+00000c10: 6e76 656e 746f 7279 4800 0000 7334 0000  nventoryH...s4..
+00000c20: 0000 0f08 0108 0110 0206 0a02 f606 0e08  ................
+00000c30: 0104 0102 0104 0104 0104 0104 0102 fa06  ................
+00000c40: 080c 0102 0102 ff04 0304 0102 0004 0004  ................
+00000c50: 0002 ff08 037a 1a44 6563 696d 6174 6f72  .....z.Decimator
+00000c60: 2e75 7064 6174 655f 696e 7665 6e74 6f72  .update_inventor
+00000c70: 79da 012a 6308 0000 0000 0000 0000 0000  y..*c...........
+00000c80: 000e 0000 000b 0000 0043 0000 0073 7400  .........C...st.
+00000c90: 0000 7c01 a000 a100 7d01 7c01 6a01 7c02  ..|.....}.|.j.|.
+00000ca0: 7c03 7c05 7c04 6401 8d04 7d08 7c08 4400  |.|.|.d...}.|.D.
+00000cb0: 5d50 7d09 7c09 4400 5d46 7d0a 7c0a a000  ]P}.|.D.]F}.|...
+00000cc0: a100 7d0b 7c0b 4400 5d34 7d0c 7c00 6a02  ..}.|.D.]4}.|.j.
+00000cd0: 7c01 7c09 6a03 7c0a 6a03 7c0c 6a04 7c0c  |.|.j.|.j.|.j.|.
+00000ce0: 6a03 7c07 6402 8d06 7d0d 7c00 6a05 7c0d  j.|.d...}.|.j.|.
+00000cf0: 7c02 7c03 7c06 6403 8d04 0100 7136 7126  |.|.|.d.....q6q&
+00000d00: 711e 7c01 5300 2904 6104 0300 000a 2020  q.|.S.).a.....  
+00000d10: 2020 2020 2020 5570 6461 7465 2069 6e76        Update inv
+00000d20: 656e 746f 7279 2062 6173 6564 206f 6e20  entory based on 
+00000d30: 6e65 7477 6f72 6b2c 2073 7461 7469 6f6e  network, station
+00000d40: 2c20 6368 616e 6e65 6c20 616e 6420 6c6f  , channel and lo
+00000d50: 6361 7469 6f6e 2063 6f64 6573 0a0a 2020  cation codes..  
+00000d60: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00000d70: 2020 2020 2020 2020 696e 7620 283a 636c          inv (:cl
+00000d80: 6173 733a 606f 6273 7079 2e63 6f72 652e  ass:`obspy.core.
+00000d90: 6576 656e 7473 2e69 6e76 656e 746f 7279  events.inventory
+00000da0: 2e49 6e76 656e 746f 7279 6029 3a20 696e  .Inventory`): in
+00000db0: 7665 6e74 6f72 790a 2020 2020 2020 2020  ventory.        
+00000dc0: 2020 2020 6e65 7477 6f72 6b20 2873 7472      network (str
+00000dd0: 293a 2046 4453 4e20 6e65 7477 6f72 6b20  ): FDSN network 
+00000de0: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
+00000df0: 2073 7461 7469 6f6e 2028 7374 7229 3a20   station (str): 
+00000e00: 7374 6174 696f 6e20 636f 6465 0a20 2020  station code.   
+00000e10: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+00000e20: 2028 7374 7229 3a20 6368 616e 6e65 6c20   (str): channel 
+00000e30: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
+00000e40: 206c 6f63 6174 696f 6e20 2873 7472 293a   location (str):
+00000e50: 2046 4453 4e20 6c6f 6361 7469 6f6e 2063   FDSN location c
+00000e60: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+00000e70: 7175 6965 7420 2862 6f6f 6c29 3a20 446f  quiet (bool): Do
+00000e80: 206e 6f74 2073 6179 2077 6861 7420 6368   not say what ch
+00000e90: 616e 6e65 6c28 7329 2077 6173 2063 6861  annel(s) was cha
+00000ea0: 6e67 6564 0a20 2020 2020 2020 2020 2020  nged.           
+00000eb0: 206e 6f72 6d61 6c69 7a65 5f66 6972 7320   normalize_firs 
+00000ec0: 2862 6f6f 6c29 3a20 6e6f 726d 616c 697a  (bool): normaliz
+00000ed0: 6520 4649 5220 6368 616e 6e65 736c 2074  e FIR channesl t
+00000ee0: 6861 7420 6172 656e 2774 2061 6c72 6561  hat aren't alrea
+00000ef0: 6479 0a0a 2020 2020 2020 2020 5265 7475  dy..        Retu
+00000f00: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00000f10: 206e 6577 696e 763a 2069 6e76 2028 3a63   newinv: inv (:c
+00000f20: 6c61 7373 3a60 6f62 7370 792e 636f 7265  lass:`obspy.core
+00000f30: 2e65 7665 6e74 732e 696e 7665 6e74 6f72  .events.inventor
+00000f40: 792e 496e 7665 6e74 6f72 7960 293a 0a20  y.Inventory`):. 
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00000f60: 7064 6174 6564 2069 6e76 656e 746f 7279  pdated inventory
+00000f70: 0a0a 2020 2020 2020 2020 6e65 7477 6f72  ..        networ
+00000f80: 6b2c 2073 7461 7469 6f6e 2c20 6368 616e  k, station, chan
+00000f90: 6e65 6c20 616e 6420 6c6f 6361 7469 6f6e  nel and location
+00000fa0: 2063 6f64 6573 2061 7265 2027 2a27 2062   codes are '*' b
+00000fb0: 7920 6465 6661 756c 742c 0a20 2020 2020  y default,.     
+00000fc0: 2020 206d 6179 2069 6e63 6c75 6465 2077     may include w
+00000fd0: 696c 6463 6172 6473 2061 7320 7370 6563  ildcards as spec
+00000fe0: 6966 6965 6420 696e 206f 6273 7079 2e63  ified in obspy.c
+00000ff0: 6f72 652e 7374 7265 616d 2e53 7472 6561  ore.stream.Strea
+00001000: 6d2e 7365 6c65 6374 0a20 2020 2020 2020  m.select.       
+00001010: 2029 0472 2100 0000 7222 0000 0072 2300   ).r!...r"...r#.
+00001020: 0000 7224 0000 0029 0172 2e00 0000 722f  ..r$...).r....r/
+00001030: 0000 0029 0672 3100 0000 da06 7365 6c65  ...).r1.....sele
+00001040: 6374 7232 0000 0072 2800 0000 7229 0000  ctr2...r(...r)..
+00001050: 0072 3400 0000 290e 7211 0000 0072 3500  .r4...).r....r5.
+00001060: 0000 7221 0000 0072 2200 0000 7224 0000  ..r!...r"...r$..
+00001070: 0072 2300 0000 7230 0000 0072 2e00 0000  .r#...r0...r....
+00001080: 5a0c 696e 765f 7365 6c65 6374 6564 722b  Z.inv_selectedr+
+00001090: 0000 0072 2c00 0000 5a07 6f6c 645f 7374  ...r,...Z.old_st
+000010a0: 61da 0363 6861 7237 0000 0072 1200 0000  a..char7...r....
+000010b0: 7212 0000 0072 1300 0000 da1a 7570 6461  r....r......upda
+000010c0: 7465 5f69 6e76 656e 746f 7279 5f66 726f  te_inventory_fro
+000010d0: 6d5f 6e73 6c63 7b00 0000 7334 0000 0000  m_nslc{...s4....
+000010e0: 1608 0104 0102 0102 0102 0102 fc06 0608  ................
+000010f0: 0108 0108 0108 0104 0102 0104 0104 0104  ................
+00001100: 0104 0102 fa06 0804 0102 0002 0002 0002  ................
+00001110: ff0c 037a 2444 6563 696d 6174 6f72 2e75  ...z$Decimator.u
+00001120: 7064 6174 655f 696e 7665 6e74 6f72 795f  pdate_inventory_
+00001130: 6672 6f6d 5f6e 736c 6363 0200 0000 0000  from_nslcc......
+00001140: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+00001150: 0000 730e 0100 0074 007c 0083 0164 016b  ..s....t.|...d.k
+00001160: 0372 1c74 0164 027c 009b 0264 039d 0383  .r.t.d.|...d....
+00001170: 0182 017c 0064 046b 0672 ae7c 0164 056b  ...|.d.k.r.|.d.k
+00001180: 0572 3064 0653 007c 0164 076b 0572 3c64  .r0d.S.|.d.k.r<d
+00001190: 0853 007c 0164 096b 0572 4864 0a53 007c  .S.|.d.k.rHd.S.|
+000011a0: 0164 0b6b 0572 5464 0c53 007c 0164 016b  .d.k.rTd.S.|.d.k
+000011b0: 0472 6064 0d53 007c 0164 0e6b 0472 6c64  .r`d.S.|.d.k.rld
+000011c0: 0f53 007c 0164 106b 0472 7864 1153 007c  .S.|.d.k.rxd.S.|
+000011d0: 0164 126b 0472 8464 1353 007c 0164 146b  .d.k.r.d.S.|.d.k
+000011e0: 0572 9064 1553 007c 0164 166b 0572 9c64  .r.d.S.|.d.k.r.d
+000011f0: 1753 007c 0164 186b 0572 a864 1953 0064  .S.|.d.k.r.d.S.d
+00001200: 1a53 006e 5c7c 0064 1b6b 0690 0072 fa7c  .S.n\|.d.k...r.|
+00001210: 0164 056b 0572 c464 1c53 007c 0164 076b  .d.k.r.d.S.|.d.k
+00001220: 0572 d064 1d53 007c 0164 096b 0572 dc64  .r.d.S.|.d.k.r.d
+00001230: 1e53 007c 0164 0b6b 0590 0072 ea64 1f53  .S.|.d.k...r.d.S
+00001240: 0074 02a0 0364 20a1 0101 0064 2153 006e  .t...d ....d!S.n
+00001250: 1074 0464 227c 009b 0064 239d 0383 0182  .t.d"|...d#.....
+00001260: 0164 2453 0029 257a dd0a 2020 2020 2020  .d$S.)%z..      
+00001270: 2020 5265 7475 726e 2074 6865 2063 6861    Return the cha
+00001280: 6e6e 656c 2062 616e 6420 636f 6465 2062  nnel band code b
+00001290: 6173 6564 206f 6e20 616e 2069 6e70 7574  ased on an input
+000012a0: 2062 616e 645f 636f 6465 0a0a 2020 2020   band_code..    
+000012b0: 2020 2020 3a70 6172 616d 2069 6e5f 6261      :param in_ba
+000012c0: 6e64 5f63 6f64 653a 2069 6e70 7574 2062  nd_code: input b
+000012d0: 616e 6420 636f 6465 2028 2742 2720 6966  and code ('B' if
+000012e0: 2063 7574 6f66 6620 3e20 3130 732c 0a20   cutoff > 10s,. 
+000012f0: 2020 2020 2020 2020 2020 2027 5327 206f             'S' o
+00001300: 7468 6572 7769 7365 290a 2020 2020 2020  therwise).      
+00001310: 2020 3a70 6172 616d 2073 616d 706c 655f    :param sample_
+00001320: 7261 7465 3a20 696e 7075 7420 7361 6d70  rate: input samp
+00001330: 6c65 2072 6174 6520 2873 7073 290a 2020  le rate (sps).  
+00001340: 2020 2020 2020 720c 0000 007a 0e22 696e        r....z."in
+00001350: 5f62 616e 645f 636f 6465 3d7a 1c22 2069  _band_code=z." i
+00001360: 7320 6d6f 7265 2074 6861 6e20 6f6e 6520  s more than one 
+00001370: 6368 6172 6163 7465 725a 0c46 4348 424d  characterZ.FCHBM
+00001380: 4c56 5552 5054 5169 e803 0000 da01 46e9  LVURPTQi......F.
+00001390: fa00 0000 da01 43e9 5000 0000 da01 48e9  ......C.P.....H.
+000013a0: 0a00 0000 da01 42da 014d 6733 3333 3333  ......B..Mg33333
+000013b0: 33d3 3fda 014c 67b8 1e85 eb51 b89e 3fda  3.?..Lg....Q..?.
+000013c0: 0156 67fa 7e6a bc74 9368 3fda 0155 672d  .Vg.~j.t.h?..Ug-
+000013d0: 431c ebe2 361a 3fda 0152 67f1 68e3 88b5  C...6.?..Rg.h...
+000013e0: f8e4 3eda 0150 678d edb5 a0f7 c6b0 3eda  ..>..Pg.......>.
+000013f0: 0154 da01 515a 0447 4445 53da 0147 da01  .T..QZ.GDES..G..
+00001400: 44da 0145 da01 537a 2853 686f 7274 2070  D..E..Sz(Short p
+00001410: 6572 696f 6420 7365 6e73 6f72 2073 616d  eriod sensor sam
+00001420: 706c 6520 7261 7465 203c 2031 3020 7370  ple rate < 10 sp
+00001430: 73da 0158 7a19 556e 6b6e 6f77 6e20 6261  s..Xz.Unknown ba
+00001440: 6e64 2062 6173 6520 636f 6465 3a20 22fa  nd base code: ".
+00001450: 0122 4e29 05da 036c 656e 7233 0000 00da  ."N)...lenr3....
+00001460: 0877 6172 6e69 6e67 73da 0477 6172 6e72  .warnings..warnr
+00001470: 1900 0000 2902 da0c 696e 5f62 616e 645f  ....)...in_band_
+00001480: 636f 6465 722a 0000 0072 1200 0000 7212  coder*...r....r.
+00001490: 0000 0072 1300 0000 da0d 6765 745f 6261  ...r......get_ba
+000014a0: 6e64 5f63 6f64 65a9 0000 0073 4c00 0000  nd_code....sL...
+000014b0: 0009 0c01 1001 0801 0801 0401 0801 0401  ................
+000014c0: 0801 0401 0801 0401 0801 0401 0801 0401  ................
+000014d0: 0801 0401 0801 0401 0801 0401 0801 0401  ................
+000014e0: 0801 0402 0601 0a01 0801 0401 0801 0401  ................
+000014f0: 0801 0401 0a01 0402 0a01 0602 7a17 4465  ............z.De
+00001500: 6369 6d61 746f 722e 6765 745f 6261 6e64  cimator.get_band
+00001510: 5f63 6f64 6563 0400 0000 0000 0000 0000  _codec..........
+00001520: 0000 0400 0000 0700 0000 4300 0000 7334  ..........C...s4
+00001530: 0000 007c 017c 00a0 007c 017c 02a1 026b  ...|.|...|.|...k
+00001540: 0372 2874 01a0 0264 017c 019b 0064 027c  .r(t...d.|...d.|
+00001550: 029b 0064 039d 05a1 0101 007c 00a0 007c  ...d.......|...|
+00001560: 017c 03a1 0253 0029 047a cc0a 2020 2020  .|...S.).z..    
+00001570: 2020 2020 5265 7475 726e 2074 6865 2063      Return the c
+00001580: 6861 6e6e 656c 2062 616e 6420 636f 6465  hannel band code
+00001590: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000015a0: 2069 6e5f 6261 6e64 5f63 6f64 653a 2069   in_band_code: i
+000015b0: 6e70 7574 2062 616e 6420 636f 6465 0a20  nput band code. 
+000015c0: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+000015d0: 5f73 616d 706c 655f 7261 7465 3a20 696e  _sample_rate: in
+000015e0: 7075 7420 7361 6d70 6c65 2072 6174 6520  put sample rate 
+000015f0: 2873 7073 290a 2020 2020 2020 2020 3a70  (sps).        :p
+00001600: 6172 616d 206f 7574 5f73 616d 706c 655f  aram out_sample_
+00001610: 7261 7465 3a20 6f75 7470 7574 2073 616d  rate: output sam
+00001620: 706c 6520 7261 7465 2028 7370 7329 0a20  ple rate (sps). 
+00001630: 2020 2020 2020 207a 1149 6e70 7574 2062         z.Input b
+00001640: 616e 6420 636f 6465 2028 7a27 2920 646f  and code (z') do
+00001650: 6573 206e 6f74 206d 6174 6368 2020 696e  es not match  in
+00001660: 7075 7420 7361 6d70 6c69 6e67 2072 6174  put sampling rat
+00001670: 6520 28fa 0129 2903 7256 0000 0072 5300  e (..)).rV...rS.
+00001680: 0000 7254 0000 0029 0472 1100 0000 7255  ..rT...).r....rU
+00001690: 0000 005a 0e69 6e5f 7361 6d70 6c65 5f72  ...Z.in_sample_r
+000016a0: 6174 655a 0f6f 7574 5f73 616d 706c 655f  ateZ.out_sample_
+000016b0: 7261 7465 7212 0000 0072 1200 0000 7213  rater....r....r.
+000016c0: 0000 00da 125f 6765 745f 6e65 775f 6261  ....._get_new_ba
+000016d0: 6e64 5f63 6f64 65dc 0000 0073 0a00 0000  nd_code....s....
+000016e0: 0009 1001 0401 10ff 0404 7a1c 4465 6369  ..........z.Deci
+000016f0: 6d61 746f 722e 5f67 6574 5f6e 6577 5f62  mator._get_new_b
+00001700: 616e 645f 636f 6465 da00 6306 0000 0000  and_code..c.....
+00001710: 0000 0000 0000 0007 0000 0009 0000 0043  ...............C
+00001720: 0000 0073 8e00 0000 7c05 6401 6b09 7230  ...s....|.d.k.r0
+00001730: 7400 6402 a001 6403 a002 7c02 7c03 7c01  t.d...d...|.|.|.
+00001740: 6a03 7c01 6a04 6704 a101 7c01 6a05 a102  j.|.j.g...|.j...
+00001750: 6404 6405 8d02 0100 7c01 6a05 7d06 7c00  d.d.....|.j.}.|.
+00001760: a006 7c01 7c06 a102 0100 7c00 a007 7c01  ..|.|.....|...|.
+00001770: 7c06 a102 0100 7c01 0400 6a05 7c00 6a08  |.....|...j.|.j.
+00001780: 1d00 0200 5f05 7c05 6401 6b09 728a 7400  ...._.|.d.k.r.t.
+00001790: 6406 a001 6403 a002 7c02 7c03 7c01 6a03  d...d...|.|.|.j.
+000017a0: 7c01 6a04 6704 a101 7c01 6a05 a102 8301  |.j.g...|.j.....
+000017b0: 0100 6407 5300 2908 619e 0100 000a 2020  ..d.S.).a.....  
+000017c0: 2020 2020 2020 6d6f 6469 6679 2072 6570        modify rep
+000017d0: 6f6e 7365 2061 6e64 206e 616d 6520 6f66  onse and name of
+000017e0: 2061 2063 6861 6e6e 656c 2074 6f20 636f   a channel to co
+000017f0: 7272 6573 706f 6e64 2074 6f20 6465 6369  rrespond to deci
+00001800: 6d61 7469 6f6e 0a0a 2020 2020 2020 2020  mation..        
+00001810: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00001820: 2020 6368 6120 283a 636c 6173 733a 606f    cha (:class:`o
+00001830: 6273 7079 2e63 6f72 652e 696e 7665 6e74  bspy.core.invent
+00001840: 6f72 792e 6368 616e 6e65 6c60 293a 206f  ory.channel`): o
+00001850: 7269 6769 6e61 6c20 6368 616e 6e65 6c0a  riginal channel.
+00001860: 2020 2020 2020 2020 2020 2020 6e65 7420              net 
+00001870: 2873 7472 293a 206e 6574 776f 726b 2063  (str): network c
+00001880: 6f64 6520 286a 7573 7420 666f 7220 636c  ode (just for cl
+00001890: 6561 7265 7220 7072 6f67 7265 7373 2070  earer progress p
+000018a0: 7269 6e74 6f75 7429 0a20 2020 2020 2020  rintout).       
+000018b0: 2020 2020 2073 7461 2028 7374 7229 3a20       sta (str): 
+000018c0: 7374 6174 696f 6e20 636f 6465 2028 6a75  station code (ju
+000018d0: 7374 2066 6f72 2063 6c65 6172 6572 2070  st for clearer p
+000018e0: 726f 6772 6573 7320 7072 696e 746f 7574  rogress printout
+000018f0: 290a 2020 2020 2020 2020 2020 2020 6e6f  ).            no
+00001900: 726d 616c 697a 655f 6669 7273 2028 626f  rmalize_firs (bo
+00001910: 6f6c 293a 206e 6f72 6d61 6c69 7a65 7320  ol): normalizes 
+00001920: 616e 7920 4649 5220 6368 616e 6e65 6c20  any FIR channel 
+00001930: 7468 6174 2069 736e 2774 0a20 2020 2020  that isn't.     
+00001940: 2020 2020 2020 2020 2020 2061 6c72 6561             alrea
+00001950: 6479 0a20 2020 2020 2020 2054 7a21 6368  dy.        Tz!ch
+00001960: 616e 6e65 6c20 6d6f 6469 6669 6564 2066  annel modified f
+00001970: 726f 6d20 7b7d 2028 7b7d 2073 7073 29da  rom {} ({} sps).
+00001980: 012e fa01 2029 01da 0365 6e64 7a10 746f  .... )...endz.to
+00001990: 207b 7d20 287b 3a67 7d20 7370 7329 4e29   {} ({:g} sps)N)
+000019a0: 09da 0570 7269 6e74 da06 666f 726d 6174  ...print..format
+000019b0: da04 6a6f 696e 7229 0000 0072 2800 0000  ..joinr)...r(...
+000019c0: 722a 0000 00da 0d5f 6164 645f 7265 7370  r*....._add_resp
+000019d0: 6f6e 7365 da10 5f63 6861 6e67 655f 6368  onse.._change_ch
+000019e0: 616e 5f6c 6f63 7214 0000 0029 0772 1100  an_locr....).r..
+000019f0: 0000 723b 0000 0072 2b00 0000 722c 0000  ..r;...r+...r,..
+00001a00: 0072 2e00 0000 7230 0000 00da 1169 6e70  .r....r0.....inp
+00001a10: 7574 5f73 616d 706c 655f 7261 7465 7212  ut_sample_rater.
+00001a20: 0000 0072 1200 0000 7213 0000 0072 3400  ...r....r....r4.
+00001a30: 0000 ec00 0000 7320 0000 0000 0c08 0106  ......s ........
+00001a40: 0114 0104 fe02 0202 fe06 0306 010c 010c  ................
+00001a50: 0110 0108 0106 0114 0104 fe7a 1644 6563  ...........z.Dec
+00001a60: 696d 6174 6f72 2e5f 6d6f 6469 6679 5f63  imator._modify_c
+00001a70: 6861 6e63 0100 0000 0000 0000 0000 0000  hanc............
+00001a80: 0200 0000 0600 0000 0300 0000 733e 0100  ............s>..
+00001a90: 007c 006a 006a 0144 0090 015d 2e7d 0174  .|.j.j.D...].}.t
+00001aa0: 027c 0174 0383 0272 be7c 016a 0464 016b  .|.t...r.|.j.d.k
+00001ab0: 0272 2e74 057c 016a 0683 0189 006e 567c  .r.t.|.j.....nV|
+00001ac0: 016a 0464 026b 0272 4864 0374 057c 016a  .j.d.k.rHd.t.|.j
+00001ad0: 0683 0114 0089 006e 3c7c 016a 0464 046b  .......n<|.j.d.k
+00001ae0: 0272 7464 0374 057c 016a 0664 0564 0685  .rtd.t.|.j.d.d..
+00001af0: 0219 0083 0114 007c 016a 0664 0619 0017  .......|.j.d....
+00001b00: 0089 006e 1074 0764 077c 016a 049b 009d  ...n.t.d.|.j....
+00001b10: 0283 0182 0174 0888 0064 0818 0083 0164  .....t...d.....d
+00001b20: 096b 0472 bc74 09a0 0a64 0a88 009b 0064  .k.r.t...d.....d
+00001b30: 0b9d 03a1 0101 0087 0066 0164 0c64 0d84  .........f.d.d..
+00001b40: 087c 016a 0644 0083 017c 015f 0671 0874  .|.j.D...|._.q.t
+00001b50: 027c 0174 0b83 0272 0874 057c 016a 0c83  .|.t...r.t.|.j..
+00001b60: 0164 0e6b 0272 ec74 057c 016a 0d83 0189  .d.k.r.t.|.j....
+00001b70: 0088 0064 0e6b 0272 ea71 086e 1474 057c  ...d.k.r.q.n.t.|
+00001b80: 016a 0d83 0174 057c 016a 0c83 011b 0089  .j...t.|.j......
+00001b90: 0074 0888 0064 0818 0083 0164 096b 0472  .t...d.....d.k.r
+00001ba0: 0874 09a0 0a64 0f88 009b 0064 0b9d 03a1  .t...d.....d....
+00001bb0: 0101 0087 0066 0164 1064 0d84 087c 016a  .....f.d.d...|.j
+00001bc0: 0d44 0083 017c 015f 0d71 0864 0553 0029  .D...|._.q.d.S.)
+00001bd0: 117a a80a 2020 2020 2020 2020 5665 7269  .z..        Veri
+00001be0: 6669 6573 2026 2c20 6966 206e 6565 6465  fies &, if neede
+00001bf0: 642c 206e 6f72 6d61 6c69 7a65 7320 6368  d, normalizes ch
+00001c00: 616e 6e65 6c27 7320 4649 5220 6f72 2043  annel's FIR or C
+00001c10: 6f65 6666 6963 6965 6e74 7320 636f 6566  oefficients coef
+00001c20: 6673 0a0a 2020 2020 2020 2020 4172 6773  fs..        Args
+00001c30: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
+00001c40: 6120 283a 636c 6173 733a 606f 6273 7079  a (:class:`obspy
+00001c50: 2e63 6f72 652e 696e 7665 6e74 6f72 792e  .core.inventory.
+00001c60: 6368 616e 6e65 6c60 293a 2063 6861 6e6e  channel`): chann
+00001c70: 656c 0a20 2020 2020 2020 20da 044e 4f4e  el.        ..NON
+00001c80: 45da 0445 5645 4ee9 0200 0000 da03 4f44  E..EVEN.......OD
+00001c90: 444e e9ff ffff ff7a 2255 6e6b 6e6f 776e  DN.....z"Unknown
+00001ca0: 2046 4952 2063 6f65 6666 6963 6965 6e74   FIR coefficient
+00001cb0: 2073 796d 6d65 7472 793a 2072 0c00 0000   symmetry: r....
+00001cc0: 677b 14ae 47e1 7a84 3f7a 1f44 4543 494d  g{..G.z.?z.DECIM
+00001cd0: 4154 4f52 3a20 5375 6d20 6f66 2046 4952  ATOR: Sum of FIR
+00001ce0: 2063 6f65 6666 7320 3d20 7a0d 2c20 6e6f   coeffs = z., no
+00001cf0: 726d 616c 697a 696e 6763 0100 0000 0000  rmalizingc......
+00001d00: 0000 0000 0000 0200 0000 0400 0000 1300  ................
+00001d10: 0000 7314 0000 0067 007c 005d 0c7d 017c  ..s....g.|.].}.|
+00001d20: 0188 001b 0091 0271 0453 0072 1200 0000  .......q.S.r....
+00001d30: 7212 0000 00a9 0272 1e00 0000 da01 78a9  r......r......x.
+00001d40: 015a 0963 6f65 6666 5f73 756d 7212 0000  .Z.coeff_sumr...
+00001d50: 0072 1300 0000 7220 0000 001e 0100 0073  .r....r .......s
+00001d60: 0400 0000 0601 02ff 7a2d 4465 6369 6d61  ........z-Decima
+00001d70: 746f 722e 5f6e 6f72 6d61 6c69 7a65 5f66  tor._normalize_f
+00001d80: 6972 732e 3c6c 6f63 616c 733e 2e3c 6c69  irs.<locals>.<li
+00001d90: 7374 636f 6d70 3e72 0100 0000 7a35 4445  stcomp>r....z5DE
+00001da0: 4349 4d41 544f 523a 2073 756d 286e 756d  CIMATOR: sum(num
+00001db0: 6572 6174 6f72 2063 6f65 6666 7329 2f73  erator coeffs)/s
+00001dc0: 756d 2864 656e 6f6d 2063 6f65 6666 7329  um(denom coeffs)
+00001dd0: 203d 2063 0100 0000 0000 0000 0000 0000   = c............
+00001de0: 0200 0000 0400 0000 1300 0000 7314 0000  ............s...
+00001df0: 0067 007c 005d 0c7d 017c 0188 001b 0091  .g.|.].}.|......
+00001e00: 0271 0453 0072 1200 0000 7212 0000 0072  .q.S.r....r....r
+00001e10: 6800 0000 726a 0000 0072 1200 0000 7213  h...rj...r....r.
+00001e20: 0000 0072 2000 0000 2c01 0000 7304 0000  ...r ...,...s...
+00001e30: 0006 0002 0029 0eda 0872 6573 706f 6e73  .....)...respons
+00001e40: 65da 0f72 6573 706f 6e73 655f 7374 6167  e..response_stag
+00001e50: 6573 7216 0000 0072 0a00 0000 da08 7379  esr....r......sy
+00001e60: 6d6d 6574 7279 da03 7375 6dda 0c63 6f65  mmetry..sum..coe
+00001e70: 6666 6963 6965 6e74 7372 3300 0000 da03  fficientsr3.....
+00001e80: 6162 73da 076c 6f67 6769 6e67 da04 696e  abs..logging..in
+00001e90: 666f 720b 0000 00da 0b64 656e 6f6d 696e  for......denomin
+00001ea0: 6174 6f72 da09 6e75 6d65 7261 746f 7229  ator..numerator)
+00001eb0: 0272 3b00 0000 5a03 7374 6772 1200 0000  .r;...Z.stgr....
+00001ec0: 726a 0000 0072 1300 0000 da0f 5f6e 6f72  rj...r......_nor
+00001ed0: 6d61 6c69 7a65 5f66 6972 7305 0100 0073  malize_firs....s
+00001ee0: 3800 0000 0008 0e01 0a01 0a01 0c01 0a01  8...............
+00001ef0: 1001 0a02 1eff 0404 0201 0aff 0403 1001  ................
+00001f00: 1202 0a01 04ff 0a02 0a01 0e01 0a01 0801  ................
+00001f10: 0402 1402 1001 0401 0aff 0403 7a19 4465  ............z.De
+00001f20: 6369 6d61 746f 722e 5f6e 6f72 6d61 6c69  cimator._normali
+00001f30: 7a65 5f66 6972 7363 0400 0000 0000 0000  ze_firsc........
+00001f40: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00001f50: 7320 0000 007c 00a0 007c 016a 017c 016a  s ...|...|.j.|.j
+00001f60: 027c 027c 03a1 045c 027c 015f 017c 015f  .|.|...\.|._.|._
+00001f70: 0264 0153 0029 0261 1c01 0000 0a20 2020  .d.S.).a.....   
+00001f80: 2020 2020 2043 6861 6e67 6520 6368 616e       Change chan
+00001f90: 6e65 6c20 286f 7220 6c6f 6361 7469 6f6e  nel (or location
+00001fa0: 2920 636f 6465 2069 6e20 706c 6163 652c  ) code in place,
+00001fb0: 2061 6363 6f72 6469 6e67 2074 6f20 6465   according to de
+00001fc0: 6369 6d61 7469 6f6e 0a0a 2020 2020 2020  cimation..      
+00001fd0: 2020 4172 6775 6d65 6e74 733a 0a20 2020    Arguments:.   
+00001fe0: 2020 2020 2020 2020 2063 6861 2028 496e           cha (In
+00001ff0: 7665 6e74 6f72 792e 4368 616e 6e65 6c29  ventory.Channel)
+00002000: 2063 6861 6e6e 656c 2074 6f20 6265 206d   channel to be m
+00002010: 6f64 6966 6965 6420 2869 6e20 706c 6163  odified (in plac
+00002020: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00002030: 6e5f 7372 2028 666c 6f61 7429 3a20 696e  n_sr (float): in
+00002040: 7075 7420 7361 6d70 6c65 2072 6174 650a  put sample rate.
+00002050: 2020 2020 2020 2020 2020 2020 6176 6f69              avoi
+00002060: 645f 636f 6465 7320 286c 6973 7429 3a20  d_codes (list): 
+00002070: 6368 616e 6e65 6c3a 6c6f 6361 7469 6f6e  channel:location
+00002080: 2063 6f64 6573 2074 6f20 6176 6f69 640a   codes to avoid.
+00002090: 2020 2020 2020 2020 4e29 03da 0d5f 6765          N)..._ge
+000020a0: 745f 6368 616e 5f6c 6f63 7228 0000 0072  t_chan_locr(...r
+000020b0: 2900 0000 2904 7211 0000 0072 3b00 0000  )...).r....r;...
+000020c0: da05 696e 5f73 72da 0b61 766f 6964 5f63  ..in_sr..avoid_c
+000020d0: 6f64 6573 7212 0000 0072 1200 0000 7213  odesr....r....r.
+000020e0: 0000 0072 6100 0000 2e01 0000 730c 0000  ...ra.......s...
+000020f0: 0000 0904 0104 0004 0002 0002 ff7a 1a44  .............z.D
+00002100: 6563 696d 6174 6f72 2e5f 6368 616e 6765  ecimator._change
+00002110: 5f63 6861 6e5f 6c6f 6363 0500 0000 0000  _chan_locc......
+00002120: 0000 0000 0000 0a00 0000 0800 0000 4300  ..............C.
+00002130: 0000 73c6 0000 007c 006a 0064 016b 0272  ..s....|.j.d.k.r
+00002140: 1274 0164 0283 0182 017c 037c 006a 001b  .t.d.....|.|.j..
+00002150: 007d 057c 00a0 027c 0164 0319 007c 037c  .}.|...|.d...|.|
+00002160: 05a1 037d 067c 067c 0164 0164 0485 0219  ...}.|.|.d.d....
+00002170: 0017 007d 077c 077c 016b 0272 767a 1474  ...}.|.|.k.rvz.t
+00002180: 037c 0283 0164 0117 0064 059b 047d 0857  .|...d...d...}.W
+00002190: 0071 7a04 0074 046b 0a72 7201 0001 0001  .qz..t.k.rr.....
+000021a0: 0064 067d 0859 0071 7a58 006e 047c 027d  .d.}.Y.qzX.n.|.}
+000021b0: 087c 0444 005d 3a7d 097c 077c 09a0 0564  .|.D.]:}.|.|...d
+000021c0: 07a1 0164 0319 006b 0272 7e7c 087c 09a0  ...d...k.r~|.|..
+000021d0: 0564 07a1 0164 0119 006b 0272 7e74 037c  .d...d...k.r~t.|
+000021e0: 0883 0164 0117 0064 059b 047d 0871 7e71  ...d...d...}.q~q
+000021f0: 7e71 be71 7a7c 077c 0866 0253 0029 0861  ~q.qz|.|.f.S.).a
+00002200: 8f01 0000 0a20 2020 2020 2020 2047 6574  .....        Get
+00002210: 206e 6577 2063 6861 6e6e 656c 2028 6f72   new channel (or
+00002220: 206c 6f63 2920 636f 6465 7320 6672 6f6d   loc) codes from
+00002230: 206f 6c64 2063 6f64 6573 2061 6e64 2064   old codes and d
+00002240: 6563 696d 6174 696f 6e20 6661 6374 6f72  ecimation factor
+00002250: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00002260: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00002270: 2063 6861 5f63 6f64 653a 2069 6e70 7574   cha_code: input
+00002280: 2063 6861 6e6e 656c 2063 6f64 650a 2020   channel code.  
+00002290: 2020 2020 2020 2020 2020 6c6f 635f 636f            loc_co
+000022a0: 6465 3a20 696e 7075 7420 6c6f 6361 7469  de: input locati
+000022b0: 6f6e 2063 6f64 650a 2020 2020 2020 2020  on code.        
+000022c0: 2020 2020 696e 5f73 723a 2069 6e70 7574      in_sr: input
+000022d0: 2073 616d 706c 696e 6720 7261 7465 0a20   sampling rate. 
+000022e0: 2020 2020 2020 2020 2020 2061 766f 6964             avoid
+000022f0: 5f63 6f64 6573 2028 6c69 7374 293a 2063  _codes (list): c
+00002300: 6861 6e6e 656c 3a6c 6f63 6174 696f 6e20  hannel:location 
+00002310: 636f 6465 7320 746f 2061 766f 6964 0a0a  codes to avoid..
+00002320: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00002330: 0a20 2020 2020 2020 2020 2020 2074 7570  .            tup
+00002340: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00002350: 2020 2020 6e65 775f 6368 616e 5f63 6f64      new_chan_cod
+00002360: 6520 2873 7472 290a 2020 2020 2020 2020  e (str).        
+00002370: 2020 2020 2020 2020 6e65 775f 6c6f 635f          new_loc_
+00002380: 636f 6465 2028 7374 7229 0a20 2020 2020  code (str).     
+00002390: 2020 2072 0c00 0000 7a10 4465 6369 6d61     r....z.Decima
+000023a0: 7469 6f6e 203d 3d20 3121 7201 0000 004e  tion == 1!r....N
+000023b0: da03 3032 645a 0230 31fa 013a 2906 7214  ..02dZ.01..:).r.
+000023c0: 0000 0072 3300 0000 7258 0000 00da 0369  ...r3...rX.....i
+000023d0: 6e74 da09 4578 6365 7074 696f 6eda 0573  nt..Exception..s
+000023e0: 706c 6974 290a 7211 0000 005a 0863 6861  plit).r....Z.cha
+000023f0: 5f63 6f64 655a 086c 6f63 5f63 6f64 6572  _codeZ.loc_coder
+00002400: 7700 0000 7278 0000 005a 066f 7574 5f73  w...rx...Z.out_s
+00002410: 725a 0d6e 6577 5f62 616e 645f 636f 6465  rZ.new_band_code
+00002420: 5a0c 6e65 775f 6368 615f 636f 6465 5a0c  Z.new_cha_codeZ.
+00002430: 6e65 775f 6c6f 635f 636f 6465 da01 6372  new_loc_code..cr
+00002440: 1200 0000 7212 0000 0072 1300 0000 7276  ....r....r....rv
+00002450: 0000 003b 0100 0073 2800 0000 000f 0a01  ...;...s(.......
+00002460: 0801 0a01 1201 1001 0802 0201 1401 0e01  ................
+00002470: 0c02 0403 0802 10ff 0202 10fe 0204 1001  ................
+00002480: 0401 0401 7a17 4465 6369 6d61 746f 722e  ....z.Decimator.
+00002490: 5f67 6574 5f63 6861 6e5f 6c6f 6363 0300  _get_chan_locc..
+000024a0: 0000 0000 0000 0000 0000 0700 0000 0800  ................
+000024b0: 0000 4300 0000 73a6 0000 007c 016a 006a  ..C...s....|.j.j
+000024c0: 0164 0119 006a 027d 037c 006a 0344 005d  .d...j.}.|.j.D.]
+000024d0: 347d 0474 04a0 057c 04a1 017d 057c 0364  4}.t...|...}.|.d
+000024e0: 0237 007d 037c 016a 006a 01a0 067c 05a0  .7.}.|.j.j...|..
+000024f0: 077c 027c 03a1 02a1 0101 007c 027c 041d  .|.|.......|.|..
+00002500: 007d 0271 147a 0e7c 016a 00a0 08a1 0001  .}.q.z.|.j......
+00002510: 0057 006e 4804 0074 096b 0a72 a001 0001  .W.nH..t.k.r....
+00002520: 0001 007c 016a 006a 0a6a 0b7d 067c 06a0  ...|.j.j.j.}.|..
+00002530: 0ca1 0064 036b 0272 9c64 047c 016a 006a  ...d.k.r.d.|.j.j
+00002540: 0a5f 0b7c 016a 00a0 08a1 0001 007c 067c  ._.|.j.......|.|
+00002550: 016a 006a 0a5f 0b59 006e 0258 0064 0553  .j.j._.Y.n.X.d.S
+00002560: 0029 067a 580a 2020 2020 2020 2020 4170  .).zX.        Ap
+00002570: 7065 6e64 2020 6465 6369 6d61 7469 6f6e  pend  decimation
+00002580: 206f 626a 6563 7427 7320 7265 7370 6f6e   object's respon
+00002590: 7365 2074 6f20 616e 2065 7869 7374 696e  se to an existin
+000025a0: 6720 6368 616e 6e65 6c27 7320 7265 7370  g channel's resp
+000025b0: 6f6e 7365 0a20 2020 2020 2020 2072 6700  onse.        rg.
+000025c0: 0000 720c 0000 00da 0250 417a 034d 2f53  ..r......PAz.M/S
+000025d0: 4e29 0d72 6b00 0000 726c 0000 00da 1573  N).rk...rl.....s
+000025e0: 7461 6765 5f73 6571 7565 6e63 655f 6e75  tage_sequence_nu
+000025f0: 6d62 6572 720f 0000 0072 0d00 0000 da08  mberr....r......
+00002600: 6672 6f6d 5f53 4143 da06 6170 7065 6e64  from_SAC..append
+00002610: da08 746f 5f6f 6273 7079 da1f 7265 6361  ..to_obspy..reca
+00002620: 6c63 756c 6174 655f 6f76 6572 616c 6c5f  lculate_overall_
+00002630: 7365 6e73 6974 6976 6974 7972 7c00 0000  sensitivityr|...
+00002640: da16 696e 7374 7275 6d65 6e74 5f73 656e  ..instrument_sen
+00002650: 7369 7469 7669 7479 da0b 696e 7075 745f  sitivity..input_
+00002660: 756e 6974 73da 0575 7070 6572 2907 7211  units..upper).r.
+00002670: 0000 0072 3b00 0000 7262 0000 00da 0c73  ...r;...rb.....s
+00002680: 7461 6765 5f6e 756d 6265 72da 0164 da0a  tage_number..d..
+00002690: 6669 725f 6669 6c74 6572 da03 695f 7572  fir_filter..i_ur
+000026a0: 1200 0000 7212 0000 0072 1300 0000 7260  ....r....r....r`
+000026b0: 0000 0063 0100 0073 2000 0000 0004 0e01  ...c...s .......
+000026c0: 0a01 0a01 0801 0801 0aff 0403 0a01 0201  ................
+000026d0: 0e01 0e01 0a01 0c01 0a01 0a01 7a17 4465  ............z.De
+000026e0: 6369 6d61 746f 722e 5f61 6464 5f72 6573  cimator._add_res
+000026f0: 706f 6e73 6563 0200 0000 0000 0000 0000  ponsec..........
+00002700: 0000 0500 0000 0600 0000 4300 0000 736a  ..........C...sj
+00002710: 0000 0074 007c 0174 0183 0273 1274 0264  ...t.|.t...s.t.d
+00002720: 0183 0182 017c 01a0 03a1 007d 0267 007d  .....|.....}.g.}
+00002730: 037c 026a 0444 005d 147d 047c 03a0 057c  .|.j.D.].}.|...|
+00002740: 00a0 067c 04a1 01a1 0101 0071 247c 037c  ...|.......q$|.|
+00002750: 025f 047c 006a 0772 5e74 0864 02a0 0964  ._.|.j.r^t.d...d
+00002760: 0364 0484 007c 0244 0083 01a1 0183 0101  .d...|.D........
+00002770: 007c 02a0 0aa1 0001 007c 0253 0029 057a  .|.......|.S.).z
+00002780: 270a 2020 2020 2020 2020 4465 6369 6d61  '.        Decima
+00002790: 7465 206f 6273 7079 2053 7472 6561 6d0a  te obspy Stream.
+000027a0: 2020 2020 2020 2020 7a24 696e 7075 7420          z$input 
+000027b0: 7374 7265 616d 2069 7320 6e6f 7420 616e  stream is not an
+000027c0: 206f 6273 7079 2053 7472 6561 6d21 7a17   obspy Stream!z.
+000027d0: 4e65 7720 6461 7461 2068 6173 207b 7d20  New data has {} 
+000027e0: 7361 6d70 6c65 7363 0100 0000 0000 0000  samplesc........
+000027f0: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00002800: 7314 0000 0067 007c 005d 0c7d 017c 016a  s....g.|.].}.|.j
+00002810: 006a 0191 0271 0453 0072 1200 0000 2902  .j...q.S.r....).
+00002820: 721a 0000 00da 0473 697a 6572 1d00 0000  r......sizer....
+00002830: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00002840: 2000 0000 8401 0000 7304 0000 0006 0102   .......s.......
+00002850: ff7a 2944 6563 696d 6174 6f72 2e5f 7275  .z)Decimator._ru
+00002860: 6e5f 7374 7265 616d 2e3c 6c6f 6361 6c73  n_stream.<locals
+00002870: 3e2e 3c6c 6973 7463 6f6d 703e 290b 7216  >.<listcomp>).r.
+00002880: 0000 0072 0700 0000 7233 0000 0072 3100  ...r....r3...r1.
+00002890: 0000 da06 7472 6163 6573 7282 0000 0072  ....tracesr....r
+000028a0: 1800 0000 7210 0000 0072 5d00 0000 725e  ....r....r]...r^
+000028b0: 0000 00da 0676 6572 6966 7929 0572 1100  .....verify).r..
+000028c0: 0000 da06 7374 7265 616d 7236 0000 005a  ....streamr6...Z
+000028d0: 056e 6577 7472 721f 0000 0072 1200 0000  .newtrr....r....
+000028e0: 7212 0000 0072 1300 0000 7217 0000 0078  r....r....r....x
+000028f0: 0100 0073 1a00 0000 0004 0a01 0801 0801  ...s............
+00002900: 0401 0a01 1201 0601 0601 0c01 02ff 0a02  ................
+00002910: 0801 7a15 4465 6369 6d61 746f 722e 5f72  ..z.Decimator._r
+00002920: 756e 5f73 7472 6561 6d63 0200 0000 0000  un_streamc......
+00002930: 0000 0000 0000 0800 0000 0600 0000 4300  ..............C.
+00002940: 0000 73f4 0000 0074 007c 0174 0183 0273  ..s....t.|.t...s
+00002950: 1274 0264 0183 0182 017c 016a 036a 047d  .t.d.....|.j.j.}
+00002960: 027c 01a0 05a1 007d 037c 036a 066a 077d  .|.....}.|.j.j.}
+00002970: 047c 006a 0872 4a74 0964 02a0 0a7c 047c  .|.j.rJt.d...|.|
+00002980: 047c 006a 0b1b 007c 006a 0ba1 0383 0101  .|.j...|.j......
+00002990: 0074 0ca0 0ca1 007d 057c 006a 0d44 005d  .t.....}.|.j.D.]
+000029a0: 2a7d 0674 0ea0 0f7c 06a1 017d 077c 07a0  *}.t...|...}.|..
+000029b0: 107c 036a 03a1 017c 035f 037c 036a 117c  .|.j...|._.|.j.|
+000029c0: 0664 0364 048d 0201 0071 587c 006a 1264  .d.d.....qX|.j.d
+000029d0: 036b 0872 a87c 036a 036a 047c 026b 0273  .k.r.|.j.j.|.k.s
+000029e0: a87c 036a 03a0 137c 02a1 017c 035f 037c  .|.j...|...|._.|
+000029f0: 00a0 147c 036a 066a 157c 036a 066a 167c  ...|.j.j.|.j.j.|
+00002a00: 036a 066a 077c 006a 0b14 00a1 035c 027c  .j.j.|.j.....\.|
+00002a10: 036a 065f 157c 036a 065f 167c 006a 0872  .j._.|.j._.|.j.r
+00002a20: f074 0964 05a0 0a74 0ca0 0ca1 007c 0518  .t.d...t.....|..
+00002a30: 00a1 0183 0101 007c 0353 0029 067a 260a  .......|.S.).z&.
+00002a40: 2020 2020 2020 2020 4465 6369 6d61 7465          Decimate
+00002a50: 206f 6273 7079 2054 7261 6365 0a20 2020   obspy Trace.   
+00002a60: 2020 2020 207a 2269 6e70 7574 2074 7261       z"input tra
+00002a70: 6365 2069 7320 6e6f 7420 616e 206f 6273  ce is not an obs
+00002a80: 7079 2054 7261 6365 217a 3044 6563 696d  py Trace!z0Decim
+00002a90: 6174 696e 6720 6461 7461 2066 726f 6d20  ating data from 
+00002aa0: 7b3a 677d 2074 6f20 7b3a 677d 2048 7a20  {:g} to {:g} Hz 
+00002ab0: 287b 3a64 7d78 292e 2e2e 2054 2901 da09  ({:d}x)... T)...
+00002ac0: 6e6f 5f66 696c 7465 727a 1354 6f6f 6b20  no_filterz.Took 
+00002ad0: 7b3a 2e31 667d 2073 6563 6f6e 6473 2917  {:.1f} seconds).
+00002ae0: 7216 0000 0072 0800 0000 7233 0000 0072  r....r....r3...r
+00002af0: 1a00 0000 da05 6474 7970 6572 3100 0000  ......dtyper1...
+00002b00: 721c 0000 0072 2500 0000 7210 0000 0072  r....r%...r....r
+00002b10: 5d00 0000 725e 0000 0072 1400 0000 da04  ]...r^...r......
+00002b20: 7469 6d65 720f 0000 0072 0d00 0000 7281  timer....r....r.
+00002b30: 0000 00da 0863 6f6e 766f 6c76 6572 1b00  .....convolver..
+00002b40: 0000 7215 0000 00da 0661 7374 7970 6572  ..r......astyper
+00002b50: 7600 0000 7224 0000 0072 2300 0000 2908  v...r$...r#...).
+00002b60: 7211 0000 00da 0574 7261 6365 7291 0000  r......tracer...
+00002b70: 0072 1f00 0000 da02 7372 da03 7469 6372  .r......sr..ticr
+00002b80: 8900 0000 728a 0000 0072 1200 0000 7212  ....r....r....r.
+00002b90: 0000 0072 1300 0000 7218 0000 0089 0100  ...r....r.......
+00002ba0: 0073 3400 0000 0004 0a01 0801 0801 0801  .s4.............
+00002bb0: 0801 0601 0601 0200 0801 04fe 0603 0801  ................
+00002bc0: 0a01 0a01 0e01 1001 1601 0e01 0401 0601  ................
+00002bd0: 0601 0cfd 1004 0601 1601 7a14 4465 6369  ..........z.Deci
+00002be0: 6d61 746f 722e 5f72 756e 5f74 7261 6365  mator._run_trace
+00002bf0: 6301 0000 0000 0000 0000 0000 000a 0000  c...............
+00002c00: 0009 0000 0003 0000 0073 f600 0000 7400  .........s....t.
+00002c10: 7401 7402 8300 8301 8301 a003 a100 6a04  t.t...........j.
+00002c20: 7d01 6401 7c00 6402 9b04 9d02 7d02 7c01  }.d.|.d.....}.|.
+00002c30: a005 7c02 a101 7d03 7406 7c03 8301 6403  ..|...}.t.|...d.
+00002c40: 6b02 733e 7407 6404 8301 8201 7408 7c03  k.s>t.d.....t.|.
+00002c50: 8301 8f5e 7d04 7c04 a009 a100 0100 7c04  ...^}.|.......|.
+00002c60: a009 a100 a00a a100 7d05 740b 7c05 6405  ........}.t.|.d.
+00002c70: 1900 8301 8900 740c 7c05 6403 1900 8301  ......t.|.d.....
+00002c80: 7d06 6700 7d07 7c04 a00d a100 4400 5d1e  }.g.}.|.....D.].
+00002c90: 7d08 7c07 8700 6601 6406 6407 8408 7c08  }.|...f.d.d...|.
+00002ca0: a00a a100 4400 8301 1700 7d07 7180 5700  ....D.....}.q.W.
+00002cb0: 3500 5100 5200 5800 7406 7c07 8301 7c06  5.Q.R.X.t.|...|.
+00002cc0: 6b02 73ca 740e 6408 a00f 7406 7c07 8301  k.s.t.d...t.|...
+00002cd0: 7c06 a102 8301 8201 7406 7c07 8301 6403  |.......t.|...d.
+00002ce0: 1800 7d09 7c07 6409 6405 6409 8503 1900  ..}.|.d.d.d.....
+00002cf0: 7c07 1700 7d07 7410 7c07 7c09 6403 640a  |...}.t.|.|.d.d.
+00002d00: 8304 5300 290b 7a2a 0a20 2020 2020 2020  ..S.).z*.       
+00002d10: 2052 6574 7572 6e73 2061 2053 4143 2046   Returns a SAC F
+00002d20: 4952 2066 696c 7465 720a 2020 2020 2020  IR filter.      
+00002d30: 2020 da03 6465 6372 8900 0000 720c 0000    ..decr....r...
+00002d40: 007a 2353 4143 2066 696c 7465 7220 6669  .z#SAC filter fi
+00002d50: 6c65 2022 7b66 6261 7365 7d22 206e 6f74  le "{fbase}" not
+00002d60: 2066 6f75 6e64 7201 0000 0063 0100 0000   foundr....c....
+00002d70: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002d80: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
+00002d90: 0174 007c 0183 0188 001b 0091 0271 0453  .t.|.........q.S
+00002da0: 0072 1200 0000 2901 da05 666c 6f61 7472  .r....)...floatr
+00002db0: 6800 0000 a901 da07 6469 7669 736f 7272  h.......divisorr
+00002dc0: 1200 0000 7213 0000 0072 2000 0000 b501  ....r....r .....
+00002dd0: 0000 7304 0000 0006 0002 007a 2b44 6563  ..s........z+Dec
+00002de0: 696d 6174 6f72 2e5f 7265 6164 5f46 4952  imator._read_FIR
+00002df0: 5f53 4143 2e3c 6c6f 6361 6c73 3e2e 3c6c  _SAC.<locals>.<l
+00002e00: 6973 7463 6f6d 703e 7a32 4649 5220 6c65  istcomp>z2FIR le
+00002e10: 6e67 7468 2069 7320 6469 6666 6572 656e  ngth is differen
+00002e20: 7420 6672 6f6d 2074 6861 7420 7374 6174  t from that stat
+00002e30: 6564 3a20 7b7d 2021 3d20 7b7d 7267 0000  ed: {} != {}rg..
+00002e40: 0072 5900 0000 2911 7205 0000 0072 0300  .rY...).r....r..
+00002e50: 0000 7204 0000 00da 0772 6573 6f6c 7665  ..r......resolve
+00002e60: da06 7061 7265 6e74 da04 676c 6f62 7252  ..parent..globrR
+00002e70: 0000 00da 094e 616d 6545 7272 6f72 da04  .....NameError..
+00002e80: 6f70 656e da08 7265 6164 6c69 6e65 727d  open..readliner}
+00002e90: 0000 0072 9900 0000 727b 0000 00da 0972  ...r....r{.....r
+00002ea0: 6561 646c 696e 6573 da0c 5275 6e74 696d  eadlines..Runtim
+00002eb0: 6545 7272 6f72 725e 0000 0072 0d00 0000  eErrorr^...r....
+00002ec0: 290a da0a 6465 6369 6d61 7469 6f6e da08  )...decimation..
+00002ed0: 6261 7365 5f64 6972 5a05 6662 6173 65da  base_dirZ.fbase.
+00002ee0: 0866 696c 656e 616d 65da 0166 da01 415a  .filename..f..AZ
+00002ef0: 076e 436f 6566 6673 da06 636f 6566 6673  .nCoeffs..coeffs
+00002f00: da04 6c69 6e65 da05 6465 6c61 7972 1200  ..line..delayr..
+00002f10: 0000 729a 0000 0072 1300 0000 da0d 5f72  ..r....r......_r
+00002f20: 6561 645f 4649 525f 5341 43a5 0100 0073  ead_FIR_SAC....s
+00002f30: 2e00 0000 0004 1401 0c01 0a01 0c01 0801  ................
+00002f40: 0a01 0801 0c01 0c01 0c01 0401 0c01 2601  ..............&.
+00002f50: 0c01 0201 0401 0600 02ff 02ff 0405 0c01  ................
+00002f60: 1201 7a17 4465 6369 6d61 746f 722e 5f72  ..z.Decimator._r
+00002f70: 6561 645f 4649 525f 5341 4363 0700 0000  ead_FIR_SACc....
+00002f80: 0000 0000 0000 0000 0d00 0000 0a00 0000  ................
+00002f90: 4300 0000 7330 0100 0067 007d 0767 007d  C...s0...g.}.g.}
+00002fa0: 087c 016a 0044 005d 907d 0974 01a0 017c  .|.j.D.].}.t...|
+00002fb0: 096a 02a0 03a1 007c 02a0 03a1 00a1 0273  .j.....|.......s
+00002fc0: 2a71 0e7c 096a 0444 005d 6c7d 0a74 01a0  *q.|.j.D.]l}.t..
+00002fd0: 017c 0a6a 02a0 03a1 007c 03a0 03a1 00a1  .|.j.....|......
+00002fe0: 0273 4c71 307c 0a6a 0544 005d 487d 0b74  .sLq0|.j.D.]H}.t
+00002ff0: 01a0 017c 0b6a 06a0 03a1 007c 04a0 03a1  ...|.j.....|....
+00003000: 00a1 0273 6e71 5274 01a0 017c 0b6a 02a0  ...snqRt...|.j..
+00003010: 03a1 007c 05a0 03a1 00a1 0273 8671 527c  ...|.......s.qR|
+00003020: 07a0 077c 0aa1 0101 007c 08a0 077c 0ba1  ...|.....|...|..
+00003030: 0101 0071 5271 3071 0e74 087c 0783 0164  ...qRq0q.t.|...d
+00003040: 016b 0272 d274 0964 027c 029b 0064 037c  .k.r.t.d.|...d.|
+00003050: 039b 0064 037c 049b 0064 037c 059b 0064  ...d.|...d.|...d
+00003060: 049d 0983 0182 0164 0553 0074 087c 0783  .......d.S.t.|..
+00003070: 0164 066b 0472 f874 0964 07a0 0a74 087c  .d.k.r.t.d...t.|
+00003080: 0783 017c 027c 037c 047c 05a1 0583 0182  ...|.|.|.|......
+00003090: 017c 0664 086b 0890 0172 107c 00a0 0b7c  .|.d.k...r.|...|
+000030a0: 0864 0119 00a1 0101 007c 0864 0119 00a0  .d.......|.d....
+000030b0: 0ca1 007d 0c7c 0764 0119 006a 05a0 077c  ...}.|.d...j...|
+000030c0: 0ca1 0101 007c 0c53 0029 0961 c301 0000  .....|.S.).a....
+000030d0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+000030e0: 5374 6174 696f 6e20 2620 4368 616e 6e65  Station & Channe
+000030f0: 6c20 6d61 7463 6869 6e67 206e 6574 776f  l matching netwo
+00003100: 726b 2c20 7374 6174 696f 6e2c 206c 6f63  rk, station, loc
+00003110: 6174 696f 6e2c 2063 6861 6e6e 656c 0a0a  ation, channel..
+00003120: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
+00003130: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
+00003140: 6574 776f 726b 2028 7374 7229 3a20 6e65  etwork (str): ne
+00003150: 7477 6f72 6b20 636f 6465 0a20 2020 2020  twork code.     
+00003160: 2020 2020 2020 2073 7461 7469 6f6e 2028         station (
+00003170: 7374 7229 3a20 7374 6174 696f 6e20 636f  str): station co
+00003180: 6465 0a20 2020 2020 2020 2020 2020 206c  de.            l
+00003190: 6f63 6174 696f 6e20 2873 7472 293a 206c  ocation (str): l
+000031a0: 6f63 6174 696f 6e20 636f 6465 0a20 2020  ocation code.   
+000031b0: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+000031c0: 2028 7374 7229 3a20 6368 616e 6e65 6c20   (str): channel 
+000031d0: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
+000031e0: 206e 6f72 6d61 6c69 7a65 5f66 6972 7320   normalize_firs 
+000031f0: 2862 6f6f 6c29 3a20 6e6f 726d 616c 697a  (bool): normaliz
+00003200: 6573 2061 6e79 2046 4952 2063 6861 6e6e  es any FIR chann
+00003210: 656c 2074 6861 7420 6973 6e27 740a 2020  el that isn't.  
+00003220: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00003230: 7265 6164 790a 0a20 2020 2020 2020 2052  ready..        R
+00003240: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00003250: 2020 2020 2843 6861 6e6e 656c 293a 2064      (Channel): d
+00003260: 7570 6c69 6361 7465 206f 6620 666f 756e  uplicate of foun
+00003270: 6420 6368 616e 6e65 6c2c 2072 6561 6479  d channel, ready
+00003280: 2074 6f20 6d6f 6469 6679 0a20 2020 2020   to modify.     
+00003290: 2020 2072 0100 0000 7a12 7472 6163 6520     r....z.trace 
+000032a0: 7761 7665 666f 726d 6964 2022 725a 0000  waveformid "rZ..
+000032b0: 007a 1822 206e 6f74 2066 6f75 6e64 2069  .z." not found i
+000032c0: 6e20 696e 7665 6e74 6f72 7929 024e 4e72  n inventory).NNr
+000032d0: 0c00 0000 7a29 7b3a 647d 2073 7461 7469  ....z){:d} stati
+000032e0: 6f6e 2d63 6861 6e6e 656c 7320 6d61 7463  on-channels matc
+000032f0: 6865 6420 7b7d 2e7b 7d2e 7b7d 2e7b 7d54  hed {}.{}.{}.{}T
+00003300: 290d da08 6e65 7477 6f72 6b73 da07 666e  )...networks..fn
+00003310: 6d61 7463 6872 2800 0000 7287 0000 00da  matchr(...r.....
+00003320: 0873 7461 7469 6f6e 73da 0863 6861 6e6e  .stations..chann
+00003330: 656c 7372 2900 0000 7282 0000 0072 5200  elsr)...r....rR.
+00003340: 0000 7233 0000 0072 5e00 0000 7275 0000  ..r3...r^...ru..
+00003350: 0072 3100 0000 290d 7211 0000 0072 3500  .r1...).r....r5.
+00003360: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00003370: 0072 2400 0000 722e 0000 0072 af00 0000  .r$...r....r....
+00003380: 72b0 0000 0072 2b00 0000 722c 0000 0072  r....r+...r,...r
+00003390: 3b00 0000 7237 0000 0072 1200 0000 7212  ;...r7...r....r.
+000033a0: 0000 0072 1300 0000 7232 0000 00c2 0100  ...r....r2......
+000033b0: 0073 4800 0000 0011 0401 0401 0a02 1601  .sH.............
+000033c0: 0201 0a01 1601 0201 0a01 0401 0800 06ff  ................
+000033d0: 0403 0201 1601 0201 0a01 1001 0c01 2202  ..............".
+000033e0: 0401 0c01 0201 0401 0600 0200 0200 0200  ................
+000033f0: 02ff 02ff 0405 0a01 0e01 0c01 1001 7a1c  ..............z.
+00003400: 4465 6369 6d61 746f 722e 5f64 7570 6c69  Decimator._dupli
+00003410: 6361 7465 5f63 6861 6e6e 656c 2901 5429  cate_channel).T)
+00003420: 034e 4646 2906 7239 0000 0072 3900 0000  .NFF).r9...r9...
+00003430: 7239 0000 0072 3900 0000 4646 2904 7259  r9...r9...FF).rY
+00003440: 0000 0072 5900 0000 4646 2901 4629 19da  ...rY...FF).F)..
+00003450: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00003460: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00003470: 655f 5fda 075f 5f64 6f63 5f5f da04 6c69  e__..__doc__..li
+00003480: 7374 da0f 5f5f 616e 6e6f 7461 7469 6f6e  st..__annotation
+00003490: 735f 5f72 1000 0000 da04 626f 6f6c da08  s__r......bool..
+000034a0: 7072 6f70 6572 7479 7214 0000 0072 1b00  propertyr....r..
+000034b0: 0000 7238 0000 0072 3c00 0000 da0c 7374  ..r8...r<.....st
+000034c0: 6174 6963 6d65 7468 6f64 7256 0000 0072  aticmethodrV...r
+000034d0: 5800 0000 7234 0000 0072 7500 0000 7261  X...r4...ru...ra
+000034e0: 0000 0072 7600 0000 7260 0000 0072 1700  ...rv...r`...r..
+000034f0: 0000 7218 0000 0072 ac00 0000 7232 0000  ..r....r....r2..
+00003500: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00003510: 7213 0000 0072 0e00 0000 2300 0000 7340  r....r....#...s@
+00003520: 0000 000a 0204 0a08 010c 0202 010a 040a  ................
+00003530: 1200 0000 0000 ff0a 3300 0100 0000 0000  ........3.......
+00003540: 0100 fe0a 2e02 010a 3208 1000 0100 ff0a  ........2.......
+00003550: 1902 010a 280c 0d0c 2808 1508 1108 1c08  ....(...(.......
+00003560: 1e00 ff72 0e00 0000 2919 72b4 0000 0072  ...r....).r....r
+00003570: 9200 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
+00003580: 7372 0200 0000 da07 696e 7370 6563 7472  sr......inspectr
+00003590: 0300 0000 7204 0000 00da 0770 6174 686c  ....r......pathl
+000035a0: 6962 7205 0000 0072 5300 0000 72ae 0000  ibr....rS...r...
+000035b0: 0072 7100 0000 da05 6e75 6d70 7972 0600  .rq.....numpyr..
+000035c0: 0000 da11 6f62 7370 792e 636f 7265 2e73  ....obspy.core.s
+000035d0: 7472 6561 6d72 0700 0000 7208 0000 00da  treamr....r.....
+000035e0: 106f 6273 7079 2e63 6f72 652e 7472 6163  .obspy.core.trac
+000035f0: 6572 0900 0000 da14 6f62 7370 792e 636f  er......obspy.co
+00003600: 7265 2e69 6e76 656e 746f 7279 720a 0000  re.inventoryr...
+00003610: 0072 0b00 0000 728a 0000 0072 0d00 0000  .r....r....r....
+00003620: 720e 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00003630: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
+00003640: 6c65 3e02 0000 0073 1c00 0000 0410 0801  le>....s........
+00003650: 0c01 1001 0c01 0801 0801 0802 0c01 1001  ................
+00003660: 0c01 1003 0c03 0201                      ........
```

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/transfer_function.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/transfer_function.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/__pycache__/utils.cpython-38.pyc` & `tiskit-py-0.3.3/tiskit/decimate/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/decimate_SDS.py` & `tiskit-py-0.3.3/tiskit/decimate/decimate_SDS.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,45 +32,44 @@
     decimator = Decimator(decim_list)
     output_sample_rate = input_sample_rate/decimator.decimation_factor
     in_band_code = Decimator.get_band_code('B', input_sample_rate)
     out_band_code = Decimator.get_band_code('B', output_sample_rate)
     logging.info('output sampling rate will be {:g} sps, band code will be {}'
                  .format(output_sample_rate, out_band_code))
     if in_band_code == out_band_code:
-        raise ValueError('identical input & output band codes: {in_band_code}')
+        raise ValueError(f'identical input & output band codes: {in_band_code}')
 
     for year_dir in [x for x in SDS_root.iterdir() if x.is_dir()]:
-        logging.info('Working on year {str(year_dir.name)}')
+        logging.info(f' year={str(year_dir.name)}')
         for net_dir in [x for x in year_dir.iterdir() if x.is_dir()]:
-            logging.info('\tWorking on net {str(net_dir.name)}')
+            logging.info(f'\tnet={str(net_dir.name)}')
             for sta_dir in [x for x in net_dir.iterdir() if x.is_dir()]:
-                logging.info('\t\tWorking on station {str(sta_dir.name)}')
+                logging.info(f'\t\tstation={str(sta_dir.name)}')
                 for cha_dir in [x for x in sta_dir.iterdir() if x.is_dir()]:
-                    logging.info('\t\t\tWorking on channel {}'
-                                 .format(str(sta_dir.name)))
+                    logging.info(f'\t\t\tchannel={str(cha_dir.name)}')
                     cha_name = cha_dir.name
                     if not cha_name[0] == in_band_code:
                         continue
                     out_cha_dir = (sta_dir / (out_band_code + cha_name[1:]))
                     out_cha_dir.mkdir()
                     logging.info('\t\t\t\tCreating output channel dir "{}"'
                                  .format(out_cha_dir.name))
-                    files = cha_dir.glob(f'*.{cha_name}.*')
-                    logging.info('\t\t\t\t{len(files):d} files to process')
+                    files = list(cha_dir.glob(f'*.{cha_name}.*'))
+                    logging.info(f'\t\t\t\t{len(files):d} files to process')
                     for f in files:
                         stream = read(str(f), 'MSEED')
                         if stream[0].stats.npts % decimator.decimation_factor == 0:
                             ValueError(
                                 f"day's stream length ({stream[0].stats.npts})"
                                 " is not divisible by decimator "
                                 f"({decimator.decimation_factor})")
                         if stream[0].stats.sampling_rate != input_sample_rate:
                             logging.warning(
                                 f"{str(f)} first block's sampling rate != "
-                                "{input_sample_rate}, skipping...")
+                                f"{input_sample_rate}, skipping...")
                         net, sta, loc, ich, typ, yr, dy = str(f.name).split('.')
                         d_stream = decimator.decimate(stream)
                         och = out_band_code + ich[1:]
                         outfname = f'{net}.{sta}.{loc}.{och}.{typ}.{yr}.{dy}'
                         d_stream.write(out_cha_dir / outfname, 'MSEED')
                     inv = decimator.update_inventory(inv, stream)
     return inv
```

### Comparing `tiskit-py-0.3.2/tiskit/decimate/decimator.py` & `tiskit-py-0.3.3/tiskit/decimate/decimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,28 @@
     verbose: bool = False
 
     @property
     def decimation_factor(self):
         """Total decimation (product of `decimates`)"""
         return prod(self.decimates)
 
-    def decimate(self, data):
+    def decimate(self, data, keep_dtype=True):
         """
         Apply decimator to data
 
         Args:
             data (:class:`obspy.Stream` or :class:`obspy.Trace`): waveform data
+            keep_dformat (bool): force output data format to be the same as
+                the input data_format
         """
+        self.keep_dtype = keep_dtype
         if isinstance(data, Stream):
             return self._run_stream(data)
         if isinstance(data, Trace):
-            return self._run_stream(Stream([data]))[0]
+            return self._run_trace(data)
         else:
             raise TypeError("data is not a Stream or Trace")
 
     def update_inventory(
         self, inv, st=None, normalize_firs=False, quiet=False
     ):
         """
@@ -368,15 +371,15 @@
             if i_u.upper() == 'PA':
                 cha.response.instrument_sensitivity.input_units = "M/S"
                 cha.response.recalculate_overall_sensitivity()
                 cha.response.instrument_sensitivity.input_units = i_u
 
     def _run_stream(self, stream):
         """
-        Return decimated obspy stream
+        Decimate obspy Stream
         """
         if not isinstance(stream, Stream):
             raise ValueError("input stream is not an obspy Stream!")
         st = stream.copy()
         newtr = []
         for tr in st.traces:
             newtr.append(self._run_trace(tr))
@@ -385,29 +388,32 @@
             print("New data has {} samples".format([tr.data.size
                                                     for tr in st]))
         st.verify()
         return st
 
     def _run_trace(self, trace):
         """
-        Decimate obspy trace
+        Decimate obspy Trace
         """
         if not isinstance(trace, Trace):
             raise ValueError("input trace is not an obspy Trace!")
+        dtype = trace.data.dtype
         tr = trace.copy()
         sr = tr.stats.sampling_rate
         if self.verbose:
             print("Decimating data from {:g} to {:g} Hz ({:d}x)... "
                   .format(sr, sr / self.decimation_factor,
                           self.decimation_factor))
         tic = time.time()
         for d in self.decimates:
             fir_filter = FIRFilter.from_SAC(d)
             tr.data = fir_filter.convolve(tr.data)
             tr.decimate(d, no_filter=True)
+        if self.keep_dtype is True and not tr.data.dtype == dtype:
+            tr.data = tr.data.astype(dtype)
         tr.stats.channel, tr.stats.location = self._get_chan_loc(
             tr.stats.channel,
             tr.stats.location,
             tr.stats.sampling_rate * self.decimation_factor)
         if self.verbose:
             print("Took {:.1f} seconds".format(time.time() - tic))
         return tr
```

### Comparing `tiskit-py-0.3.2/tiskit/decimate/fir_filter.py` & `tiskit-py-0.3.3/tiskit/decimate/fir_filter.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec2` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec2`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec3` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec3`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec4` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec4`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec5` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec5`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec6` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec6`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/decimate/sac_fir/dec7` & `tiskit-py-0.3.3/tiskit/decimate/sac_fir/dec7`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/fir_corr/fir2caus.py` & `tiskit-py-0.3.3/tiskit/fir_corr/fir2caus.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/read_mseed.py` & `tiskit-py-0.3.3/tiskit/read_mseed.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/rptransient/dirac_comb.py` & `tiskit-py-0.3.3/tiskit/rptransient/dirac_comb.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/rptransient/periodic_transient.py` & `tiskit-py-0.3.3/tiskit/rptransient/periodic_transient.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/rptransient/transients.py` & `tiskit-py-0.3.3/tiskit/rptransient/transients.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/rptransient/utils.py` & `tiskit-py-0.3.3/tiskit/rptransient/utils.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/spectral_density/Peterson_noise_model.py` & `tiskit-py-0.3.3/tiskit/spectral_density/Peterson_noise_model.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/spectral_density/spectral_density.py` & `tiskit-py-0.3.3/tiskit/spectral_density/spectral_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,14 +384,16 @@
 
         Args:
             in_channel (str): input channel name
             out_channel (str): output channel name
         Returns:
             (:class:`numpy.ndarray`): cross-spectral density function
         """
+        if in_channel == out_channel:
+            return self.autospect(in_channel)
         ichn = self.channel_name(in_channel, "in_channel")
         ochn = self.channel_name(out_channel, "out_channel")
         return (self._ds["spectra"].sel(input=ichn,
                                         output=ochn).values.flatten())
 
     def channel_name(self, channel, ch_identifier='chname'):
         """
```

### Comparing `tiskit-py-0.3.2/tiskit/spectral_density/utils.py` & `tiskit-py-0.3.3/tiskit/spectral_density/utils.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/time_spans.py` & `tiskit-py-0.3.3/tiskit/time_spans.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit/transfer_functions.py` & `tiskit-py-0.3.3/tiskit/transfer_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2021 Wayne Crawford
 import pickle
 import fnmatch  # Allows Unix filename pattern matching
+import copy
 
 import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
 
 from .spectral_density.utils import coherence_significance_level
 from .spectral_density import SpectralDensity
@@ -121,14 +122,20 @@
     def __str__(self):
         s = "TransferFunctions object:\n"
         s += f"\tinput_channel='{self.input_channel}'\n"
         s += f"\toutput_channels={self.output_channels}\n"
         s += f"\tnoise_channels={self.noise_channels}\n"
         s += f"\tn_windows={self.n_windows}"
         return s
+    
+    def copy(self):
+        return copy.copy(self)
+
+    def deepcopy(self):
+        return copy.deepcopy(self)
 
     @property
     def freqs(self):
         """Transfer function frequencies"""
         return self._ds.coords["f"].values
 
     @property
@@ -233,14 +240,32 @@
 
         Divide count-based response by this to get unit-based response
         Multiply unit-based response by this to get count-based response
         """
         oc = self._match_out_chan(output_channel)
         return np.squeeze(self._ds["response"].sel(output=oc).values)
 
+    def to_norm_compliance(self, water_depth):
+        """
+        Change tfs from m/s^2 / Pa to 1 / Pa by multiplying by k / omega^2
+        """
+        if not self.input_units.upper() == 'PA':
+            raise ValueError(f'{self.input_units=}, not "PA"')
+        om = np.pi * self.freqs
+        k = _gravd(om, water_depth)
+        tf_multiplier = k / (om**2)
+        for oc in self.output_channels:
+            if not self.output_units(oc).upper() == 'M/S^2':
+                raise ValueError('{self.output_units(oc)=}, not "M/2^2"')
+            # 'value' is in physical units, have to change response so that
+            # value w.r.t. counts remains constant
+            self._ds["value"].loc[dict(output=oc)] = self.frf(oc) * tf_multiplier
+            self._ds["response"].loc[dict(output=oc)] = self.response(oc) / tf_multiplier
+            self._ds.coords["out_units"].loc[dict(output=oc)] = '1'
+
     def uncert_mult(self, output_channel):
         """Return transfer function uncertainty as a fraction of the transfer function"""
         oc = self._match_out_chan(output_channel)
         return np.squeeze(self._ds["uncert_mult"].sel(output=oc).values)
 
     def uncertainty(self, output_channel):
         """Return transfer function uncertainty for the given output channel"""
@@ -271,14 +296,17 @@
 
         # Validate out_chan
         if out_chans is None:
             # Select all channels except in_chan
             out_chans = [x for x in sdm.channel_names if not x == in_chan]
         if not isinstance(out_chans, list):
             raise TypeError("Error: out_chans is not a list")
+        else:
+            out_chans = [fnmatch.filter(sdm.channel_names, oc)[0]
+                         for oc in out_chans]
         return in_chan, out_chans
 
     def _match_out_chan(self, value):
         """
         Returns output_channel matching string (may have *,? wildcards)
 
         Error if there is not exactly one response
@@ -373,21 +401,22 @@
         H = self._zero_bad(H, coh, n_to_reject, f, min_freq, max_freq)
 
         # Calculate uncertainty
         # Crawford et al. 1991 eqn 4,  from BP2010 eqn 9.90
         H_err_mult = np.sqrt((np.ones(coh.shape) - coh) / (2*coh*self.n_windows))
         return H, H_err_mult, corr_mult
 
-    def plot(self, errorbars=True, show=True):
+    def plot(self, errorbars=True, show=True, outfile=None):
         """
         Plot transfer functions
 
         Args:
             errorbars (bool): plot error bars
             show (bool): show on the screen
+            outfile (str): save figure to this filename
         Returns:
             (numpy.ndarray): array of axis pairs (amplitude, phase)
         """
         inp = self.input_channel
         outputs = self.output_channels
         rows = 1
         cols = len(outputs)
@@ -397,14 +426,16 @@
         for out_chan, j in zip(outputs, range(len(outputs))):
             axa, axp = self.plot_one(inp, out_chan, fig, (rows, cols),
                                      (0, j), show_ylabel=j == 0,
                                      errorbars=errorbars,
                                      title=f"{out_chan}/{in_suffix}",
                                      show_xlabel=True)
         ax_array[0, j] = (axa, axp)
+        if outfile:
+            plt.savefig(outfile)
         if show:
             plt.show()
         return ax_array
 
     def _plot_progress(self, spect_dens, show=True):
         """
         Plot transfer functions and the coherences that made them
@@ -591,7 +622,66 @@
                         goods,
                         goods_orig.roll(
                             f=-both_sides - 1, fill_value=goods_orig[-1]
                         ),
                     )
             H[~goods] = 0
         return H
+
+
+def _gravd(W, h):
+    """
+    Linear ocean surface gravity wave dispersion
+
+    Args:
+        W (:class:`numpy.ndarray`): angular frequencies (rad/s)
+        h (float): water depth (m)
+
+    Returns:
+        K (:class:`numpy.ndarray`): wavenumbers (rad/m)
+    """
+    # W must be array
+    if not isinstance(W, np.ndarray):
+        W = np.array([W])
+    G = 9.79329
+    N = len(W)
+    W2 = W*W
+    kDEEP = W2/G
+    kSHAL = W/(np.sqrt(G*h))
+    erDEEP = np.ones(np.shape(W)) - G*kDEEP*_dtanh(kDEEP*h)/W2
+    one = np.ones(np.shape(W))
+    d = np.copy(one)
+    done = np.zeros(np.shape(W))
+    nd = np.where(done == 0)
+
+    k1 = np.copy(kDEEP)
+    k2 = np.copy(kSHAL)
+    e1 = np.copy(erDEEP)
+    ktemp = np.copy(done)
+    e2 = np.copy(done)
+
+    while True:
+        e2[nd] = one[nd] - G*k2[nd] * _dtanh(k2[nd]*h)/W2[nd]
+        d = e2*e2
+        done = d < 1e-20
+        if done.all():
+            K = k2
+            break
+        nd = np.where(done == 0)
+        ktemp[nd] = k1[nd]-e1[nd]*(k2[nd]-k1[nd])/(e2[nd]-e1[nd])
+        k1[nd] = k2[nd]
+        k2[nd] = ktemp[nd]
+        e1[nd] = e2[nd]
+    return K
+
+def _dtanh(x):
+    """
+    Stable hyperbolic tangent
+
+    Args:
+        x (:class:`numpy.ndarray`)
+    """
+    a = np.exp(x*(x <= 50))
+    one = np.ones(np.shape(x))
+
+    y = (abs(x) > 50) * (abs(x)/x) + (abs(x) <= 50)*((a-one/a) / (a+one/a))
+    return y
```

### Comparing `tiskit-py-0.3.2/tiskit/utils/seis_rotate.py` & `tiskit-py-0.3.3/tiskit/utils/seis_rotate.py`

 * *Files identical despite different names*

### Comparing `tiskit-py-0.3.2/tiskit_py.egg-info/PKG-INFO` & `tiskit-py-0.3.3/tiskit_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tiskit-py
-Version: 0.3.2
-Summary: TIme Series  toolKIT
+Version: 0.3.3
+Summary: TIme Series toolKIT
 Home-page: https://github.com/WayneCrawford/tiskit
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: oceanography,marine,OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tiskit-py-0.3.2/tiskit_py.egg-info/SOURCES.txt` & `tiskit-py-0.3.3/tiskit_py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 tiskit/decimate/decimator.py
 tiskit/decimate/fir_filter.py
 tiskit/decimate/version.py
 tiskit/decimate/__pycache__/FIR_filter.cpython-38.pyc
 tiskit/decimate/__pycache__/PSD.cpython-38.pyc
 tiskit/decimate/__pycache__/Peterson_noise_model.cpython-38.pyc
 tiskit/decimate/__pycache__/__init__.cpython-38.pyc
+tiskit/decimate/__pycache__/__init__.cpython-39.pyc
 tiskit/decimate/__pycache__/coherence.cpython-38.pyc
 tiskit/decimate/__pycache__/decimate.cpython-38.pyc
 tiskit/decimate/__pycache__/decimate_SDS.cpython-38.pyc
 tiskit/decimate/__pycache__/decimator.cpython-38.pyc
+tiskit/decimate/__pycache__/decimator.cpython-39.pyc
+tiskit/decimate/__pycache__/fir_filter.cpython-39.pyc
 tiskit/decimate/__pycache__/transfer_function.cpython-38.pyc
 tiskit/decimate/__pycache__/utils.cpython-38.pyc
 tiskit/decimate/sac_fir/dec2
 tiskit/decimate/sac_fir/dec3
 tiskit/decimate/sac_fir/dec4
 tiskit/decimate/sac_fir/dec5
 tiskit/decimate/sac_fir/dec6
```

