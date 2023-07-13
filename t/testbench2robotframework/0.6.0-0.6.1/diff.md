# Comparing `tmp/testbench2robotframework-0.6.0.tar.gz` & `tmp/testbench2robotframework-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testbench2robotframework-0.6.0.tar", last modified: Mon Jul 10 17:12:25 2023, max compression
+gzip compressed data, was "dist\testbench2robotframework-0.6.1.tar", last modified: Thu Jul 13 18:16:20 2023, max compression
```

## Comparing `testbench2robotframework-0.6.0.tar` & `testbench2robotframework-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,81 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.598090 testbench2robotframework-0.6.0/
--rwxr-xr-x   0 rener      (502) wheel        (0)      133 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/CreatePiPWheel.bat
--rwxr-xr-x   0 rener      (502) wheel        (0)      133 2023-02-02 12:59:06.000000 testbench2robotframework-0.6.0/CreatePiPWheel.sh
--rw-r--r--   0 rener      (502) wheel        (0)     2511 2023-07-10 10:03:03.000000 testbench2robotframework-0.6.0/DEVELOPMENT.md
--rw-r--r--   0 rener      (502) wheel        (0)    11357 2023-02-02 13:01:04.000000 testbench2robotframework-0.6.0/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      275 2022-11-28 14:39:21.000000 testbench2robotframework-0.6.0/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)    15345 2023-07-10 17:12:25.598207 testbench2robotframework-0.6.0/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)    14921 2023-02-02 12:59:35.000000 testbench2robotframework-0.6.0/README.md
--rw-r--r--   0 rener      (502) wheel        (0)     1028 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/config.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.591794 testbench2robotframework-0.6.0/images/
--rw-r--r--   0 rener      (502) wheel        (0)     5625 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/LibrarySubdivision.PNG
--rw-r--r--   0 rener      (502) wheel        (0)      167 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/Unbenannt.PNG
--rw-r--r--   0 rener      (502) wheel        (0)    29769 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/generated.png
--rw-r--r--   0 rener      (502) wheel        (0)     5625 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/libraries.PNG
--rw-r--r--   0 rener      (502) wheel        (0)     5627 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/resources.PNG
--rw-r--r--   0 rener      (502) wheel        (0)     6384 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/rfLibraryRootsTestBench.PNG
--rw-r--r--   0 rener      (502) wheel        (0)     5407 2022-11-03 23:53:27.000000 testbench2robotframework-0.6.0/images/testbench_rfLibraryRegex.PNG
--rw-r--r--   0 rener      (502) wheel        (0)     4944 2022-11-03 23:53:27.000000 testbench2robotframework-0.6.0/images/testbench_rfResourceRegex.PNG
--rw-r--r--   0 rener      (502) wheel        (0)    13816 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/images/testthemen.PNG
--rw-r--r--   0 rener      (502) wheel        (0)     2392 2023-07-10 17:07:51.000000 testbench2robotframework-0.6.0/pyproject.toml
--rw-r--r--   0 rener      (502) wheel        (0)     1623 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/requirements.txt
--rw-r--r--   0 rener      (502) wheel        (0)      923 2023-07-10 17:12:25.598585 testbench2robotframework-0.6.0/setup.cfg
--rw-r--r--   0 rener      (502) wheel        (0)       69 2022-10-26 13:43:50.000000 testbench2robotframework-0.6.0/setup.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.595711 testbench2robotframework-0.6.0/testbench2robotframework/
--rw-r--r--   0 rener      (502) wheel        (0)      678 2023-07-10 15:51:18.000000 testbench2robotframework-0.6.0/testbench2robotframework/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)     1679 2023-07-10 13:09:41.000000 testbench2robotframework-0.6.0/testbench2robotframework/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)     5888 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/config.py
--rw-r--r--   0 rener      (502) wheel        (0)     5226 2023-07-10 16:55:23.000000 testbench2robotframework-0.6.0/testbench2robotframework/json_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     1144 2023-07-10 13:24:22.000000 testbench2robotframework-0.6.0/testbench2robotframework/json_writer.py
--rw-r--r--   0 rener      (502) wheel        (0)      878 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/log.py
--rw-r--r--   0 rener      (502) wheel        (0)    23595 2023-07-10 10:40:18.000000 testbench2robotframework-0.6.0/testbench2robotframework/model.py
--rw-r--r--   0 rener      (502) wheel        (0)    28537 2023-07-10 15:28:36.000000 testbench2robotframework-0.6.0/testbench2robotframework/result_writer.py
--rw-r--r--   0 rener      (502) wheel        (0)      968 2023-07-10 14:57:23.000000 testbench2robotframework-0.6.0/testbench2robotframework/robotframework2testbench.py
--rw-r--r--   0 rener      (502) wheel        (0)    28269 2023-07-10 17:10:29.000000 testbench2robotframework-0.6.0/testbench2robotframework/testbench2rf.py
--rw-r--r--   0 rener      (502) wheel        (0)     1164 2023-02-03 13:47:35.000000 testbench2robotframework-0.6.0/testbench2robotframework/testbench2robotframework.py
--rw-r--r--   0 rener      (502) wheel        (0)     1789 2023-07-10 15:29:48.000000 testbench2robotframework-0.6.0/testbench2robotframework/testsuite_write.py
--rw-r--r--   0 rener      (502) wheel        (0)     6979 2023-07-10 15:48:25.000000 testbench2robotframework-0.6.0/testbench2robotframework/utils.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.596856 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)    15345 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     1473 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      132 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-02-03 13:42:07.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/not-zip-safe
--rw-r--r--   0 rener      (502) wheel        (0)      120 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       25 2023-07-10 17:12:25.000000 testbench2robotframework-0.6.0/testbench2robotframework.egg-info/top_level.txt
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.597569 testbench2robotframework-0.6.0/tests/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.587396 testbench2robotframework-0.6.0/tests/test_data/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-07-10 17:12:25.597944 testbench2robotframework-0.6.0/tests/test_data/configurations/
--rw-r--r--   0 rener      (502) wheel        (0)     1150 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_data/configurations/invalid_config.json
--rw-r--r--   0 rener      (502) wheel        (0)     1128 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_data/configurations/valid_config.json
--rw-r--r--   0 rener      (502) wheel        (0)      227 2022-07-13 23:03:21.000000 testbench2robotframework-0.6.0/tests/test_missing_files.py
--rw-r--r--   0 rener      (502) wheel        (0)      415 2022-10-26 13:44:46.000000 testbench2robotframework-0.6.0/tests/test_robot_files_should_not_contain_invalid_characters.py
--rw-r--r--   0 rener      (502) wheel        (0)      928 2022-11-01 23:24:18.000000 testbench2robotframework-0.6.0/tests/test_zip_file_generation.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.939087 testbench2robotframework-0.6.1/
+-rwxrwxrwx   0        0        0      133 2023-02-22 15:56:30.000000 testbench2robotframework-0.6.1/CreatePiPWheel.bat
+-rw-rw-rw-   0        0        0      139 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/CreatePiPWheel.sh
+-rw-rw-rw-   0        0        0     2614 2023-02-24 15:19:12.000000 testbench2robotframework-0.6.1/DEVELOPMENT.md
+-rw-rw-rw-   0        0        0    11558 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    17951 2023-07-13 18:16:20.939998 testbench2robotframework-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15210 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/README.md
+-rw-rw-rw-   0        0        0     1069 2023-07-13 14:40:56.000000 testbench2robotframework-0.6.1/config.json
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.774873 testbench2robotframework-0.6.1/images/
+-rw-rw-rw-   0        0        0     5625 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/LibrarySubdivision.PNG
+-rw-rw-rw-   0        0        0      167 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/Unbenannt.PNG
+-rw-rw-rw-   0        0        0    29769 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/generated.png
+-rw-rw-rw-   0        0        0     5625 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/libraries.PNG
+-rw-rw-rw-   0        0        0     5627 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/resources.PNG
+-rw-rw-rw-   0        0        0     6384 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/rfLibraryRootsTestBench.PNG
+-rw-rw-rw-   0        0        0     5407 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/testbench_rfLibraryRegex.PNG
+-rw-rw-rw-   0        0        0     4944 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/testbench_rfResourceRegex.PNG
+-rw-rw-rw-   0        0        0    13816 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/images/testthemen.PNG
+-rw-rw-rw-   0        0        0     2514 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0     3431 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/requirements.txt
+-rw-rw-rw-   0        0        0      988 2023-07-13 18:16:20.940996 testbench2robotframework-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.816000 testbench2robotframework-0.6.1/testbench2robotframework/
+-rw-rw-rw-   0        0        0      695 2023-07-13 18:00:37.000000 testbench2robotframework-0.6.1/testbench2robotframework/__init__.py
+-rw-rw-rw-   0        0        0     1732 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/__main__.py
+-rw-rw-rw-   0        0        0     6071 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/testbench2robotframework/config.py
+-rw-rw-rw-   0        0        0     5363 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/json_reader.py
+-rw-rw-rw-   0        0        0     1177 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/json_writer.py
+-rw-rw-rw-   0        0        0      903 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/testbench2robotframework/log.py
+-rw-rw-rw-   0        0        0    24397 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/model.py
+-rw-rw-rw-   0        0        0    29220 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/result_writer.py
+-rw-rw-rw-   0        0        0      997 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/robotframework2testbench.py
+-rw-rw-rw-   0        0        0    29335 2023-07-13 18:01:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/testbench2rf.py
+-rw-rw-rw-   0        0        0     1196 2023-02-21 12:18:27.000000 testbench2robotframework-0.6.1/testbench2robotframework/testbench2robotframework.py
+-rw-rw-rw-   0        0        0     1840 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/testsuite_write.py
+-rw-rw-rw-   0        0        0     7162 2023-07-13 14:40:59.000000 testbench2robotframework-0.6.1/testbench2robotframework/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.838996 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/
+-rw-rw-rw-   0        0        0    17951 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 14:07:22.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      135 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-13 18:16:20.000000 testbench2robotframework-0.6.1/testbench2robotframework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.846997 testbench2robotframework-0.6.1/tests/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.718874 testbench2robotframework-0.6.1/tests/test_data/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.854004 testbench2robotframework-0.6.1/tests/test_data/configurations/
+-rw-rw-rw-   0        0        0     1196 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/tests/test_data/configurations/invalid_config.json
+-rw-rw-rw-   0        0        0     1173 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/tests/test_data/configurations/valid_config.json
+-rw-rw-rw-   0        0        0      236 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/tests/test_missing_files.py
+-rw-rw-rw-   0        0        0      426 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/tests/test_robot_files_should_not_contain_invalid_characters.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.857001 testbench2robotframework-0.6.1/tests/test_setup/
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.860078 testbench2robotframework-0.6.1/tests/test_setup/test_data/
+-rw-rw-rw-   0        0        0      642 2023-02-27 12:42:27.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/config.json
+drwxrwxrwx   0        0        0        0 2023-07-13 18:16:20.936997 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/
+-rw-rw-rw-   0        0        0     6538 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/TestThemeTree.json
+-rw-rw-rw-   0        0        0    23984 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2184-PC-21637.json
+-rw-rw-rw-   0        0        0     1038 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2184.json
+-rw-rw-rw-   0        0        0    24699 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2185-PC-21639.json
+-rw-rw-rw-   0        0        0     1041 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2185.json
+-rw-rw-rw-   0        0        0    24918 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2231-PC-21643.json
+-rw-rw-rw-   0        0        0     1210 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2231.json
+-rw-rw-rw-   0        0        0    24754 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2232-PC-21645.json
+-rw-rw-rw-   0        0        0     1044 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2232.json
+-rw-rw-rw-   0        0        0     8682 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2233-PC-21647.json
+-rw-rw-rw-   0        0        0     8677 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2233-PC-21649.json
+-rw-rw-rw-   0        0        0     1439 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2233.json
+-rw-rw-rw-   0        0        0    14003 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2241-PC-21667.json
+-rw-rw-rw-   0        0        0    13993 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2241-PC-21668.json
+-rw-rw-rw-   0        0        0     1459 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2241.json
+-rw-rw-rw-   0        0        0    12223 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2242-PC-21671.json
+-rw-rw-rw-   0        0        0     1052 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2242.json
+-rw-rw-rw-   0        0        0     2318 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2243-PC-21673.json
+-rw-rw-rw-   0        0        0     1042 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2243.json
+-rw-rw-rw-   0        0        0     3155 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2244-PC-21675.json
+-rw-rw-rw-   0        0        0     1056 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2244.json
+-rw-rw-rw-   0        0        0     4795 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2261-PC-21683.json
+-rw-rw-rw-   0        0        0     1086 2023-02-27 14:12:05.000000 testbench2robotframework-0.6.1/tests/test_setup/test_data/json-report/itba-TC-2261.json
+-rw-rw-rw-   0        0        0     2337 2023-02-27 16:41:38.000000 testbench2robotframework-0.6.1/tests/test_setup/test_setup_name.py
+-rw-rw-rw-   0        0        0      957 2023-02-10 14:36:22.000000 testbench2robotframework-0.6.1/tests/test_zip_file_generation.py
```

### Comparing `testbench2robotframework-0.6.0/DEVELOPMENT.md` & `testbench2robotframework-0.6.1/DEVELOPMENT.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-# Contributing
-
-## Development Environment Setup
-
-1. Install Python 3.8 and VS Code
-
-2. Open a terminal in this repository
-
-3. Create the virtual environment .venv
-
-    > /path/to/python38/python -m venv .venv
-
-4. Activate the virtual environment
-
-    > .venv/scripts/activate
-
-4. Install the dependencies
-
-    > pip install -r requirements.txt
-
-5. [Install Pandoc](https://pandoc.org/installing.html)
-
-
-## Generate documentation in Word format
-
-```shell
-pandoc -s README.md -M title="imbus TestBench - Robot Code Generator" -M subtitle=Benutzerhandbuch -M toc-title=Inhaltsverzeichnis --toc -o Benutzerhandbuch.docx
-```
-
-
-## Build, Install and Run
-
-The package is built using setuptools. The build configuration is defined in `setup.cfg`.
-
-- Build and install the package
-    > pip install -e .
-
-- Run the application
-    > tb2robot
-
-- Build a pure-Python wheel
-    > pip install wheel
-    > python setup.py bdist_wheel
-
-- Build a pure-Python wheel and publish new version to pypi
-    > pip install wheel
-    > pip install twine
-    > CreatePipWheel.bat oder CreatePipWheel.sh
-
-
-## Adding New Dependencies
-1. Install pip-tools (to pin dependencies)
-
-    > python -m pip install pip-tools
-
-
-2. In `setup.cfg` add a package to the corresponding section
-
-    - Development dependencies: `dev` extra under `options.extras_require`
-
-    - Runtime dependencies: `install-requires`
-
-3. Update `requirements.txt`
-    - Development dependencies
-        > pip-compile --extra dev setup.cfg
-
-    - Runtime dependencies
-        > pip-compile setup.cfg
-
-4. Create a commit with `setup.cfg`, `requirements.txt`, `pyproject.toml` explaining why the dependency was added.
-
-
-## Static Analysis and Code Formatting
-
-Static analysis and code formatting tools are configured in `pyproject.toml`.
-
-### Static Analysis
-
-- `mypy`: static type checker
-    * [The mypy configuration file](https://mypy.readthedocs.io/en/stable/config_file.html)
-
-- `pylint`: syntax and code quality checks
-
-    * [Pylint Global options and switches](https://pylint.pycqa.org/en/latest/technical_reference/features.html)
-
-    * [Overview of all Pylint messages](https://pylint.pycqa.org/en/latest/messages/messages_list.html)
-
-    * [Naming Styles](https://pylint.pycqa.org/en/latest/user_guide/options.html)
-
-
-### Code Formatting
-
-- `black`: Format the code according to a subset of PEP 8
-    > black .
-
-- `isort`: Sort the package imports following PEP 8
-    > isort .
-
-
-## Testing
-
-- `pytest` is configured in `pyproject.toml`
-    > python -m pytest
+# Contributing
+
+## Development Environment Setup
+
+1. Install Python 3.8 and VS Code
+
+2. Open a terminal in this repository
+
+3. Create the virtual environment .venv
+
+    > /path/to/python38/python -m venv .venv
+
+4. Activate the virtual environment
+
+    > .venv/scripts/activate
+
+4. Install the dependencies
+
+    > pip install -r requirements.txt
+
+5. [Install Pandoc](https://pandoc.org/installing.html)
+
+
+## Generate documentation in Word format
+
+```shell
+pandoc -s README.md -M title="imbus TestBench - Robot Code Generator" -M subtitle=Benutzerhandbuch -M toc-title=Inhaltsverzeichnis --toc -o Benutzerhandbuch.docx
+```
+
+
+## Build, Install and Run
+
+The package is built using setuptools. The build configuration is defined in `setup.cfg`.
+
+- Build and install the package
+    > pip install -e .
+
+- Run the application
+    > tb2robot
+
+- Build a pure-Python wheel
+    > pip install wheel
+    > python setup.py bdist_wheel
+
+- Build a pure-Python wheel and publish new version to pypi
+    > pip install wheel
+    > pip install twine
+    > CreatePipWheel.bat oder CreatePipWheel.sh
+
+
+## Adding New Dependencies
+1. Install pip-tools (to pin dependencies)
+
+    > python -m pip install pip-tools
+
+
+2. In `setup.cfg` add a package to the corresponding section
+
+    - Development dependencies: `dev` extra under `options.extras_require`
+
+    - Runtime dependencies: `install-requires`
+
+3. Update `requirements.txt`
+    - Development dependencies
+        > pip-compile --extra dev setup.cfg
+
+    - Runtime dependencies
+        > pip-compile setup.cfg
+
+4. Create a commit with `setup.cfg`, `requirements.txt`, `pyproject.toml` explaining why the dependency was added.
+
+
+## Static Analysis and Code Formatting
+
+Static analysis and code formatting tools are configured in `pyproject.toml`.
+
+### Static Analysis
+
+- `mypy`: static type checker
+    * [The mypy configuration file](https://mypy.readthedocs.io/en/stable/config_file.html)
+
+- `pylint`: syntax and code quality checks
+
+    * [Pylint Global options and switches](https://pylint.pycqa.org/en/latest/technical_reference/features.html)
+
+    * [Overview of all Pylint messages](https://pylint.pycqa.org/en/latest/messages/messages_list.html)
+
+    * [Naming Styles](https://pylint.pycqa.org/en/latest/user_guide/options.html)
+
+
+### Code Formatting
+
+- `black`: Format the code according to a subset of PEP 8
+    > black .
+
+- `isort`: Sort the package imports following PEP 8
+    > isort .
+
+
+## Testing
+
+- `pytest` is configured in `pyproject.toml`
+    > python -m pytest
```

### Comparing `testbench2robotframework-0.6.0/LICENSE` & `testbench2robotframework-0.6.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `testbench2robotframework-0.6.0/PKG-INFO` & `testbench2robotframework-0.6.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,303 +1,289 @@
-Metadata-Version: 2.1
-Name: testbench2robotframework
-Version: 0.6.0
-Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
-Home-page: https://github.com/imbus/testbench2robotframework
-Author: imbus AG
-Author-email: support@imbus.de
-License: Apache 2.0 License
-Platform: any
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Installation des Robot Code Generators
-
-Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-
-```powershell
-python --version
-```
-
-Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-
-```powershell
-python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-```
-
-Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-```powershell
-pip install testbench2robotframework
-```
-
-Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-
-```powershell
-tb2robot --version
-```
-
-# Verwendung des Robot Code Generators
-Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-
-Der Befehl ``tb2robot --help
-`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-
-Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-
-(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-
-(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-```powershell
-tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-```
-Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-
-![](./images/testthemen.PNG)
-![](./images/generated.PNG)
-
-Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-
-Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-
-(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-
-(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-
-(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-```powershell
-tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-```
-
-# Konfiguration der Ergebnisse
-Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-
-## rfLibraryRegex
-Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-
-![](./images/testbench_rfLibraryRegex.PNG)
-
-```python
-*** Settings ***
-Library    Browser
-Library    BuiltIn
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfLibraryRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-  ]
-```
-
-## rfResourceRegex
-Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-
-![](./images/testbench_rfResourceRegex.PNG)
-
-```python
-*** Settings ***
-Resource    keywords.resource
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfResourceRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-  ]
-```
-## rfLibraryRoots
-Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-
-Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-
-Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-
-```json
-"rfLibraryRoots": ["RobotLibraries"]
-```
-
-![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-
-Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-
-```python
-*** Settings ***
-Library    BuiltIn
-Library    OperatingSystem
-# UNKNOWN    Process
-```
-
-## rfResourceRoots
-Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-
-Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-
-```json
-"rfResourceRoots": ["RF-Resources"]
-```
-
-![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-
-Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-
-```python
-*** Settings ***
-Resource    keywords.resource
-# UNKNOWN    unknownKeywords
-```
-
-## fullyQualified
-Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-
-Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-
-```python
-SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-```
-Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-
-```python
-Open Browser      https://robotframework.org/    firefox
-```
-
-## resourceDirectory
-Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-
-```json
-"resourceDirectory": "{root}/Resources",
-```
-
-```robotframework
-*** Settings ***
-Resource    ../Resources/myKeywords.resource
-```
-
-## generationDirectory
-Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-```json
-"generationDirectory": "{root}/generatedRobotFiles"
-```
-
-## createOutputZip
-Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-
-## logSuiteNumbering
-Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-
-```json
-"logSuiteNumbering": true
-```
-## clearGenerationDirectory
-Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-
-```json
-"clearGenerationDirectory": true,
-```
-
-## logCompoundInteractions
-Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-
-```json
-"logCompoundInteractions": true,
-```
-
-## subdivisionsMapping
-Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-
-```json
-"subdivisionsMapping": {
-    "libraries": {
-      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-    },
-    "resources": {
-      "MyKeywords": "{root}/../MyKeywords.resource",
-      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-    }
-  }
-```
-
-
-## forcedImport
-Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-
-```json
-"forcedImport": {
-    "libraries": [
-      "SeleniumLibrary"
-    ],
-    "resources":
-    [
-      "technical_keywords.resource"
-    ],
-    "variables": [
-      "myVars.py"
-    ]
-  }
-```
-
-## loggingConfiguration
-Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-Gültige Optionen sind:
-
-* "CRITICAL"
-
-* "FATAL"
-
-* "ERROR"
-
-* "WARNING"
-
-* "WARN"
-
-* "INFO"
-
-* "DEBUG"
-
-* "NOTSET"
-
-Das Default Log-Level ist ``INFO``.
-```json
-"loggingConfiguration": {
-  "console": {
-    "logLevel": "info"
-  }
-}
-```
-
-## referenceBehaviour
-Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-
-```json
-"referenceBehaviour": "ATTACHMENT"
-```
-
-## attachmentConflictBehaviour
-Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-
-Die möglichen Werte haben dabei die folgende Bedeutung:
-- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-```json
-"attachmentConflictBehaviour": "USE_EXISTING"
-```
-
-## testCaseSplitPathRegEx
-Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-
+# Installation des Robot Code Generators
+
+Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+
+```powershell
+python --version
+```
+
+Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+
+```powershell
+python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+```
+
+Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+```powershell
+pip install testbench2robotframework
+```
+
+Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+
+```powershell
+tb2robot --version
+```
+
+# Verwendung des Robot Code Generators
+Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+
+Der Befehl ``tb2robot --help
+`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+
+Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+
+(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+
+(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+```powershell
+tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+```
+Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+
+![](./images/testthemen.PNG)
+![](./images/generated.PNG)
+
+Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+
+Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+
+(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+
+(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+
+(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+
+Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+```powershell
+tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+```
+
+# Konfiguration der Ergebnisse
+Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+
+## rfLibraryRegex
+Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+
+![](./images/testbench_rfLibraryRegex.PNG)
+
+```python
+*** Settings ***
+Library    Browser
+Library    BuiltIn
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfLibraryRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+  ]
+```
+
+## rfResourceRegex
+Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+
+![](./images/testbench_rfResourceRegex.PNG)
+
+```python
+*** Settings ***
+Resource    keywords.resource
+```
+In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+```json
+"rfResourceRegex": [
+    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+  ]
+```
+## rfLibraryRoots
+Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+
+Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+
+Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+
+```json
+"rfLibraryRoots": ["RobotLibraries"]
+```
+
+![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+
+Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+
+```python
+*** Settings ***
+Library    BuiltIn
+Library    OperatingSystem
+# UNKNOWN    Process
+```
+
+## rfResourceRoots
+Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+
+Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+
+```json
+"rfResourceRoots": ["RF-Resources"]
+```
+
+![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+
+Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+
+```python
+*** Settings ***
+Resource    keywords.resource
+# UNKNOWN    unknownKeywords
+```
+
+## fullyQualified
+Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+
+Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+
+```python
+SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+```
+Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+
+```python
+Open Browser      https://robotframework.org/    firefox
+```
+
+## resourceDirectory
+Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+
+```json
+"resourceDirectory": "{root}/Resources",
+```
+
+```robotframework
+*** Settings ***
+Resource    ../Resources/myKeywords.resource
+```
+
+## generationDirectory
+Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+```json
+"generationDirectory": "{root}/generatedRobotFiles"
+```
+
+## createOutputZip
+Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+
+## logSuiteNumbering
+Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+
+```json
+"logSuiteNumbering": true
+```
+## clearGenerationDirectory
+Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+
+```json
+"clearGenerationDirectory": true,
+```
+
+## logCompoundInteractions
+Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+
+```json
+"logCompoundInteractions": true,
+```
+
+## subdivisionsMapping
+Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+
+```json
+"subdivisionsMapping": {
+    "libraries": {
+      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+    },
+    "resources": {
+      "MyKeywords": "{root}/../MyKeywords.resource",
+      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+    }
+  }
+```
+
+
+## forcedImport
+Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+
+```json
+"forcedImport": {
+    "libraries": [
+      "SeleniumLibrary"
+    ],
+    "resources":
+    [
+      "technical_keywords.resource"
+    ],
+    "variables": [
+      "myVars.py"
+    ]
+  }
+```
+
+## loggingConfiguration
+Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+Gültige Optionen sind:
+
+* "CRITICAL"
+
+* "FATAL"
+
+* "ERROR"
+
+* "WARNING"
+
+* "WARN"
+
+* "INFO"
+
+* "DEBUG"
+
+* "NOTSET"
+
+Das Default Log-Level ist ``INFO``.
+```json
+"loggingConfiguration": {
+  "console": {
+    "logLevel": "info"
+  }
+}
+```
+
+## referenceBehaviour
+Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+
+```json
+"referenceBehaviour": "ATTACHMENT"
+```
+
+## attachmentConflictBehaviour
+Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+
+Die möglichen Werte haben dabei die folgende Bedeutung:
+- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+```json
+"attachmentConflictBehaviour": "USE_EXISTING"
+```
+
+## testCaseSplitPathRegEx
+Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+
```

### Comparing `testbench2robotframework-0.6.0/README.md` & `testbench2robotframework-0.6.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,302 @@
-# Installation des Robot Code Generators
-
-Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-
-```powershell
-python --version
-```
-
-Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-
-```powershell
-python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-```
-
-Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-```powershell
-pip install testbench2robotframework
-```
-
-Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-
-```powershell
-tb2robot --version
-```
-
-# Verwendung des Robot Code Generators
-Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-
-Der Befehl ``tb2robot --help
-`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-
-Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-
-(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-
-(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-```powershell
-tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-```
-Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-
-![](./images/testthemen.PNG)
-![](./images/generated.PNG)
-
-Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-
-Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-
-(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-
-(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-
-(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-```powershell
-tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-```
-
-# Konfiguration der Ergebnisse
-Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-
-## rfLibraryRegex
-Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-
-![](./images/testbench_rfLibraryRegex.PNG)
-
-```python
-*** Settings ***
-Library    Browser
-Library    BuiltIn
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfLibraryRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-  ]
-```
-
-## rfResourceRegex
-Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-
-![](./images/testbench_rfResourceRegex.PNG)
-
-```python
-*** Settings ***
-Resource    keywords.resource
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfResourceRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-  ]
-```
-## rfLibraryRoots
-Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-
-Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-
-Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-
-```json
-"rfLibraryRoots": ["RobotLibraries"]
-```
-
-![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-
-Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-
-```python
-*** Settings ***
-Library    BuiltIn
-Library    OperatingSystem
-# UNKNOWN    Process
-```
-
-## rfResourceRoots
-Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-
-Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-
-```json
-"rfResourceRoots": ["RF-Resources"]
-```
-
-![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-
-Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-
-```python
-*** Settings ***
-Resource    keywords.resource
-# UNKNOWN    unknownKeywords
-```
-
-## fullyQualified
-Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-
-Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-
-```python
-SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-```
-Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-
-```python
-Open Browser      https://robotframework.org/    firefox
-```
-
-## resourceDirectory
-Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-
-```json
-"resourceDirectory": "{root}/Resources",
-```
-
-```robotframework
-*** Settings ***
-Resource    ../Resources/myKeywords.resource
-```
-
-## generationDirectory
-Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-```json
-"generationDirectory": "{root}/generatedRobotFiles"
-```
-
-## createOutputZip
-Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-
-## logSuiteNumbering
-Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-
-```json
-"logSuiteNumbering": true
-```
-## clearGenerationDirectory
-Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-
-```json
-"clearGenerationDirectory": true,
-```
-
-## logCompoundInteractions
-Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-
-```json
-"logCompoundInteractions": true,
-```
-
-## subdivisionsMapping
-Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-
-```json
-"subdivisionsMapping": {
-    "libraries": {
-      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-    },
-    "resources": {
-      "MyKeywords": "{root}/../MyKeywords.resource",
-      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-    }
-  }
-```
-
-
-## forcedImport
-Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-
-```json
-"forcedImport": {
-    "libraries": [
-      "SeleniumLibrary"
-    ],
-    "resources":
-    [
-      "technical_keywords.resource"
-    ],
-    "variables": [
-      "myVars.py"
-    ]
-  }
-```
-
-## loggingConfiguration
-Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-Gültige Optionen sind:
-
-* "CRITICAL"
-
-* "FATAL"
-
-* "ERROR"
-
-* "WARNING"
-
-* "WARN"
-
-* "INFO"
-
-* "DEBUG"
-
-* "NOTSET"
-
-Das Default Log-Level ist ``INFO``.
-```json
-"loggingConfiguration": {
-  "console": {
-    "logLevel": "info"
-  }
-}
-```
-
-## referenceBehaviour
-Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-
-```json
-"referenceBehaviour": "ATTACHMENT"
-```
-
-## attachmentConflictBehaviour
-Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-
-Die möglichen Werte haben dabei die folgende Bedeutung:
-- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-```json
-"attachmentConflictBehaviour": "USE_EXISTING"
-```
-
-## testCaseSplitPathRegEx
-Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-
+Metadata-Version: 2.1
+Name: testbench2robotframework
+Version: 0.6.1
+Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
+Home-page: https://github.com/imbus/testbench2robotframework
+Author: imbus AG
+Author-email: support@imbus.de
+License: Apache 2.0 License
+Description: # Installation des Robot Code Generators
+        
+        Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+        
+        ```powershell
+        python --version
+        ```
+        
+        Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+        Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+        
+        ```powershell
+        python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+        ```
+        
+        Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+        ```powershell
+        pip install testbench2robotframework
+        ```
+        
+        Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+        
+        ```powershell
+        tb2robot --version
+        ```
+        
+        # Verwendung des Robot Code Generators
+        Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+        
+        Der Befehl ``tb2robot --help
+        `` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+        
+        Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+        
+        (@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+        
+        (@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+        
+        Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+        ```powershell
+        tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+        ```
+        Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+        
+        ![](./images/testthemen.PNG)
+        ![](./images/generated.PNG)
+        
+        Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+        
+        Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+        Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+        
+        (@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+        
+        (@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+        
+        (@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+        
+        Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+        ```powershell
+        tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+        ```
+        
+        # Konfiguration der Ergebnisse
+        Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+        
+        ## rfLibraryRegex
+        Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+        Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+        Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+        
+        ![](./images/testbench_rfLibraryRegex.PNG)
+        
+        ```python
+        *** Settings ***
+        Library    Browser
+        Library    BuiltIn
+        ```
+        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+        ```json
+        "rfLibraryRegex": [
+            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+          ]
+        ```
+        
+        ## rfResourceRegex
+        Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+        Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+        Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+        
+        ![](./images/testbench_rfResourceRegex.PNG)
+        
+        ```python
+        *** Settings ***
+        Resource    keywords.resource
+        ```
+        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+        ```json
+        "rfResourceRegex": [
+            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+          ]
+        ```
+        ## rfLibraryRoots
+        Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+        Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+        
+        Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+        
+        Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+        
+        ```json
+        "rfLibraryRoots": ["RobotLibraries"]
+        ```
+        
+        ![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+        
+        Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+        
+        ```python
+        *** Settings ***
+        Library    BuiltIn
+        Library    OperatingSystem
+        # UNKNOWN    Process
+        ```
+        
+        ## rfResourceRoots
+        Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+        
+        Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+        
+        ```json
+        "rfResourceRoots": ["RF-Resources"]
+        ```
+        
+        ![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+        
+        Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+        
+        ```python
+        *** Settings ***
+        Resource    keywords.resource
+        # UNKNOWN    unknownKeywords
+        ```
+        
+        ## fullyQualified
+        Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+        
+        Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+        
+        ```python
+        SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+        ```
+        Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+        
+        ```python
+        Open Browser      https://robotframework.org/    firefox
+        ```
+        
+        ## resourceDirectory
+        Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+        Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+        
+        ```json
+        "resourceDirectory": "{root}/Resources",
+        ```
+        
+        ```robotframework
+        *** Settings ***
+        Resource    ../Resources/myKeywords.resource
+        ```
+        
+        ## generationDirectory
+        Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+        ```json
+        "generationDirectory": "{root}/generatedRobotFiles"
+        ```
+        
+        ## createOutputZip
+        Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+        
+        ## logSuiteNumbering
+        Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+        
+        ```json
+        "logSuiteNumbering": true
+        ```
+        ## clearGenerationDirectory
+        Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+        
+        ```json
+        "clearGenerationDirectory": true,
+        ```
+        
+        ## logCompoundInteractions
+        Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+        
+        ```json
+        "logCompoundInteractions": true,
+        ```
+        
+        ## subdivisionsMapping
+        Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+        
+        ```json
+        "subdivisionsMapping": {
+            "libraries": {
+              "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+              "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+            },
+            "resources": {
+              "MyKeywords": "{root}/../MyKeywords.resource",
+              "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+            }
+          }
+        ```
+        
+        
+        ## forcedImport
+        Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+        
+        ```json
+        "forcedImport": {
+            "libraries": [
+              "SeleniumLibrary"
+            ],
+            "resources":
+            [
+              "technical_keywords.resource"
+            ],
+            "variables": [
+              "myVars.py"
+            ]
+          }
+        ```
+        
+        ## loggingConfiguration
+        Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+        Gültige Optionen sind:
+        
+        * "CRITICAL"
+        
+        * "FATAL"
+        
+        * "ERROR"
+        
+        * "WARNING"
+        
+        * "WARN"
+        
+        * "INFO"
+        
+        * "DEBUG"
+        
+        * "NOTSET"
+        
+        Das Default Log-Level ist ``INFO``.
+        ```json
+        "loggingConfiguration": {
+          "console": {
+            "logLevel": "info"
+          }
+        }
+        ```
+        
+        ## referenceBehaviour
+        Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+        Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+        Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+        
+        ```json
+        "referenceBehaviour": "ATTACHMENT"
+        ```
+        
+        ## attachmentConflictBehaviour
+        Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+        Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+        
+        Die möglichen Werte haben dabei die folgende Bedeutung:
+        - ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+        - USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+        - USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+        - RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+        ```json
+        "attachmentConflictBehaviour": "USE_EXISTING"
+        ```
+        
+        ## testCaseSplitPathRegEx
+        Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+        
+        
+Platform: any
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `testbench2robotframework-0.6.0/config.json` & `testbench2robotframework-0.6.1/tests/test_data/configurations/invalid_config.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'forcedImport'": "{'libraries': ['SuperRemoteLibrary', 'SeleniumLibrary'], 'resources': "*

 * *                   "['technical_keywords.resource'], 'variables': ['myVars.py']}",*

 * * "'testCaseSplitPathRegEx'": "'^splitting\\\\..*'",*

 * * "'testbalala'": 'True'}*

```diff
@@ -1,14 +1,21 @@
 {
     "clearGenerationDirectory": true,
     "createOutputZip": true,
     "forcedImport": {
-        "libraries": [],
-        "resources": [],
-        "variables": []
+        "libraries": [
+            "SuperRemoteLibrary",
+            "SeleniumLibrary"
+        ],
+        "resources": [
+            "technical_keywords.resource"
+        ],
+        "variables": [
+            "myVars.py"
+        ]
     },
     "fullyQualified": true,
     "generationDirectory": "{root}/Generated",
     "logCompoundInteractions": true,
     "logSuiteNumbering": true,
     "loggingConfiguration": {
         "console": {
@@ -29,9 +36,10 @@
             "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
         },
         "resources": {
             "MyKeywords": "{root}/../MyKeywords.resource",
             "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
         }
     },
-    "testCaseSplitPathRegEx": "^StopWithRestart\\..*"
+    "testCaseSplitPathRegEx": "^splitting\\..*",
+    "testbalala": true
 }
```

### Comparing `testbench2robotframework-0.6.0/images/LibrarySubdivision.PNG` & `testbench2robotframework-0.6.1/images/LibrarySubdivision.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/generated.png` & `testbench2robotframework-0.6.1/images/generated.png`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/libraries.PNG` & `testbench2robotframework-0.6.1/images/libraries.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/resources.PNG` & `testbench2robotframework-0.6.1/images/resources.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/rfLibraryRootsTestBench.PNG` & `testbench2robotframework-0.6.1/images/rfLibraryRootsTestBench.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/testbench_rfLibraryRegex.PNG` & `testbench2robotframework-0.6.1/images/testbench_rfLibraryRegex.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/testbench_rfResourceRegex.PNG` & `testbench2robotframework-0.6.1/images/testbench_rfResourceRegex.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/images/testthemen.PNG` & `testbench2robotframework-0.6.1/images/testthemen.PNG`

 * *Files identical despite different names*

### Comparing `testbench2robotframework-0.6.0/pyproject.toml` & `testbench2robotframework-0.6.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[tool.pylint.FORMAT]
-max-line-length = 100
-max-module-lines = 1000
-
-[tool.pylint.MASTER]
-ignore = "tests"
-
-[tool.pylint.BASIC]
-argument-naming-style = 'snake_case'
-attr-naming-style = 'snake_case'
-class-naming-style = 'PascalCase'
-const-naming-style = 'UPPER_CASE'
-function-naming-style = 'snake_case'
-method-naming-style = 'snake_case'
-module-naming-style = 'snake_case'
-variable-naming-style = 'snake_case'
-
-[tool.pylint.DESIGN]
-# Maximum number of arguments for function / method.
-max-args = 5
-# Maximum number of statements in function / method body.
-max-statements = 50
-
-[tool.pylint."MESSAGES CONTROL"]
-disable = '''
-    logging-fstring-interpolation,
-    fixme,
-    import-error,
-    missing-module-docstring,
-    missing-class-docstring,
-    missing-function-docstring,
-    too-many-instance-attributes,
-    too-few-public-methods,
-'''
-
-[tool.pylint.REFACTORING]
-# Maximum number of nested blocks for function / method body
-max-nested-blocks = 3
-
-[tool.mypy]
-python_version = "3.8"
-ignore_missing_imports = true
-no_implicit_optional = true
-strict_optional = true
-warn_return_any = true
-warn_no_return = true
-warn_unreachable = true
-pretty = true
-
-[tool.black]
-target-version = ['py38']
-line-length = 100
-include_trailing_comma = false
-skip-string-normalization = true
-
-[tool.isort]
-profile = "black"
-src_paths = ["testbench2robotframework"]
-skip_gitignore = true
-skip = ['external']
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra --spec"
-testpaths = [
-    "tests",
-]
-spec_header_format = "{test_case}"
-
-[tool.ruff]
-unfixable = [
-    "UP007"
-]
-exclude = [
-  "__pycache__",
-  "config.py",
-  "model.py",
-  "tests"
-]
-ignore = [
-  "B008",  # do not perform function calls in argument defaults
-  "E501",  # line too long
-  # "N815",  # mixedCase variable in class scope
-  # "N803",  # argument name should be lowercase
-  # "N806",  # variable in function should be lowercase
-  # "N812",  # lowercase imported as non lowercase
-  # "N999",  # Invalid module name: 'Browser'
-  "PLR0913",  # too many arguments
-  # "T201",  # Print statements
-  "UP007",
-]
-target-version = "py37"
-select = [
-  "E",
-  "F",
-  "W",
-  "C90",
-  "I",
-  "N",
-  "B",
-  "PYI",
-  "PL",
-  "PTH",
-  "UP",
-  "A",
-  "C4",
-  "DTZ",
-  "ISC",
-  "ICN",
-  "INP",
-  "PIE",
-  "T20",
-  "PYI",
-  "PT",
-  "RSE",
-  "RET",
-  "SIM",
-  "RUF"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[tool.pylint.FORMAT]
+max-line-length = 100
+max-module-lines = 1000
+
+[tool.pylint.MASTER]
+ignore = "tests"
+
+[tool.pylint.BASIC]
+argument-naming-style = 'snake_case'
+attr-naming-style = 'snake_case'
+class-naming-style = 'PascalCase'
+const-naming-style = 'UPPER_CASE'
+function-naming-style = 'snake_case'
+method-naming-style = 'snake_case'
+module-naming-style = 'snake_case'
+variable-naming-style = 'snake_case'
+
+[tool.pylint.DESIGN]
+# Maximum number of arguments for function / method.
+max-args = 5
+# Maximum number of statements in function / method body.
+max-statements = 50
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = '''
+    logging-fstring-interpolation,
+    fixme,
+    import-error,
+    missing-module-docstring,
+    missing-class-docstring,
+    missing-function-docstring,
+    too-many-instance-attributes,
+    too-few-public-methods,
+'''
+
+[tool.pylint.REFACTORING]
+# Maximum number of nested blocks for function / method body
+max-nested-blocks = 3
+
+[tool.mypy]
+python_version = "3.8"
+ignore_missing_imports = true
+no_implicit_optional = true
+strict_optional = true
+warn_return_any = true
+warn_no_return = true
+warn_unreachable = true
+pretty = true
+
+[tool.black]
+target-version = ['py38']
+line-length = 100
+include_trailing_comma = false
+skip-string-normalization = true
+
+[tool.isort]
+profile = "black"
+src_paths = ["testbench2robotframework"]
+skip_gitignore = true
+skip = ['external']
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra --spec"
+testpaths = [
+    "tests",
+]
+spec_header_format = "{test_case}"
+
+[tool.ruff]
+unfixable = [
+    "UP007"
+]
+exclude = [
+  "__pycache__",
+  "config.py",
+  "model.py",
+  "tests"
+]
+ignore = [
+  "B008",  # do not perform function calls in argument defaults
+  "E501",  # line too long
+  # "N815",  # mixedCase variable in class scope
+  # "N803",  # argument name should be lowercase
+  # "N806",  # variable in function should be lowercase
+  # "N812",  # lowercase imported as non lowercase
+  # "N999",  # Invalid module name: 'Browser'
+  "PLR0913",  # too many arguments
+  # "T201",  # Print statements
+  "UP007",
+]
+target-version = "py37"
+select = [
+  "E",
+  "F",
+  "W",
+  "C90",
+  "I",
+  "N",
+  "B",
+  "PYI",
+  "PL",
+  "PTH",
+  "UP",
+  "A",
+  "C4",
+  "DTZ",
+  "ISC",
+  "ICN",
+  "INP",
+  "PIE",
+  "T20",
+  "PYI",
+  "PT",
+  "RSE",
+  "RET",
+  "SIM",
+  "RUF"
 ]
```

### Comparing `testbench2robotframework-0.6.0/setup.cfg` & `testbench2robotframework-0.6.1/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 7465 7374 6265 6e63 6832 726f 626f  = testbench2robo
-00000020: 7466 7261 6d65 776f 726b 0a61 7574 686f  tframework.autho
-00000030: 7220 3d20 696d 6275 7320 4147 0a61 7574  r = imbus AG.aut
-00000040: 686f 725f 656d 6169 6c20 3d20 7375 7070  hor_email = supp
-00000050: 6f72 7440 696d 6275 732e 6465 0a76 6572  ort@imbus.de.ver
-00000060: 7369 6f6e 203d 2061 7474 723a 2074 6573  sion = attr: tes
-00000070: 7462 656e 6368 3272 6f62 6f74 6672 616d  tbench2robotfram
-00000080: 6577 6f72 6b2e 5f5f 7665 7273 696f 6e5f  ework.__version_
-00000090: 5f0a 6465 7363 7269 7074 696f 6e20 3d20  _.description = 
-000000a0: 526f 626f 7420 4672 616d 6577 6f72 6b20  Robot Framework 
-000000b0: 436f 6465 2047 656e 6572 6174 6f72 2066  Code Generator f
-000000c0: 726f 6d20 4b65 7977 6f72 642d 4472 6976  rom Keyword-Driv
-000000d0: 656e 2054 6573 7473 2069 6e20 696d 6275  en Tests in imbu
-000000e0: 7320 5465 7374 4265 6e63 6820 332e 3020  s TestBench 3.0 
-000000f0: 616e 6420 6e65 7765 720a 6c6f 6e67 5f64  and newer.long_d
-00000100: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000110: 653a 2052 4541 444d 452e 6d64 0a6c 6f6e  e: README.md.lon
-00000120: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000130: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000140: 742f 6d61 726b 646f 776e 0a6c 6963 656e  t/markdown.licen
-00000150: 7365 203d 2041 7061 6368 6520 322e 3020  se = Apache 2.0 
-00000160: 4c69 6365 6e73 650a 7572 6c20 3d20 6874  License.url = ht
-00000170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000180: 2f69 6d62 7573 2f74 6573 7462 656e 6368  /imbus/testbench
-00000190: 3272 6f62 6f74 6672 616d 6577 6f72 6b0a  2robotframework.
-000001a0: 706c 6174 666f 726d 7320 3d20 616e 790a  platforms = any.
-000001b0: 0a5b 6f70 7469 6f6e 735d 0a7a 6970 5f73  .[options].zip_s
-000001c0: 6166 6520 3d20 4661 6c73 650a 7061 636b  afe = False.pack
-000001d0: 6167 6573 203d 2066 696e 643a 0a70 7974  ages = find:.pyt
-000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001f0: 3d20 332e 380a 696e 7374 616c 6c5f 7265  = 3.8.install_re
-00000200: 7175 6972 6573 203d 200a 0972 6f62 6f74  quires = ..robot
-00000210: 6672 616d 6577 6f72 6b20 3e3d 2034 2e30  framework >= 4.0
-00000220: 0a0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
-00000230: 5f70 6f69 6e74 735d 0a63 6f6e 736f 6c65  _points].console
-00000240: 5f73 6372 6970 7473 203d 200a 0974 6232  _scripts = ..tb2
-00000250: 726f 626f 7420 3d20 7465 7374 6265 6e63  robot = testbenc
-00000260: 6832 726f 626f 7466 7261 6d65 776f 726b  h2robotframework
-00000270: 2e5f 5f6d 6169 6e5f 5f3a 7275 6e0a 0974  .__main__:run..t
-00000280: 6573 7462 656e 6368 3272 6f62 6f74 6672  estbench2robotfr
-00000290: 616d 6577 6f72 6b20 3d20 7465 7374 6265  amework = testbe
-000002a0: 6e63 6832 726f 626f 7466 7261 6d65 776f  nch2robotframewo
-000002b0: 726b 2e5f 5f6d 6169 6e5f 5f3a 7275 6e0a  rk.__main__:run.
-000002c0: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-000002d0: 5f72 6571 7569 7265 5d0a 6465 7620 3d20  _require].dev = 
-000002e0: 0a09 626c 6163 6b0a 0966 6c61 6b65 380a  ..black..flake8.
-000002f0: 0970 796c 696e 740a 096d 7970 790a 0970  .pylint..mypy..p
-00000300: 7974 6573 740a 0970 7974 6573 742d 636f  ytest..pytest-co
-00000310: 760a 0970 7974 6573 742d 7370 6563 0a09  v..pytest-spec..
-00000320: 6368 6563 6b2d 6d61 6e69 6665 7374 0a09  check-manifest..
-00000330: 7477 696e 650a 0977 6865 656c 0a09 7365  twine..wheel..se
-00000340: 7475 7074 6f6f 6c73 0a0a 5b6f 7074 696f  tuptools..[optio
-00000350: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000360: 5d0a 6578 636c 7564 6520 3d20 0a09 7465  ].exclude = ..te
-00000370: 7374 730a 0a5b 6567 675f 696e 666f 5d0a  sts..[egg_info].
-00000380: 7461 675f 6275 696c 6420 3d20 0a74 6167  tag_build = .tag
-00000390: 5f64 6174 6520 3d20 300a 0a              _date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2074 6573 7462 656e 6368 3272 6f62   = testbench2rob
+00000020: 6f74 6672 616d 6577 6f72 6b0d 0a61 7574  otframework..aut
+00000030: 686f 7220 3d20 696d 6275 7320 4147 0d0a  hor = imbus AG..
+00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2073  author_email = s
+00000050: 7570 706f 7274 4069 6d62 7573 2e64 650d  upport@imbus.de.
+00000060: 0a76 6572 7369 6f6e 203d 2061 7474 723a  .version = attr:
+00000070: 2074 6573 7462 656e 6368 3272 6f62 6f74   testbench2robot
+00000080: 6672 616d 6577 6f72 6b2e 5f5f 7665 7273  framework.__vers
+00000090: 696f 6e5f 5f0d 0a64 6573 6372 6970 7469  ion__..descripti
+000000a0: 6f6e 203d 2052 6f62 6f74 2046 7261 6d65  on = Robot Frame
+000000b0: 776f 726b 2043 6f64 6520 4765 6e65 7261  work Code Genera
+000000c0: 746f 7220 6672 6f6d 204b 6579 776f 7264  tor from Keyword
+000000d0: 2d44 7269 7665 6e20 5465 7374 7320 696e  -Driven Tests in
+000000e0: 2069 6d62 7573 2054 6573 7442 656e 6368   imbus TestBench
+000000f0: 2033 2e30 2061 6e64 206e 6577 6572 0d0a   3.0 and newer..
+00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000110: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000120: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+00000130: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000140: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000150: 6e0d 0a6c 6963 656e 7365 203d 2041 7061  n..license = Apa
+00000160: 6368 6520 322e 3020 4c69 6365 6e73 650d  che 2.0 License.
+00000170: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000180: 6974 6875 622e 636f 6d2f 696d 6275 732f  ithub.com/imbus/
+00000190: 7465 7374 6265 6e63 6832 726f 626f 7466  testbench2robotf
+000001a0: 7261 6d65 776f 726b 0d0a 706c 6174 666f  ramework..platfo
+000001b0: 726d 7320 3d20 616e 790d 0a0d 0a5b 6f70  rms = any....[op
+000001c0: 7469 6f6e 735d 0d0a 7a69 705f 7361 6665  tions]..zip_safe
+000001d0: 203d 2046 616c 7365 0d0a 7061 636b 6167   = False..packag
+000001e0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000001f0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000200: 2033 2e38 0d0a 696e 7374 616c 6c5f 7265   3.8..install_re
+00000210: 7175 6972 6573 203d 200d 0a09 726f 626f  quires = ...robo
+00000220: 7466 7261 6d65 776f 726b 203e 3d20 352e  tframework >= 5.
+00000230: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  0....[options.en
+00000240: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+00000250: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+00000260: 0a09 7462 3272 6f62 6f74 203d 2074 6573  ..tb2robot = tes
+00000270: 7462 656e 6368 3272 6f62 6f74 6672 616d  tbench2robotfram
+00000280: 6577 6f72 6b2e 5f5f 6d61 696e 5f5f 3a72  ework.__main__:r
+00000290: 756e 0d0a 0974 6573 7462 656e 6368 3272  un...testbench2r
+000002a0: 6f62 6f74 6672 616d 6577 6f72 6b20 3d20  obotframework = 
+000002b0: 7465 7374 6265 6e63 6832 726f 626f 7466  testbench2robotf
+000002c0: 7261 6d65 776f 726b 2e5f 5f6d 6169 6e5f  ramework.__main_
+000002d0: 5f3a 7275 6e0d 0a0d 0a5b 6f70 7469 6f6e  _:run....[option
+000002e0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+000002f0: 5d0d 0a64 6576 203d 200d 0a09 626c 6163  ]..dev = ...blac
+00000300: 6b0d 0a09 666c 616b 6538 0d0a 0970 796c  k...flake8...pyl
+00000310: 696e 740d 0a09 6d79 7079 0d0a 0970 7974  int...mypy...pyt
+00000320: 6573 740d 0a09 7079 7465 7374 2d63 6f76  est...pytest-cov
+00000330: 0d0a 0970 7974 6573 742d 7370 6563 0d0a  ...pytest-spec..
+00000340: 0963 6865 636b 2d6d 616e 6966 6573 740d  .check-manifest.
+00000350: 0a09 7477 696e 650d 0a09 7768 6565 6c0d  ..twine...wheel.
+00000360: 0a09 7365 7475 7074 6f6f 6c73 0d0a 0972  ..setuptools...r
+00000370: 7566 660d 0a09 7069 702d 746f 6f6c 730d  uff...pip-tools.
+00000380: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000390: 6167 6573 2e66 696e 645d 0d0a 6578 636c  ages.find]..excl
+000003a0: 7564 6520 3d20 0d0a 0974 6573 7473 0d0a  ude = ...tests..
+000003b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000003c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000003d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/__init__.py` & `testbench2robotframework-0.6.1/testbench2robotframework/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2022-     imbus AG
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .testbench2robotframework import testbench2robotframework  # noqa: F401
-
-__version__ = "0.6.0"
+# Copyright 2022-     imbus AG
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from .testbench2robotframework import testbench2robotframework  # noqa: F401
+
+__version__ = "0.6.1"
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/__main__.py` & `testbench2robotframework-0.6.1/testbench2robotframework/__main__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# Copyright 2022-     imbus AG
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-import sys
-from pathlib import Path
-
-import robot
-
-from testbench2robotframework import __version__
-
-from .config import write_default_config
-from .json_reader import read_json
-from .robotframework2testbench import robot2testbench
-from .testbench2robotframework import testbench2robotframework
-from .utils import arg_parser
-
-
-def run():
-    args = arg_parser.parse_args()
-    if args.subcommand is None and not args.version:
-        arg_parser.print_help()
-        sys.exit()
-    if args.version:
-        print_version()
-        sys.exit()
-    if not Path(args.config).is_file():
-        write_default_config(args.config)
-    configuration = read_json(args.config)
-    if args.subcommand == 'write':
-        testbench2robotframework(args.jsonReport[0], configuration)
-    elif args.subcommand == 'read':
-        robot2testbench(args.jsonReport[0], args.output, args.result, configuration)
-
-
-def print_version():
-    print(  # noqa: T201
-        f'TestBench2RobotFramework {__version__} with '
-        f'[Robot Framework {robot.version.get_full_version()}]'
-    )
-
-
-if __name__ == "__main__":
-    run()
+# Copyright 2022-     imbus AG
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+import sys
+from pathlib import Path
+
+import robot
+
+from testbench2robotframework import __version__
+
+from .config import write_default_config
+from .json_reader import read_json
+from .robotframework2testbench import robot2testbench
+from .testbench2robotframework import testbench2robotframework
+from .utils import arg_parser
+
+
+def run():
+    args = arg_parser.parse_args()
+    if args.subcommand is None and not args.version:
+        arg_parser.print_help()
+        sys.exit()
+    if args.version:
+        print_version()
+        sys.exit()
+    if not Path(args.config).is_file():
+        write_default_config(args.config)
+    configuration = read_json(args.config)
+    if args.subcommand == 'write':
+        testbench2robotframework(args.jsonReport[0], configuration)
+    elif args.subcommand == 'read':
+        robot2testbench(args.jsonReport[0], args.output, args.result, configuration)
+
+
+def print_version():
+    print(  # noqa: T201
+        f'TestBench2RobotFramework {__version__} with '
+        f'[Robot Framework {robot.version.get_full_version()}]'
+    )
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/config.py` & `testbench2robotframework-0.6.1/testbench2robotframework/config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# pylint: skip-file
-from __future__ import annotations
-
-import json
-from dataclasses import dataclass
-from typing import Dict, List, Union
-
-from .model import StrEnum
-
-
-@dataclass
-class SubdivisionsMapping:
-    libraries: Dict
-    resources: Dict
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            libraries=dictionary.get("libraries", {}), resources=dictionary.get("resources", {})
-        )
-
-
-@dataclass
-class ForcedImport:
-    libraries: List[str]
-    resources: List[str]
-    variables: List[str]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            libraries=dictionary.get("libraries", []),
-            resources=dictionary.get("resources", []),
-            variables=dictionary.get("variables", []),
-        )
-
-
-class LogLevel(StrEnum):
-    CRITICAL = "CRITICAL"
-    FATAL = CRITICAL
-    ERROR = "ERROR"
-    WARNING = "WARNING"
-    WARN = WARNING
-    INFO = "INFO"
-    DEBUG = "DEBUG"
-    NOTSET = "NOTSET"
-
-
-@dataclass
-class ConsoleLoggerConfig:
-    logLevel: LogLevel
-    logFormat: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        log_level = dictionary.get("logLevel", "INFO").upper()
-        if log_level not in LogLevel.__members__:
-            print(
-                f"ValueError: {log_level} is not a valid logLevel. "
-                f"Available logLevel are: {list(LogLevel.__members__)}"
-            )
-            log_level = LogLevel.INFO
-        return cls(
-            logLevel=LogLevel(log_level),
-            logFormat=dictionary.get("logFormat", "%(levelname)s: %(message)s"),
-        )
-
-
-@dataclass
-class FileLoggerConfig(ConsoleLoggerConfig):
-    fileName: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        log_level = dictionary.get("logLevel", "DEBUG").upper()
-        if log_level not in LogLevel.__members__:
-            print(
-                f"ValueError: {log_level} is not a valid logLevel. "
-                f"Available logLevel are: {list(LogLevel.__members__)}"
-            )
-            log_level = LogLevel.DEBUG
-        return cls(
-            logLevel=log_level,
-            logFormat=dictionary.get(
-                "logFormat", "%(asctime)s - %(filename)s:%(lineno)d - %(levelname)8s - %(message)s"
-            ),
-            fileName=dictionary.get("fileName", "testbench2robotframework.log"),
-        )
-
-
-@dataclass
-class LoggingConfig:
-    console: ConsoleLoggerConfig
-    file: FileLoggerConfig
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            console=ConsoleLoggerConfig.from_dict(dictionary.get("console", {})),
-            file=FileLoggerConfig.from_dict(dictionary.get("file", {})),
-        )
-
-
-class ReferenceBehaviour(StrEnum):
-    ATTACHMENT = "ATTACHMENT"
-    REFERENCE = "REFERENCE"
-    NONE = "NONE"
-
-
-class AttachmentConflictBehaviour(StrEnum):
-    ERROR = "ERROR"
-    USE_NEW = "USE_NEW"
-    USE_EXISTING = "USE_EXISTING"
-    RENAME_NEW = "RENAME_NEW"
-
-
-@dataclass
-class Configuration:
-    rfLibraryRegex: List[str]
-    rfResourceRegex: List[str]
-    rfLibraryRoots: List[str]
-    rfResourceRoots: List[str]
-    fullyQualified: bool
-    subdivisionsMapping: SubdivisionsMapping
-    forcedImport: ForcedImport
-    generationDirectory: str
-    createOutputZip: bool
-    resourceDirectory: str
-    logSuiteNumbering: bool
-    clearGenerationDirectory: bool
-    loggingConfiguration: LoggingConfig
-    logCompoundInteractions: bool
-    testCaseSplitPathRegEx: str
-    phasePattern: str
-    referenceBehaviour: ReferenceBehaviour
-    attachmentConflictBehaviour: AttachmentConflictBehaviour
-
-    @classmethod
-    def from_dict(cls, dictionary) -> Configuration:
-        return cls(
-            rfLibraryRegex=dictionary.get(
-                "rfLibraryRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Library\].*"]
-            ),
-            rfResourceRegex=dictionary.get(
-                "rfResourceRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Resource\].*"]
-            ),
-            rfLibraryRoots=dictionary.get("rfLibraryRoots", ["RF", "RF-Library"]),
-            rfResourceRoots=dictionary.get("rfResourceRoots", ["RF-Resource"]),
-            fullyQualified=dictionary.get("fullyQualified", False),
-            subdivisionsMapping=SubdivisionsMapping.from_dict(
-                dictionary.get("subdivisionsMapping", {})
-            ),
-            forcedImport=ForcedImport.from_dict(dictionary.get("forcedImport", {})),
-            generationDirectory=dictionary.get("generationDirectory", "{root}/Generated"),
-            createOutputZip=dictionary.get("createOutputZip", False),
-            logSuiteNumbering=dictionary.get("logSuiteNumbering", False),
-            clearGenerationDirectory=dictionary.get("clearGenerationDirectory", True),
-            loggingConfiguration=LoggingConfig.from_dict(
-                dictionary.get("loggingConfiguration", {})
-            ),
-            logCompoundInteractions=dictionary.get("logCompoundInteractions", True),
-            resourceDirectory=dictionary.get("resourceDirectory", "{root}/Resources").replace(
-                '\\', '/'
-            ),
-            testCaseSplitPathRegEx=dictionary.get("testCaseSplitPathRegEx", ".*StopWithRestart.*"),
-            phasePattern=dictionary.get("phasePattern", "{testcase} : Phase {index}/{length}"),
-            referenceBehaviour=ReferenceBehaviour(
-                dictionary.get("referenceBehaviour", "ATTACHMENT").upper()
-            ),
-            attachmentConflictBehaviour=AttachmentConflictBehaviour(
-                dictionary.get("attachmentConflictBehaviour", "USE_EXISTING").upper()
-            ),
-        )
-
-
-def write_default_config(config_file):
-    with open(config_file, 'w', encoding='utf-8') as file:
-        json.dump(
-            Configuration.from_dict({}).__dict__,
-            file,
-            default=lambda o: o.__dict__,
-            indent=2,
-        )
+# pylint: skip-file
+from __future__ import annotations
+
+import json
+from dataclasses import dataclass
+from typing import Dict, List, Union
+
+from .model import StrEnum
+
+
+@dataclass
+class SubdivisionsMapping:
+    libraries: Dict
+    resources: Dict
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            libraries=dictionary.get("libraries", {}), resources=dictionary.get("resources", {})
+        )
+
+
+@dataclass
+class ForcedImport:
+    libraries: List[str]
+    resources: List[str]
+    variables: List[str]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            libraries=dictionary.get("libraries", []),
+            resources=dictionary.get("resources", []),
+            variables=dictionary.get("variables", []),
+        )
+
+
+class LogLevel(StrEnum):
+    CRITICAL = "CRITICAL"
+    FATAL = CRITICAL
+    ERROR = "ERROR"
+    WARNING = "WARNING"
+    WARN = WARNING
+    INFO = "INFO"
+    DEBUG = "DEBUG"
+    NOTSET = "NOTSET"
+
+
+@dataclass
+class ConsoleLoggerConfig:
+    logLevel: LogLevel
+    logFormat: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        log_level = dictionary.get("logLevel", "INFO").upper()
+        if log_level not in LogLevel.__members__:
+            print(
+                f"ValueError: {log_level} is not a valid logLevel. "
+                f"Available logLevel are: {list(LogLevel.__members__)}"
+            )
+            log_level = LogLevel.INFO
+        return cls(
+            logLevel=LogLevel(log_level),
+            logFormat=dictionary.get("logFormat", "%(levelname)s: %(message)s"),
+        )
+
+
+@dataclass
+class FileLoggerConfig(ConsoleLoggerConfig):
+    fileName: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        log_level = dictionary.get("logLevel", "DEBUG").upper()
+        if log_level not in LogLevel.__members__:
+            print(
+                f"ValueError: {log_level} is not a valid logLevel. "
+                f"Available logLevel are: {list(LogLevel.__members__)}"
+            )
+            log_level = LogLevel.DEBUG
+        return cls(
+            logLevel=log_level,
+            logFormat=dictionary.get(
+                "logFormat", "%(asctime)s - %(filename)s:%(lineno)d - %(levelname)8s - %(message)s"
+            ),
+            fileName=dictionary.get("fileName", "testbench2robotframework.log"),
+        )
+
+
+@dataclass
+class LoggingConfig:
+    console: ConsoleLoggerConfig
+    file: FileLoggerConfig
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            console=ConsoleLoggerConfig.from_dict(dictionary.get("console", {})),
+            file=FileLoggerConfig.from_dict(dictionary.get("file", {})),
+        )
+
+
+class ReferenceBehaviour(StrEnum):
+    ATTACHMENT = "ATTACHMENT"
+    REFERENCE = "REFERENCE"
+    NONE = "NONE"
+
+
+class AttachmentConflictBehaviour(StrEnum):
+    ERROR = "ERROR"
+    USE_NEW = "USE_NEW"
+    USE_EXISTING = "USE_EXISTING"
+    RENAME_NEW = "RENAME_NEW"
+
+
+@dataclass
+class Configuration:
+    rfLibraryRegex: List[str]
+    rfResourceRegex: List[str]
+    rfLibraryRoots: List[str]
+    rfResourceRoots: List[str]
+    fullyQualified: bool
+    subdivisionsMapping: SubdivisionsMapping
+    forcedImport: ForcedImport
+    generationDirectory: str
+    createOutputZip: bool
+    resourceDirectory: str
+    logSuiteNumbering: bool
+    clearGenerationDirectory: bool
+    loggingConfiguration: LoggingConfig
+    logCompoundInteractions: bool
+    testCaseSplitPathRegEx: str
+    phasePattern: str
+    referenceBehaviour: ReferenceBehaviour
+    attachmentConflictBehaviour: AttachmentConflictBehaviour
+
+    @classmethod
+    def from_dict(cls, dictionary) -> Configuration:
+        return cls(
+            rfLibraryRegex=dictionary.get(
+                "rfLibraryRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Library\].*"]
+            ),
+            rfResourceRegex=dictionary.get(
+                "rfResourceRegex", [r"(?:.*\.)?(?P<resourceName>[^.]+?)\s*\[Robot-Resource\].*"]
+            ),
+            rfLibraryRoots=dictionary.get("rfLibraryRoots", ["RF", "RF-Library"]),
+            rfResourceRoots=dictionary.get("rfResourceRoots", ["RF-Resource"]),
+            fullyQualified=dictionary.get("fullyQualified", False),
+            subdivisionsMapping=SubdivisionsMapping.from_dict(
+                dictionary.get("subdivisionsMapping", {})
+            ),
+            forcedImport=ForcedImport.from_dict(dictionary.get("forcedImport", {})),
+            generationDirectory=dictionary.get("generationDirectory", "{root}/Generated"),
+            createOutputZip=dictionary.get("createOutputZip", False),
+            logSuiteNumbering=dictionary.get("logSuiteNumbering", False),
+            clearGenerationDirectory=dictionary.get("clearGenerationDirectory", True),
+            loggingConfiguration=LoggingConfig.from_dict(
+                dictionary.get("loggingConfiguration", {})
+            ),
+            logCompoundInteractions=dictionary.get("logCompoundInteractions", True),
+            resourceDirectory=dictionary.get("resourceDirectory", "{root}/Resources").replace(
+                '\\', '/'
+            ),
+            testCaseSplitPathRegEx=dictionary.get("testCaseSplitPathRegEx", ".*StopWithRestart.*"),
+            phasePattern=dictionary.get("phasePattern", "{testcase} : Phase {index}/{length}"),
+            referenceBehaviour=ReferenceBehaviour(
+                dictionary.get("referenceBehaviour", "ATTACHMENT").upper()
+            ),
+            attachmentConflictBehaviour=AttachmentConflictBehaviour(
+                dictionary.get("attachmentConflictBehaviour", "USE_EXISTING").upper()
+            ),
+        )
+
+
+def write_default_config(config_file):
+    with open(config_file, 'w', encoding='utf-8') as file:
+        json.dump(
+            Configuration.from_dict({}).__dict__,
+            file,
+            default=lambda o: o.__dict__,
+            indent=2,
+        )
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/json_reader.py` & `testbench2robotframework-0.6.1/testbench2robotframework/json_reader.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import json
-import sys
-from dataclasses import dataclass
-from json import JSONDecodeError
-from pathlib import Path
-from typing import Dict, List, Optional
-
-from .log import logger
-from .model import (
-    TestCaseDetails,
-    TestCaseSetDetails,
-    TestStructureTree,
-    TestStructureTreeNodeType,
-)
-
-TEST_STRUCTURE_TREE_FILE = "TestThemeTree.json"
-
-
-@dataclass
-class TestCaseSet:
-    details: TestCaseSetDetails
-    test_cases: Dict[str, TestCaseDetails]
-
-    @property
-    def metadata(self) -> Dict[str, str]:
-        return {
-            "UniqueID": self.details.uniqueID,
-            "Name": self.details.name,
-            "Numbering": self.details.numbering,
-        }
-
-
-class TestBenchJsonReader:
-    def __init__(self, json_dir):
-        self.json_dir = json_dir
-        self._test_theme_tree: Optional[TestStructureTree] = None
-        self._test_case_sets: Dict[str, TestCaseSetDetails] = {}
-        self._test_cases: Dict[str, TestCaseDetails] = {}
-        if not json_dir:
-            logger.warning("No jsonReport path given.")
-            sys.exit()
-
-    @property
-    def test_theme_tree(self) -> TestStructureTree:
-        if not self._test_theme_tree:
-            test_theme_path = Path(self.json_dir) / TEST_STRUCTURE_TREE_FILE
-            logger.debug(f"Loading TestThemeTree from {test_theme_path}")
-            test_structure_tree = read_json(str(test_theme_path))
-            self._test_theme_tree = TestStructureTree.from_dict(test_structure_tree)
-            logger.info(f"{len(self._test_theme_tree.nodes)} nodes from TestThemeTree loaded.")
-        return self._test_theme_tree
-
-    @property
-    def test_case_sets(self) -> Dict[str, TestCaseSetDetails]:
-        if not self._test_case_sets:
-            for tcs_uid in self.get_test_case_set_uids():
-                test_case_set = self.read_test_case_set(tcs_uid)
-                if test_case_set is not None:
-                    self._test_case_sets[tcs_uid] = test_case_set
-                    logger.debug(f"TestCaseSetDetails {tcs_uid} loaded.")
-                else:
-                    logger.debug(f"TestCaseSetDetails {tcs_uid} not found.")
-            logger.info(f"{len(self._test_case_sets)} TestCaseSetDetails loaded.")
-        return self._test_case_sets
-
-    @property
-    def test_cases(self) -> Dict[str, TestCaseDetails]:
-        if not self._test_cases:
-            for tcs_uid in self.test_case_sets:
-                tc_uids = self.get_test_case_uids(tcs_uid)
-                self._read_test_cases(tc_uids)
-        return self._test_cases
-
-    def _read_test_cases(self, tc_uids):
-        for tc_uid in tc_uids:
-            test_case = self.read_test_case(tc_uid)
-            if test_case is not None:
-                self._test_cases[tc_uid] = test_case
-                logger.debug(f"TestCaseDetails {tc_uid} loaded.")
-
-    def get_test_case_set_catalog(self):
-        tcs_catalog: Dict[str, TestCaseSet] = {}
-        for tcs_uid, tcs in self.test_case_sets.items():
-            tc_catalog: Dict[str, TestCaseDetails] = {}
-            for tc_uid in self.get_test_case_uids(tcs_uid):
-                tc_catalog[tc_uid] = self.test_cases[tc_uid]
-            tcs_catalog[tcs_uid] = TestCaseSet(tcs, tc_catalog)
-        return tcs_catalog
-
-    def get_test_case_set_uids(self) -> List[str]:
-        nodes = self.test_theme_tree.nodes
-        return [
-            tse.baseInformation.uniqueID
-            for tse in nodes
-            if tse.elementType == TestStructureTreeNodeType.TestCaseSet
-        ]
-
-    def get_test_case_uids(self, test_case_set_uid: str) -> List[str]:
-        if not self._test_case_sets:
-            test_case_set = self.read_test_case_set(test_case_set_uid)
-            if test_case_set is None:
-                logger.debug(f"TestCaseSet with uid '{test_case_set_uid}' not found.")
-                return []
-        else:
-            test_case_set = self.test_case_sets[test_case_set_uid]
-        return [tc.uniqueID for tc in test_case_set.testCases]
-
-    def read_test_case_set(self, uid) -> Optional[TestCaseSetDetails]:
-        tcs_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
-        if tcs_dict is None:
-            return None
-        return TestCaseSetDetails.from_dict(tcs_dict)
-
-    def read_test_case(self, uid) -> Optional[TestCaseDetails]:
-        tc_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
-        if tc_dict is None:
-            return None
-        return TestCaseDetails.from_dict(tc_dict)
-
-    def read_test_theme_tree(self) -> Optional[TestStructureTree]:
-        test_structure_tree = read_json(str(Path(self.json_dir, TEST_STRUCTURE_TREE_FILE)))
-        if test_structure_tree is None:
-            return None
-        return TestStructureTree.from_dict(test_structure_tree)
-
-
-def read_json(filepath: str):  # ToDo Configure to run silent or raise
-    try:
-        with Path(filepath).open(encoding='utf-8') as json_file:
-            return json.load(json_file)
-    except FileNotFoundError:
-        logger.debug(f"Cannot find json file {filepath}:")
-        return None
-    except JSONDecodeError as error:  # pylint: disable=broad-except
-        logger.warning(f"Cannot decode json file {filepath}:")
-        logger.warning(error)
-        return None
+import json
+import sys
+from dataclasses import dataclass
+from json import JSONDecodeError
+from pathlib import Path
+from typing import Dict, List, Optional
+
+from .log import logger
+from .model import (
+    TestCaseDetails,
+    TestCaseSetDetails,
+    TestStructureTree,
+    TestStructureTreeNodeType,
+)
+
+TEST_STRUCTURE_TREE_FILE = "TestThemeTree.json"
+
+
+@dataclass
+class TestCaseSet:
+    details: TestCaseSetDetails
+    test_cases: Dict[str, TestCaseDetails]
+
+    @property
+    def metadata(self) -> Dict[str, str]:
+        return {
+            "UniqueID": self.details.uniqueID,
+            "Name": self.details.name,
+            "Numbering": self.details.numbering,
+        }
+
+
+class TestBenchJsonReader:
+    def __init__(self, json_dir):
+        self.json_dir = json_dir
+        self._test_theme_tree: Optional[TestStructureTree] = None
+        self._test_case_sets: Dict[str, TestCaseSetDetails] = {}
+        self._test_cases: Dict[str, TestCaseDetails] = {}
+        if not json_dir:
+            logger.warning("No jsonReport path given.")
+            sys.exit()
+
+    @property
+    def test_theme_tree(self) -> TestStructureTree:
+        if not self._test_theme_tree:
+            test_theme_path = Path(self.json_dir) / TEST_STRUCTURE_TREE_FILE
+            logger.debug(f"Loading TestThemeTree from {test_theme_path}")
+            test_structure_tree = read_json(str(test_theme_path))
+            self._test_theme_tree = TestStructureTree.from_dict(test_structure_tree)
+            logger.info(f"{len(self._test_theme_tree.nodes)} nodes from TestThemeTree loaded.")
+        return self._test_theme_tree
+
+    @property
+    def test_case_sets(self) -> Dict[str, TestCaseSetDetails]:
+        if not self._test_case_sets:
+            for tcs_uid in self.get_test_case_set_uids():
+                test_case_set = self.read_test_case_set(tcs_uid)
+                if test_case_set is not None:
+                    self._test_case_sets[tcs_uid] = test_case_set
+                    logger.debug(f"TestCaseSetDetails {tcs_uid} loaded.")
+                else:
+                    logger.debug(f"TestCaseSetDetails {tcs_uid} not found.")
+            logger.info(f"{len(self._test_case_sets)} TestCaseSetDetails loaded.")
+        return self._test_case_sets
+
+    @property
+    def test_cases(self) -> Dict[str, TestCaseDetails]:
+        if not self._test_cases:
+            for tcs_uid in self.test_case_sets:
+                tc_uids = self.get_test_case_uids(tcs_uid)
+                self._read_test_cases(tc_uids)
+        return self._test_cases
+
+    def _read_test_cases(self, tc_uids):
+        for tc_uid in tc_uids:
+            test_case = self.read_test_case(tc_uid)
+            if test_case is not None:
+                self._test_cases[tc_uid] = test_case
+                logger.debug(f"TestCaseDetails {tc_uid} loaded.")
+
+    def get_test_case_set_catalog(self):
+        tcs_catalog: Dict[str, TestCaseSet] = {}
+        for tcs_uid, tcs in self.test_case_sets.items():
+            tc_catalog: Dict[str, TestCaseDetails] = {}
+            for tc_uid in self.get_test_case_uids(tcs_uid):
+                tc_catalog[tc_uid] = self.test_cases[tc_uid]
+            tcs_catalog[tcs_uid] = TestCaseSet(tcs, tc_catalog)
+        return tcs_catalog
+
+    def get_test_case_set_uids(self) -> List[str]:
+        nodes = self.test_theme_tree.nodes
+        return [
+            tse.baseInformation.uniqueID
+            for tse in nodes
+            if tse.elementType == TestStructureTreeNodeType.TestCaseSet
+        ]
+
+    def get_test_case_uids(self, test_case_set_uid: str) -> List[str]:
+        if not self._test_case_sets:
+            test_case_set = self.read_test_case_set(test_case_set_uid)
+            if test_case_set is None:
+                logger.debug(f"TestCaseSet with uid '{test_case_set_uid}' not found.")
+                return []
+        else:
+            test_case_set = self.test_case_sets[test_case_set_uid]
+        return [tc.uniqueID for tc in test_case_set.testCases]
+
+    def read_test_case_set(self, uid) -> Optional[TestCaseSetDetails]:
+        tcs_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
+        if tcs_dict is None:
+            return None
+        return TestCaseSetDetails.from_dict(tcs_dict)
+
+    def read_test_case(self, uid) -> Optional[TestCaseDetails]:
+        tc_dict = read_json(str(Path(self.json_dir, f"{uid}.json")))
+        if tc_dict is None:
+            return None
+        return TestCaseDetails.from_dict(tc_dict)
+
+    def read_test_theme_tree(self) -> Optional[TestStructureTree]:
+        test_structure_tree = read_json(str(Path(self.json_dir, TEST_STRUCTURE_TREE_FILE)))
+        if test_structure_tree is None:
+            return None
+        return TestStructureTree.from_dict(test_structure_tree)
+
+
+def read_json(filepath: str):  # ToDo Configure to run silent or raise
+    try:
+        with Path(filepath).open(encoding='utf-8') as json_file:
+            return json.load(json_file)
+    except FileNotFoundError:
+        logger.debug(f"Cannot find json file {filepath}:")
+        return None
+    except JSONDecodeError as error:  # pylint: disable=broad-except
+        logger.warning(f"Cannot decode json file {filepath}:")
+        logger.warning(error)
+        return None
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/json_writer.py` & `testbench2robotframework-0.6.1/testbench2robotframework/json_writer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import json
-from dataclasses import asdict
-from pathlib import Path
-from typing import Union
-
-from .config import Configuration
-from .log import logger
-from .model import TestCaseDetails, TestCaseSetDetails, TestStructureTree
-
-TEST_STRUCTURE_TREE_FILE = "TestThemeTree"
-
-
-def write_test_structure_element(
-    json_dir: str,
-    test_structure_element: Union[TestStructureTree, TestCaseSetDetails, TestCaseDetails],
-) -> None:
-    if isinstance(test_structure_element, TestStructureTree):
-        filepath = Path(json_dir) / Path(TEST_STRUCTURE_TREE_FILE + ".json")
-    else:
-        filepath = Path(json_dir) / Path(f"{test_structure_element.uniqueID}.json")
-    with Path(filepath).open('w+', encoding="utf8") as output_file:
-        json.dump(asdict(test_structure_element), output_file, indent=2)
-
-
-def write_default_config(config_file):
-    with Path(config_file).open('w+', encoding='utf-8') as file:
-        json.dump(
-            Configuration.from_dict({}).__dict__,
-            file,
-            default=lambda o: o.__dict__,
-            indent=2,
-        )
-        logger.warning(f"Default Configuration generated to {config_file}")
+import json
+from dataclasses import asdict
+from pathlib import Path
+from typing import Union
+
+from .config import Configuration
+from .log import logger
+from .model import TestCaseDetails, TestCaseSetDetails, TestStructureTree
+
+TEST_STRUCTURE_TREE_FILE = "TestThemeTree"
+
+
+def write_test_structure_element(
+    json_dir: str,
+    test_structure_element: Union[TestStructureTree, TestCaseSetDetails, TestCaseDetails],
+) -> None:
+    if isinstance(test_structure_element, TestStructureTree):
+        filepath = Path(json_dir) / Path(TEST_STRUCTURE_TREE_FILE + ".json")
+    else:
+        filepath = Path(json_dir) / Path(f"{test_structure_element.uniqueID}.json")
+    with Path(filepath).open('w+', encoding="utf8") as output_file:
+        json.dump(asdict(test_structure_element), output_file, indent=2)
+
+
+def write_default_config(config_file):
+    with Path(config_file).open('w+', encoding='utf-8') as file:
+        json.dump(
+            Configuration.from_dict({}).__dict__,
+            file,
+            default=lambda o: o.__dict__,
+            indent=2,
+        )
+        logger.warning(f"Default Configuration generated to {config_file}")
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/log.py` & `testbench2robotframework-0.6.1/testbench2robotframework/log.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import logging
-from logging.handlers import RotatingFileHandler
-
-from .config import Configuration
-
-logger = logging.Logger("iTB2RF", logging.DEBUG)
-
-
-def setup_logger(config: Configuration):
-    console_handler = logging.StreamHandler()
-    console_handler.setLevel(config.loggingConfiguration.console.logLevel)
-    console_handler.setFormatter(logging.Formatter(config.loggingConfiguration.console.logFormat))
-    logger.addHandler(console_handler)
-
-    file_handler = RotatingFileHandler(
-        filename=config.loggingConfiguration.file.fileName,
-        mode="a",
-        maxBytes=1 * 1024 * 1024,
-        backupCount=2,
-        encoding="utf_8",
-        delay=False,
-    )
-    file_handler.setLevel(config.loggingConfiguration.file.logLevel)
-    file_handler.setFormatter(logging.Formatter(config.loggingConfiguration.file.logFormat))
-    logger.addHandler(file_handler)
+import logging
+from logging.handlers import RotatingFileHandler
+
+from .config import Configuration
+
+logger = logging.Logger("iTB2RF", logging.DEBUG)
+
+
+def setup_logger(config: Configuration):
+    console_handler = logging.StreamHandler()
+    console_handler.setLevel(config.loggingConfiguration.console.logLevel)
+    console_handler.setFormatter(logging.Formatter(config.loggingConfiguration.console.logFormat))
+    logger.addHandler(console_handler)
+
+    file_handler = RotatingFileHandler(
+        filename=config.loggingConfiguration.file.fileName,
+        mode="a",
+        maxBytes=1 * 1024 * 1024,
+        backupCount=2,
+        encoding="utf_8",
+        delay=False,
+    )
+    file_handler.setLevel(config.loggingConfiguration.file.logLevel)
+    file_handler.setFormatter(logging.Formatter(config.loggingConfiguration.file.logFormat))
+    logger.addHandler(file_handler)
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/model.py` & `testbench2robotframework-0.6.1/testbench2robotframework/model.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,802 +1,802 @@
-# pylint: skip-file
-from __future__ import annotations
-
-from dataclasses import dataclass
-from enum import Enum, auto
-from optparse import Option
-from typing import List, Optional
-
-
-class StrEnum(str, Enum):
-    def __new__(cls, *args):
-        for arg in args:
-            if not isinstance(arg, (str, auto)):
-                raise TypeError(f"Values of StrEnums must be strings: {repr(arg)} is a {type(arg)}")
-        return super().__new__(cls, *args)
-
-    def __str__(self):
-        return self.value
-
-    def _generate_next_value_(name, *_):
-        return name
-
-
-class FilterType(StrEnum):
-    TestThemeFilter = "TestThemeFilter"
-    TestCaseSetFilter = "TestCaseSetFilter"
-    TestCaseFilter = "TestCaseFilter"
-
-
-class TestStructureTreeNodeType(StrEnum):
-    Root = "Root"
-    TestTheme = "TestTheme"
-    TestCaseSet = "TestCaseSet"
-
-
-class Priority(StrEnum):
-    High = "High"
-    Medium = "Medium"
-    Low = "Low"
-
-
-class ReferenceType(StrEnum):
-    Reference = "Reference"
-    Hyperlink = "Hyperlink"
-    Attachment = "Attachment"
-
-
-class SpecificationStatus(StrEnum):
-    NotPlanned = "NotPlanned"
-    Planned = "Planned"
-    InProgress = "InProgress"
-    InReview = "InReview"
-    Released = "Released"
-
-
-class InteractionVerdict(StrEnum):
-    Pass = "Pass"
-    Fail = "Fail"
-    Skipped = "Skipped"
-    ToVerify = "ToVerify"
-    Warn = "Warn"
-    Undefined = "Undefined"
-    Blocked = "Blocked"
-
-
-class ExecutionVerdict(StrEnum):
-    Undefined = "Undefined"
-    Pass = "Pass"
-    Fail = "Fail"
-    ToVerify = "ToVerify"
-
-
-class ActivityStatus(StrEnum):
-    NotPlanned = "NotPlanned"
-    Planned = "Planned"
-    Assigned = "Assigned"
-    Running = "Running"
-    Canceled = "Canceled"
-    Skipped = "Skipped"
-    Performed = "Performed"
-
-
-class ExecutionStatus(StrEnum):
-    NotBlocked = "NotBlocked"
-    Blocked = "Blocked"
-
-
-class UdfType(StrEnum):
-    String = "String"
-    Enumeration = "Enumeration"
-    Boolean = "Boolean"
-
-
-class SequencePhase(StrEnum):
-    Setup = "Setup"
-    TestStep = "TestStep"
-    Teardown = "Teardown"
-
-
-class CallType(StrEnum):
-    Check = "Check"
-    Flow = "Flow"
-
-
-class InteractionType(StrEnum):
-    Compound = "Compound"
-    Atomic = "Atomic"
-    Textuell = "Textuell"
-
-
-class ParameterType(StrEnum):
-    DetailedInstance = "DetailedInstance"
-    Unknown = "Unknown"
-    InstanceTable = "InstanceTable"
-    AtomicInstance = "AtomicInstance"
-
-
-class ParameterUseType(StrEnum):
-    CallByReference = "CallByReference"
-    CallByValue = "CallByValue"
-    CallByReferenceMandatory = "CallByReferenceMandatory"
-
-
-@dataclass
-class ProjectMember:
-    userkey: str
-    userLogin: str
-    userName: str
-    projectkey: str
-    projectName: str
-    roles: List[str]
-
-
-@dataclass
-class ProjectDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    tovsCount: int
-    cyclesCount: int
-    description: str
-    lockerKey: Optional[int] = None
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class TOVDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    cyclesCount: int
-    description: str
-    lockerKey: Optional[int] = None
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class CycleDetails:
-    key: str
-    creationTime: str
-    name: str
-    status: str
-    visibility: bool
-    description: str
-    startDate: Optional[str] = None
-    endDate: Optional[str] = None
-
-
-@dataclass
-class UserDetails:
-    key: str
-    login: str
-    name: str
-    email: str
-    passwordExpired: bool
-    active: bool
-
-
-@dataclass
-class UserSummary:
-    key: str
-    login: str
-    name: str
-    active: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            login=dictionary.get("login", ""),
-            name=dictionary.get("name", ""),
-            active=dictionary.get("active", True),
-        )
-
-
-@dataclass
-class UserDefinedField:
-    key: str
-    name: str
-    value: str
-    valueType: UdfType
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            name=dictionary.get("name", ""),
-            value=dictionary.get("value", ""),
-            valueType=UdfType(dictionary.get("valueType", UdfType.String)),
-        )
-
-    @property
-    def robot_tag(self) -> Optional[str]:
-        if self.valueType == UdfType.Enumeration and self.value:
-            return f"{self.name}:{self.value}"
-        elif self.valueType == UdfType.String and self.value:
-            return f"{self.name}:{self.value}"
-        elif self.valueType == UdfType.Boolean and self.value == "true":
-            return self.name
-        return None
-
-
-@dataclass
-class Keyword:
-    key: str
-    name: str
-    isVariantsMarker: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            name=dictionary.get("name", ""),
-            isVariantsMarker=dictionary.get("isVariantsMarker", False),
-        )
-
-
-@dataclass
-class Reference:
-    type: ReferenceType
-    path: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            type=ReferenceType(dictionary.get("type", ReferenceType.Reference)),
-            path=dictionary.get("path", ""),
-        )
-
-
-@dataclass
-class UserReference:
-    key: str
-    name: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(key=dictionary.get("key", ""), name=dictionary.get("name", ""))
-
-
-@dataclass
-class RequirementReference:
-    key: str
-    edited: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(key=dictionary.get("key", ""), edited=dictionary.get("edited", False))
-
-
-@dataclass
-class ConditionSummary:
-    key: str
-    uniqueId: str
-    name: str
-    description: str
-    version: Optional[str] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            uniqueId=dictionary.get("uniqueId", ""),
-            name=dictionary.get("name", ""),
-            description=dictionary.get("description", ""),
-            version=dictionary.get("version", None),
-        )
-
-
-@dataclass
-class TestCaseSetSpecificationSummary:
-    key: str
-    description: str
-    reviewComment: str
-    status: SpecificationStatus
-    priority: Optional[Priority]
-    responsible: Optional[UserReference]
-    dueDate: Optional[str]
-    reviewer: Optional[UserReference]
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    references: List[Reference]
-    requirements: List[RequirementReference]
-    preConditions: List[ConditionSummary]
-    postConditions: List[ConditionSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            description=dictionary.get("description", ""),
-            reviewComment=dictionary.get("reviewComment", ""),
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-            priority=Priority(dictionary.get("priority")) if dictionary.get("priority") else None,
-            responsible=UserReference.from_dict(dictionary.get("responsible", {}))
-            if dictionary.get("responsible")
-            else None,
-            dueDate=dictionary.get("dueDate", None),
-            reviewer=UserReference.from_dict(dictionary.get("reviewer", {}))
-            if dictionary.get("reviewer")
-            else None,
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            references=dictionary.get("references", ""),
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-            preConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("preConditions", [])
-            ],
-            postConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("postConditions", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseSpecificationDetails:
-    key: str
-    comments: str
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    requirements: List[RequirementReference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseSetExecutionSummary:
-    key: str
-    comments: str
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-        )
-
-
-@dataclass
-class TestCaseSpecificationSummary:
-    key: str
-    comments: str
-    requirements: List[RequirementReference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            comments=dictionary.get("comments", ""),
-            requirements=[
-                RequirementReference.from_dict(requirement)
-                for requirement in dictionary.get("requirements", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseExecutionSummary:
-    key: str
-    comments: str = ""
-    status: ActivityStatus = ActivityStatus.Planned
-    execStatus: ExecutionStatus = ExecutionStatus.NotBlocked
-    verdict: ExecutionVerdict = ExecutionVerdict.Undefined
-    defects: Optional[List[int]] = None
-    tester: Optional[UserReference] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-            comments=dictionary.get("comments", ""),
-            defects=dictionary.get("defects", []),
-            tester=UserReference.from_dict(dictionary.get("tester"))
-            if dictionary.get("tester")
-            else None,
-        )
-
-
-@dataclass
-class TestCaseSummary:
-    uniqueID: str
-    index: int
-    spec: TestCaseSpecificationSummary
-    exec: Optional[TestCaseExecutionSummary] = None
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            uniqueID=dictionary.get("uniqueID", ""),
-            index=dictionary.get("index", 0),
-            spec=TestCaseSpecificationSummary.from_dict(dictionary.get("spec", {})),
-            exec=TestCaseExecutionSummary.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-        )
-
-
-@dataclass
-class TestCaseExecutionDetails:
-    key: str
-    status: ActivityStatus
-    execStatus: ExecutionStatus
-    verdict: ExecutionVerdict
-    plannedDuration: int
-    actualDuration: int
-    currentUser: UserReference
-    tester: Optional[UserReference]
-    comments: str  # TODO: Insert htmlComment
-    version: Optional[str]
-    defects: List[int]
-    udfs: List[UserDefinedField]
-    keywords: List[Keyword]
-    references: List[Reference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-            plannedDuration=dictionary.get("plannedDuration", 0),
-            actualDuration=dictionary.get("actualDuration", 0),
-            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
-            tester=UserReference.from_dict(dictionary.get("tester", {}))
-            if dictionary.get("tester")
-            else None,
-            comments=dictionary.get("comments", ""),
-            version=dictionary.get("version", None),
-            defects=dictionary.get("defects", []),
-            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
-            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
-            references=dictionary.get("references", []),
-        )
-
-
-@dataclass
-class TestCaseSetDetails:
-    key: str
-    numbering: str
-    uniqueID: str
-    name: str
-    spec: TestCaseSetSpecificationSummary
-    exec: Optional[TestCaseSetExecutionSummary]
-    testCases: List[TestCaseSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestCaseSetDetails:
-        return cls(
-            key=dictionary.get("key", ""),
-            numbering=dictionary.get("numbering", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            name=dictionary.get("name", ""),
-            spec=TestCaseSetSpecificationSummary.from_dict(dictionary.get("spec", {})),
-            exec=TestCaseSetExecutionSummary.from_dict(dictionary.get("exec", {}))
-            if dictionary.get("exec")
-            else None,
-            testCases=[
-                TestCaseSummary.from_dict(test_case)
-                for test_case in dictionary.get("testCases", [])
-            ],
-        )
-
-
-@dataclass
-class InteractionExecutionSummary:
-    verdict: InteractionVerdict
-    time: str
-    duration: int
-    currentUser: UserReference
-    tester: UserReference
-    comments: str
-    references: List[Reference]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            verdict=InteractionVerdict(dictionary.get("verdict", InteractionVerdict.Undefined)),
-            time=dictionary.get("time", ""),
-            duration=dictionary.get("duration", 0),
-            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
-            tester=UserReference.from_dict(dictionary.get("tester", {})),
-            comments=dictionary.get("comments", ""),
-            references=dictionary.get("references", []),
-        )
-
-
-@dataclass
-class InteractionSpecificationSummary:
-    callId: int
-    sequencePhase: SequencePhase
-    callType: CallType
-    description: str
-    comments: str
-    references: List[Reference]
-    preConditions: List[ConditionSummary]
-    postConditions: List[ConditionSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            callId=dictionary.get("callId", ""),
-            sequencePhase=SequencePhase(dictionary.get("sequencePhase", SequencePhase.TestStep)),
-            callType=CallType(dictionary.get("callType", CallType.Flow)),
-            description=dictionary.get("description", ""),
-            comments=dictionary.get("comments", ""),
-            references=dictionary.get("references", ""),
-            preConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("preConditions", [])
-            ],
-            postConditions=[
-                ConditionSummary.from_dict(condition)
-                for condition in dictionary.get("postConditions", [])
-            ],
-        )
-
-
-@dataclass
-class ParameterSummary:
-    name: str
-    value: str
-    version: Optional[str]
-    parameterType: ParameterType
-    parameterUseType: ParameterUseType
-    dataTypeName: str
-    dataTypePath: str
-    dataTypeUniqueID: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            name=dictionary.get("name", ""),
-            value=dictionary.get("value", ""),
-            version=dictionary.get(
-                "version",
-            ),
-            parameterType=ParameterType(
-                dictionary.get("parameterType", ParameterType.AtomicInstance)
-            ),
-            parameterUseType=ParameterUseType(
-                dictionary.get("parameterUseType", ParameterUseType.CallByValue)
-            ),
-            dataTypeName=dictionary.get("dataTypeName", ""),
-            dataTypePath=dictionary.get("dataTypePath", ""),
-            dataTypeUniqueID=dictionary.get("dataTypeUniqueID", ""),
-        )
-
-
-@dataclass
-class InteractionDetails:
-    key: str
-    uniqueID: str
-    name: str
-    version: Optional[str]
-    interactionType: InteractionType
-    path: str
-    spec: InteractionSpecificationSummary
-    exec: Optional[InteractionExecutionSummary]
-    parameters: List[ParameterSummary]
-    interactions: List[InteractionDetails]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            name=dictionary.get("name", ""),
-            version=dictionary.get("version", ""),
-            interactionType=InteractionType(
-                dictionary.get("interactionType", InteractionType.Atomic)
-            ),
-            path=dictionary.get("path", ""),
-            spec=InteractionSpecificationSummary.from_dict(dictionary.get("spec")),
-            exec=InteractionExecutionSummary.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-            parameters=[
-                ParameterSummary.from_dict(param) for param in dictionary.get("parameters", [])
-            ],
-            interactions=[
-                InteractionDetails.from_dict(interaction)
-                for interaction in dictionary.get("interactions", [])
-            ],
-        )
-
-
-@dataclass
-class TestCaseDetails:
-    uniqueID: str
-    spec: TestCaseSpecificationDetails
-    exec: Optional[TestCaseExecutionDetails]
-    interactions: List[InteractionDetails]
-    parameters: List[ParameterSummary]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestCaseDetails:
-        return cls(
-            uniqueID=dictionary.get("uniqueID"),
-            spec=TestCaseSpecificationDetails.from_dict(dictionary.get("spec")),
-            exec=TestCaseExecutionDetails.from_dict(dictionary.get("exec"))
-            if dictionary.get("exec")
-            else None,
-            interactions=[
-                InteractionDetails.from_dict(interaction)
-                for interaction in dictionary.get("interactions", [])
-            ],
-            parameters=[
-                ParameterSummary.from_dict(parameter)
-                for parameter in dictionary.get("parameters", [])
-            ],
-        )
-
-
-@dataclass
-class TestStructureSpecification:
-    key: str
-    locker: Optional[UserReference]
-    status: SpecificationStatus
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-        )
-
-
-@dataclass
-class TestStructureAutomation:
-    key: str
-    locker: Optional[UserReference]
-    status: SpecificationStatus
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
-        )
-
-
-@dataclass
-class TestStructureExecution:
-    key: str
-    locker: Optional[UserReference]
-    status: ActivityStatus
-    execStatus: ExecutionStatus
-    verdict: ExecutionVerdict
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            locker=UserReference.from_dict(dictionary.get("locker", {}))
-            if dictionary.get("locker")
-            else None,
-            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
-            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
-            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
-        )
-
-
-@dataclass
-class AttachedFilter:
-    key: str
-    name: str
-    filterType: FilterType
-    content: str
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            name=dictionary.get("name", ""),
-            filterType=FilterType(dictionary.get("filterType", FilterType.TestCaseSetFilter)),
-            content=dictionary.get("content", ""),
-        )
-
-
-@dataclass
-class TestStructureTreeNodeInformation:
-    key: str
-    numbering: str
-    parentKey: str
-    name: str
-    uniqueID: str
-    orderPos: int
-    matchesFilter: bool
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            key=dictionary.get("key", "-1"),
-            numbering=dictionary.get("numbering", "-1"),
-            parentKey=dictionary.get("parentKey", "-1"),
-            name=dictionary.get("name", ""),
-            uniqueID=dictionary.get("uniqueID", ""),
-            orderPos=dictionary.get("orderPos", "-1"),
-            matchesFilter=dictionary.get("matchesFilter", True),
-        )
-
-
-@dataclass
-class TestStructureTreeNode:
-    elementType: TestStructureTreeNodeType
-    baseInformation: TestStructureTreeNodeInformation
-    specification: Optional[TestStructureSpecification]
-    automation: Optional[TestStructureAutomation]
-    execution: Optional[TestStructureExecution]
-    filters: List[AttachedFilter]
-
-    @classmethod
-    def from_dict(cls, dictionary):
-        return cls(
-            elementType=TestStructureTreeNodeType(
-                dictionary.get("elementType", TestStructureTreeNodeType.TestTheme)
-            ),
-            baseInformation=TestStructureTreeNodeInformation.from_dict(
-                dictionary.get("baseInformation", {})
-            ),
-            specification=TestStructureSpecification.from_dict(dictionary.get("specification"))
-            if dictionary.get("specification")
-            else None,
-            automation=TestStructureAutomation.from_dict(dictionary.get("automation"))
-            if dictionary.get("automation")
-            else None,
-            execution=TestStructureExecution.from_dict(dictionary.get("execution"))
-            if dictionary.get("execution")
-            else None,
-            filters=[AttachedFilter.from_dict(filter) for filter in dictionary.get("filters", [])],
-        )
-
-
-@dataclass
-class TestStructureTree:
-    root: TestStructureTreeNode
-    nodes: List[TestStructureTreeNode]
-
-    @classmethod
-    def from_dict(cls, dictionary) -> TestStructureTree:
-        return cls(
-            root=TestStructureTreeNode.from_dict(dictionary.get("root", {}))
-            if "root" in dictionary
-            else None,
-            nodes=[TestStructureTreeNode.from_dict(node) for node in dictionary.get("nodes", [])],
-        )
+# pylint: skip-file
+from __future__ import annotations
+
+from dataclasses import dataclass
+from enum import Enum, auto
+from optparse import Option
+from typing import List, Optional
+
+
+class StrEnum(str, Enum):
+    def __new__(cls, *args):
+        for arg in args:
+            if not isinstance(arg, (str, auto)):
+                raise TypeError(f"Values of StrEnums must be strings: {repr(arg)} is a {type(arg)}")
+        return super().__new__(cls, *args)
+
+    def __str__(self):
+        return self.value
+
+    def _generate_next_value_(name, *_):
+        return name
+
+
+class FilterType(StrEnum):
+    TestThemeFilter = "TestThemeFilter"
+    TestCaseSetFilter = "TestCaseSetFilter"
+    TestCaseFilter = "TestCaseFilter"
+
+
+class TestStructureTreeNodeType(StrEnum):
+    Root = "Root"
+    TestTheme = "TestTheme"
+    TestCaseSet = "TestCaseSet"
+
+
+class Priority(StrEnum):
+    High = "High"
+    Medium = "Medium"
+    Low = "Low"
+
+
+class ReferenceType(StrEnum):
+    Reference = "Reference"
+    Hyperlink = "Hyperlink"
+    Attachment = "Attachment"
+
+
+class SpecificationStatus(StrEnum):
+    NotPlanned = "NotPlanned"
+    Planned = "Planned"
+    InProgress = "InProgress"
+    InReview = "InReview"
+    Released = "Released"
+
+
+class InteractionVerdict(StrEnum):
+    Pass = "Pass"
+    Fail = "Fail"
+    Skipped = "Skipped"
+    ToVerify = "ToVerify"
+    Warn = "Warn"
+    Undefined = "Undefined"
+    Blocked = "Blocked"
+
+
+class ExecutionVerdict(StrEnum):
+    Undefined = "Undefined"
+    Pass = "Pass"
+    Fail = "Fail"
+    ToVerify = "ToVerify"
+
+
+class ActivityStatus(StrEnum):
+    NotPlanned = "NotPlanned"
+    Planned = "Planned"
+    Assigned = "Assigned"
+    Running = "Running"
+    Canceled = "Canceled"
+    Skipped = "Skipped"
+    Performed = "Performed"
+
+
+class ExecutionStatus(StrEnum):
+    NotBlocked = "NotBlocked"
+    Blocked = "Blocked"
+
+
+class UdfType(StrEnum):
+    String = "String"
+    Enumeration = "Enumeration"
+    Boolean = "Boolean"
+
+
+class SequencePhase(StrEnum):
+    Setup = "Setup"
+    TestStep = "TestStep"
+    Teardown = "Teardown"
+
+
+class CallType(StrEnum):
+    Check = "Check"
+    Flow = "Flow"
+
+
+class InteractionType(StrEnum):
+    Compound = "Compound"
+    Atomic = "Atomic"
+    Textuell = "Textuell"
+
+
+class ParameterType(StrEnum):
+    DetailedInstance = "DetailedInstance"
+    Unknown = "Unknown"
+    InstanceTable = "InstanceTable"
+    AtomicInstance = "AtomicInstance"
+
+
+class ParameterUseType(StrEnum):
+    CallByReference = "CallByReference"
+    CallByValue = "CallByValue"
+    CallByReferenceMandatory = "CallByReferenceMandatory"
+
+
+@dataclass
+class ProjectMember:
+    userkey: str
+    userLogin: str
+    userName: str
+    projectkey: str
+    projectName: str
+    roles: List[str]
+
+
+@dataclass
+class ProjectDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    tovsCount: int
+    cyclesCount: int
+    description: str
+    lockerKey: Optional[int] = None
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class TOVDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    cyclesCount: int
+    description: str
+    lockerKey: Optional[int] = None
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class CycleDetails:
+    key: str
+    creationTime: str
+    name: str
+    status: str
+    visibility: bool
+    description: str
+    startDate: Optional[str] = None
+    endDate: Optional[str] = None
+
+
+@dataclass
+class UserDetails:
+    key: str
+    login: str
+    name: str
+    email: str
+    passwordExpired: bool
+    active: bool
+
+
+@dataclass
+class UserSummary:
+    key: str
+    login: str
+    name: str
+    active: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            login=dictionary.get("login", ""),
+            name=dictionary.get("name", ""),
+            active=dictionary.get("active", True),
+        )
+
+
+@dataclass
+class UserDefinedField:
+    key: str
+    name: str
+    value: str
+    valueType: UdfType
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            name=dictionary.get("name", ""),
+            value=dictionary.get("value", ""),
+            valueType=UdfType(dictionary.get("valueType", UdfType.String)),
+        )
+
+    @property
+    def robot_tag(self) -> Optional[str]:
+        if self.valueType == UdfType.Enumeration and self.value:
+            return f"{self.name}:{self.value}"
+        elif self.valueType == UdfType.String and self.value:
+            return f"{self.name}:{self.value}"
+        elif self.valueType == UdfType.Boolean and self.value == "true":
+            return self.name
+        return None
+
+
+@dataclass
+class Keyword:
+    key: str
+    name: str
+    isVariantsMarker: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            name=dictionary.get("name", ""),
+            isVariantsMarker=dictionary.get("isVariantsMarker", False),
+        )
+
+
+@dataclass
+class Reference:
+    type: ReferenceType
+    path: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            type=ReferenceType(dictionary.get("type", ReferenceType.Reference)),
+            path=dictionary.get("path", ""),
+        )
+
+
+@dataclass
+class UserReference:
+    key: str
+    name: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(key=dictionary.get("key", ""), name=dictionary.get("name", ""))
+
+
+@dataclass
+class RequirementReference:
+    key: str
+    edited: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(key=dictionary.get("key", ""), edited=dictionary.get("edited", False))
+
+
+@dataclass
+class ConditionSummary:
+    key: str
+    uniqueId: str
+    name: str
+    description: str
+    version: Optional[str] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            uniqueId=dictionary.get("uniqueId", ""),
+            name=dictionary.get("name", ""),
+            description=dictionary.get("description", ""),
+            version=dictionary.get("version", None),
+        )
+
+
+@dataclass
+class TestCaseSetSpecificationSummary:
+    key: str
+    description: str
+    reviewComment: str
+    status: SpecificationStatus
+    priority: Optional[Priority]
+    responsible: Optional[UserReference]
+    dueDate: Optional[str]
+    reviewer: Optional[UserReference]
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    references: List[Reference]
+    requirements: List[RequirementReference]
+    preConditions: List[ConditionSummary]
+    postConditions: List[ConditionSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            description=dictionary.get("description", ""),
+            reviewComment=dictionary.get("reviewComment", ""),
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+            priority=Priority(dictionary.get("priority")) if dictionary.get("priority") else None,
+            responsible=UserReference.from_dict(dictionary.get("responsible", {}))
+            if dictionary.get("responsible")
+            else None,
+            dueDate=dictionary.get("dueDate", None),
+            reviewer=UserReference.from_dict(dictionary.get("reviewer", {}))
+            if dictionary.get("reviewer")
+            else None,
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            references=dictionary.get("references", ""),
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+            preConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("preConditions", [])
+            ],
+            postConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("postConditions", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseSpecificationDetails:
+    key: str
+    comments: str
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    requirements: List[RequirementReference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseSetExecutionSummary:
+    key: str
+    comments: str
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+        )
+
+
+@dataclass
+class TestCaseSpecificationSummary:
+    key: str
+    comments: str
+    requirements: List[RequirementReference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            comments=dictionary.get("comments", ""),
+            requirements=[
+                RequirementReference.from_dict(requirement)
+                for requirement in dictionary.get("requirements", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseExecutionSummary:
+    key: str
+    comments: str = ""
+    status: ActivityStatus = ActivityStatus.Planned
+    execStatus: ExecutionStatus = ExecutionStatus.NotBlocked
+    verdict: ExecutionVerdict = ExecutionVerdict.Undefined
+    defects: Optional[List[int]] = None
+    tester: Optional[UserReference] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+            comments=dictionary.get("comments", ""),
+            defects=dictionary.get("defects", []),
+            tester=UserReference.from_dict(dictionary.get("tester"))
+            if dictionary.get("tester")
+            else None,
+        )
+
+
+@dataclass
+class TestCaseSummary:
+    uniqueID: str
+    index: int
+    spec: TestCaseSpecificationSummary
+    exec: Optional[TestCaseExecutionSummary] = None
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            uniqueID=dictionary.get("uniqueID", ""),
+            index=dictionary.get("index", 0),
+            spec=TestCaseSpecificationSummary.from_dict(dictionary.get("spec", {})),
+            exec=TestCaseExecutionSummary.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+        )
+
+
+@dataclass
+class TestCaseExecutionDetails:
+    key: str
+    status: ActivityStatus
+    execStatus: ExecutionStatus
+    verdict: ExecutionVerdict
+    plannedDuration: int
+    actualDuration: int
+    currentUser: UserReference
+    tester: Optional[UserReference]
+    comments: str  # TODO: Insert htmlComment
+    version: Optional[str]
+    defects: List[int]
+    udfs: List[UserDefinedField]
+    keywords: List[Keyword]
+    references: List[Reference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+            plannedDuration=dictionary.get("plannedDuration", 0),
+            actualDuration=dictionary.get("actualDuration", 0),
+            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
+            tester=UserReference.from_dict(dictionary.get("tester", {}))
+            if dictionary.get("tester")
+            else None,
+            comments=dictionary.get("comments", ""),
+            version=dictionary.get("version", None),
+            defects=dictionary.get("defects", []),
+            udfs=[UserDefinedField.from_dict(udf) for udf in dictionary.get("udfs", [])],
+            keywords=[Keyword.from_dict(keyword) for keyword in dictionary.get("keywords", [])],
+            references=dictionary.get("references", []),
+        )
+
+
+@dataclass
+class TestCaseSetDetails:
+    key: str
+    numbering: str
+    uniqueID: str
+    name: str
+    spec: TestCaseSetSpecificationSummary
+    exec: Optional[TestCaseSetExecutionSummary]
+    testCases: List[TestCaseSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestCaseSetDetails:
+        return cls(
+            key=dictionary.get("key", ""),
+            numbering=dictionary.get("numbering", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            name=dictionary.get("name", ""),
+            spec=TestCaseSetSpecificationSummary.from_dict(dictionary.get("spec", {})),
+            exec=TestCaseSetExecutionSummary.from_dict(dictionary.get("exec", {}))
+            if dictionary.get("exec")
+            else None,
+            testCases=[
+                TestCaseSummary.from_dict(test_case)
+                for test_case in dictionary.get("testCases", [])
+            ],
+        )
+
+
+@dataclass
+class InteractionExecutionSummary:
+    verdict: InteractionVerdict
+    time: str
+    duration: int
+    currentUser: UserReference
+    tester: UserReference
+    comments: str
+    references: List[Reference]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            verdict=InteractionVerdict(dictionary.get("verdict", InteractionVerdict.Undefined)),
+            time=dictionary.get("time", ""),
+            duration=dictionary.get("duration", 0),
+            currentUser=UserReference.from_dict(dictionary.get("currentUser", {})),
+            tester=UserReference.from_dict(dictionary.get("tester", {})),
+            comments=dictionary.get("comments", ""),
+            references=dictionary.get("references", []),
+        )
+
+
+@dataclass
+class InteractionSpecificationSummary:
+    callId: int
+    sequencePhase: SequencePhase
+    callType: CallType
+    description: str
+    comments: str
+    references: List[Reference]
+    preConditions: List[ConditionSummary]
+    postConditions: List[ConditionSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            callId=dictionary.get("callId", ""),
+            sequencePhase=SequencePhase(dictionary.get("sequencePhase", SequencePhase.TestStep)),
+            callType=CallType(dictionary.get("callType", CallType.Flow)),
+            description=dictionary.get("description", ""),
+            comments=dictionary.get("comments", ""),
+            references=dictionary.get("references", ""),
+            preConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("preConditions", [])
+            ],
+            postConditions=[
+                ConditionSummary.from_dict(condition)
+                for condition in dictionary.get("postConditions", [])
+            ],
+        )
+
+
+@dataclass
+class ParameterSummary:
+    name: str
+    value: str
+    version: Optional[str]
+    parameterType: ParameterType
+    parameterUseType: ParameterUseType
+    dataTypeName: str
+    dataTypePath: str
+    dataTypeUniqueID: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            name=dictionary.get("name", ""),
+            value=dictionary.get("value", ""),
+            version=dictionary.get(
+                "version",
+            ),
+            parameterType=ParameterType(
+                dictionary.get("parameterType", ParameterType.AtomicInstance)
+            ),
+            parameterUseType=ParameterUseType(
+                dictionary.get("parameterUseType", ParameterUseType.CallByValue)
+            ),
+            dataTypeName=dictionary.get("dataTypeName", ""),
+            dataTypePath=dictionary.get("dataTypePath", ""),
+            dataTypeUniqueID=dictionary.get("dataTypeUniqueID", ""),
+        )
+
+
+@dataclass
+class InteractionDetails:
+    key: str
+    uniqueID: str
+    name: str
+    version: Optional[str]
+    interactionType: InteractionType
+    path: str
+    spec: InteractionSpecificationSummary
+    exec: Optional[InteractionExecutionSummary]
+    parameters: List[ParameterSummary]
+    interactions: List[InteractionDetails]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            name=dictionary.get("name", ""),
+            version=dictionary.get("version", ""),
+            interactionType=InteractionType(
+                dictionary.get("interactionType", InteractionType.Atomic)
+            ),
+            path=dictionary.get("path", ""),
+            spec=InteractionSpecificationSummary.from_dict(dictionary.get("spec")),
+            exec=InteractionExecutionSummary.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+            parameters=[
+                ParameterSummary.from_dict(param) for param in dictionary.get("parameters", [])
+            ],
+            interactions=[
+                InteractionDetails.from_dict(interaction)
+                for interaction in dictionary.get("interactions", [])
+            ],
+        )
+
+
+@dataclass
+class TestCaseDetails:
+    uniqueID: str
+    spec: TestCaseSpecificationDetails
+    exec: Optional[TestCaseExecutionDetails]
+    interactions: List[InteractionDetails]
+    parameters: List[ParameterSummary]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestCaseDetails:
+        return cls(
+            uniqueID=dictionary.get("uniqueID"),
+            spec=TestCaseSpecificationDetails.from_dict(dictionary.get("spec")),
+            exec=TestCaseExecutionDetails.from_dict(dictionary.get("exec"))
+            if dictionary.get("exec")
+            else None,
+            interactions=[
+                InteractionDetails.from_dict(interaction)
+                for interaction in dictionary.get("interactions", [])
+            ],
+            parameters=[
+                ParameterSummary.from_dict(parameter)
+                for parameter in dictionary.get("parameters", [])
+            ],
+        )
+
+
+@dataclass
+class TestStructureSpecification:
+    key: str
+    locker: Optional[UserReference]
+    status: SpecificationStatus
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+        )
+
+
+@dataclass
+class TestStructureAutomation:
+    key: str
+    locker: Optional[UserReference]
+    status: SpecificationStatus
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=SpecificationStatus(dictionary.get("status", SpecificationStatus.Planned)),
+        )
+
+
+@dataclass
+class TestStructureExecution:
+    key: str
+    locker: Optional[UserReference]
+    status: ActivityStatus
+    execStatus: ExecutionStatus
+    verdict: ExecutionVerdict
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            locker=UserReference.from_dict(dictionary.get("locker", {}))
+            if dictionary.get("locker")
+            else None,
+            status=ActivityStatus(dictionary.get("status", ActivityStatus.Planned)),
+            execStatus=ExecutionStatus(dictionary.get("execStatus", ExecutionStatus.NotBlocked)),
+            verdict=ExecutionVerdict(dictionary.get("verdict", ExecutionVerdict.Undefined)),
+        )
+
+
+@dataclass
+class AttachedFilter:
+    key: str
+    name: str
+    filterType: FilterType
+    content: str
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            name=dictionary.get("name", ""),
+            filterType=FilterType(dictionary.get("filterType", FilterType.TestCaseSetFilter)),
+            content=dictionary.get("content", ""),
+        )
+
+
+@dataclass
+class TestStructureTreeNodeInformation:
+    key: str
+    numbering: str
+    parentKey: str
+    name: str
+    uniqueID: str
+    orderPos: int
+    matchesFilter: bool
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            key=dictionary.get("key", "-1"),
+            numbering=dictionary.get("numbering", "-1"),
+            parentKey=dictionary.get("parentKey", "-1"),
+            name=dictionary.get("name", ""),
+            uniqueID=dictionary.get("uniqueID", ""),
+            orderPos=dictionary.get("orderPos", "-1"),
+            matchesFilter=dictionary.get("matchesFilter", True),
+        )
+
+
+@dataclass
+class TestStructureTreeNode:
+    elementType: TestStructureTreeNodeType
+    baseInformation: TestStructureTreeNodeInformation
+    specification: Optional[TestStructureSpecification]
+    automation: Optional[TestStructureAutomation]
+    execution: Optional[TestStructureExecution]
+    filters: List[AttachedFilter]
+
+    @classmethod
+    def from_dict(cls, dictionary):
+        return cls(
+            elementType=TestStructureTreeNodeType(
+                dictionary.get("elementType", TestStructureTreeNodeType.TestTheme)
+            ),
+            baseInformation=TestStructureTreeNodeInformation.from_dict(
+                dictionary.get("baseInformation", {})
+            ),
+            specification=TestStructureSpecification.from_dict(dictionary.get("specification"))
+            if dictionary.get("specification")
+            else None,
+            automation=TestStructureAutomation.from_dict(dictionary.get("automation"))
+            if dictionary.get("automation")
+            else None,
+            execution=TestStructureExecution.from_dict(dictionary.get("execution"))
+            if dictionary.get("execution")
+            else None,
+            filters=[AttachedFilter.from_dict(filter) for filter in dictionary.get("filters", [])],
+        )
+
+
+@dataclass
+class TestStructureTree:
+    root: TestStructureTreeNode
+    nodes: List[TestStructureTreeNode]
+
+    @classmethod
+    def from_dict(cls, dictionary) -> TestStructureTree:
+        return cls(
+            root=TestStructureTreeNode.from_dict(dictionary.get("root", {}))
+            if "root" in dictionary
+            else None,
+            nodes=[TestStructureTreeNode.from_dict(node) for node in dictionary.get("nodes", [])],
+        )
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/result_writer.py` & `testbench2robotframework-0.6.1/testbench2robotframework/result_writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,673 +1,673 @@
-import html
-import os
-import re
-import shutil
-import tempfile
-import uuid
-from datetime import datetime, timedelta
-from pathlib import Path
-from shutil import copytree
-from typing import Dict, List, Optional, Union
-from urllib.parse import unquote
-
-from robot.result import Keyword, ResultVisitor, TestCase, TestSuite
-from robot.result.model import Body
-
-from .config import AttachmentConflictBehaviour, Configuration, ReferenceBehaviour
-from .json_reader import TestBenchJsonReader
-from .json_writer import write_test_structure_element
-from .log import logger
-from .model import (
-    ActivityStatus,
-    ExecutionVerdict,
-    InteractionDetails,
-    InteractionExecutionSummary,
-    InteractionType,
-    InteractionVerdict,
-    Reference,
-    ReferenceType,
-    SequencePhase,
-    TestCaseDetails,
-    TestCaseExecutionDetails,
-)
-from .utils import directory_to_zip, ensure_dir_exists, get_directory
-
-BACKGROUND_COLOR = {
-    "PASS": "#04AF91",
-    "FAIL": "#ce3e01",
-    "ERROR": "#ce3e01",
-    "SKIP": "#F3E96A",
-    "WARN": "#D48627",
-    "INFO": "#ddd",
-}
-COLOR = {
-    "PASS": "#fff",
-    "FAIL": "#fff",
-    "ERROR": "#fff",
-    "SKIP": "#000",
-    "WARN": "#fff",
-    "INFO": "#000",
-}
-
-MEGABYTE = 1000 * 1000
-
-
-class ResultWriter(ResultVisitor):
-    def __init__(
-        self, json_report: str, json_result: str, config: Configuration, output_xml
-    ) -> None:
-        self.json_dir = get_directory(json_report)
-        self.output_xml = output_xml
-        self.reference_behaviour = config.referenceBehaviour
-        self.attachment_conflict_behaviour = config.attachmentConflictBehaviour
-        self.tempdir = tempfile.TemporaryDirectory(dir=os.curdir)
-        self._test_setup_passed: Optional[bool] = None
-        if json_result is None:
-            self.create_zip = bool(Path(json_report).suffix == ".zip")
-            self.json_result = self.json_dir
-            self.json_result_path = self.json_dir
-        else:
-            self.json_result_path = str(Path(json_result).parent / Path(json_report).stem)
-            self.create_zip = bool(Path(json_report).suffix == ".zip")
-            self.json_result = self.tempdir.name
-            if self.create_zip:
-                copytree(self.json_dir, self.json_result, dirs_exist_ok=True)
-        self.json_reader = TestBenchJsonReader(self.json_dir)
-        self.attachments_path = Path(self.json_result, "attachments")
-        # if self.attachments_path.exists():  TODO: RR Sollten wir löschen????
-        #     shutil.rmtree(self.attachments_path)
-        # os.mkdir(self.attachments_path)
-        self.test_suites: Dict[str, TestSuite] = {}
-        self.keywords: List[Keyword] = []
-        self.itb_test_case_catalog: Dict[str, TestCaseDetails] = {}
-        self.phase_pattern = config.phasePattern
-        self.test_chain: List[TestCase] = []
-
-    def start_suite(self, suite: TestSuite):
-        if suite.metadata:
-            self.test_suites[suite.metadata["uniqueID"]] = suite
-
-    def _get_interactions_by_type(
-        self, interactions: List[InteractionDetails], interaction_type: InteractionType
-    ):
-        for interaction in interactions:
-            if interaction.interactionType == interaction_type:
-                yield interaction
-            if interaction.interactionType == InteractionType.Compound:
-                yield from self._get_interactions_by_type(
-                    interaction.interactions, interaction_type
-                )
-
-    def end_test(self, test: TestCase):
-        self._test_setup_passed = None
-        test_chain = get_test_chain(test.name, self.phase_pattern)
-        if test_chain:
-            if test_chain.index == 1:
-                self.test_chain = [test]
-            else:
-                self.test_chain.append(test)
-            if test_chain.index != test_chain.length:
-                return
-        else:
-            self.test_chain = [test]
-
-        test_uid = test_chain.name if test_chain else test.name
-        itb_test_case = self.json_reader.read_test_case(test_uid)  # TODO What if name != UID
-        if itb_test_case.exec is None:
-            itb_test_case.exec = TestCaseExecutionDetails.from_dict({})
-        if itb_test_case.exec.key in ["", "-1"]:
-            logger.warning(
-                f"Test case {itb_test_case.uniqueID} was not exported based on "
-                f"execution and is therefore not importable."
-            )
-        try:
-            atomic_interactions = list(
-                self._get_interactions_by_type(itb_test_case.interactions, InteractionType.Atomic)
-            )
-            compound_interactions = list(
-                self._get_interactions_by_type(itb_test_case.interactions, InteractionType.Compound)
-            )
-            self._set_atomic_interactions_execution_result(atomic_interactions, self.test_chain)
-            for interaction in compound_interactions:
-                self._set_compound_interaction_execution_result(interaction)
-            self._set_itb_testcase_execution_result(itb_test_case, self.test_chain)
-            self._set_itb_testcase_execution_comment(itb_test_case, self.test_chain)
-            if self.reference_behaviour != ReferenceBehaviour.NONE:
-                self._set_itb_testcase_references(itb_test_case, self.test_chain)
-        except TypeError:
-            logger.error(
-                "Could not find an itb testcase that corresponds "
-                "to the given Robot Framework testcase."
-            )
-        self.itb_test_case_catalog[test_uid] = itb_test_case
-        write_test_structure_element(self.json_result, itb_test_case)
-        logger.debug(
-            f"Successfully wrote the result from test "
-            f"{itb_test_case.uniqueID} to TestBench's Json Report."
-        )
-
-    def _set_itb_testcase_references(
-        self, itb_test_case: TestCaseDetails, test_chain: List[TestCase]
-    ):
-        for test in test_chain:
-            itb_references = self._get_itb_reference(test.message)
-            for reference in itb_references:
-                if reference not in itb_test_case.exec.references:
-                    itb_test_case.exec.references.append(reference)
-
-    def _get_itb_reference(self, test_message: str) -> List[Reference]:
-        references = []
-        for path in re.findall(r"itb-reference:\s*(\S*)", test_message):
-            if path.startswith("file:///"):
-                file_path = Path(unquote(path[len("file:///") :]))
-                output_dir = Path(self.output_xml).parent
-                if file_path.exists():
-                    reference_path = file_path
-                elif Path(output_dir, file_path).exists():
-                    reference_path = Path(output_dir, file_path)
-                else:
-                    if (
-                        file_path.is_absolute()
-                        and self.reference_behaviour == ReferenceBehaviour.REFERENCE
-                    ):
-                        references.append(self._create_reference(file_path))
-                    else:
-                        logger.warning(f"Referenced file '{file_path}' does not exist.")
-                    continue
-                file_size = os.path.getsize(reference_path)
-                if file_size >= 10 * MEGABYTE:
-                    logger.error(
-                        f"Trying to attach file '{reference_path}'. "
-                        "Attachment file size must not exceed 10 MB "
-                        f"but is {file_size / MEGABYTE} MB."
-                    )
-                    reference = self._create_reference(reference_path.name)
-                else:
-                    reference = self._create_attachment(reference_path)
-                if reference:
-                    references.append(reference)
-            elif re.match(r"\S+://", path):
-                references.append(Reference(ReferenceType.Hyperlink, path))
-            else:
-                logger.warning(f"Could not identify type of test message reference '{path}'.")
-        return references
-
-    @staticmethod
-    def _create_reference(reference_path: Union[Path, str]) -> Reference:
-        return Reference(ReferenceType.Reference, str(reference_path))
-
-    def _create_attachment(self, filepath: Path) -> Optional[Reference]:
-        if self.reference_behaviour == ReferenceBehaviour.REFERENCE:
-            return self._create_reference(filepath.resolve())
-        ensure_dir_exists(self.attachments_path)
-        filename = Path(filepath).name
-        if (
-            not Path(self.attachments_path, filename).exists()
-            or self.attachment_conflict_behaviour == AttachmentConflictBehaviour.USE_NEW
-        ):
-            shutil.copyfile(filepath, self.attachments_path / filename, follow_symlinks=True)
-            return Reference(ReferenceType.Attachment, f"attachments/{filename}")
-        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.USE_EXISTING:
-            return Reference(ReferenceType.Attachment, f"attachments/{filename}")
-        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.RENAME_NEW:
-            unique_path = self._create_unique_path(self.attachments_path / filename)
-            shutil.copyfile(filepath, unique_path, follow_symlinks=True)
-            unique_file = Path(unique_path).name
-            logger.info(
-                f"Attachment '{filename}' does already exist. "
-                f"Creating new unique attachment '{unique_file}'."
-            )
-            return Reference(ReferenceType.Attachment, f"attachments/{unique_file}")
-        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.ERROR:
-            logger.error(f"Attachment '{filename}' does already exist.")
-            return None
-        return None
-
-    @staticmethod
-    def _create_unique_path(attachement_path: Path) -> Path:
-        counter = 1
-        attachment_stem = attachement_path.stem
-        while attachement_path.exists():
-            attachement_path = Path(
-                f"{attachement_path.parent}",
-                f"{attachment_stem}_{counter}{attachement_path.suffix}",
-            )
-            counter += 1
-        return attachement_path
-
-    def _set_itb_testcase_execution_comment(self, itb_test_case, test_chain: List[TestCase]):
-        exec_comments = []
-        for test in test_chain:
-            message = re.sub(r"\s*itb-reference:\s*(\S*)", "", test.message)
-            html_message = (
-                message[len("*HTML*") :].replace("<hr>", "<br/>").replace("<br>", "<br/>").strip()
-                if test.message.startswith("*HTML*")
-                else html.escape(message)
-            )
-            test_chain_obj = get_test_chain(test.name, self.phase_pattern)
-            test_phase_name = (
-                f"<b>Phase {test_chain_obj.index}/{test_chain_obj.length} : "
-                f"<span {self.render_status(test.status)}>{test.status}</span></b>"
-                if test_chain_obj
-                else f"<b><span {self.render_status(test.status)}>{test.status}</span></b>"
-            )
-            exec_comment = (
-                f"{test_phase_name}"
-                "<pre>"
-                f"Start Time:   {self.get_isotime_from_robot_timestamp(test.starttime)}\n"
-                f"End Time:     {self.get_isotime_from_robot_timestamp(test.endtime)}\n"
-                f"Elapsed Time: {timedelta(milliseconds=test.elapsedtime)!s}\n"
-                "</pre>"
-                f"Message: <p><pre>{html_message}</pre></p>\n"
-            )
-            exec_comments.append(exec_comment)
-        itb_test_case.exec.comments = f"<html><body>{''.join(exec_comments)}</body></html>"
-
-    def _set_itb_testcase_execution_result(self, itb_test_case, test_chain):
-        has_failed_chain = list(filter(lambda tc: tc.status.upper() == "FAIL", test_chain))
-        passed_keywords = all(tc.status.upper() == "PASS" for tc in test_chain)
-        itb_test_case.exec.actualDuration = sum([tc.elapsedtime for tc in test_chain])
-        if has_failed_chain:
-            self._set_itb_test_case_status(itb_test_case, "fail")
-        elif passed_keywords:
-            self._set_itb_test_case_status(itb_test_case, "pass")
-        else:
-            self._set_itb_test_case_status(itb_test_case, "undef")
-
-    def _get_test_phase_body(self, test_phase: TestCase) -> Body:
-        return test_phase.body
-
-    def _get_test_phase_setup(self, test_phase: TestCase) -> List[Keyword]:
-        test_phase_setup = []
-        if test_phase.has_setup and test_phase.setup:
-            self._test_setup_passed = test_phase.setup.passed
-            if test_phase.setup.name == f"Setup-{test_phase.name}":
-                test_phase_setup = list(
-                    filter(
-                        lambda kw: isinstance(kw, Keyword)
-                        and kw.parent.name == f"Setup-{test_phase.name}",
-                        test_phase.setup.body,
-                    )
-                )
-            else:
-                test_phase_setup = [test_phase.setup]
-        return test_phase_setup
-
-    def _get_test_phase_teardown(self, test_phase: TestCase) -> List[Keyword]:
-        test_phase_teardown = []
-        if test_phase.has_teardown and test_phase.teardown:
-            if test_phase.teardown.name == f"Teardown-{test_phase.name}":
-                test_phase_teardown = list(
-                    filter(
-                        lambda kw: isinstance(kw, Keyword)
-                        and kw.parent.name == f"Teardown-{test_phase.name}",
-                        test_phase.teardown.body,
-                    )
-                )
-            else:
-                test_phase_teardown = [test_phase.teardown]
-        return test_phase_teardown
-
-    def _set_atomic_interactions_execution_result(
-        self, atomic_interactions: List[InteractionDetails], test_chain: List[TestCase]
-    ):
-        self._test_setup_passed = True
-        test_chain_setup = [
-            keyword
-            for test_phase in test_chain
-            for keyword in self._get_test_phase_setup(test_phase)
-        ]
-        test_chain_body = [
-            keyword
-            for test_phase in test_chain
-            for keyword in self._get_test_phase_body(test_phase)
-        ]
-        test_chain_teardown = [
-            keyword
-            for test_phase in test_chain
-            for keyword in self._get_test_phase_teardown(test_phase)
-        ]
-        setup_interactions = self._filter_atomic_interactions_by_sequence_phase(
-            atomic_interactions, SequencePhase.Setup
-        )
-        test_step_interactions = self._filter_atomic_interactions_by_sequence_phase(
-            atomic_interactions, SequencePhase.TestStep
-        )
-        teardown_interactions = self._filter_atomic_interactions_by_sequence_phase(
-            atomic_interactions, SequencePhase.Teardown
-        )
-        self._set_interaction_verdicts(setup_interactions, test_chain_setup, SequencePhase.Setup)
-        self._set_interaction_verdicts(
-            test_step_interactions, test_chain_body, SequencePhase.TestStep
-        )
-        self._set_interaction_verdicts(
-            teardown_interactions, test_chain_teardown, SequencePhase.Teardown
-        )
-
-    def _set_interaction_verdicts(
-        self,
-        interaction_list: List[InteractionDetails],
-        test_chain_body: List[Keyword],
-        sequence_phase: SequencePhase,
-    ):
-        for index, interaction in enumerate(interaction_list):
-            if interaction.exec is None:
-                interaction.exec = InteractionExecutionSummary.from_dict({})
-            if sequence_phase == SequencePhase.TestStep and not self._test_setup_passed:
-                interaction.exec.verdict = InteractionVerdict.Skipped
-                continue
-            if index < len(test_chain_body):
-                keyword = test_chain_body[index]
-                self._check_matching_interaction_and_keyword_name(keyword, interaction)
-                interaction.exec = self._get_interaction_exec_from_keyword(keyword)
-                continue
-            if sequence_phase == SequencePhase.Setup and not self._test_setup_passed:
-                interaction.exec.verdict = InteractionVerdict.Skipped
-                continue
-            interaction.exec.verdict = InteractionVerdict.Undefined
-
-    def _filter_atomic_interactions_by_sequence_phase(
-        self, atomic_interactions: List[InteractionDetails], sequence_phase: SequencePhase
-    ):
-        return list(
-            filter(
-                lambda atomic_interaction: atomic_interaction.spec.sequencePhase == sequence_phase,
-                atomic_interactions,
-            )
-        )
-
-    def _get_interaction_exec_from_keyword(self, keyword: Keyword) -> InteractionExecutionSummary:
-        return InteractionExecutionSummary.from_dict(
-            {
-                'verdict': self._get_interaction_result(keyword.status),
-                'time': keyword.endtime,
-                'duration': keyword.elapsedtime,
-                'comments': self.get_html_keyword_comment(keyword),
-            }
-        )
-
-    def _check_matching_interaction_and_keyword_name(
-        self, keyword: Keyword, interaction: InteractionDetails
-    ) -> None:
-        if not is_normalized_equal(keyword.kwname, interaction.name) and not is_normalized_equal(
-            keyword.kwname.split('.')[-1], interaction.name
-        ):
-            raise NameError(
-                f"Execution can not be parsed, "
-                f"because keyword name '{keyword.kwname}' does not match with "
-                f"interaction '{interaction.name}' name."
-            )
-
-    def _get_keyword_messages(self, keyword: Keyword):
-        if hasattr(keyword, "messages"):
-            for message in keyword.messages:
-                yield self._create_itb_exec_comment(message)
-        if hasattr(keyword, "body"):
-            for kw in keyword.body:
-                yield from self._get_keyword_messages(kw)
-
-    def get_html_keyword_comment(self, keyword: Keyword):
-        messages = list(self._get_keyword_messages(keyword))
-        return (
-            "<html>"
-            "<body>"
-            "<style>"
-            "td {padding: 5px; border: none;} "
-            "table {font-family: monospace; border: none;}"
-            "</style>"
-            "<pre>"
-            f"Start Time:   {self.get_isotime_from_robot_timestamp(keyword.starttime)}\n"
-            f"End Time:     {self.get_isotime_from_robot_timestamp(keyword.endtime)}\n"
-            f"Elapsed Time: {timedelta(milliseconds=keyword.elapsedtime)!s}\n"
-            "</pre>"
-            "<table>"
-            "<tr>"
-            f"{'</tr><tr>'.join(messages)}"
-            "</tr>"
-            "</table>"
-            "</body>"
-            "</html>"
-        )
-
-    def _create_itb_exec_comment(
-        self,
-        message,
-    ) -> str:  # Todo: low prio: pattern für message in config festlegen
-        message_time = self.get_isotime_from_robot_timestamp(
-            message.timestamp, time_format="%H:%M:%S.%f"
-        )
-        msg = message.html_message.replace("<hr>", "<br/>").replace("<br>", "<br/>").strip()
-        return (
-            f"<td {self.render_status(message.level)}><b>{message.level}</b></td>"
-            f"<td><pre>{msg}</pre></td><td>{message_time}</td>"
-        )
-
-    @staticmethod
-    def get_isotime_from_robot_timestamp(timestamp, time_format="%Y-%m-%d %H:%M:%S.%f"):
-        return (
-            datetime.strptime(timestamp, "%Y%m%d %H:%M:%S.%f")
-            .astimezone()
-            .strftime(time_format)[:-3]
-        )
-
-    def _set_compound_interaction_execution_result(self, compound_interaction: InteractionDetails):
-        atomic_interactions = list(
-            self._get_interactions_by_type(
-                compound_interaction.interactions, InteractionType.Atomic
-            )
-        )
-        if compound_interaction.exec is None:
-            compound_interaction.exec = InteractionExecutionSummary.from_dict({})
-        compound_interaction.exec.verdict = InteractionVerdict.Skipped
-        for atomic in atomic_interactions:
-            if atomic.exec is None:
-                logger.debug(
-                    f"Atomic interaction {atomic.uniqueID} "
-                    f"had no exec details and therefore ignored."
-                )
-                atomic.exec = InteractionExecutionSummary.from_dict({})
-            if atomic.exec.verdict is InteractionVerdict.Fail:
-                compound_interaction.exec.verdict = InteractionVerdict.Fail
-                break
-            if atomic.exec.verdict is InteractionVerdict.Pass:
-                compound_interaction.exec.verdict = InteractionVerdict.Pass
-
-        compound_interaction.exec.duration = sum(
-            [interaction.exec.duration for interaction in atomic_interactions]
-        )
-        compound_interaction.exec.time = atomic_interactions[-1].exec.time
-
-    @staticmethod
-    def _set_itb_test_case_status(itb_test_case: TestCaseDetails, robot_status: str):
-        robot_status = robot_status.lower()
-        if robot_status == "pass":
-            itb_test_case.exec.status = ActivityStatus.Performed
-            itb_test_case.exec.verdict = ExecutionVerdict.Pass
-        elif robot_status == "fail":
-            itb_test_case.exec.status = ActivityStatus.Performed
-            itb_test_case.exec.verdict = ExecutionVerdict.Fail
-        else:
-            itb_test_case.exec.status = ActivityStatus.Running
-            itb_test_case.exec.verdict = ExecutionVerdict.Undefined
-
-    def end_suite(self, suite: TestSuite):
-        if not suite.metadata.get("uniqueID") or len(suite.suites):
-            return
-        test_case_set = self.json_reader.read_test_case_set(suite.metadata["uniqueID"])
-        if not test_case_set:
-            return
-        test_case_set.exec.verdict = suite.status
-
-        for testcase in test_case_set.testCases:
-            current_itb_test_case = self.itb_test_case_catalog.get(testcase.uniqueID)
-            if current_itb_test_case is None:
-                continue
-            testcase.exec.verdict = current_itb_test_case.exec.verdict
-            testcase.exec.status = current_itb_test_case.exec.status
-            testcase.exec.execStatus = current_itb_test_case.exec.execStatus
-            testcase.exec.comments = current_itb_test_case.exec.comments
-        suite_start_time = "99999999 00:00:00.000"
-        suite_end_time = "00000000 00:00:00.000"
-        table_content = []
-        for test in suite.tests:
-            suite_start_time = min(suite_start_time, test.starttime)
-            suite_end_time = max(suite_end_time, test.endtime)
-            test_chain = get_test_chain(test.name, self.phase_pattern)
-
-            if test_chain:
-                name = test_chain.name if test_chain.index == 1 else ""
-                phase = f"Phase {test_chain.index}/{test_chain.length}"
-            else:
-                name = test.name
-                phase = ""
-            if test.status != "PASS":
-                message = re.sub(r"\s*itb-reference:\s*(\S*)", "", test.message)
-                message = (
-                    message[len("*HTML*") :]
-                    .replace('<hr>', '<br />')
-                    .replace('<br>', '<br />')
-                    .strip()
-                    if message.startswith("*HTML*")
-                    else message
-                )
-            else:
-                message = self.get_isotime_from_robot_timestamp(test.endtime)
-
-            table_content.append(
-                f"<td>{name}</td>"
-                f"<td>{phase}</td>"
-                f"<td {self.render_status(test.status)}><b>{test.status}</b></td>"
-                f"<td><pre>{message}</pre></td>"
-            )
-
-        test_case_set.exec.comments = (
-            "<html>"
-            "<head>"
-            "<style>"
-            "td {padding: 5px; border: none; white-space: pre-wrap;} "
-            "table {font-family: monospace; border: none;}"
-            "</style>"
-            "</head>"
-            "<body>"
-            "<pre>"
-            f"Start Time:   {self.get_isotime_from_robot_timestamp(suite_start_time)}\n"
-            f"End Time:     {self.get_isotime_from_robot_timestamp(suite_end_time)}\n"
-            "</pre>"
-            "<table>"
-            "<tr>"
-            f"{'</tr><tr>'.join(table_content)}"
-            "</tr>"
-            "</table>"
-            "</body>"
-            "</html>"
-        )
-        write_test_structure_element(self.json_result, test_case_set)
-        logger.debug(
-            f"Successfully wrote the result from suite "
-            f"{test_case_set.uniqueID} to TestBench's Json Report."
-        )
-
-    @staticmethod
-    def render_status(status):
-        return (
-            "style='"
-            f"background-color: {BACKGROUND_COLOR.get(status, '#fff')}; "
-            f"color: {COLOR.get(status, '#000')};'"
-        )
-
-    def end_result(self, result):
-        tt_tree = self.json_reader.read_test_theme_tree()
-        if tt_tree:
-            test_suite_counter = 0
-            for tse in tt_tree.nodes:
-                if self.test_suites.get(tse.baseInformation.uniqueID) is None:
-                    continue
-                execution_result = self._get_execution_result(
-                    self.test_suites[tse.baseInformation.uniqueID].status
-                )
-                tse.execution.verdict = execution_result["execution_verdict"]
-                tse.execution.status = execution_result["activity_status"]
-                test_suite_counter += 1
-            write_test_structure_element(self.json_result, tt_tree)
-            if test_suite_counter and self.itb_test_case_catalog:
-                logger.info(f"Successfully read {test_suite_counter} test suites.")
-            else:
-                logger.warning("No test suites with execution information found.")
-            if self.create_zip:
-                directory_to_zip(self.json_result, self.json_result_path)
-            elif self.json_result != self.json_result_path:
-                copytree(self.json_dir, self.json_result_path, dirs_exist_ok=True)
-                copytree(self.json_result, self.json_result_path, dirs_exist_ok=True)
-            self.tempdir.cleanup()
-        logger.info("Successfully wrote the robot execution results to TestBench's Json Report.")
-
-    @staticmethod
-    def _get_execution_result(robot_status: str) -> Dict:
-        robot_status = robot_status.lower()
-        if robot_status == "pass":
-            return {
-                "execution_verdict": ExecutionVerdict.Pass,
-                "activity_status": ActivityStatus.Performed,
-            }
-        if robot_status == "fail":
-            return {
-                "execution_verdict": ExecutionVerdict.Fail,
-                "activity_status": ActivityStatus.Performed,
-            }
-        return {
-            "execution_verdict": ExecutionVerdict.Undefined,
-            "activity_status": ActivityStatus.Skipped,
-        }
-
-    @staticmethod
-    def _get_interaction_result(robot_status: str) -> InteractionVerdict:
-        robot_status = robot_status.upper()
-        if robot_status == "PASS":
-            return InteractionVerdict.Pass
-        if robot_status == "FAIL":
-            return InteractionVerdict.Fail
-        if robot_status == "NOT RUN":
-            return InteractionVerdict.Skipped
-        return InteractionVerdict.Skipped
-
-
-class TestChain:
-    def __init__(self, name, index, length):
-        self.name = str(name)
-        self.index = int(index)
-        self.length = int(length)
-
-
-def get_test_chain(test_name: str, phase_pattern: str) -> Optional[TestChain]:
-    matcher = re.match(get_test_chain_pattern(phase_pattern), test_name)
-    if matcher:
-        return TestChain(*matcher.groups())
-    return None
-
-
-def get_test_chain_pattern(phase_pattern: str) -> str:
-    testcase_placeholder = str(uuid.uuid4().int)
-    index_placeholder = str(uuid.uuid4().int)
-    length_placeholder = str(uuid.uuid4().int)
-    raw_pattern = re.escape(
-        phase_pattern.format(
-            testcase=testcase_placeholder,
-            index=index_placeholder,
-            length=length_placeholder,
-        )
-    )
-    return (
-        raw_pattern.replace(testcase_placeholder, r"(.+?)")
-        .replace(index_placeholder, r"(\d)")
-        .replace(length_placeholder, r"(\d)")
-    )
-
-
-def get_normalized_keyword_name(keyword_name: str) -> str:
-    return re.sub(r"[\s_]", "", keyword_name.lower())
-
-
-def is_normalized_equal(kw_one: str, kw_two: str) -> bool:
-    norm_kw_one = get_normalized_keyword_name(kw_one)
-    norm_kw_two = get_normalized_keyword_name(kw_two)
-    return norm_kw_one == norm_kw_two
+import html
+import os
+import re
+import shutil
+import tempfile
+import uuid
+from datetime import datetime, timedelta
+from pathlib import Path
+from shutil import copytree
+from typing import Dict, List, Optional, Union
+from urllib.parse import unquote
+
+from robot.result import Keyword, ResultVisitor, TestCase, TestSuite
+from robot.result.model import Body
+
+from .config import AttachmentConflictBehaviour, Configuration, ReferenceBehaviour
+from .json_reader import TestBenchJsonReader
+from .json_writer import write_test_structure_element
+from .log import logger
+from .model import (
+    ActivityStatus,
+    ExecutionVerdict,
+    InteractionDetails,
+    InteractionExecutionSummary,
+    InteractionType,
+    InteractionVerdict,
+    Reference,
+    ReferenceType,
+    SequencePhase,
+    TestCaseDetails,
+    TestCaseExecutionDetails,
+)
+from .utils import directory_to_zip, ensure_dir_exists, get_directory
+
+BACKGROUND_COLOR = {
+    "PASS": "#04AF91",
+    "FAIL": "#ce3e01",
+    "ERROR": "#ce3e01",
+    "SKIP": "#F3E96A",
+    "WARN": "#D48627",
+    "INFO": "#ddd",
+}
+COLOR = {
+    "PASS": "#fff",
+    "FAIL": "#fff",
+    "ERROR": "#fff",
+    "SKIP": "#000",
+    "WARN": "#fff",
+    "INFO": "#000",
+}
+
+MEGABYTE = 1000 * 1000
+
+
+class ResultWriter(ResultVisitor):
+    def __init__(
+        self, json_report: str, json_result: Optional[str], config: Configuration, output_xml
+    ) -> None:
+        self.json_dir = get_directory(json_report)
+        self.output_xml = output_xml
+        self.reference_behaviour = config.referenceBehaviour
+        self.attachment_conflict_behaviour = config.attachmentConflictBehaviour
+        self.tempdir = tempfile.TemporaryDirectory(dir=os.curdir)
+        self._test_setup_passed: Optional[bool] = None
+        if json_result is None:
+            self.create_zip = bool(Path(json_report).suffix == ".zip")
+            self.json_result = self.json_dir
+            self.json_result_path = self.json_dir
+        else:
+            self.json_result_path = str(Path(json_result).parent / Path(json_report).stem)
+            self.create_zip = bool(Path(json_report).suffix == ".zip")
+            self.json_result = self.tempdir.name
+            if self.create_zip:
+                copytree(self.json_dir, self.json_result, dirs_exist_ok=True)
+        self.json_reader = TestBenchJsonReader(self.json_dir)
+        self.attachments_path = Path(self.json_result, "attachments")
+        # if self.attachments_path.exists():  TODO: RR Sollten wir löschen????
+        #     shutil.rmtree(self.attachments_path)
+        # os.mkdir(self.attachments_path)
+        self.test_suites: Dict[str, TestSuite] = {}
+        self.keywords: List[Keyword] = []
+        self.itb_test_case_catalog: Dict[str, TestCaseDetails] = {}
+        self.phase_pattern = config.phasePattern
+        self.test_chain: List[TestCase] = []
+
+    def start_suite(self, suite: TestSuite):
+        if suite.metadata:
+            self.test_suites[suite.metadata["uniqueID"]] = suite
+
+    def _get_interactions_by_type(
+        self, interactions: List[InteractionDetails], interaction_type: InteractionType
+    ):
+        for interaction in interactions:
+            if interaction.interactionType == interaction_type:
+                yield interaction
+            if interaction.interactionType == InteractionType.Compound:
+                yield from self._get_interactions_by_type(
+                    interaction.interactions, interaction_type
+                )
+
+    def end_test(self, test: TestCase):
+        self._test_setup_passed = None
+        test_chain = get_test_chain(test.name, self.phase_pattern)
+        if test_chain:
+            if test_chain.index == 1:
+                self.test_chain = [test]
+            else:
+                self.test_chain.append(test)
+            if test_chain.index != test_chain.length:
+                return
+        else:
+            self.test_chain = [test]
+
+        test_uid = test_chain.name if test_chain else test.name
+        itb_test_case = self.json_reader.read_test_case(test_uid)  # TODO What if name != UID
+        if itb_test_case.exec is None:
+            itb_test_case.exec = TestCaseExecutionDetails.from_dict({})
+        if itb_test_case.exec.key in ["", "-1"]:
+            logger.warning(
+                f"Test case {itb_test_case.uniqueID} was not exported based on "
+                f"execution and is therefore not importable."
+            )
+        try:
+            atomic_interactions = list(
+                self._get_interactions_by_type(itb_test_case.interactions, InteractionType.Atomic)
+            )
+            compound_interactions = list(
+                self._get_interactions_by_type(itb_test_case.interactions, InteractionType.Compound)
+            )
+            self._set_atomic_interactions_execution_result(atomic_interactions, self.test_chain)
+            for interaction in compound_interactions:
+                self._set_compound_interaction_execution_result(interaction)
+            self._set_itb_testcase_execution_result(itb_test_case, self.test_chain)
+            self._set_itb_testcase_execution_comment(itb_test_case, self.test_chain)
+            if self.reference_behaviour != ReferenceBehaviour.NONE:
+                self._set_itb_testcase_references(itb_test_case, self.test_chain)
+        except TypeError:
+            logger.error(
+                "Could not find an itb testcase that corresponds "
+                "to the given Robot Framework testcase."
+            )
+        self.itb_test_case_catalog[test_uid] = itb_test_case
+        write_test_structure_element(self.json_result, itb_test_case)
+        logger.debug(
+            f"Successfully wrote the result from test "
+            f"{itb_test_case.uniqueID} to TestBench's Json Report."
+        )
+
+    def _set_itb_testcase_references(
+        self, itb_test_case: TestCaseDetails, test_chain: List[TestCase]
+    ):
+        for test in test_chain:
+            itb_references = self._get_itb_reference(test.message)
+            for reference in itb_references:
+                if reference not in itb_test_case.exec.references:
+                    itb_test_case.exec.references.append(reference)
+
+    def _get_itb_reference(self, test_message: str) -> List[Reference]:
+        references = []
+        for path in re.findall(r"itb-reference:\s*(\S*)", test_message):
+            if path.startswith("file:///"):
+                file_path = Path(unquote(path[len("file:///") :]))
+                output_dir = Path(self.output_xml).parent
+                if file_path.exists():
+                    reference_path = file_path
+                elif Path(output_dir, file_path).exists():
+                    reference_path = Path(output_dir, file_path)
+                else:
+                    if (
+                        file_path.is_absolute()
+                        and self.reference_behaviour == ReferenceBehaviour.REFERENCE
+                    ):
+                        references.append(self._create_reference(file_path))
+                    else:
+                        logger.warning(f"Referenced file '{file_path}' does not exist.")
+                    continue
+                file_size = os.path.getsize(reference_path)
+                if file_size >= 10 * MEGABYTE:
+                    logger.error(
+                        f"Trying to attach file '{reference_path}'. "
+                        "Attachment file size must not exceed 10 MB "
+                        f"but is {file_size / MEGABYTE} MB."
+                    )
+                    reference = self._create_reference(reference_path.name)
+                else:
+                    reference = self._create_attachment(reference_path)
+                if reference:
+                    references.append(reference)
+            elif re.match(r"\S+://", path):
+                references.append(Reference(ReferenceType.Hyperlink, path))
+            else:
+                logger.warning(f"Could not identify type of test message reference '{path}'.")
+        return references
+
+    @staticmethod
+    def _create_reference(reference_path: Union[Path, str]) -> Reference:
+        return Reference(ReferenceType.Reference, str(reference_path))
+
+    def _create_attachment(self, filepath: Path) -> Optional[Reference]:
+        if self.reference_behaviour == ReferenceBehaviour.REFERENCE:
+            return self._create_reference(filepath.resolve())
+        ensure_dir_exists(self.attachments_path)
+        filename = Path(filepath).name
+        if (
+            not Path(self.attachments_path, filename).exists()
+            or self.attachment_conflict_behaviour == AttachmentConflictBehaviour.USE_NEW
+        ):
+            shutil.copyfile(filepath, self.attachments_path / filename, follow_symlinks=True)
+            return Reference(ReferenceType.Attachment, f"attachments/{filename}")
+        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.USE_EXISTING:
+            return Reference(ReferenceType.Attachment, f"attachments/{filename}")
+        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.RENAME_NEW:
+            unique_path = self._create_unique_path(self.attachments_path / filename)
+            shutil.copyfile(filepath, unique_path, follow_symlinks=True)
+            unique_file = Path(unique_path).name
+            logger.info(
+                f"Attachment '{filename}' does already exist. "
+                f"Creating new unique attachment '{unique_file}'."
+            )
+            return Reference(ReferenceType.Attachment, f"attachments/{unique_file}")
+        if self.attachment_conflict_behaviour == AttachmentConflictBehaviour.ERROR:
+            logger.error(f"Attachment '{filename}' does already exist.")
+            return None
+        return None
+
+    @staticmethod
+    def _create_unique_path(attachement_path: Path) -> Path:
+        counter = 1
+        attachment_stem = attachement_path.stem
+        while attachement_path.exists():
+            attachement_path = Path(
+                f"{attachement_path.parent}",
+                f"{attachment_stem}_{counter}{attachement_path.suffix}",
+            )
+            counter += 1
+        return attachement_path
+
+    def _set_itb_testcase_execution_comment(self, itb_test_case, test_chain: List[TestCase]):
+        exec_comments = []
+        for test in test_chain:
+            message = re.sub(r"\s*itb-reference:\s*(\S*)", "", test.message)
+            html_message = (
+                message[len("*HTML*") :].replace("<hr>", "<br/>").replace("<br>", "<br/>").strip()
+                if test.message.startswith("*HTML*")
+                else html.escape(message)
+            )
+            test_chain_obj = get_test_chain(test.name, self.phase_pattern)
+            test_phase_name = (
+                f"<b>Phase {test_chain_obj.index}/{test_chain_obj.length} : "
+                f"<span {self.render_status(test.status)}>{test.status}</span></b>"
+                if test_chain_obj
+                else f"<b><span {self.render_status(test.status)}>{test.status}</span></b>"
+            )
+            exec_comment = (
+                f"{test_phase_name}"
+                "<pre>"
+                f"Start Time:   {self.get_isotime_from_robot_timestamp(test.starttime)}\n"
+                f"End Time:     {self.get_isotime_from_robot_timestamp(test.endtime)}\n"
+                f"Elapsed Time: {timedelta(milliseconds=test.elapsedtime)!s}\n"
+                "</pre>"
+                f"Message: <p><pre>{html_message}</pre></p>\n"
+            )
+            exec_comments.append(exec_comment)
+        itb_test_case.exec.comments = f"<html><body>{''.join(exec_comments)}</body></html>"
+
+    def _set_itb_testcase_execution_result(self, itb_test_case, test_chain):
+        has_failed_chain = list(filter(lambda tc: tc.status.upper() == "FAIL", test_chain))
+        passed_keywords = all(tc.status.upper() == "PASS" for tc in test_chain)
+        itb_test_case.exec.actualDuration = sum([tc.elapsedtime for tc in test_chain])
+        if has_failed_chain:
+            self._set_itb_test_case_status(itb_test_case, "fail")
+        elif passed_keywords:
+            self._set_itb_test_case_status(itb_test_case, "pass")
+        else:
+            self._set_itb_test_case_status(itb_test_case, "undef")
+
+    def _get_test_phase_body(self, test_phase: TestCase) -> Body:
+        return test_phase.body
+
+    def _get_test_phase_setup(self, test_phase: TestCase) -> List[Keyword]:
+        test_phase_setup = []
+        if test_phase.has_setup and test_phase.setup:
+            self._test_setup_passed = test_phase.setup.passed
+            if test_phase.setup.name == f"Setup-{test_phase.name}":
+                test_phase_setup = list(
+                    filter(
+                        lambda kw: isinstance(kw, Keyword)
+                        and kw.parent.name == f"Setup-{test_phase.name}",
+                        test_phase.setup.body,
+                    )
+                )
+            else:
+                test_phase_setup = [test_phase.setup]
+        return test_phase_setup
+
+    def _get_test_phase_teardown(self, test_phase: TestCase) -> List[Keyword]:
+        test_phase_teardown = []
+        if test_phase.has_teardown and test_phase.teardown:
+            if test_phase.teardown.name == f"Teardown-{test_phase.name}":
+                test_phase_teardown = list(
+                    filter(
+                        lambda kw: isinstance(kw, Keyword)
+                        and kw.parent.name == f"Teardown-{test_phase.name}",
+                        test_phase.teardown.body,
+                    )
+                )
+            else:
+                test_phase_teardown = [test_phase.teardown]
+        return test_phase_teardown
+
+    def _set_atomic_interactions_execution_result(
+        self, atomic_interactions: List[InteractionDetails], test_chain: List[TestCase]
+    ):
+        self._test_setup_passed = True
+        test_chain_setup = [
+            keyword
+            for test_phase in test_chain
+            for keyword in self._get_test_phase_setup(test_phase)
+        ]
+        test_chain_body = [
+            keyword
+            for test_phase in test_chain
+            for keyword in self._get_test_phase_body(test_phase)
+        ]
+        test_chain_teardown = [
+            keyword
+            for test_phase in test_chain
+            for keyword in self._get_test_phase_teardown(test_phase)
+        ]
+        setup_interactions = self._filter_atomic_interactions_by_sequence_phase(
+            atomic_interactions, SequencePhase.Setup
+        )
+        test_step_interactions = self._filter_atomic_interactions_by_sequence_phase(
+            atomic_interactions, SequencePhase.TestStep
+        )
+        teardown_interactions = self._filter_atomic_interactions_by_sequence_phase(
+            atomic_interactions, SequencePhase.Teardown
+        )
+        self._set_interaction_verdicts(setup_interactions, test_chain_setup, SequencePhase.Setup)
+        self._set_interaction_verdicts(
+            test_step_interactions, test_chain_body, SequencePhase.TestStep
+        )
+        self._set_interaction_verdicts(
+            teardown_interactions, test_chain_teardown, SequencePhase.Teardown
+        )
+
+    def _set_interaction_verdicts(
+        self,
+        interaction_list: List[InteractionDetails],
+        test_chain_body: List[Keyword],
+        sequence_phase: SequencePhase,
+    ):
+        for index, interaction in enumerate(interaction_list):
+            if interaction.exec is None:
+                interaction.exec = InteractionExecutionSummary.from_dict({})
+            if sequence_phase == SequencePhase.TestStep and not self._test_setup_passed:
+                interaction.exec.verdict = InteractionVerdict.Skipped
+                continue
+            if index < len(test_chain_body):
+                keyword = test_chain_body[index]
+                self._check_matching_interaction_and_keyword_name(keyword, interaction)
+                interaction.exec = self._get_interaction_exec_from_keyword(keyword)
+                continue
+            if sequence_phase == SequencePhase.Setup and not self._test_setup_passed:
+                interaction.exec.verdict = InteractionVerdict.Skipped
+                continue
+            interaction.exec.verdict = InteractionVerdict.Undefined
+
+    def _filter_atomic_interactions_by_sequence_phase(
+        self, atomic_interactions: List[InteractionDetails], sequence_phase: SequencePhase
+    ):
+        return list(
+            filter(
+                lambda atomic_interaction: atomic_interaction.spec.sequencePhase == sequence_phase,
+                atomic_interactions,
+            )
+        )
+
+    def _get_interaction_exec_from_keyword(self, keyword: Keyword) -> InteractionExecutionSummary:
+        return InteractionExecutionSummary.from_dict(
+            {
+                'verdict': self._get_interaction_result(keyword.status),
+                'time': keyword.endtime,
+                'duration': keyword.elapsedtime,
+                'comments': self.get_html_keyword_comment(keyword),
+            }
+        )
+
+    def _check_matching_interaction_and_keyword_name(
+        self, keyword: Keyword, interaction: InteractionDetails
+    ) -> None:
+        if not is_normalized_equal(keyword.kwname, interaction.name) and not is_normalized_equal(
+            keyword.kwname.split('.')[-1], interaction.name
+        ):
+            raise NameError(
+                f"Execution can not be parsed, "
+                f"because keyword name '{keyword.kwname}' does not match with "
+                f"interaction '{interaction.name}' name."
+            )
+
+    def _get_keyword_messages(self, keyword: Keyword):
+        if hasattr(keyword, "messages"):
+            for message in keyword.messages:
+                yield self._create_itb_exec_comment(message)
+        if hasattr(keyword, "body"):
+            for kw in keyword.body:
+                yield from self._get_keyword_messages(kw)
+
+    def get_html_keyword_comment(self, keyword: Keyword):
+        messages = list(self._get_keyword_messages(keyword))
+        return (
+            "<html>"
+            "<body>"
+            "<style>"
+            "td {padding: 5px; border: none;} "
+            "table {font-family: monospace; border: none;}"
+            "</style>"
+            "<pre>"
+            f"Start Time:   {self.get_isotime_from_robot_timestamp(keyword.starttime)}\n"
+            f"End Time:     {self.get_isotime_from_robot_timestamp(keyword.endtime)}\n"
+            f"Elapsed Time: {timedelta(milliseconds=keyword.elapsedtime)!s}\n"
+            "</pre>"
+            "<table>"
+            "<tr>"
+            f"{'</tr><tr>'.join(messages)}"
+            "</tr>"
+            "</table>"
+            "</body>"
+            "</html>"
+        )
+
+    def _create_itb_exec_comment(
+        self,
+        message,
+    ) -> str:  # Todo: low prio: pattern für message in config festlegen
+        message_time = self.get_isotime_from_robot_timestamp(
+            message.timestamp, time_format="%H:%M:%S.%f"
+        )
+        msg = message.html_message.replace("<hr>", "<br/>").replace("<br>", "<br/>").strip()
+        return (
+            f"<td {self.render_status(message.level)}><b>{message.level}</b></td>"
+            f"<td><pre>{msg}</pre></td><td>{message_time}</td>"
+        )
+
+    @staticmethod
+    def get_isotime_from_robot_timestamp(timestamp, time_format="%Y-%m-%d %H:%M:%S.%f"):
+        return (
+            datetime.strptime(timestamp, "%Y%m%d %H:%M:%S.%f")
+            .astimezone()
+            .strftime(time_format)[:-3]
+        )
+
+    def _set_compound_interaction_execution_result(self, compound_interaction: InteractionDetails):
+        atomic_interactions = list(
+            self._get_interactions_by_type(
+                compound_interaction.interactions, InteractionType.Atomic
+            )
+        )
+        if compound_interaction.exec is None:
+            compound_interaction.exec = InteractionExecutionSummary.from_dict({})
+        compound_interaction.exec.verdict = InteractionVerdict.Skipped
+        for atomic in atomic_interactions:
+            if atomic.exec is None:
+                logger.debug(
+                    f"Atomic interaction {atomic.uniqueID} "
+                    f"had no exec details and therefore ignored."
+                )
+                atomic.exec = InteractionExecutionSummary.from_dict({})
+            if atomic.exec.verdict is InteractionVerdict.Fail:
+                compound_interaction.exec.verdict = InteractionVerdict.Fail
+                break
+            if atomic.exec.verdict is InteractionVerdict.Pass:
+                compound_interaction.exec.verdict = InteractionVerdict.Pass
+
+        compound_interaction.exec.duration = sum(
+            [interaction.exec.duration for interaction in atomic_interactions]
+        )
+        compound_interaction.exec.time = atomic_interactions[-1].exec.time
+
+    @staticmethod
+    def _set_itb_test_case_status(itb_test_case: TestCaseDetails, robot_status: str):
+        robot_status = robot_status.lower()
+        if robot_status == "pass":
+            itb_test_case.exec.status = ActivityStatus.Performed
+            itb_test_case.exec.verdict = ExecutionVerdict.Pass
+        elif robot_status == "fail":
+            itb_test_case.exec.status = ActivityStatus.Performed
+            itb_test_case.exec.verdict = ExecutionVerdict.Fail
+        else:
+            itb_test_case.exec.status = ActivityStatus.Running
+            itb_test_case.exec.verdict = ExecutionVerdict.Undefined
+
+    def end_suite(self, suite: TestSuite):
+        if not suite.metadata.get("uniqueID") or len(suite.suites):
+            return
+        test_case_set = self.json_reader.read_test_case_set(suite.metadata["uniqueID"])
+        if not test_case_set:
+            return
+        test_case_set.exec.verdict = suite.status
+
+        for testcase in test_case_set.testCases:
+            current_itb_test_case = self.itb_test_case_catalog.get(testcase.uniqueID)
+            if current_itb_test_case is None:
+                continue
+            testcase.exec.verdict = current_itb_test_case.exec.verdict
+            testcase.exec.status = current_itb_test_case.exec.status
+            testcase.exec.execStatus = current_itb_test_case.exec.execStatus
+            testcase.exec.comments = current_itb_test_case.exec.comments
+        suite_start_time = "99999999 00:00:00.000"
+        suite_end_time = "00000000 00:00:00.000"
+        table_content = []
+        for test in suite.tests:
+            suite_start_time = min(suite_start_time, test.starttime)
+            suite_end_time = max(suite_end_time, test.endtime)
+            test_chain = get_test_chain(test.name, self.phase_pattern)
+
+            if test_chain:
+                name = test_chain.name if test_chain.index == 1 else ""
+                phase = f"Phase {test_chain.index}/{test_chain.length}"
+            else:
+                name = test.name
+                phase = ""
+            if test.status != "PASS":
+                message = re.sub(r"\s*itb-reference:\s*(\S*)", "", test.message)
+                message = (
+                    message[len("*HTML*") :]
+                    .replace('<hr>', '<br />')
+                    .replace('<br>', '<br />')
+                    .strip()
+                    if message.startswith("*HTML*")
+                    else message
+                )
+            else:
+                message = self.get_isotime_from_robot_timestamp(test.endtime)
+
+            table_content.append(
+                f"<td>{name}</td>"
+                f"<td>{phase}</td>"
+                f"<td {self.render_status(test.status)}><b>{test.status}</b></td>"
+                f"<td><pre>{message}</pre></td>"
+            )
+
+        test_case_set.exec.comments = (
+            "<html>"
+            "<head>"
+            "<style>"
+            "td {padding: 5px; border: none; white-space: pre-wrap;} "
+            "table {font-family: monospace; border: none;}"
+            "</style>"
+            "</head>"
+            "<body>"
+            "<pre>"
+            f"Start Time:   {self.get_isotime_from_robot_timestamp(suite_start_time)}\n"
+            f"End Time:     {self.get_isotime_from_robot_timestamp(suite_end_time)}\n"
+            "</pre>"
+            "<table>"
+            "<tr>"
+            f"{'</tr><tr>'.join(table_content)}"
+            "</tr>"
+            "</table>"
+            "</body>"
+            "</html>"
+        )
+        write_test_structure_element(self.json_result, test_case_set)
+        logger.debug(
+            f"Successfully wrote the result from suite "
+            f"{test_case_set.uniqueID} to TestBench's Json Report."
+        )
+
+    @staticmethod
+    def render_status(status):
+        return (
+            "style='"
+            f"background-color: {BACKGROUND_COLOR.get(status, '#fff')}; "
+            f"color: {COLOR.get(status, '#000')};'"
+        )
+
+    def end_result(self, result):
+        tt_tree = self.json_reader.read_test_theme_tree()
+        if tt_tree:
+            test_suite_counter = 0
+            for tse in tt_tree.nodes:
+                if self.test_suites.get(tse.baseInformation.uniqueID) is None:
+                    continue
+                execution_result = self._get_execution_result(
+                    self.test_suites[tse.baseInformation.uniqueID].status
+                )
+                tse.execution.verdict = execution_result["execution_verdict"]
+                tse.execution.status = execution_result["activity_status"]
+                test_suite_counter += 1
+            write_test_structure_element(self.json_result, tt_tree)
+            if test_suite_counter and self.itb_test_case_catalog:
+                logger.info(f"Successfully read {test_suite_counter} test suites.")
+            else:
+                logger.warning("No test suites with execution information found.")
+            if self.create_zip:
+                directory_to_zip(self.json_result, self.json_result_path)
+            elif self.json_result != self.json_result_path:
+                copytree(self.json_dir, self.json_result_path, dirs_exist_ok=True)
+                copytree(self.json_result, self.json_result_path, dirs_exist_ok=True)
+            self.tempdir.cleanup()
+        logger.info("Successfully wrote the robot execution results to TestBench's Json Report.")
+
+    @staticmethod
+    def _get_execution_result(robot_status: str) -> Dict:
+        robot_status = robot_status.lower()
+        if robot_status == "pass":
+            return {
+                "execution_verdict": ExecutionVerdict.Pass,
+                "activity_status": ActivityStatus.Performed,
+            }
+        if robot_status == "fail":
+            return {
+                "execution_verdict": ExecutionVerdict.Fail,
+                "activity_status": ActivityStatus.Performed,
+            }
+        return {
+            "execution_verdict": ExecutionVerdict.Undefined,
+            "activity_status": ActivityStatus.Skipped,
+        }
+
+    @staticmethod
+    def _get_interaction_result(robot_status: str) -> InteractionVerdict:
+        robot_status = robot_status.upper()
+        if robot_status == "PASS":
+            return InteractionVerdict.Pass
+        if robot_status == "FAIL":
+            return InteractionVerdict.Fail
+        if robot_status == "NOT RUN":
+            return InteractionVerdict.Skipped
+        return InteractionVerdict.Skipped
+
+
+class TestChain:
+    def __init__(self, name, index, length):
+        self.name = str(name)
+        self.index = int(index)
+        self.length = int(length)
+
+
+def get_test_chain(test_name: str, phase_pattern: str) -> Optional[TestChain]:
+    matcher = re.match(get_test_chain_pattern(phase_pattern), test_name)
+    if matcher:
+        return TestChain(*matcher.groups())
+    return None
+
+
+def get_test_chain_pattern(phase_pattern: str) -> str:
+    testcase_placeholder = str(uuid.uuid4().int)
+    index_placeholder = str(uuid.uuid4().int)
+    length_placeholder = str(uuid.uuid4().int)
+    raw_pattern = re.escape(
+        phase_pattern.format(
+            testcase=testcase_placeholder,
+            index=index_placeholder,
+            length=length_placeholder,
+        )
+    )
+    return (
+        raw_pattern.replace(testcase_placeholder, r"(.+?)")
+        .replace(index_placeholder, r"(\d)")
+        .replace(length_placeholder, r"(\d)")
+    )
+
+
+def get_normalized_keyword_name(keyword_name: str) -> str:
+    return re.sub(r"[\s_]", "", keyword_name.lower())
+
+
+def is_normalized_equal(kw_one: str, kw_two: str) -> bool:
+    norm_kw_one = get_normalized_keyword_name(kw_one)
+    norm_kw_two = get_normalized_keyword_name(kw_two)
+    return norm_kw_one == norm_kw_two
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/robotframework2testbench.py` & `testbench2robotframework-0.6.1/testbench2robotframework/robotframework2testbench.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import sys
-from pathlib import Path
-from typing import Dict, Optional
-
-from robot.api import ExecutionResult
-
-from .config import Configuration
-from .log import logger, setup_logger
-from .result_writer import ResultWriter
-
-
-def robot2testbench(
-    json_input_report: str,
-    robot_result_xml: str,
-    json_output_result: Optional[str] = None,
-    config: Optional[Dict] = None,
-):
-    if not Path(json_input_report).exists():
-        sys.exit("Could not find json directory or zip file at the given path.")
-    if not Path(robot_result_xml).exists():
-        sys.exit("Robot result xml does not exist at the given path.")
-    configuration = Configuration.from_dict(config)
-    setup_logger(configuration)
-    logger.debug("Config file loaded.")
-    result = ExecutionResult(robot_result_xml)
-    logger.debug("Robot framework result xml loaded.")
-    result.visit(
-        ResultWriter(json_input_report, json_output_result, configuration, robot_result_xml)
-    )
+import sys
+from pathlib import Path
+from typing import Dict, Optional
+
+from robot.api import ExecutionResult
+
+from .config import Configuration
+from .log import logger, setup_logger
+from .result_writer import ResultWriter
+
+
+def robot2testbench(
+    json_input_report: str,
+    robot_result_xml: str,
+    json_output_result: Optional[str] = None,
+    config: Optional[Dict] = None,
+):
+    if not Path(json_input_report).exists():
+        sys.exit("Could not find json directory or zip file at the given path.")
+    if not Path(robot_result_xml).exists():
+        sys.exit("Robot result xml does not exist at the given path.")
+    configuration = Configuration.from_dict(config)
+    setup_logger(configuration)
+    logger.debug("Config file loaded.")
+    result = ExecutionResult(robot_result_xml)
+    logger.debug("Robot framework result xml loaded.")
+    result.visit(
+        ResultWriter(json_input_report, json_output_result, configuration, robot_result_xml)
+    )
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/testbench2robotframework.py` & `testbench2robotframework-0.6.1/testbench2robotframework/testbench2robotframework.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Dict
-
-from .config import Configuration
-from .json_reader import TestBenchJsonReader
-from .log import logger, setup_logger
-
-# from .robot_run import RobotSuiteRunner
-from .testbench2rf import create_test_suites
-from .testsuite_write import write_test_suites
-from .utils import PathResolver, get_directory
-
-
-def testbench2robotframework(json_report: str, config: Dict):
-    configuration = Configuration.from_dict(config)
-    setup_logger(configuration)
-    logger.debug("Config file loaded.")
-    json_report = get_directory(json_report)
-    reader = TestBenchJsonReader(json_report)
-    path_resolver = PathResolver(
-        reader.test_theme_tree,
-        tuple(reader.get_test_case_set_catalog().keys()),
-        configuration.logSuiteNumbering,
-    )
-    test_suites = create_test_suites(
-        reader.get_test_case_set_catalog(), path_resolver, configuration
-    )
-    # suite_runner = RobotSuiteRunner(test_suites, path_resolver)
-    # suite_runner.run_suites()
-    if not test_suites:
-        logger.warning("There are no test suites in the exported TestBench Projekt.")
-        return
-    write_test_suites(test_suites, configuration)
+from typing import Dict
+
+from .config import Configuration
+from .json_reader import TestBenchJsonReader
+from .log import logger, setup_logger
+
+# from .robot_run import RobotSuiteRunner
+from .testbench2rf import create_test_suites
+from .testsuite_write import write_test_suites
+from .utils import PathResolver, get_directory
+
+
+def testbench2robotframework(json_report: str, config: Dict):
+    configuration = Configuration.from_dict(config)
+    setup_logger(configuration)
+    logger.debug("Config file loaded.")
+    json_report = get_directory(json_report)
+    reader = TestBenchJsonReader(json_report)
+    path_resolver = PathResolver(
+        reader.test_theme_tree,
+        tuple(reader.get_test_case_set_catalog().keys()),
+        configuration.logSuiteNumbering,
+    )
+    test_suites = create_test_suites(
+        reader.get_test_case_set_catalog(), path_resolver, configuration
+    )
+    # suite_runner = RobotSuiteRunner(test_suites, path_resolver)
+    # suite_runner.run_suites()
+    if not test_suites:
+        logger.warning("There are no test suites in the exported TestBench Projekt.")
+        return
+    write_test_suites(test_suites, configuration)
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework/testsuite_write.py` & `testbench2robotframework-0.6.1/testbench2robotframework/testsuite_write.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import os
-import re
-import shutil
-from pathlib import Path
-from typing import Dict
-
-from robot.parsing.model.blocks import File
-
-from .config import Configuration
-from .log import logger
-from .utils import directory_to_zip
-
-
-def write_test_suites(test_suites: Dict[str, File], config: Configuration) -> None:
-    generation_directory = get_generation_directory(config.generationDirectory)
-    if config.clearGenerationDirectory:
-        clear_generation_directory(generation_directory)
-    write_test_suite_files(test_suites, generation_directory)
-    if config.createOutputZip:
-        directory_to_zip(generation_directory)
-    logger.info(f"Successfully wrote {len(test_suites)} robot files.")
-    logger.info(f"Path: {Path(generation_directory).resolve()!s}")
-
-
-def get_generation_directory(generation_directory: str) -> Path:
-    root_path = Path(os.curdir).absolute()
-    if not generation_directory:
-        return root_path / "Generated"
-    return Path(
-        re.sub(
-            r"^{root}",
-            str(root_path).replace('\\', '\\\\'),
-            generation_directory,
-            flags=re.IGNORECASE,
-        )
-    )
-
-
-def clear_generation_directory(generation_dir: Path) -> None:
-    if generation_dir.is_dir():
-        shutil.rmtree(str(generation_dir))
-        logger.info("Files in generation directory deleted.")
-    zip_file = "".join([str(generation_dir), ".zip"])
-    Path(zip_file).unlink(missing_ok=True)
-
-
-def write_test_suite_files(test_suites: Dict[str, File], generation_directory: Path) -> None:
-    for test_suite_file in test_suites.values():
-        test_suite_file.source = Path(generation_directory / f"{test_suite_file.source}.robot")
-        logger.debug(f"File written to {os.path.relpath(test_suite_file.source)}")
-        test_suite_file.save()
+import os
+import re
+import shutil
+from pathlib import Path
+from typing import Dict
+
+from robot.parsing.model.blocks import File
+
+from .config import Configuration
+from .log import logger
+from .utils import directory_to_zip
+
+
+def write_test_suites(test_suites: Dict[str, File], config: Configuration) -> None:
+    generation_directory = get_generation_directory(config.generationDirectory)
+    if config.clearGenerationDirectory:
+        clear_generation_directory(generation_directory)
+    write_test_suite_files(test_suites, generation_directory)
+    if config.createOutputZip:
+        directory_to_zip(generation_directory)
+    logger.info(f"Successfully wrote {len(test_suites)} robot files.")
+    logger.info(f"Path: {Path(generation_directory).resolve()!s}")
+
+
+def get_generation_directory(generation_directory: str) -> Path:
+    root_path = Path(os.curdir).absolute()
+    if not generation_directory:
+        return root_path / "Generated"
+    return Path(
+        re.sub(
+            r"^{root}",
+            str(root_path).replace('\\', '\\\\'),
+            generation_directory,
+            flags=re.IGNORECASE,
+        )
+    )
+
+
+def clear_generation_directory(generation_dir: Path) -> None:
+    if generation_dir.is_dir():
+        shutil.rmtree(str(generation_dir))
+        logger.info("Files in generation directory deleted.")
+    zip_file = "".join([str(generation_dir), ".zip"])
+    Path(zip_file).unlink(missing_ok=True)
+
+
+def write_test_suite_files(test_suites: Dict[str, File], generation_directory: Path) -> None:
+    for test_suite_file in test_suites.values():
+        test_suite_file.source = Path(generation_directory / f"{test_suite_file.source}.robot")
+        logger.debug(f"File written to {os.path.relpath(test_suite_file.source)}")
+        test_suite_file.save()
```

### Comparing `testbench2robotframework-0.6.0/testbench2robotframework.egg-info/PKG-INFO` & `testbench2robotframework-0.6.1/testbench2robotframework.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,303 +1,302 @@
-Metadata-Version: 2.1
-Name: testbench2robotframework
-Version: 0.6.0
-Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
-Home-page: https://github.com/imbus/testbench2robotframework
-Author: imbus AG
-Author-email: support@imbus.de
-License: Apache 2.0 License
-Platform: any
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Installation des Robot Code Generators
-
-Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
-
-```powershell
-python --version
-```
-
-Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
-Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
-
-```powershell
-python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
-```
-
-Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
-```powershell
-pip install testbench2robotframework
-```
-
-Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
-
-```powershell
-tb2robot --version
-```
-
-# Verwendung des Robot Code Generators
-Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
-
-Der Befehl ``tb2robot --help
-`` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
-
-Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
-
-(@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
-
-(@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
-```powershell
-tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
-```
-Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
-
-![](./images/testthemen.PNG)
-![](./images/generated.PNG)
-
-Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
-
-Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
-Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
-
-(@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
-
-(@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
-
-(@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
-
-Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
-```powershell
-tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
-```
-
-# Konfiguration der Ergebnisse
-Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
-
-## rfLibraryRegex
-Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
-Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
-Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
-
-![](./images/testbench_rfLibraryRegex.PNG)
-
-```python
-*** Settings ***
-Library    Browser
-Library    BuiltIn
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfLibraryRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
-  ]
-```
-
-## rfResourceRegex
-Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
-Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
-Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
-
-![](./images/testbench_rfResourceRegex.PNG)
-
-```python
-*** Settings ***
-Resource    keywords.resource
-```
-In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
-```json
-"rfResourceRegex": [
-    "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
-  ]
-```
-## rfLibraryRoots
-Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
-Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
-
-Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
-
-Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
-
-```json
-"rfLibraryRoots": ["RobotLibraries"]
-```
-
-![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
-
-Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
-
-```python
-*** Settings ***
-Library    BuiltIn
-Library    OperatingSystem
-# UNKNOWN    Process
-```
-
-## rfResourceRoots
-Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
-
-Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
-
-```json
-"rfResourceRoots": ["RF-Resources"]
-```
-
-![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
-
-Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
-
-```python
-*** Settings ***
-Resource    keywords.resource
-# UNKNOWN    unknownKeywords
-```
-
-## fullyQualified
-Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
-
-Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
-
-```python
-SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
-```
-Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
-
-```python
-Open Browser      https://robotframework.org/    firefox
-```
-
-## resourceDirectory
-Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
-Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
-
-```json
-"resourceDirectory": "{root}/Resources",
-```
-
-```robotframework
-*** Settings ***
-Resource    ../Resources/myKeywords.resource
-```
-
-## generationDirectory
-Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
-```json
-"generationDirectory": "{root}/generatedRobotFiles"
-```
-
-## createOutputZip
-Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
-
-## logSuiteNumbering
-Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
-
-```json
-"logSuiteNumbering": true
-```
-## clearGenerationDirectory
-Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
-
-```json
-"clearGenerationDirectory": true,
-```
-
-## logCompoundInteractions
-Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
-
-```json
-"logCompoundInteractions": true,
-```
-
-## subdivisionsMapping
-Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
-
-```json
-"subdivisionsMapping": {
-    "libraries": {
-      "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
-      "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
-    },
-    "resources": {
-      "MyKeywords": "{root}/../MyKeywords.resource",
-      "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
-    }
-  }
-```
-
-
-## forcedImport
-Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
-
-```json
-"forcedImport": {
-    "libraries": [
-      "SeleniumLibrary"
-    ],
-    "resources":
-    [
-      "technical_keywords.resource"
-    ],
-    "variables": [
-      "myVars.py"
-    ]
-  }
-```
-
-## loggingConfiguration
-Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
-Gültige Optionen sind:
-
-* "CRITICAL"
-
-* "FATAL"
-
-* "ERROR"
-
-* "WARNING"
-
-* "WARN"
-
-* "INFO"
-
-* "DEBUG"
-
-* "NOTSET"
-
-Das Default Log-Level ist ``INFO``.
-```json
-"loggingConfiguration": {
-  "console": {
-    "logLevel": "info"
-  }
-}
-```
-
-## referenceBehaviour
-Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
-Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
-Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
-
-```json
-"referenceBehaviour": "ATTACHMENT"
-```
-
-## attachmentConflictBehaviour
-Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
-Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
-
-Die möglichen Werte haben dabei die folgende Bedeutung:
-- ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
-- USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
-- USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
-- RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
-```json
-"attachmentConflictBehaviour": "USE_EXISTING"
-```
-
-## testCaseSplitPathRegEx
-Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
-
+Metadata-Version: 2.1
+Name: testbench2robotframework
+Version: 0.6.1
+Summary: Robot Framework Code Generator from Keyword-Driven Tests in imbus TestBench 3.0 and newer
+Home-page: https://github.com/imbus/testbench2robotframework
+Author: imbus AG
+Author-email: support@imbus.de
+License: Apache 2.0 License
+Description: # Installation des Robot Code Generators
+        
+        Voraussetzung für die Installation der Software ist eine vorhandene Python Installation. Die minimal benötigte Version ist Python 3.8. Zum Überprüfen, ob die korrekte Python Version installiert ist, kann der folgende Kommandozeilen Befehl verwendet werden:
+        
+        ```powershell
+        python --version
+        ```
+        
+        Die Installation des Code Generators erfolgt mithilfe eines Python Wheels, welches in der Lieferung enthalten ist.
+        Dieses kann durch Ausführung des folgenden Kommandozeilenbefehls installiert werden, wobei ``testbench2robotframework-0.4.1-py3-none-any.whl`` für den Pfad zu der heruntergeladenen whl-Datei steht:
+        
+        ```powershell
+        python -m pip install testbench2robotframework-0.4.1-py3-none-any.whl
+        ```
+        
+        Alternativ kann die Installation direkt online aus dem Python Package Index installiert werden.
+        ```powershell
+        pip install testbench2robotframework
+        ```
+        
+        Wenn die Installation durchgeführt wurde, liefert folgender Befehl die aktuell installierte Version:
+        
+        ```powershell
+        tb2robot --version
+        ```
+        
+        # Verwendung des Robot Code Generators
+        Nach erfolgreicher Installation des Robot Code Generators kann dieser durch den Befehl ``tb2robot`` oder ``testbench2robotframework`` ausgeführt werden.
+        
+        Der Befehl ``tb2robot --help
+        `` zeigt, wie aus einem TestBench JSON Report, Robot Framework Testsuites generiert werden können und wie die Durchführungsergebnisse wieder eingelesen werden können.
+        
+        Zum Generieren von Robot Framework Testsuites wird der Subcommand ``write`` mit  zwei Parametern aufgerufen:
+        
+        (@) Dem Pfad zu einer JSON Datei, die als Konfigurationsdatei für die Ausgabe des Generators dient. Wird diese beim Aufruf des Code Generators nicht übergeben, so wird automatisch eine Konfigurationsdatei mit dem Namen ``config.json`` generiert.
+        
+        (@) Dem Pfad zu den TestBech JSON Report Dateien. Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+        
+        Der folgende Aufruf demonstriert die Verwendung anhand eines Beispiels:
+        ```powershell
+        tb2robot write -c .\Konfigurationsdatei.json E:\TestBench\report.zip
+        ```
+        Das folgende Beispiel zeigt, wie auf diese Weise der Testthemenbaum der TestBench in Robot Framework Testsuites konvertiert wird.
+        
+        ![](./images/testthemen.PNG)
+        ![](./images/generated.PNG)
+        
+        Beispiel für die Generierung von Robot Framework Testsuites aus dem Testthemenbaum der TestBench. Für jedes Testthema wird ein Verzeichnis erstellt. Dieses Verzeichnis enthält eine ``__init__.robot`` Datei mit Informationen über das Testthema. Außerdem wird für jeden Testfallsatz eine Robot Framework Testsuite erzeugt, die die eigentlichen Testfälle enthält.
+        
+        Nach Ausführung der Robotframework Test Suites können die Ergebnisse zurück in den Json Report der Tesbench geschrieben werden.
+        Zu diesem Zweck wird der Subcommand ``read`` verwendet, der eine XML-Ergebnisdatei liest und die Ergebnisse in die JSON-Dateien schreibt.
+        
+        (@) Den Pfad zu einer XML-Ergebnisdatei, aus der die Ergebnisse der Testdurchführung gelesen werden.
+        
+        (@) Den Pfad zu einem Verzeichnis oder einer ZIP Datei in der die Ergebnisse gespeichert werden sollen. Dies ist ein optionaler Parameter. Wird der Parameter nicht übergeben, so wird der übergebene JSON Report überschrieben.
+        
+        (@) Den Pfad zu den TestBech JSON Report Dateien (ohne Ergebnisse). Diese können in einem Verzeichnis oder in einer ZIP Datei liegen.
+        
+        Der folgende Aufruf demonstriert das Lesen der Ergebnisse anhand eines Beispiels:
+        ```powershell
+        tb2robot write -o .\output.xml -r .\ReportWithResults.zip E:\TestBench\report.zip
+        ```
+        
+        # Konfiguration der Ergebnisse
+        Zur Konfiguration des Ergebnisses sollte beim Aufruf des Robot Code Generators der Pfad zu einer JSON Konfigurationsdatei übergeben werden. Auf diese Weise kann beispielsweise der Pfad angegeben werden, in welchem die *.robot Dateien erzeugt werden. Die Konfigurationsdatei kann die folgenden Einstellungen enthalten:
+        
+        ## rfLibraryRegex
+        Eine Liste von regulären Ausdrücken, mittels derer TestBench Subdivisionen als Robot Framework Bibliotheken identifiziert werden können.
+        Der standardmäßig eingestellte Regex findet alle Subdivisionen, deren Name auf "[Robot-Library]" enden. Wenn eine Interaktion aus einer der gefundenen Subdivisionen verwendet wird, so wird diese Subdivision in der generierten Robot Framework Testsuite als Bibliothek importiert.
+        Auf diese Weise führt beispielsweise die Verwendung von Interaktionen aus den folgenden TestBench Subdivisionen zum Import der ``Browser-`` und ``BuiltIn`` Bibliotheken.
+        
+        ![](./images/testbench_rfLibraryRegex.PNG)
+        
+        ```python
+        *** Settings ***
+        Library    Browser
+        Library    BuiltIn
+        ```
+        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Bibliothek, in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+        ```json
+        "rfLibraryRegex": [
+            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Library\\].*"
+          ]
+        ```
+        
+        ## rfResourceRegex
+        Analog zum ``rfLibraryRegex`` gibt es auch einen regulären Ausdruck, der für das Identifizieren von Subdivisionen zuständig ist, die als Robot Framework Ressourcen importiert werden sollen.
+        Standardmäßig werden über diesen Regex alle Subdivisionen, deren Namen auf "[Robot-Resource]" enden, als Ressourcen in den Robot Framework Testsuiten importiert.
+        Im folgenden Beispiel wird die Robot Framework Ressource mit dem Namen ``keywords.resource`` importiert, da die zugehörige Subdivision mit ``[Robot-Resource]`` endet.
+        
+        ![](./images/testbench_rfResourceRegex.PNG)
+        
+        ```python
+        *** Settings ***
+        Resource    keywords.resource
+        ```
+        In der Konfigurationsdatei kann der reguläre Ausdruck abgeändert werden. Der Name, mit dem die Ressource in der Robot Framework Testsuite eingebunden werden soll, muss dabei über die named group ``?P<resourceName>`` angegeben werden.
+        ```json
+        "rfResourceRegex": [
+            "(?:.*\\.)?(?P<resourceName>[^.]+?)\\s*\\[Robot-Resource\\].*"
+          ]
+        ```
+        ## rfLibraryRoots
+        Eine Liste der verschiedenen TestBench Root Subdivisionen, die Robotframework Bibliotheken enthalten.
+        Das Verwenden einer Interaktion aus einer ``rfLibraryRoots`` Subdivision, führt dazu, dass die Subdivision der zweiten Ebene, unter welcher die verwendete Interaktion (in einer beliebiger Tiefe) zu finden ist, als Library in der Robot Framework Test Suite importiert wird.
+        
+        Bibliotheken (Subdivisionen der zweiten Ebene des Testelementebaumes), die nicht in einer der Root Subdivision enthalten sind, werden als ``Unknown`` Import in der Robotdatei markiert.
+        
+        Im folgenden Beispiel ist lediglich die ``RobotLibraries`` Subdivision als ``rfLibraryRoot`` vorgegeben.
+        
+        ```json
+        "rfLibraryRoots": ["RobotLibraries"]
+        ```
+        
+        ![Robot Framework Bibliotheken werden in der TestBench als Subdivisionen dargestellt](./images/libraries.PNG)
+        
+        Dies führt dazu, dass nur die in dieser Subdivision enthaltenden Bibliotheken ``BuiltIn`` und ``OperatingSystem`` importiert werden. Die ``Process`` Bibliothek ist hingegen in einer Subdivision definiert, die nicht als ``rfLibraryRoot`` angegeben ist. Aus diesem Grund wird sie nicht importiert:
+        
+        ```python
+        *** Settings ***
+        Library    BuiltIn
+        Library    OperatingSystem
+        # UNKNOWN    Process
+        ```
+        
+        ## rfResourceRoots
+        Analog zu den Bibliotheken müssen auch die Root Subdivision der Robot Framework Ressourcen Dateien in der Konfigurationsdatei angegeben werden.
+        
+        Das folgende Beispiel zeigt, den Import von Subdivisionen, die nicht als ``rfResourceRoots`` angegeben sind:
+        
+        ```json
+        "rfResourceRoots": ["RF-Resources"]
+        ```
+        
+        ![Robot Framework Ressourcen Dateien werden in der TestBench als Subdivisionen dargestellt](./images/resources.PNG)
+        
+        Da ``UnknownResources`` nicht in den ``rfResourceRoots`` enthalten ist, wird die in dieser Subdivision enthaltende Ressourcedatei ``unknownKeywords`` nicht importiert.
+        
+        ```python
+        *** Settings ***
+        Resource    keywords.resource
+        # UNKNOWN    unknownKeywords
+        ```
+        
+        ## fullyQualified
+        Boolesche Variable, die angibt, ob die Keywords in den generierten Robot Dateien lediglich durch den Keywordnamen aufgerufen werden oder, ob zusätzlich der Bibliotheksname vorangestellt werden soll.
+        
+        Die Konfiguration ``"fullyQualified": true`` führt beispielsweise zu dem folgenden Keyword Aufruf:
+        
+        ```python
+        SeleniumLibrary.Open Browser      https://robotframework.org/    firefox
+        ```
+        Wird hingegen ``"fullyQualified": false`` verwendet, so wird das Keyword ohne den zugehörigen Bibliotheksnamen aufgerufen:
+        
+        ```python
+        Open Browser      https://robotframework.org/    firefox
+        ```
+        
+        ## resourceDirectory
+        Damit der Robot Code Generator die korrekten Ressourcen in der Setting Section der Testsuites einbindet, muss in der Konfigurationsdatei der Pfad zu einem Verzeichnis angegeben werden, das sämtliche für das Projekt benötigten Ressourcen Dateien enthält. Dieser Pfad kann absolut oder relativ zu dem Verzeichnis, in dem der Robot Code Generator ausgeführt wurde, angegeben werden.
+        Im Falle eines relativen Pfades muss ein ``{root}`` vorangestellt werden.
+        
+        ```json
+        "resourceDirectory": "{root}/Resources",
+        ```
+        
+        ```robotframework
+        *** Settings ***
+        Resource    ../Resources/myKeywords.resource
+        ```
+        
+        ## generationDirectory
+        Der Pfad zu dem Verzeichnis mit den generierten Robot Framework Testsuites kann über den Parameter ``generationDirectory`` vorgegeben werden. Wie bereits beim ``resourceDirectory`` kann auch dieser Pfad relativ oder absolut angegeben werden:
+        ```json
+        "generationDirectory": "{root}/generatedRobotFiles"
+        ```
+        
+        ## createOutputZip
+        Für den Fall, dass die Ausgabe des Robot Code Generators auch in Form einer ZIP Datei erfolgen soll, muss die Variable createOutputZip auf true gesetzt werden. Dies hat zur Folge, dass sowohl ein Verzeichnis als auch eine ZIP Datei mit den generierten Robotframework Testsuites erstellt wird.
+        
+        ## logSuiteNumbering
+        Über die Boolesche Variable ``logSuiteNumbering`` kann angegeben werden, ob der Präfix eines Verzeichnisses in den Logs angezeigt werden soll. Der Präfix eines Verzeichnisses/einer Robot Framework Testsuite bestimmt die Reihenfolge, in der die Test Suites ausgeführt werden.
+        
+        ```json
+        "logSuiteNumbering": true
+        ```
+        ## clearGenerationDirectory
+        Wird  die Variable ``clearGenerationDirectory`` auf ``true`` gesetzt, so werden bei jeder Ausführung des Robot Code Generators die Dateien der vorherigen Läufe gelöscht.
+        
+        ```json
+        "clearGenerationDirectory": true,
+        ```
+        
+        ## logCompoundInteractions
+        Bei der Konvertierung der TestBench Testfallsätze nach Robotframework werden lediglich die atomaren Interaktionen in Robotframework aufgerufen. Damit ein Benutzer die gesamte Hierarchie eines Testfallsatzes in Robotframework sehen kann, muss der Wert der Variablen ``logCompoundInteractions`` ``true`` sein. Dies hat zur Folge, dass auch die zusammengesetzten Interaktionen als Kommentare in den Testsuites erscheinen. Durch eine entsprechende Einrückung kann ein Benutzer erkennen, in welcher zusammengesetzten Interaktion eine atomare Interaktion aufgerufen wird.
+        
+        ```json
+        "logCompoundInteractions": true,
+        ```
+        
+        ## subdivisionsMapping
+        Im ``subdivisionsMapping`` kann definiert werden, welche TestBench Subdivision welchem Import Statement in Robotframework entspricht. Auf diese Weise können auch Bibliotheken mit bestimmten Parametern und "Remote Libraries" eingebunden werden. Bibliotheken und Ressourcen, die an dieser Stelle definiert werden, werden nur importiert, wenn auch ein Keyword der entsprechenden Bibliothek/Ressource verwendet wird.
+        
+        ```json
+        "subdivisionsMapping": {
+            "libraries": {
+              "SeleniumLibrary": "SeleniumLibrary    timeout=10    implicit_wait=1    run_on_failure=Capture Page Screenshot",
+              "SuperRemoteLibrary": "Remote    http://127.0.0.1:8270       WITH NAME    SuperRemoteLibrary"
+            },
+            "resources": {
+              "MyKeywords": "{root}/../MyKeywords.resource",
+              "MyOtherKeywords": "{resourceDirectory}/subdir/MyOtherKeywords.resource"
+            }
+          }
+        ```
+        
+        
+        ## forcedImport
+        Damit eine Bibliotheks-, Ressourcen- oder eine Variablendatei importiert wird, ohne dass es eine entsprechende Subdivision in der TestBench gibt, muss diese als ``forcedImport`` hinterlegt sein. Dateien, die auf diese Weise importiert werden, werden in jeder Testsuite importiert, unabhängig davon, ob ein Keyword aus dieser Datei verwendet wird.
+        
+        ```json
+        "forcedImport": {
+            "libraries": [
+              "SeleniumLibrary"
+            ],
+            "resources":
+            [
+              "technical_keywords.resource"
+            ],
+            "variables": [
+              "myVars.py"
+            ]
+          }
+        ```
+        
+        ## loggingConfiguration
+        Über die Einstellung ``loggingConfiguration`` kann das Log-Level gesetzt werden.
+        Gültige Optionen sind:
+        
+        * "CRITICAL"
+        
+        * "FATAL"
+        
+        * "ERROR"
+        
+        * "WARNING"
+        
+        * "WARN"
+        
+        * "INFO"
+        
+        * "DEBUG"
+        
+        * "NOTSET"
+        
+        Das Default Log-Level ist ``INFO``.
+        ```json
+        "loggingConfiguration": {
+          "console": {
+            "logLevel": "info"
+          }
+        }
+        ```
+        
+        ## referenceBehaviour
+        Damit die Referenzen, die während der Testdurchführung erstellt werden, in die TestBench importiert werden können, muss die ``referenceBehaviour`` angegeben werden.
+        Diese definiert, ob eine Referenz als Anhang oder als Referenz auf eine im Dateisystem liegende Datei importiert werden soll.
+        Der Parameter kann somit einen der beiden Werte ``REFERENCE`` oder ``ATTACHMENT`` annehmen.
+        
+        ```json
+        "referenceBehaviour": "ATTACHMENT"
+        ```
+        
+        ## attachmentConflictBehaviour
+        Für den Fall, dass eine Referenz als Attachment importiert werden soll, muss angegeben werden, wie gleiche Dateinamen zu behandeln sind.
+        Zu diesem Zweck kann der Parameter attachmentConflictBehaviour mit einem der Werte ``ERROR``, ``USE_NEW``, ``USE_EXISTING`` oder ``RENAME_NEW`` angegeben werden.
+        
+        Die möglichen Werte haben dabei die folgende Bedeutung:
+        - ERROR: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird eine Fehlermeldung geworfen. Es wird lediglich das zuerst gelesene Attachment importiert.
+        - USE_EXISTING: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuerst gelesene Attachment importiert.
+        - USE_NEW: Für den Fall, dass mehrere Attachments mit dem gleichen Namen existieren, wird lediglich das zuletzt gelesene Attachment importiert.
+        - RENAME_NEW: Für den Fall, dass ein Attachment gelesen wird und bereits ein gleichnamiges existiert, wird der Name des neuen Attachments abgewandelt, dass er einzigartig ist und importiert werden kann.
+        ```json
+        "attachmentConflictBehaviour": "USE_EXISTING"
+        ```
+        
+        ## testCaseSplitPathRegEx
+        Über den im Parameter ``testCaseSplitPathRegEx`` angegebenen Wert kann ein Benutzer bestimmen, ob ein Testfallsatz aus der TestBench in mehrere Robot Framework Testfälle unterteilt werden soll. Zu diesem Zweck muss der Benutzer in ``testCaseSplitPathRegEx`` den Namen einer Interaktion definieren, anhand welcher der Code Generator erkennt, dass ein Testfall an dieser Stelle unterteilt werden soll. Anschließend kann diese ``Splitting interaction`` in einem Testfallsatz zum Unterteilen von Testfällen verwendet werden.
+        
+        
+Platform: any
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

