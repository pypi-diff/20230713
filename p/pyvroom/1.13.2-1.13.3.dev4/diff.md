# Comparing `tmp/pyvroom-1.13.2.tar.gz` & `tmp/pyvroom-1.13.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvroom-1.13.2.tar", last modified: Tue Jun 27 20:01:15 2023, max compression
+gzip compressed data, was "pyvroom-1.13.3.dev4.tar", last modified: Thu Jul 13 12:43:51 2023, max compression
```

## Comparing `pyvroom-1.13.2.tar` & `pyvroom-1.13.3.dev4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.004866 pyvroom-1.13.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.008866 pyvroom-1.13.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/main_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-27 20:01:05.000000 pyvroom-1.13.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 20:01:05.000000 pyvroom-1.13.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 20:01:05.000000 pyvroom-1.13.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-27 20:01:05.000000 pyvroom-1.13.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 20:01:15.016867 pyvroom-1.13.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-27 20:01:05.000000 pyvroom-1.13.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 20:01:05.000000 pyvroom-1.13.2/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 20:01:05.000000 pyvroom-1.13.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-27 20:01:05.000000 pyvroom-1.13.2/conanfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-27 20:01:05.000000 pyvroom-1.13.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-27 20:01:05.000000 pyvroom-1.13.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-27 20:01:15.020866 pyvroom-1.13.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-27 20:01:05.000000 pyvroom-1.13.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.008866 pyvroom-1.13.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/_vroom.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/_main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/amount.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/break.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/exception.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/generic/matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/input/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/input/input.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/input/vehicle_step.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/job.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/location.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/bind/solution/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/route.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/solution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/step.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/solution/summary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/time_window.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/bind/vehicle.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.012866 pyvroom-1.13.2/src/pyvroom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-27 20:01:15.000000 pyvroom-1.13.2/src/pyvroom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 20:01:14.000000 pyvroom-1.13.2/src/pyvroom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/break_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/forced_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/input/vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/location.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/src/vroom/solution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/solution/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-27 20:01:05.000000 pyvroom-1.13.2/src/vroom/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 20:01:15.016867 pyvroom-1.13.2/test/input/
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/input/test_vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_break.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_file_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_libvroom_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-27 20:01:05.000000 pyvroom-1.13.2/test/test_vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.048336 pyvroom-1.13.3.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.048336 pyvroom-1.13.3.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/.github/workflows/main_push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/conanfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/_vroom.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/bind/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/amount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/break.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/exception.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/bind/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/generic/matrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/bind/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/input/input.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/input/vehicle_step.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/location.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/bind/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/solution/route.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/solution/solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/solution/step.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/solution/summary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/time_window.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/bind/vehicle.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.052336 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:43:50.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 12:43:51.000000 pyvroom-1.13.3.dev4/src/pyvroom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/src/vroom/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/break_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/src/vroom/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/input/forced_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/input/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/input/vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/location.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/src/vroom/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/solution/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/src/vroom/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:43:51.056336 pyvroom-1.13.3.dev4/test/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/input/test_vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_libvroom_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-13 12:43:38.000000 pyvroom-1.13.3.dev4/test/test_vehicle.py
```

### Comparing `pyvroom-1.13.2/.github/workflows/main_push.yml` & `pyvroom-1.13.3.dev4/.github/workflows/main_push.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/.github/workflows/pull_request.yml` & `pyvroom-1.13.3.dev4/.github/workflows/pull_request.yml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         submodules: recursive
 
     - uses: "actions/setup-python@v2"
       with:
         python-version: "3.7"
 
     - name: "Install system dependencies"
-      run: sudo apt update -y && sudo apt install -y libssl-dev libasio-dev
+      run: sudo apt update -y && sudo apt install -y libssl-dev libasio-dev libglpk-dev glpk-utils
 
     - name: "Install python environment"
       run: |
         python -m pip install black coverage flake8 mypy pytest
         python -m pip install -r build-requirements.txt
 
     - name: "Install pyvroom"
```

### Comparing `pyvroom-1.13.2/.github/workflows/release.yml` & `pyvroom-1.13.3.dev4/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
       fail-fast: false
       matrix:
         include:
           - image: ubuntu-latest
             platform: linux
           - image: macos-latest
             platform: macos
-          - image: windows-latest
-            platform: windows
+          # - image: windows-latest
+          #   platform: windows
 
     steps:
     - uses: actions/checkout@v2
       with:
         submodules: recursive
 
     - name: Cache Conan
```

### Comparing `pyvroom-1.13.2/.gitignore` & `pyvroom-1.13.3.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/LICENSE` & `pyvroom-1.13.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/Makefile` & `pyvroom-1.13.3.dev4/Makefile`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/PKG-INFO` & `pyvroom-1.13.3.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvroom
-Version: 1.13.2
+Version: 1.13.3.dev4
 Summary: Vehicle routing open-source optimization machine (VROOM)
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyvroom-1.13.2/README.rst` & `pyvroom-1.13.3.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/pyproject.toml` & `pyvroom-1.13.3.dev4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -28,21 +28,24 @@
 archs = "native"
 
 [tool.cibuildwheel.linux]
 before-all = """
 yum update -y
 yum install -y epel-release
 yum install -y openssl-devel asio-devel
+yum install -y glpk-devel glpk-utils
 """
 
 [[tool.cibuildwheel.overrides]]
 select = "*musllinux*"
 before-all = """
 apk add asio-dev
 apk add openssl-dev
+apk add glpk
 """
 
 [tool.cibuildwheel.macos]
 
 before-all = """
 brew install asio
+brew install glpk
 """
```

### Comparing `pyvroom-1.13.2/setup.cfg` & `pyvroom-1.13.3.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/setup.py` & `pyvroom-1.13.3.dev4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,35 +18,38 @@
 if platform.system() == "Windows":
     extra_compile_args = [
         "-DNOGDI",
         "-DNOMINMAX",
         "-DWIN32_LEAN_AND_MEAN",
         "-DASIO_STANDALONE",
         "-DUSE_PYTHON_BINDINGS",
-        "-DUSE_ROUTING=true"
+        "-DUSE_ROUTING=true",
+        "-DUSE_LIBGLPK=true",
     ]
     extra_link_args = []
 
 else:  # anything *nix
     extra_compile_args = [
         "-MMD",
         "-MP",
         "-Wextra",
         "-Wpedantic",
         "-Wall",
         "-O3",
         "-DASIO_STANDALONE",
         "-DNDEBUG",
         "-DUSE_PYTHON_BINDINGS",
-        "-DUSE_ROUTING=true"
+        "-DUSE_ROUTING=true",
+        "-DUSE_LIBGLPK=true",
     ]
     extra_link_args = [
         "-lpthread",
         "-lssl",
         "-lcrypto",
+        "-lglpk",
     ]
 
     if platform.system() == "Darwin":
         # Homebrew puts include folders in weird places.
         include_dirs.append("/usr/local/opt/openssl@1.1/include")
         extra_link_args.insert(0, "-L/usr/local/opt/openssl@1.1/lib")
```

### Comparing `pyvroom-1.13.2/src/_vroom.cpp` & `pyvroom-1.13.3.dev4/src/_vroom.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 #include "algorithms/kruskal.cpp"
 #include "algorithms/munkres.cpp"
 
 #include "algorithms/heuristics/heuristics.cpp"
 #include "algorithms/local_search/local_search.cpp"
 #include "algorithms/local_search/operator.cpp"
-#include "algorithms/validation/check.h"
+#include "algorithms/validation/check.cpp"
+#include "algorithms/validation/choose_ETA.cpp"
 
 // #include "routing/libosrm_wrapper.cpp"
 #include "routing/http_wrapper.cpp"
 #include "routing/ors_wrapper.cpp"
 #include "routing/osrm_routed_wrapper.cpp"
 #include "routing/valhalla_wrapper.cpp"
```

### Comparing `pyvroom-1.13.2/src/bind/_main.cpp` & `pyvroom-1.13.3.dev4/src/bind/_main.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/amount.cpp` & `pyvroom-1.13.3.dev4/src/bind/amount.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/break.cpp` & `pyvroom-1.13.3.dev4/src/bind/break.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/enums.cpp` & `pyvroom-1.13.3.dev4/src/bind/enums.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/generic/matrix.cpp` & `pyvroom-1.13.3.dev4/src/bind/generic/matrix.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/input/input.cpp` & `pyvroom-1.13.3.dev4/src/bind/input/input.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/input/vehicle_step.cpp` & `pyvroom-1.13.3.dev4/src/bind/input/vehicle_step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/job.cpp` & `pyvroom-1.13.3.dev4/src/bind/job.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/location.cpp` & `pyvroom-1.13.3.dev4/src/bind/location.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/solution/route.cpp` & `pyvroom-1.13.3.dev4/src/bind/solution/route.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/solution/solution.cpp` & `pyvroom-1.13.3.dev4/src/bind/solution/solution.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/solution/step.cpp` & `pyvroom-1.13.3.dev4/src/bind/solution/step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/solution/summary.cpp` & `pyvroom-1.13.3.dev4/src/bind/solution/summary.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/time_window.cpp` & `pyvroom-1.13.3.dev4/src/bind/time_window.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/bind/vehicle.cpp` & `pyvroom-1.13.3.dev4/src/bind/vehicle.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/pyvroom.egg-info/PKG-INFO` & `pyvroom-1.13.3.dev4/src/pyvroom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvroom
-Version: 1.13.2
+Version: 1.13.3.dev4
 Summary: Vehicle routing open-source optimization machine (VROOM)
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyvroom-1.13.2/src/pyvroom.egg-info/SOURCES.txt` & `pyvroom-1.13.3.dev4/src/pyvroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/__init__.py` & `pyvroom-1.13.3.dev4/src/vroom/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/amount.py` & `pyvroom-1.13.3.dev4/src/vroom/amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/break_.py` & `pyvroom-1.13.3.dev4/src/vroom/break_.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/input/forced_service.py` & `pyvroom-1.13.3.dev4/src/vroom/input/forced_service.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/input/input.py` & `pyvroom-1.13.3.dev4/src/vroom/input/input.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/input/vehicle_step.py` & `pyvroom-1.13.3.dev4/src/vroom/input/vehicle_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,18 +462,26 @@
             assert service_after is None
             assert service_before is None
 
             id = step_type._id
             if step_type._step_type in (_vroom.STEP_TYPE.START, _vroom.STEP_TYPE.END):
                 assert id == 0
                 id = None
+            
             service_at = step_type._forced_service._service_at
             service_after = step_type._forced_service._service_after
             service_before = step_type._forced_service._service_before
 
+            if service_at:
+                service_at = _vroom.scale_to_user_duration(service_at)
+            if service_after:
+                service_after = _vroom.scale_to_user_duration(service_after)
+            if service_before:
+                service_before = _vroom.scale_to_user_duration(service_before)
+
             if step_type._step_type == _vroom.STEP_TYPE.JOB:
                 step_type_map = {
                     _vroom.JOB_TYPE.SINGLE: VEHICLE_STEP_TYPE.SINGLE,
                     _vroom.JOB_TYPE.DELIVERY: VEHICLE_STEP_TYPE.DELIVERY,
                     _vroom.JOB_TYPE.PICKUP: VEHICLE_STEP_TYPE.PICKUP,
                 }
                 step_type = step_type_map[step_type._job_type]
```

### Comparing `pyvroom-1.13.2/src/vroom/job.py` & `pyvroom-1.13.3.dev4/src/vroom/job.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/location.py` & `pyvroom-1.13.3.dev4/src/vroom/location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/solution/solution.py` & `pyvroom-1.13.3.dev4/src/vroom/solution/solution.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/time_window.py` & `pyvroom-1.13.3.dev4/src/vroom/time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/src/vroom/vehicle.py` & `pyvroom-1.13.3.dev4/src/vroom/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             time_window=(TimeWindow() if time_window is None else TimeWindow(time_window)),
             breaks=[Break(break_) for break_ in breaks],
             description=str(description),
             costs=costs,
             speed_factor=self._speed_factor,
             max_tasks=max_tasks,
             max_travel_time=max_travel_time,
-            steps=[VehicleStep(step) for step in steps],
+            steps=steps,
         )
         assert isinstance(self.capacity, Amount)
 
     def __repr__(self) -> str:
         args = [f"{self.id}"]
         if self.start is not None:
             if isinstance(self.start, Location):
```

### Comparing `pyvroom-1.13.2/test/input/test_vehicle_step.py` & `pyvroom-1.13.3.dev4/test/input/test_vehicle_step.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_amount.py` & `pyvroom-1.13.3.dev4/test/test_amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_break.py` & `pyvroom-1.13.3.dev4/test/test_break.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_file_handle.py` & `pyvroom-1.13.3.dev4/test/test_file_handle.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_job.py` & `pyvroom-1.13.3.dev4/test/test_job.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_libvroom_examples.py` & `pyvroom-1.13.3.dev4/test/test_libvroom_examples.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_location.py` & `pyvroom-1.13.3.dev4/test/test_location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_time_window.py` & `pyvroom-1.13.3.dev4/test/test_time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.2/test/test_vehicle.py` & `pyvroom-1.13.3.dev4/test/test_vehicle.py`

 * *Files identical despite different names*

