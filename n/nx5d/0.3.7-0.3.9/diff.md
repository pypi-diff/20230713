# Comparing `tmp/nx5d-0.3.7.tar.gz` & `tmp/nx5d-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nx5d-0.3.7.tar", last modified: Tue May 16 06:51:00 2023, max compression
+gzip compressed data, was "nx5d-0.3.9.tar", last modified: Thu Jul 13 10:20:53 2023, max compression
```

## Comparing `nx5d-0.3.7.tar` & `nx5d-0.3.9.tar`

### file list

```diff
@@ -1,225 +1,231 @@
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/
--rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.7/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.7/.gitlab-ci.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.7/.readthedocs.yaml
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.7/COPYING.md
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-16 06:51:00.839137 nx5d-0.3.7/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.7/README.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.817137 nx5d-0.3.7/doc/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.818137 nx5d-0.3.7/doc/mkdocs/
--rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.7/doc/mkdocs/about.md
--rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.7/doc/mkdocs/api.md
--rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 09:48:18.000000 nx5d-0.3.7/doc/mkdocs/concepts.md
--rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.7/doc/mkdocs/frame.svg
--rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 09:48:18.000000 nx5d-0.3.7/doc/mkdocs/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.7/doc/mkdocs/license.md
--rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.7/doc/mkdocs/module-nx.md
--rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.7/doc/mkdocs/scan.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.7/doc/mkdocs/streak1.svg
--rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.7/doc/mkdocs/streak2.svg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.818137 nx5d-0.3.7/doc/mkdocs/tutorials/
--rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.7/doc/mkdocs/tutorials/index.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/
--rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
--rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
--rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
--rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
--rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
--rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/
--rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.819137 nx5d-0.3.7/doc/mkdocs/user-guide/
--rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.7/doc/mkdocs/user-guide/index.md
--rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.7/doc/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.7/mkdocs.yml
--rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.7/pyproject.toml
--rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.7/scratch.org
--rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-05-16 06:51:00.839137 nx5d-0.3.7/setup.cfg
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.815137 nx5d-0.3.7/src/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.820137 nx5d-0.3.7/src/nx5d/
--rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d/_version.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/edf.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.821137 nx5d-0.3.7/src/nx5d/h5like/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.7/src/nx5d/h5like/__init__.py
--rw-r--r--   0 florin    (1000) florin    (1000)    12534 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/petra3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.7/src/nx5d/h5like/pypod.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11003 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/spec.py
--rw-r--r--   0 florin    (1000) florin    (1000)    11159 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/h5like/tools.py
--rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.7/src/nx5d/h5like/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/nx.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/runlog.py
--rw-r--r--   0 florin    (1000) florin    (1000)    14860 2023-04-27 14:19:57.000000 nx5d-0.3.7/src/nx5d/scan.py
--rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.7/src/nx5d/streaks.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.823137 nx5d-0.3.7/src/nx5d/xrd/
--rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/ColonelSandersFinest.py
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/__init__.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/analysis.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/esrf_id09.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/experiment-xpp.yml
--rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/experiment.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-04-27 14:16:35.000000 nx5d-0.3.7/src/nx5d/xrd/kmc3.py
--rw-r--r--   0 florin    (1000) florin    (1000)      779 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/xrd/petra3.py
--rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/roi.py
--rw-r--r--   0 florin    (1000) florin    (1000)    19952 2023-05-16 06:50:26.000000 nx5d-0.3.7/src/nx5d/xrd/signal.py
--rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-25 09:48:18.000000 nx5d-0.3.7/src/nx5d/xrd/xfel.py
--rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/xraytest.py
--rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.7/src/nx5d/xrd/xrd_helpers.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.821137 nx5d-0.3.7/src/nx5d.egg-info/
--rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/PKG-INFO
--rw-r--r--   0 florin    (1000) florin    (1000)    11943 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/SOURCES.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/dependency_links.txt
--rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/requires.txt
--rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-05-16 06:51:00.000000 nx5d-0.3.7/src/nx5d.egg-info/top_level.txt
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.823137 nx5d-0.3.7/tests/
--rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/.gitignore
--rw-r--r--   0 florin    (1000) florin    (1000)     1167 2023-04-27 15:21:20.000000 nx5d-0.3.7/tests/fio_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)      961 2023-04-17 15:45:54.000000 nx5d-0.3.7/tests/pabst_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1559 2023-04-17 15:45:54.000000 nx5d-0.3.7/tests/pypod_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/runlog_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     2219 2023-05-16 06:50:26.000000 nx5d-0.3.7/tests/spec_test.py
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.824137 nx5d-0.3.7/tests/test_data/fioh5/
--rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-04-25 09:48:18.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00342.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.824137 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/
--rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-04-25 10:50:01.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
--rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-04-25 09:48:18.000000 nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744.fio
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.828137 nx5d-0.3.7/tests/test_data/runfile/
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokendata1.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokendata2.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_brokenheader.log
--rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/run105_simple.log
--rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04.log
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0001.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0002.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0003.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0004.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0005.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0006.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0007.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0008.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0009.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0010.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0011.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0012.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0013.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0014.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0015.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0016.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0017.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0018.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0019.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0020.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0021.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0022.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0023.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0024.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0025.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0026.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0027.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0028.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0029.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0030.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0031.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0032.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0033.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0034.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0035.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0036.edf
--rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/runfile/short_run04_0037.edf
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.828137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.834137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
--rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.829137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/
--rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/231-cw7-12083-roessle-missing.spec
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.816137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.834137 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/
--rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_1.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_10.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_11.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_14.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_15.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_16.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_17.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_18.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_19.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_2.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_20.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_21.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_22.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_23.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_24.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_25.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_26.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_27.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_28.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_29.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_3.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_30.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_31.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_32.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_33.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_34.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_35.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_36.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_37.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_38.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_39.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_4.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_40.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_5.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_6.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_7.tif
--rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_8.tif
-drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-05-16 06:51:00.839137 nx5d-0.3.7/tests/test_data/spech5/empty-spec/
--rw-r--r--   0 florin    (1000) florin    (1000)     5209 2023-05-16 06:50:26.000000 nx5d-0.3.7/tests/test_data/spech5/empty-spec/empty-spec.spec
--rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.7/tests/xfel_test.py
--rw-r--r--   0 florin    (1000) florin    (1000)     1059 2023-03-14 11:33:48.000000 nx5d-0.3.7/tests/xrd_data_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.050817 nx5d-0.3.9/
+-rw-r--r--   0 florin    (1000) florin    (1000)       72 2023-04-13 14:23:04.000000 nx5d-0.3.9/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     3261 2023-04-12 13:31:40.000000 nx5d-0.3.9/.gitlab-ci.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      227 2023-03-15 11:10:41.000000 nx5d-0.3.9/.readthedocs.yaml
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-14 11:33:48.000000 nx5d-0.3.9/COPYING.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-07-13 10:20:53.050817 nx5d-0.3.9/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)     2724 2023-03-27 10:49:57.000000 nx5d-0.3.9/README.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.027816 nx5d-0.3.9/doc/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.029816 nx5d-0.3.9/doc/mkdocs/
+-rw-r--r--   0 florin    (1000) florin    (1000)       11 2023-03-15 10:15:42.000000 nx5d-0.3.9/doc/mkdocs/about.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      147 2023-04-12 12:52:07.000000 nx5d-0.3.9/doc/mkdocs/api.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    27056 2023-04-25 09:48:18.000000 nx5d-0.3.9/doc/mkdocs/concepts.md
+-rw-r--r--   0 florin    (1000) florin    (1000)     5970 2023-03-25 14:27:00.000000 nx5d-0.3.9/doc/mkdocs/frame.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)     2483 2023-04-25 09:48:18.000000 nx5d-0.3.9/doc/mkdocs/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    34916 2023-03-15 10:32:22.000000 nx5d-0.3.9/doc/mkdocs/license.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      723 2023-03-27 10:50:49.000000 nx5d-0.3.9/doc/mkdocs/module-nx.md
+-rw-r--r--   0 florin    (1000) florin    (1000)    36207 2023-03-25 14:25:35.000000 nx5d-0.3.9/doc/mkdocs/scan.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    25024 2023-03-25 14:49:22.000000 nx5d-0.3.9/doc/mkdocs/streak1.svg
+-rw-r--r--   0 florin    (1000) florin    (1000)    11491 2023-03-25 14:49:37.000000 nx5d-0.3.9/doc/mkdocs/streak2.svg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.029816 nx5d-0.3.9/doc/mkdocs/tutorials/
+-rw-r--r--   0 florin    (1000) florin    (1000)      516 2023-03-15 10:35:31.000000 nx5d-0.3.9/doc/mkdocs/tutorials/index.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.030816 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/
+-rw-------   0 florin    (1000) florin    (1000)    44315 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md
+-rw-------   0 florin    (1000) florin    (1000)    19430 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png
+-rw-------   0 florin    (1000) florin    (1000)    25263 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png
+-rw-------   0 florin    (1000) florin    (1000)    23184 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png
+-rw-------   0 florin    (1000) florin    (1000)    13289 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png
+-rw-------   0 florin    (1000) florin    (1000)    16038 2023-03-14 14:52:34.000000 nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.030816 nx5d-0.3.9/doc/mkdocs/tutorials/scansource-howto/
+-rw-r--r--   0 florin    (1000) florin    (1000)     8968 2023-03-14 12:31:08.000000 nx5d-0.3.9/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.031816 nx5d-0.3.9/doc/mkdocs/user-guide/
+-rw-r--r--   0 florin    (1000) florin    (1000)      322 2023-04-12 12:48:11.000000 nx5d-0.3.9/doc/mkdocs/user-guide/index.md
+-rw-r--r--   0 florin    (1000) florin    (1000)      513 2023-03-15 14:06:55.000000 nx5d-0.3.9/doc/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      273 2023-03-15 10:49:21.000000 nx5d-0.3.9/mkdocs.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)      280 2023-03-14 11:33:48.000000 nx5d-0.3.9/pyproject.toml
+-rw-r--r--   0 florin    (1000) florin    (1000)     2974 2022-08-02 20:02:56.000000 nx5d-0.3.9/scratch.org
+-rw-r--r--   0 florin    (1000) florin    (1000)      946 2023-07-13 10:20:53.051817 nx5d-0.3.9/setup.cfg
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.024816 nx5d-0.3.9/src/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.032816 nx5d-0.3.9/src/nx5d/
+-rw-r--r--   0 florin    (1000) florin    (1000)      117 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      160 2023-07-13 10:20:52.000000 nx5d-0.3.9/src/nx5d/_version.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7559 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/edf.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.033816 nx5d-0.3.9/src/nx5d/h5like/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-04-12 12:44:54.000000 nx5d-0.3.9/src/nx5d/h5like/__init__.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19039 2023-07-13 10:14:38.000000 nx5d-0.3.9/src/nx5d/h5like/fio.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     5686 2023-04-17 15:45:54.000000 nx5d-0.3.9/src/nx5d/h5like/pypod.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    10887 2023-07-13 09:54:49.000000 nx5d-0.3.9/src/nx5d/h5like/spec.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    11159 2023-05-16 06:50:26.000000 nx5d-0.3.9/src/nx5d/h5like/tools.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    31529 2023-04-13 15:04:17.000000 nx5d-0.3.9/src/nx5d/h5like/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)    15796 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/nx.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     7585 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/runlog.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    14864 2023-07-12 08:33:59.000000 nx5d-0.3.9/src/nx5d/scan.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     7572 2023-04-17 15:45:54.000000 nx5d-0.3.9/src/nx5d/streaks.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.034816 nx5d-0.3.9/src/nx5d/xrd/
+-rw-r--r--   0 florin    (1000) florin    (1000)      756 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/ColonelSandersFinest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/__init__.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     4859 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/analysis.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/esrf_id09.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1481 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/experiment-xpp.yml
+-rw-r--r--   0 florin    (1000) florin    (1000)     4201 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/experiment.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1939 2023-04-27 14:16:35.000000 nx5d-0.3.9/src/nx5d/xrd/kmc3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      779 2023-05-16 06:50:26.000000 nx5d-0.3.9/src/nx5d/xrd/petra3.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     4316 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/roi.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    19952 2023-05-16 06:50:26.000000 nx5d-0.3.9/src/nx5d/xrd/signal.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      972 2023-04-25 09:48:18.000000 nx5d-0.3.9/src/nx5d/xrd/xfel.py
+-rwxr-xr-x   0 florin    (1000) florin    (1000)     3960 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/xraytest.py
+-rw-r--r--   0 florin    (1000) florin    (1000)    15899 2023-03-14 11:33:48.000000 nx5d-0.3.9/src/nx5d/xrd/xrd_helpers.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.032816 nx5d-0.3.9/src/nx5d.egg-info/
+-rw-r--r--   0 florin    (1000) florin    (1000)     3514 2023-07-13 10:20:52.000000 nx5d-0.3.9/src/nx5d.egg-info/PKG-INFO
+-rw-r--r--   0 florin    (1000) florin    (1000)    12162 2023-07-13 10:20:53.000000 nx5d-0.3.9/src/nx5d.egg-info/SOURCES.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        1 2023-07-13 10:20:52.000000 nx5d-0.3.9/src/nx5d.egg-info/dependency_links.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)      157 2023-07-13 10:20:52.000000 nx5d-0.3.9/src/nx5d.egg-info/requires.txt
+-rw-r--r--   0 florin    (1000) florin    (1000)        5 2023-07-13 10:20:52.000000 nx5d-0.3.9/src/nx5d.egg-info/top_level.txt
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.035816 nx5d-0.3.9/tests/
+-rw-r--r--   0 florin    (1000) florin    (1000)        0 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/.gitignore
+-rw-r--r--   0 florin    (1000) florin    (1000)     1601 2023-07-13 10:01:26.000000 nx5d-0.3.9/tests/fio_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)      963 2023-07-13 10:17:26.000000 nx5d-0.3.9/tests/pabst_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1575 2023-07-13 10:18:20.000000 nx5d-0.3.9/tests/pypod_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1342 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/runlog_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     2553 2023-07-12 08:33:59.000000 nx5d-0.3.9/tests/spec_test.py
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.025816 nx5d-0.3.9/tests/test_data/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.035816 nx5d-0.3.9/tests/test_data/fioh5/
+-rw-r--r--   0 florin    (1000) florin    (1000)    13611 2023-04-25 09:48:18.000000 nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00342.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.024816 nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.036816 nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744/lambda/
+-rw-r--r--   0 florin    (1000) florin    (1000)   302228 2023-04-25 10:50:01.000000 nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
+-rw-r--r--   0 florin    (1000) florin    (1000)    13952 2023-04-25 09:48:18.000000 nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.036816 nx5d-0.3.9/tests/test_data/fiotiff/
+-rw-r--r--   0 florin    (1000) florin    (1000)    75171 2023-07-12 09:00:53.000000 nx5d-0.3.9/tests/test_data/fiotiff/s1_1161_00484.fio
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.036816 nx5d-0.3.9/tests/test_data/fiotiff/s1_1161_484/
+-rw-r--r--   0 florin    (1000) florin    (1000)   383956 2023-05-22 09:58:30.000000 nx5d-0.3.9/tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00000.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)   383956 2023-05-22 09:58:32.000000 nx5d-0.3.9/tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00001.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)   383956 2023-05-22 09:58:42.000000 nx5d-0.3.9/tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00002.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.041816 nx5d-0.3.9/tests/test_data/runfile/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10599 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run105.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run105_brokendata1.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run105_brokendata2.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10591 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run105_brokenheader.log
+-rw-r--r--   0 florin    (1000) florin    (1000)    10588 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/run105_simple.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     5668 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04.log
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0001.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0002.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0003.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0004.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0005.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0006.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0007.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0008.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0009.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0010.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0011.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0012.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0013.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0014.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0015.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0016.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0017.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0018.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0019.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0020.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0021.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0022.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0023.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0024.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0025.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0026.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0027.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0028.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0029.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0030.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0031.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0032.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0033.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0034.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0035.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0036.edf
+-rw-r--r--   0 florin    (1000) florin    (1000)     1824 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/runfile/short_run04_0037.edf
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.025816 nx5d-0.3.9/tests/test_data/spech5/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.041816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.025816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.046816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/
+-rw-r--r--   0 florin    (1000) florin    (1000)    32118 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.050817 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2133 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3609 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3668 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3164 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.042816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/
+-rw-r--r--   0 florin    (1000) florin    (1000)  1374025 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/231-cw7-12083-roessle-missing.spec
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.025816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.046816 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/
+-rw-r--r--   0 florin    (1000) florin    (1000)     2204 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_1.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3368 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_10.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3429 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_11.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3827 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_14.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4037 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_15.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4216 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_16.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4322 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_17.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4305 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_18.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_19.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2228 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_2.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4307 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_20.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     4165 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_21.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3937 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_22.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3842 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_23.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3835 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_24.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3592 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_25.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3479 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_26.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3270 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_27.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3221 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_28.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3065 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_29.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2427 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_3.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2901 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_30.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2931 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_31.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2707 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_32.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2548 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_33.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2512 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_34.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2306 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_35.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2260 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_36.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2162 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_37.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2078 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_38.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2026 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_39.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2556 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_4.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2013 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_40.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2654 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_5.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2786 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_6.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     2845 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_7.tif
+-rw-r--r--   0 florin    (1000) florin    (1000)     3019 2023-03-14 11:33:48.000000 nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_8.tif
+drwxr-xr-x   0 florin    (1000) florin    (1000)        0 2023-07-13 10:20:53.050817 nx5d-0.3.9/tests/test_data/spech5/empty-spec/
+-rw-r--r--   0 florin    (1000) florin    (1000)     5209 2023-05-16 06:50:26.000000 nx5d-0.3.9/tests/test_data/spech5/empty-spec/empty-spec.spec
+-rw-r--r--   0 florin    (1000) florin    (1000)     3341 2023-04-13 14:23:04.000000 nx5d-0.3.9/tests/xfel_test.py
+-rw-r--r--   0 florin    (1000) florin    (1000)     1087 2023-07-13 10:16:49.000000 nx5d-0.3.9/tests/xrd_data_test.py
```

### Comparing `nx5d-0.3.7/.gitlab-ci.yml` & `nx5d-0.3.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/COPYING.md` & `nx5d-0.3.9/COPYING.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/PKG-INFO` & `nx5d-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.7
+Version: 0.3.9
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.7/README.md` & `nx5d-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/concepts.md` & `nx5d-0.3.9/doc/mkdocs/concepts.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/frame.svg` & `nx5d-0.3.9/doc/mkdocs/frame.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/index.md` & `nx5d-0.3.9/doc/mkdocs/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/license.md` & `nx5d-0.3.9/doc/mkdocs/license.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/module-nx.md` & `nx5d-0.3.9/doc/mkdocs/module-nx.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/scan.svg` & `nx5d-0.3.9/doc/mkdocs/scan.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/streak1.svg` & `nx5d-0.3.9/doc/mkdocs/streak1.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/streak2.svg` & `nx5d-0.3.9/doc/mkdocs/streak2.svg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/index.md` & `nx5d-0.3.9/doc/mkdocs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/kmc3-data-processing-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_15_2.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_33_0.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png` & `nx5d-0.3.9/doc/mkdocs/tutorials/kmc3-data-processing-howto/output_52_1.png`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md` & `nx5d-0.3.9/doc/mkdocs/tutorials/scansource-howto/scansource-howto.md`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/doc/mkdocs.yml` & `nx5d-0.3.9/doc/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/scratch.org` & `nx5d-0.3.9/scratch.org`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/setup.cfg` & `nx5d-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/edf.py` & `nx5d-0.3.9/src/nx5d/edf.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/h5like/petra3.py` & `nx5d-0.3.9/src/nx5d/h5like/fio.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import silx.io.commonh5 as ch5
 import numpy as np
 
 from os import path, walk
 from glob import glob
 from itertools import chain
+from nx5d.h5like.spec import SpecH5LazyTiffNode, H5Group
 
 import h5py
 import re
 
 import logging
 
 ''' Selected data formats for the PETRA3 synchrotron at DESY.
@@ -175,30 +176,33 @@
     def visit(self, *a, **kw):
         return self.h5node.visit(*a, **kw)
 
     def visititems(self, *a, **kw):
         return self.h5node.visititems(*a, **kw)
         
             
-class FioH5(ch5.File):
+class FioH5Base(ch5.File):
     ''' Bastard HDF5 API fake for the "FIO" data format, e.g. for PETRA3/P08.
 
     Currently (as of: April 2023) the data format appears to be this:
     
       - A master `.fio` file appearing somewhere on the filesystem, containing
         variables with scalar data, variables with vector data, and some
         "scanning values" a.k.a. positioners. This is an ASCII file with
         a proprietary format, but not terribly complicated to parse.
 
       - A folder with the same base name as the `.fio` file (only without the
         `.fio` extension), on the same level as the file; it contains one
         or more subdirectories with detector names (e.g. `lambda/`)
 
-      - Within the subdirectory, one or more `.nxs` files (Nexus/HDF5 files)
-        usually containing detector data. Currently,
+      - There appear to be two formats in use for the detector data: HDF5
+        or TIFF images.
+
+        For the HDF5 version, Within the subdirectory, one or more `.nxs`
+        files (Nexus/HDF5 files) usually containing detector data. Currently,
         the following subfolder structure has been seen in the wild:
         ```
         $ tree .
         .
         ├── m3_2507_00342
         │   └── lambda
         │       └── m3_2507_00342_00000.nxs
@@ -209,15 +213,83 @@
         │       └── m3_2507_00744_00000.nxs
         └── m3_2507_00744.fio
         ```
         We don't have exact information as to what the `ct_file_00000.nxs` is.
         Also, we don't have exact information as to what the `_00000.nxs`
         trail of the `.nxs` file is.
 
-    Seamlessly integrating HDF5 files ("overlaying") with the parameters of the FIO
+        For the TIFF files, a subfolder containing TIFF files is available,
+        with a name similar, but slightly different from the FIO file
+        (can be inferred by parsing the individual FIO constituents).
+        For instance:
+        ```
+        $ tree .
+        .
+        ├── s1_1161_00484.fio
+        └── s1_1161_484
+            ├── s1_1161_00484_00000.tif
+            ├── s1_1161_00484_00001.tif
+            ├── s1_1161_00484_00002.tif
+            ...
+        ```
+
+    This is the base class containing the FIO information. Subclasses
+    `FioH5` and `FioTiff` implement one, respectively the other version
+    '''
+
+    def __init__(self, fio, fiogrp=None, h5extra=None):
+        ''' Loads FIO (text) file, underlining its data with existing HDF5 data.
+
+        Normally with every `.fio` file comes a directory of the same name, containing
+        subdirectories named after a detector, containing HDF5 files of the same
+        (or a similar) name.
+        This can be overriden, or augmented with other files, using the `h5glob`
+        parameter.
+
+        Args:
+        
+            fio: The `.fio` file path.
+        
+            fiogrp: The HDF5 group name of the `.fio` file. For uniformity, we
+              propose `fio`. But if this is `None`, we're using the FIO base name
+              of the file (i.e. the filename only component, without extension).
+
+            h5extra: Python `dict()` with target HDF5 folder as key, and HDF5 file
+              paths as values, for HDF5 data files to integrate. If the path
+              name does not begin with `/` or `.`, the data path of the current
+              FIO file is prepended.      
+        '''
+        super().__init__()
+
+        # base of the filename (no dirs, no extension)
+        self.fio_base = '.'.join(path.basename(fio).split('.')[:-1])
+
+        self.fio_dir = path.abspath(path.dirname(fio))
+
+        if fiogrp is None:
+            fiogrp = self.fio_base
+
+        self.fioGroup = FioGroup(fio, name=fiogrp or fio_base, parent=self)
+        self.add_node(self.fioGroup)
+
+        dkey = next(iter(self.fioGroup["data"].keys()))
+        self.fio_num_frames = len(self.fioGroup["data"][dkey])
+
+        logging.debug(f'{fio} with {self.fio_num_frames} data frames')
+
+
+class FioH5(FioH5Base):
+    ''' Implements a H5-like API for .fio files with detector images in HDF5.
+
+    This uses the `FioH5Base` to initialize a H5-like API for a FIO
+    file, then tries to offer a view of the associated HDF5 files
+    from within this interface.
+    
+    Seamlessly integrating HDF5 files ("overlaying" hierachical structures)
+    with the parameters of the FIO
     files would be the king's version, but it is tricky for various reasons:
     
       - What do we do on ambiguous parameters? Error and bail out?
 
       - How do we easily iterate through all the sub-groups? (HDF5 has several
         distinct ways of retrieving subnodes: ["path"]["subpath"], ["path/subpath"],
         and several `.visit...()` functions.)
@@ -264,15 +336,14 @@
     ```
 
     (Note that the example "m3_2507_00744.fio" provided as test data with this package's
     source code does _not_ have a dataset named `data` -- it's called `"mock_data"`
     instead, and has a reduced shape of `"(61, 100, 100)"` for size reasons.)
     '''
 
-
     def __init__(self, fio, fiogrp='fio', h5extra=None):
         ''' Loads FIO (text) file, underlining its data with existing HDF5 data.
 
         Normally with every `.fio` file comes a directory of the same name, containing
         subdirectories named after a detector, containing HDF5 files of the same
         (or a similar) name.
         This can be overriden, or augmented with other files, using the `h5glob`
@@ -287,63 +358,174 @@
               of the file (i.e. the filename only component, without extension).
 
             h5extra: Python `dict()` with target HDF5 folder as key, and HDF5 file
               paths as values, for HDF5 data files to integrate. If the path
               name does not begin with `/` or `.`, the data path of the current
               FIO file is prepended.      
         '''
-        super().__init__()
-
-        # base of the filename (no dirs, no extension)
-        fio_base = '.'.join(path.basename(fio).split('.')[:-1])
+        super().__init__(fio, fiogrp)
 
         # base directory of where the current FIO file's HDF5 stuff is located
-        fio_datadir = path.join(path.dirname(fio), fio_base)
+        self.fio_h5dir = path.join(path.dirname(fio), self.fio_base)        
 
         # Searching for <base>/<device>/<base><extra>.nxs. This will produce a
         # nested dict(): { 'device': { 'extra': <file path...> } }.
-        extra_re = re.compile(fio_base+"(.*)[.]nxs")
+        extra_re = re.compile(self.fio_base+"(.*)[.]nxs")
         devices = {
             path.basename(device) : {
                 extra_re.match(path.basename(f)).groups()[0] : f
-                for f in glob(path.join(device, fio_base+"*.nxs"))
+                for f in glob(path.join(device, self.fio_base+"*.nxs"))
             } 
-            for device in glob(path.join(fio_datadir, '*'))
+            for device in glob(path.join(self.fio_h5dir, '*'))
         }
 
         # This is a flat {<device><extra>: <file path>, ...} map.
         flat_devices = { dev+ext:devices[dev][ext] \
                          for dev in devices \
                          for ext in devices[dev] }
         
         if h5extra is not None:
             devices.update(h5extra)
 
-        self.fioGroup = FioGroup(fio, name=fiogrp or fio_base, parent=self)
-        self.add_node(self.fioGroup)            
-        
         # Open the full list of HDF5 files specified as a base.
         self.h5sub = { k:h5py.File(p, 'r') for k,p in flat_devices.items() }
         
         self.h5nodes = { }
         for h5name,h5file in self.h5sub.items():
             node = H5pyRebaseGroup(h5file["/"], name=h5name, parent=self)
             self.add_node(node)
             self.h5nodes[h5name] = node
 
 
     def _get(self, name, getlink):
-        # Overrides original _get() to deal with H5pyRebaseGroup(). We essentially
-        # end up here when we have a multi-path __getitem__ (e.g. self["h5file/entry"],
-        # where "h5file" is the rebase group, and "entry" a node within that group.
+        # Overrides original _get() from silx.io.commonh5.File()
+        # to deal with H5pyRebaseGroup(). We essentially
+        # end up here when we have a multi-path __getitem__
+        # (e.g. self["h5file/entry"], where "h5file" is the rebase
+        # group, and "entry" a node within that group.
         
-        # Quick n dirty strategy is to just check the first element of "name" against
-        # the self.h5sub keys, and just pass the rest on to the subnode if found
+        # Quick n dirty strategy is to just check the first element
+        # of "name" against the self.h5sub keys, and just pass the
+        # rest on to the subnode, if found.
 
         paths = name.split('/')
         first = paths[0]
         rest = '/'.join(paths[1:])
         
         if first in self.h5nodes.keys() and len(paths) > 1:
             return self.h5nodes[first].__getitem__(rest)
         else:
             return super()._get(name, getlink)
+        
+
+class FioTiff(FioH5Base):
+    ''' Loas a FIO file into an HDF5 API and imports TIFF data as detector images.
+
+    NOTE: Uses components from `nx5d.spech5`, and a lot of copy-pasta code.
+    Should probably be consolidated at one point.
+
+    Use like this:
+    ```
+    f = FioTiff('path/to/my_fio_file.fio')
+    f['my_fio_file/detector/data'][()]
+    ...
+    ```
+
+    The Fio-H5 layout, by default, is rougly this:
+    ```
+      . <fiobase>
+      ├── detector
+      │    └── data (the TIFF files as a FxNxM dataset)
+      ├── data
+      │    ├── ...  (angles and other paramters)
+      │    ...
+      └── parameters
+           ├── ...  (fio header parameters0
+           ...
+    ```
+    
+    You know the rest of the drill.
+    '''
+    
+    def __init__(self, fiofile, fiogrp=None):
+        ''' Loads the FIO file `fiofile` with associated TIFF data.
+
+        The FIO file name is required to have the format `{label}_{run}_{scan}.fio`.
+        The TIFF files will be searched in a similar directory, but with a slightly
+        different formatting (`{label}_{run}_{scan:05d}/`), and with a similar
+        name structure, again, with different formatting
+        (`{label}_{run:d}_{scan:05d}_{frameidx:05d}`). This is hardcoded for
+        now.
+
+        Args:
+        
+            fiofile: The FIO file path.
+
+            fiogrp: The HDF5 group name to use for the FIO file. If none
+              is specified, the base name of the file (no path, no extension)
+              will be used.
+        '''
+        super().__init__(fiofile, fiogrp)
+
+        parts = self.fio_base.split("_")
+        if len(parts) != 3:
+            raise RuntimeError(f'Expecting FIO file as <label>_<run>_<scan>; got {fiofile} instead.')
+
+        label = parts[0]
+        run = int(parts[1])
+        scan = int(parts[2])
+        
+        #tiffdir = '%s_%s_%.5d' % (label, run, scan)
+
+
+        tiffPartialFmt = "{fiodir}/{label}_{run:d}_{scan:d}/"\
+            "{label}_{run:d}_{scan:05d}_{frameidx}.tif".format(**{
+                "fiodir": self.fio_dir,
+                "label": label,
+                "run": run,
+                "scan": scan,
+                "frameidx": "{frameidx:05d}"
+                
+            })
+
+        self._adopt_scan("detector", tiffPartialFmt)
+
+        self._enter_cnt = 0
+        self._enter_data = None
+
+
+    def __enter__(self, *args, **kwargs):
+        '''
+        Opening / closing a SpecTiffH5 is pretty expensive. We usually want to
+        employ with-guards (enter/exit) when doing that, but the original SpecH5
+        does not support "nested" guards (i.e. entering/exitting multiple
+        times on the same object).
+
+        This is an extension to do just that. (Need to check if h5py.File supports
+        this... the original Python open() / file object definitely does.)
+        '''
+        if self._enter_cnt == 0:
+            self._enter_data = super().__enter__(*args, **kwargs)
+        self._enter_cnt += 1
+        return self._enter_data
+
+
+    def __exit__(self, *args, **kwargs):
+        if self._enter_cnt > 0:
+            self._enter_cnt -= 1
+        if self._enter_cnt == 0:
+            super().__exit__(*args, **kwargs)
+
+
+    def _adopt_scan(self, instrumentName, tiffFormat, dataNodeArgs=None):
+        # place data inside "instrument/<name>/data"
+        parent = self.fioGroup
+        
+        parent.add_node(H5Group(parent=parent, name=instrumentName,
+                              attrs={'NX_class': 'NXinstrument'} ))
+        instrObj = parent[instrumentName]
+
+        instrObj.add_node(SpecH5LazyTiffNode(tiffPathFmt=tiffFormat,
+                                             numFrames=self.fio_num_frames,
+                                             name="data",
+                                             parent=parent,
+                                             **(dataNodeArgs or {})))
```

### Comparing `nx5d-0.3.7/src/nx5d/h5like/pypod.py` & `nx5d-0.3.9/src/nx5d/h5like/pypod.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/h5like/spec.py` & `nx5d-0.3.9/src/nx5d/h5like/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,18 +59,19 @@
 '''
 
 class SpecH5LazyTiffNode(SpecH5LazyNodeDataset):
     '''
     Implements a NodeDataset that lazily loads a list of TIFF files,
     specified as a path format that relies on an index variable.
     '''
-    def __init__(self, *args, tiffPathFmt="{frameidx}.tiff", numFrames=0, **kwargs):
+    def __init__(self, *args, tiffPathFmt="{frameidx}.tiff", numFrames=0, cache=True, **kwargs):
         super().__init__(*args, **kwargs)
         self._tiff_path_fmt = tiffPathFmt
         self._tiff_frames_no = int(numFrames)
+        self._cache_tiffs = cache
 
 
     def _create_data(self):
         data = []
         shape = None
         lasterr = None
         missing = []
@@ -93,84 +94,73 @@
         # of the appropriate shape. But if we have no shape at this
         # point, this means that _all_ TIFFs are missing. We
         # want to get loud about that (don't we?...)
         if shape is None:
             logging.warning("Dataset had no frames at all.")
             return np.array(np.NaN)
         
-        return np.array([ (i if i is not None else np.full(shape, np.nan)) \
-                          for i in data])
-    
+        a = np.array([ (i if i is not None else np.full(shape, np.nan)) for i in data])
+        
+        return a
 
-    def __getitem__(self, item):
-        '''
-        Apparently we can optimize this so that only a single file is
-        loaded if not already initialized (...so we don't have to load
-        the whole bunch for single-frame access). In that case, `item`
-        is the index of the file, and all we have to do is plug it
-        into the name formatter.
-
-        OTOH the ESRF H5 library is slow af in specific instances (e.g.
-        when doing itermittend slicing a 3D dataset from HDF5.) Not sure if
-        this is a problem of HDF5 or of some ESRF trickery. So we might keep
-        an eye on this (...in case it's something like this).
-        '''
-        if not self._is_initialized: 
-            try:            
-                idx = None
-                slc = None
-                if isinstance(item, int):
-                    idx = item
-                    slc = None
-                else:
-                    idx, slc = item
-                    assert isinstance(idx, int)
-
-                # Access the frame from 'idx'
-                p = self._tiff_path_fmt.format(index=item)
-                frame = np.array([tifffile.imread(p)])
 
-                # ...and possibly a sub-slice ('None' is the same as [:])
-                return frame[slc]
+    def _get_data(self):
+        if self._cache_tiffs:
+            return super()._get_data()
+
+        # Avoid caching
+        return self._create_data()
 
-            except:
-                pass
 
+    def __getitem__(self, item):
+        if not self._cache_tiffs:
+            data = self._create_data()
+            return data.__getitem__(item)
         return super().__getitem__(item)
 
     
 class SpecTiffH5(SpecH5):
     '''
     Mocks a HDF5 file using the Spec H5 module from Silx.
 
     In addition the "regular" `slix.io.spech5.SpecH5` functionality, after loading the
     SPEC file, this module also injects lazy-loading nodes for the TIFF files
     correspondng to a typical KMC3 setup.
     '''
 
     def __init__(self, *args, instrumentName="pilatus",
                  framePathFmt='{dirname}/{instr}/S{scannr:05}/{basename}_{scannr}_{frameidx}.tif',
+                 cache=True,
                  **kwargs):
-        '''
-        Parameters:
-
-          - `instrument`: A name/label for the instrument. For one, this is used to compile
-            the location of where to insert the data from the external TIFF files (as
-            specified by `tiffInsertFmt` and `tiffLinkFmt`); for another, this is used
-            to determine the location of the TIFF files on disk relative to the
-            SPEC file (as specified by `scanPathFmt`).
-        
-          - `framePathFmt`: format for the image scan filepath.
+        ''' Initializes a HDF5-like object based on a SPEC file with data in TIFF images.
 
-          - `scanIndexNameFmt`: string formatting that ties the scan number (on disk)
-            and scan name (in teh SpecH5 naming) together.
+        Args:
+            instrumentName: A name/label for the instrument. For one, this is used to compile
+              the location of where to insert the data from the external TIFF files (as
+              specified by `tiffInsertFmt` and `tiffLinkFmt`); for another, this is used
+              to determine the location of the TIFF files on disk relative to the
+              SPEC file (as specified by `scanPathFmt`).
+        
+            framePathFmt: format for the image scan filepath.
+
+            scanIndexNameFmt: string formatting that ties the scan number (on disk)
+              and scan name (in teh SpecH5 naming) together.
+
+            cache: This parameter is passed to `SpecH5LazyNode`. If set to `True` (the default),
+              data from TIFF files in subnodes is cached in memory. This is generally what you
+              want, except for rare cases where you are going to read all the data in memory
+              first, and risk overwhelming your local RAM. This is the case, for instance,
+              when you call `silx.io.convert.write_to_h5()` on a `SpecTiffH5` object which
+              represents a large set of scans.
 
          All string formatters can make use of any or all of the following variables:
         
            - `{dirname}`: folder-only component of the spec file name
+
+           - `{instr}`: the instrument name (from the `instrumentName` parameter above)
         
            - `{basename}`: base name the SPEC file, with the last component after a dot
              (typically ".spec" removed
 
            - `{scannr}`: scan number; this is typically an integer, assigned by "the
              algorithm", and typically starting with 1 for the first scan
 
@@ -186,14 +176,15 @@
            - `filename` (position 0): the path of the SPEC file to read
         
         '''
         super().__init__(*args, **kwargs)
         
         self._specBaseName = '.'.join(path.basename(self.filename).split('.')[:-1]) \
             or path.base(self.filename)
+        
         self._specDirName = path.abspath(path.dirname(self.filename))
 
         for scanName in self.keys():
             
             scan = self[scanName]
             scanNr, foo = scanName.split('.')
 
@@ -201,16 +192,17 @@
                 "basename": self._specBaseName,
                 "dirname": self._specDirName,
                 "scannr": int(scanNr),
                 "instr": instrumentName,
                 "scanidx": "{scanidx}",
                 "frameidx": "{frameidx}"
             })
-            
-            self._adopt_scan(scan, instrumentName, tiffPartialFmt)
+
+            datakw = {'cache': cache}
+            self._adopt_scan(scan, instrumentName, tiffPartialFmt, datakw)
 
             self._enter_cnt = 0
             self._enter_data = None
 
 
     def __enter__(self, *args, **kwargs):
         '''
@@ -231,15 +223,15 @@
     def __exit__(self, *args, **kwargs):
         if self._enter_cnt > 0:
             self._enter_cnt -= 1
         if self._enter_cnt == 0:
             super().__exit__(*args, **kwargs)
 
 
-    def _adopt_scan(self, scanObj, instrumentName, tiffFormat):
+    def _adopt_scan(self, scanObj, instrumentName, tiffFormat, dataNodeArgs=None):
 
         measRoot = scanObj['measurement']
         instrRoot = scanObj['instrument']
         posnrs = instrRoot['positioners']
         
 
         # Let's hope they're all the same... :-)
@@ -253,14 +245,15 @@
         instrRoot.add_node(H5Group(parent=instrRoot, name=instrumentName,
                                    attrs={'NX_class': 'NXinstrument'} ))
         instrObj = instrRoot[instrumentName]
 
         instrObj.add_node(SpecH5LazyTiffNode(tiffPathFmt=tiffFormat,
                                              numFrames=numFrames,
                                              name="data",
-                                             parent=instrObj))
+                                             parent=instrObj,
+                                             **(dataNodeArgs or {})))
 
         # create a link inside "measurement" that points to "instrument/<name>/data"
         link_target = instrObj.name.replace('measurement', 'instrument')
         measRoot.add_node(H5SoftLink(name=instrumentName,
                                      path=link_target + "/data",
                                      parent=measRoot))
```

### Comparing `nx5d-0.3.7/src/nx5d/h5like/tools.py` & `nx5d-0.3.9/src/nx5d/h5like/tools.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/h5like/xfel.py` & `nx5d-0.3.9/src/nx5d/h5like/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/nx.py` & `nx5d-0.3.9/src/nx5d/nx.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/runlog.py` & `nx5d-0.3.9/src/nx5d/runlog.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/scan.py` & `nx5d-0.3.9/src/nx5d/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         elif isinstance(locator, tuple) and isinstance(locator[0], str):
             return (path_mangler(locator[0]), *(locator[1:]))
 
         else:
             return locator
 
 
-    def read (self, frameSlicer, _h5like=None, lean=True, **dataKeys):
+    def read (self, frameSlicer, _h5like=None, lean=False, **dataKeys):
         '''
         Returns a bunch of image(s) starting with `start`
         (default: last image taken). If `number` is None,
         all the images to the end of the scan are read.
         Parameters:
         
           - `frameSlicer`: A slice object for selecting frames within a scan
@@ -238,16 +238,16 @@
             factory is used. Meant only for internal use (e.g. by `.streaks()`)
             and may disappear in the future, but is otherwise safe for any kind
             abuse. The reasoning is that sometimes fake h5py-like objects
             are expensive and open (more so than HDF5 objects), so re-use might
             improve speed.
 
           - `lean`: If `True`, the "required datasets" (i.e. those that were
-            specified with `__init__()`) are omitted from the result. This is
-            the default.
+            specified with `__init__()`) are omitted from the result. The
+            default is `False`.
         
           - `**dataKeys`: Data sets to retrieve; the name of the parameter will
             result in a key, and the value of the parameter should refer to the
             corresponding HDF5-like dataset path. This is passed to
             `HdfCarver`, so please also refer to the documentation
             of that class.
```

### Comparing `nx5d-0.3.7/src/nx5d/streaks.py` & `nx5d-0.3.9/src/nx5d/streaks.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/ColonelSandersFinest.py` & `nx5d-0.3.9/src/nx5d/xrd/ColonelSandersFinest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/analysis.py` & `nx5d-0.3.9/src/nx5d/xrd/analysis.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/esrf_id09.py` & `nx5d-0.3.9/src/nx5d/xrd/esrf_id09.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/experiment-xpp.yml` & `nx5d-0.3.9/src/nx5d/xrd/experiment-xpp.yml`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/experiment.py` & `nx5d-0.3.9/src/nx5d/xrd/experiment.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/kmc3.py` & `nx5d-0.3.9/src/nx5d/xrd/kmc3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/petra3.py` & `nx5d-0.3.9/src/nx5d/xrd/petra3.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/roi.py` & `nx5d-0.3.9/src/nx5d/xrd/roi.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/signal.py` & `nx5d-0.3.9/src/nx5d/xrd/signal.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/xfel.py` & `nx5d-0.3.9/src/nx5d/xrd/xfel.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/xraytest.py` & `nx5d-0.3.9/src/nx5d/xrd/xraytest.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d/xrd/xrd_helpers.py` & `nx5d-0.3.9/src/nx5d/xrd/xrd_helpers.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/src/nx5d.egg-info/PKG-INFO` & `nx5d-0.3.9/src/nx5d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nx5d
-Version: 0.3.7
+Version: 0.3.9
 Summary: NX5 Duct Tape
 Author: Florin Boariu
 Author-email: florin.pt@rootshell.ro
 Project-URL: Source Code, https://gitlab.com/codedump2/nx5d
 Project-URL: Bug Tracker, https://gitlab.com/codedump2/nx5d/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `nx5d-0.3.7/src/nx5d.egg-info/SOURCES.txt` & `nx5d-0.3.9/src/nx5d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 src/nx5d/streaks.py
 src/nx5d.egg-info/PKG-INFO
 src/nx5d.egg-info/SOURCES.txt
 src/nx5d.egg-info/dependency_links.txt
 src/nx5d.egg-info/requires.txt
 src/nx5d.egg-info/top_level.txt
 src/nx5d/h5like/__init__.py
-src/nx5d/h5like/petra3.py
+src/nx5d/h5like/fio.py
 src/nx5d/h5like/pypod.py
 src/nx5d/h5like/spec.py
 src/nx5d/h5like/tools.py
 src/nx5d/h5like/xfel.py
 src/nx5d/xrd/ColonelSandersFinest.py
 src/nx5d/xrd/__init__.py
 src/nx5d/xrd/analysis.py
@@ -65,14 +65,18 @@
 tests/runlog_test.py
 tests/spec_test.py
 tests/xfel_test.py
 tests/xrd_data_test.py
 tests/test_data/fioh5/m3_2507_00342.fio
 tests/test_data/fioh5/m3_2507_00744.fio
 tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs
+tests/test_data/fiotiff/s1_1161_00484.fio
+tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00000.tif
+tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00001.tif
+tests/test_data/fiotiff/s1_1161_484/s1_1161_00484_00002.tif
 tests/test_data/runfile/run04.log
 tests/test_data/runfile/run105.log
 tests/test_data/runfile/run105_brokendata1.log
 tests/test_data/runfile/run105_brokendata2.log
 tests/test_data/runfile/run105_brokenheader.log
 tests/test_data/runfile/run105_simple.log
 tests/test_data/runfile/short_run04.log
```

### Comparing `nx5d-0.3.7/tests/pabst_test.py` & `nx5d-0.3.9/tests/pabst_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,11 +37,11 @@
         #print([k for k in h5.keys()])
 
     #print(h5ex.keys())
 
     pbs = Pabst(moo="@/moo", idx="@/idx").moo(idx=3)
     #pbs = Pabst(idx="@/idx").moo(idx=3)
 
-    tmp = pbs(h5ex)
+    #tmp = pbs(h5ex)
     #return tmp
 
-    print(tmp)
+    #print(tmp)
```

### Comparing `nx5d-0.3.7/tests/pypod_test.py` & `nx5d-0.3.9/tests/pypod_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     concat_h5(h5, {"boron": {"theMoron": np_array(range(30)).reshape(6,5)}})
 
     s = h5["boron/theMoron"]
 
     assert s.shape == (10, 5)
             
 
+@pytest.fixture
 def test_concat_hetero():
     '''Returns a HDF5 object with virtual data.'''
 
     data = {
         "idx": np_array(range(100)),
         "moo": np_array(range(300)).reshape(100,3)
     }
```

### Comparing `nx5d-0.3.7/tests/runlog_test.py` & `nx5d-0.3.9/tests/runlog_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/spec_test.py` & `nx5d-0.3.9/tests/spec_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,9 +83,25 @@
     assert not isnan(d1[1]).all()
 
 
 def test_missingcolumns(badfile2):
     h5like = SpecTiffH5(badfile2)
 
     tmp = h5like["2.1/measurement/pilatus"]
+
+
+def test_nocache(testfile):
+
+    h5like = SpecTiffH5(testfile, cache=False)
+    node = h5like["44.1/instrument/pilatus/data"]
+
+    d1 = node[0:3,0:10,20:30]    
+    assert node._is_initialized == False
+
+    data = node[()]    
+
+    d2 = node[0:3,0:10,20:30]
+
+    assert (d1 == d2).all()
+    assert node._is_initialized == False
```

### Comparing `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00342.fio` & `nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00342.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs` & `nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744/lambda/m3_2507_00744_00000.nxs`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/fioh5/m3_2507_00744.fio` & `nx5d-0.3.9/tests/test_data/fioh5/m3_2507_00744.fio`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run04.log` & `nx5d-0.3.9/tests/test_data/runfile/run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run105.log` & `nx5d-0.3.9/tests/test_data/runfile/run105.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run105_brokendata1.log` & `nx5d-0.3.9/tests/test_data/runfile/run105_brokendata1.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run105_brokendata2.log` & `nx5d-0.3.9/tests/test_data/runfile/run105_brokendata2.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run105_brokenheader.log` & `nx5d-0.3.9/tests/test_data/runfile/run105_brokenheader.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/run105_simple.log` & `nx5d-0.3.9/tests/test_data/runfile/run105_simple.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04.log` & `nx5d-0.3.9/tests/test_data/runfile/short_run04.log`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0001.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0001.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0002.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0002.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0003.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0003.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0004.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0004.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0005.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0005.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0006.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0006.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0007.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0007.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0008.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0008.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0009.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0009.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0010.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0010.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0011.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0011.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0012.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0012.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0013.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0013.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0014.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0014.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0015.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0015.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0016.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0016.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0017.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0017.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0018.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0018.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0019.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0019.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0020.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0020.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0021.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0021.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0022.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0022.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0023.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0023.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0024.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0024.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0025.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0025.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0026.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0026.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0027.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0027.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0028.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0028.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0029.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0029.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0030.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0030.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0031.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0031.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0032.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0032.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0033.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0033.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0034.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0034.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0035.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0035.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0036.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0036.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/runfile/short_run04_0037.edf` & `nx5d-0.3.9/tests/test_data/runfile/short_run04_0037.edf`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/231-cw7-12083-roessle.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00002/231-cw7-12083-roessle_2_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_0.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_12.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_13.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle/pilatus/S00044/231-cw7-12083-roessle_44_9.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/231-cw7-12083-roessle-missing.spec` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/231-cw7-12083-roessle-missing.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_1.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_1.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_10.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_10.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_11.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_11.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_14.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_14.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_15.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_15.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_16.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_16.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_17.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_17.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_18.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_18.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_19.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_19.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_2.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_2.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_20.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_20.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_21.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_21.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_22.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_22.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_23.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_23.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_24.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_24.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_25.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_25.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_26.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_26.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_27.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_27.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_28.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_28.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_29.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_29.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_3.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_3.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_30.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_30.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_31.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_31.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_32.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_32.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_33.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_33.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_34.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_34.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_35.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_35.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_36.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_36.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_37.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_37.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_38.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_38.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_39.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_39.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_4.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_4.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_40.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_40.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_5.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_5.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_6.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_6.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_7.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_7.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_8.tif` & `nx5d-0.3.9/tests/test_data/spech5/231-cw7-12083-roessle-missing/pilatus/S00044/231-cw7-12083-roessle-missing_44_8.tif`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/test_data/spech5/empty-spec/empty-spec.spec` & `nx5d-0.3.9/tests/test_data/spech5/empty-spec/empty-spec.spec`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/xfel_test.py` & `nx5d-0.3.9/tests/xfel_test.py`

 * *Files identical despite different names*

### Comparing `nx5d-0.3.7/tests/xrd_data_test.py` & `nx5d-0.3.9/tests/xrd_data_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/python
 
-from nx5d.xrd import data as xd
-from nx5d.xrd import kmc3 as kmc3
+#from nx5d.xrd import data as xd
+#from nx5d.xrd import kmc3 as kmc3
 
 import pytest, random
 
 from pprint import pprint
 
 @pytest.fixture
 def testfile():
 
     # Note that, for data storage reasons within the git project,
     # our testfile contains only TIFF data for scan "2.1".
     return "./tests/test_data/spech5/231-cw7-12083-roessle.spec"
 
 
-def test_experimentsetup(testfile):
-
-    h5like = kmc3.SpecTiffH5(testfile)
-    
-    templ = kmc3.ExperimentTemplate
-    
-    setupGen = xd.SetupGenerator(templ)
-    setup = setupGen(h5like)
-
-    for i in templ:
-        assert i in setup
-
-    for i in setup:
-        assert i in templ
-
-    # Test setting of values fpr keys that already exist.
-    ev = random.random()*1000
-    assert xd.SetupGenerator(templ, beamEnergy=ev)(h5like)['beamEnergy'] == ev
-
-    # Test that keys not in template are rejected
-    with pytest.raises(KeyError):
-        xd.SetupGenerator(templ, jinkies=ev)
-    
-    #print("Experiment template:")
-    #pprint(templ)
-    #print("Experiment definition:")
-    #pprint(setup)
+#def test_experimentsetup(testfile):
+#
+#    h5like = kmc3.SpecTiffH5(testfile)
+#    
+#    templ = kmc3.ExperimentTemplate
+#    
+#    setupGen = xd.SetupGenerator(templ)
+#    setup = setupGen(h5like)
+#
+#    for i in templ:
+#        assert i in setup
+#
+#    for i in setup:
+#        assert i in templ
+
+#    # Test setting of values fpr keys that already exist.
+#    ev = random.random()*1000
+#    assert xd.SetupGenerator(templ, beamEnergy=ev)(h5like)['beamEnergy'] == ev
+#
+#    # Test that keys not in template are rejected
+#    with pytest.raises(KeyError):
+#        xd.SetupGenerator(templ, jinkies=ev)
+#    
+#    #print("Experiment template:")
+#    #pprint(templ)
+#    #print("Experiment definition:")
+#    #pprint(setup)
```

