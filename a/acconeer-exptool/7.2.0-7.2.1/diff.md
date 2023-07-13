# Comparing `tmp/acconeer-exptool-7.2.0.tar.gz` & `tmp/acconeer-exptool-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-7.2.0.tar", last modified: Tue Jul  4 08:42:24 2023, max compression
+gzip compressed data, was "acconeer-exptool-7.2.1.tar", last modified: Thu Jul 13 09:11:02 2023, max compression
```

## Comparing `acconeer-exptool-7.2.0.tar` & `acconeer-exptool-7.2.1.tar`

### file list

```diff
@@ -1,624 +1,625 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15293 2023-07-04 08:38:59.000000 acconeer-exptool-7.2.0/CHANGELOG.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2023-07-04 08:38:59.000000 acconeer-exptool-7.2.0/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/docker/requirements-dev.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/bilateration/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/distance/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/distance/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 14:12:33.000000 acconeer-exptool-7.2.0/examples/a121/phase_tracking/phase_tracking.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/presence/detector.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/examples/a121/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/examples/a121/record_data/with_cli.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/smart_presence/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/smart_presence/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17513 2023-07-03 11:33:15.000000 acconeer-exptool-7.2.0/examples/a121/smart_presence/ref_app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/speed/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9030 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/examples/a121/speed/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9179 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/examples/a121/speed/processor.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/stress.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/surface_velocity/example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/touchless_button/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/examples/a121/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/gui/main.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6585 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/portable/package/update.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2361 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/pyproject.toml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.335974 acconeer-exptool-7.2.0/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.343974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.347974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.351974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1207 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:37:09.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22075 2023-06-20 09:52:28.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10223 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11481 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.355974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6983 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15557 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11180 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18924 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-31 21:00:04.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7945 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      720 2023-06-15 10:34:10.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8056 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10729 2023-06-15 10:34:10.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:47:51.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24992 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20031 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8542 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31517 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6541 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.359974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59450 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26179 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      235 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2856 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15804 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30047 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8375 2023-06-30 09:00:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18184 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    32608 2023-06-30 09:00:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10926 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      347 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14635 2023-06-30 13:44:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21150 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4909 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_processors.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-23 09:13:41.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29464 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:15:54.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:17:58.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-07-03 12:37:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-07-03 13:15:15.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.363974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/__main__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      909 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27095 2023-06-21 08:08:07.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_tasks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1685 2023-07-03 10:00:04.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      445 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 08:17:48.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/icons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3910 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/main_window.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.367974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      798 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7130 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6271 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6159 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:59.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3612 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27081 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      227 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1757 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6112 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13043 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6682 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3848 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4912 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12509 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84005 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/modules.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.339974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.371974 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5843 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3629 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-21 06:44:46.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.0/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26313 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-04 08:42:23.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-07-04 08:42:24.000000 acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-06-22 13:14:00.000000 acconeer-exptool-7.2.0/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_permissions.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.0/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.0/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-04 08:42:24.375974 acconeer-exptool-7.2.0/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14763 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.0/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.632808 acconeer-exptool-7.2.1/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      389 2023-07-06 12:50:36.000000 acconeer-exptool-7.2.1/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15362 2023-07-13 07:59:26.000000 acconeer-exptool-7.2.1/CHANGELOG.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.1/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9113 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/PKG-INFO
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8071 2023-07-11 09:58:01.000000 acconeer-exptool-7.2.1/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       86 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/docker/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.632808 acconeer-exptool-7.2.1/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/bilateration/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/distance/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/distance/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 14:12:33.000000 acconeer-exptool-7.2.1/examples/a121/phase_tracking/phase_tracking.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/presence/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/examples/a121/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/examples/a121/record_data/with_cli.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/smart_presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/smart_presence/processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17513 2023-07-03 11:33:15.000000 acconeer-exptool-7.2.1/examples/a121/smart_presence/ref_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9030 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.1/examples/a121/speed/detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9179 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.1/examples/a121/speed/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/stress.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/surface_velocity/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.1/examples/a121/surface_velocity/example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:03.000000 acconeer-exptool-7.2.1/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/touchless_button/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/examples/a121/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.1/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/gui/main.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6629 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.640808 acconeer-exptool-7.2.1/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/portable/package/update.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2374 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/pyproject.toml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2456 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.636808 acconeer-exptool-7.2.1/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.632808 acconeer-exptool-7.2.1/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.644808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.648808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1207 2023-07-04 08:36:53.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.652808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:37:09.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22075 2023-06-20 09:52:28.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10223 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11481 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6983 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15557 2023-07-11 09:53:51.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:58.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11180 2023-07-03 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19022 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5134 2023-07-11 09:58:01.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7945 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.656808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      720 2023-06-15 10:34:10.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 12:37:45.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8056 2023-07-04 08:07:41.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      729 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8735 2023-07-11 12:19:57.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6475 2023-07-11 12:25:24.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10729 2023-07-07 10:27:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:47:51.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25002 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      303 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      759 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20493 2023-07-06 12:50:36.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8542 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31545 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    60027 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26209 2023-07-13 07:59:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    31101 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7371 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      235 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2856 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15875 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30417 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18544 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8375 2023-06-30 09:00:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18350 2023-07-10 10:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    32205 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:20.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.660808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      347 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14635 2023-06-30 13:44:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21182 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4909 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_processors.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-23 09:13:41.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21976 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14256 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    29494 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-06-27 15:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:15:54.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-07-07 10:27:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7830 2023-07-07 10:27:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      909 2023-07-11 11:38:13.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27149 2023-07-11 13:00:20.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2042 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_tasks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1685 2023-07-07 13:36:32.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.664808 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      445 2023-07-11 11:38:13.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14151 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4638 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15066 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 07:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2142 2023-06-13 09:45:17.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/icons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3952 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1994 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      798 2023-07-11 11:38:13.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7147 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1358 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6393 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6213 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:59.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3677 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      764 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3729 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2062 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27557 2023-07-11 12:25:24.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2022 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      227 2023-06-13 21:00:27.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1775 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6112 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4004 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13043 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6749 2023-07-11 12:19:57.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7965 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-07-11 12:21:30.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 07:00:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4025 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9284 2023-07-11 12:19:57.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:26:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10439 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4912 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12638 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4721 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2572 2023-07-11 09:37:15.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1410 2023-07-11 11:38:13.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84005 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.668809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:12.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/modules.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-15 14:29:42.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.636808 acconeer-exptool-7.2.1/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5843 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3629 2023-06-20 13:22:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 13:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.672809 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-21 06:44:46.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-27 07:25:26.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/mpl_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      206 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1411 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/api.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11251 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/builtin_persistors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11793 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/core.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13019 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/optimizing_persistors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3536 2023-07-05 12:00:03.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/opser/registry_persistor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 13:05:40.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-07-07 14:42:52.000000 acconeer-exptool-7.2.1/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9113 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    26200 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      497 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-07-13 09:11:02.000000 acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3930 2023-06-22 13:14:00.000000 acconeer-exptool-7.2.1/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/tools/check_permissions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-09 21:08:02.000000 acconeer-exptool-7.2.1/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 09:58:23.000000 acconeer-exptool-7.2.1/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-07-13 09:11:02.676808 acconeer-exptool-7.2.1/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14763 2023-06-30 11:48:25.000000 acconeer-exptool-7.2.1/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-7.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/CHANGELOG.md` & `acconeer-exptool-7.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## v7.2.1
+
+This release only contains minor fixes and improvements.
+
 ## v7.2.0
 
 ### Added
 - A121: Smart presence: Add wake up mode
 - A121: Client now raises an error if no sensors can be detected
         on the server.
 - Documentation for the speed detector
```

### Comparing `acconeer-exptool-7.2.0/Jenkinsfile` & `acconeer-exptool-7.2.1/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/LICENSE.md` & `acconeer-exptool-7.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/PKG-INFO` & `acconeer-exptool-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.2.0
+Version: 7.2.1
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
@@ -65,14 +65,15 @@
 ## News
 
 * v6.0.0 released. See the [Changelog](https://docs.acconeer.com/en/latest/changelog.html).
 
 ## Setting up your evaluation kit
 
 * [XC120 + XE121 (A121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xc120_xe121.html)
+* [Raspberry Pi (A121 on XE121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a121_xe121.html)
 * [Raspberry Pi (A111 on XC111+XR111 or XC112+XR112)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a111.html)
 * [XM112](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm112.html)
 * [XM122](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm122.html)
 * [XM132](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm132.html)
 
 For additional resources, head over to the [Acconeer developer page](https://developer.acconeer.com/). There you will find both a getting started guide and a video showing you how to set up your evaluation kit. There you will also find the SDK download.
```

### Comparing `acconeer-exptool-7.2.0/README.md` & `acconeer-exptool-7.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 ## News
 
 * v6.0.0 released. See the [Changelog](https://docs.acconeer.com/en/latest/changelog.html).
 
 ## Setting up your evaluation kit
 
 * [XC120 + XE121 (A121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xc120_xe121.html)
+* [Raspberry Pi (A121 on XE121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a121_xe121.html)
 * [Raspberry Pi (A111 on XC111+XR111 or XC112+XR112)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a111.html)
 * [XM112](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm112.html)
 * [XM122](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm122.html)
 * [XM132](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm132.html)
 
 For additional resources, head over to the [Acconeer developer page](https://developer.acconeer.com/). There you will find both a getting started guide and a video showing you how to set up your evaluation kit. There you will also find the SDK download.
```

### Comparing `acconeer-exptool-7.2.0/docker/Dockerfile` & `acconeer-exptool-7.2.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/dodo.py` & `acconeer-exptool-7.2.1/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/basic.py` & `acconeer-exptool-7.2.1/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/basic_continuous.py` & `acconeer-exptool-7.2.1/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/load_record.py` & `acconeer-exptool-7.2.1/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/load_record_h5.m` & `acconeer-exptool-7.2.1/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.2.1/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.2.1/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.2.1/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.2.1/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.2.1/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/services/envelope.py` & `acconeer-exptool-7.2.1/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/services/iq.py` & `acconeer-exptool-7.2.1/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/services/power_bins.py` & `acconeer-exptool-7.2.1/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/services/sparse.py` & `acconeer-exptool-7.2.1/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/utils/ping.py` & `acconeer-exptool-7.2.1/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.2.1/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/basic.py` & `acconeer-exptool-7.2.1/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-7.2.1/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/distance/detector.py` & `acconeer-exptool-7.2.1/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/distance/processor.py` & `acconeer-exptool-7.2.1/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/extended_config.py` & `acconeer-exptool-7.2.1/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/load_record.py` & `acconeer-exptool-7.2.1/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/load_record_h5.m` & `acconeer-exptool-7.2.1/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.2.1/examples/a121/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/plot.py` & `acconeer-exptool-7.2.1/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/presence/detector.py` & `acconeer-exptool-7.2.1/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/presence/processor.py` & `acconeer-exptool-7.2.1/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.2.1/examples/a121/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.2.1/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.2.1/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/smart_presence/processor.py` & `acconeer-exptool-7.2.1/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-7.2.1/examples/a121/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/speed/detector.py` & `acconeer-exptool-7.2.1/examples/a121/speed/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/speed/processor.py` & `acconeer-exptool-7.2.1/examples/a121/speed/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/stress.py` & `acconeer-exptool-7.2.1/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/subsweeps.py` & `acconeer-exptool-7.2.1/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-7.2.1/examples/a121/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-7.2.1/examples/a121/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/touchless_button/processor.py` & `acconeer-exptool-7.2.1/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/examples/a121/vibration/vibration.py` & `acconeer-exptool-7.2.1/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/gui/main.py` & `acconeer-exptool-7.2.1/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/noxfile.py` & `acconeer-exptool-7.2.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 nox.options.sessions = ["lint", "docs", f"test(python='{py_ver}')"]
 nox.options.stop_on_first_error = True
 nox.options.reuse_existing_virtualenvs = True
 
 
 BLACK_SPEC = "black==22.12.0"
 RUFF_SPEC = "ruff==0.0.270"
-MYPY_SPEC = "mypy==1.3.0"
+MYPY_SPEC = "mypy==1.4.1"
+PYSIDE_SPEC = "PySide6==6.4.3"
 PIP_SPEC = "pip>=21.3"
 PYTEST_MOCK_SPEC = "pytest-mock==3.3.1"
 PYTEST_SPEC = "pytest==7.2"
 PYTEST_XDIST_SPEC = "pytest-xdist==3.1.0"
 DIRTY_EQUALS_SPEC = "dirty-equals==0.5.0"
 
 SPHINX_SOURCE_DIR = "docs"
@@ -92,15 +93,15 @@
     session.run("python", "-m", "black", ".")
     session.run("python", "-m", "ruff", "--fix", ".")
 
 
 @nox.session
 @nox.parametrize("python", ["3.7"])
 def mypy(session):
-    session.install("-e", ".", MYPY_SPEC, PYTEST_SPEC)
+    session.install("-e", ".", MYPY_SPEC, PYTEST_SPEC, PYSIDE_SPEC)
     session.run("python", "-m", "mypy")
 
 
 @nox.session
 def docs(session):
     args = Parser().parse_args(session.posargs)
```

### Comparing `acconeer-exptool-7.2.0/portable/make.py` & `acconeer-exptool-7.2.1/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/portable/package/tools/update.py` & `acconeer-exptool-7.2.1/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/pyproject.toml` & `acconeer-exptool-7.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 "acconeer" = ["acconeer"]
 
 [tool.mypy]
 packages = [
     "acconeer.exptool.a121",
     "acconeer.exptool.app.new",
     "acconeer.exptool.setup",
+    "acconeer.exptool.opser",
     "tests.unit.a121",
     "tests.app",
 ]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
@@ -104,15 +105,14 @@
 module = [
     "dirty_equals.*",
     "h5py.*",
     "platformdirs.*",
     "psutil.*",
     "pyperclip.*",
     "pyqtgraph.*",
-    "PySide6.*",
     "pytest.*",
     "qdarktheme.*",
     "qtawesome.*",
     "requests.*",
     "scipy.*",
     "serial.*",
 ]
```

### Comparing `acconeer-exptool-7.2.0/setup.cfg` & `acconeer-exptool-7.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 	packaging
 	pyserial>=3.5
 	pyusb>=1.2.1
 	pyyaml
 	requests>=2.0,<3
 	typing-extensions>=4,<5
 	textual==0.1.18
+	exceptiongroup==1.1.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 algo = 
 	scipy
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/mediators/recorder.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/mediators/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -331,23 +331,23 @@
 
     def start_session(self) -> None:
         self._assert_session_setup()
 
         if self.session_is_started:
             raise ClientError("Session is already started.")
 
-        self._recorder_start_session()
-        self._session_is_started = True
-
         self._link.timeout = self._link_timeout
         _ = self._send_command_and_wait_for_response(
             self._protocol.start_streaming_command(),
             messages.StartStreamingResponse,
         )
 
+        self._recorder_start_session()
+        self._session_is_started = True
+
     def get_next(self) -> Union[Result, list[dict[int, Result]]]:
         self._assert_session_started()
 
         result_message = self._wait_for_response(messages.ResultMessage)
 
         if self._metadata is None:
             raise RuntimeError(f"{self} has no metadata")
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,15 +538,15 @@
 
 
 def indent_strs(strs: list[str], level: int) -> list[str]:
     return ["  " * level + s for s in strs]
 
 
 def ndarray_isclose(a: npt.ArrayLike, b: npt.ArrayLike) -> bool:
-    return bool(np.isclose(a, b).all())
+    return bool(np.isclose(a, b, equal_nan=True).all())
 
 
 def _dict_wrapper(f: Callable[[S, T], bool]) -> Callable[[dict[U, S], dict[U, T]], bool]:
     def wrapper(a: dict[U, S], b: dict[U, T]) -> bool:
         if a.keys() != b.keys():
             return False
 
@@ -566,14 +566,15 @@
         else:
             return f(a, b)
 
     return wrapper
 
 
 attrs_ndarray_eq = attrs.cmp_using(eq=np.array_equal)
+attrs_optional_ndarray_eq = attrs.cmp_using(eq=_optional_wrapper(np.array_equal))
 attrs_ndarray_isclose = attrs.cmp_using(eq=ndarray_isclose)
 attrs_optional_ndarray_isclose = attrs.cmp_using(eq=_optional_wrapper(ndarray_isclose))
 attrs_dict_ndarray_isclose = attrs.cmp_using(eq=_dict_wrapper(ndarray_isclose))
 
 
 def no_dynamic_member_creation(cls: Type[T]) -> Type[T]:
     """
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,27 +24,35 @@
 
 
 class _StopReplay(Exception):
     pass
 
 
 class _ReplayingClient(Client):
-    def __init__(self, record: Record, *, cycled_session_idx: Optional[int] = None):
+    def __init__(
+        self,
+        record: Record,
+        *,
+        cycled_session_idx: Optional[int] = None,
+        realtime_replay: bool = True,
+    ):
         """
         :param record: The Record to replay from
         :param cycled_session_idx:
             If specified, cycle (reuse as next session) the session
             specified by 'cycled_session_idx'.
+        :param realtime_replay: If True, replays the data at the rate of recording
         """
         self._record = record
         self._is_started: bool = False
         self._result_iterator: Iterator[list[dict[int, Result]]] = iter([])
         self._origin_time: Optional[float] = None
         self._session_idx = 0
         self._cycled_session_idx = cycled_session_idx
+        self._realtime_replay = realtime_replay
 
     @property
     def _actual_session_idx(self) -> int:
         if self._cycled_session_idx is not None:
             return self._cycled_session_idx
         else:
             return self._session_idx
@@ -96,23 +104,24 @@
         try:
             result = next(self._result_iterator)
         except StopIteration:
             raise _StopReplay
 
         some_result = next(core_utils.iterate_extended_structure_values(result))
 
-        now = time.monotonic() - some_result.tick_time
+        if self._realtime_replay:
+            now = time.monotonic() - some_result.tick_time
 
-        if self._origin_time is None:
-            self._origin_time = now
+            if self._origin_time is None:
+                self._origin_time = now
 
-        delta = now - self._origin_time
+            delta = now - self._origin_time
 
-        if delta < 0:
-            time.sleep(-delta)
+            if delta < 0:
+                time.sleep(-delta)
 
         if self.session_config.extended:
             return result
         else:
             return core_utils.unextend(result)
 
     def stop_session(self) -> Any:
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from acconeer.exptool.app.new import (
     BackendLogger,
     GeneralMessage,
     Message,
     PluginGeneration,
     is_task,
 )
+from acconeer.exptool.app.new.backend import StatusMessage
 
 
 CALIBRATION_NEEDED_MESSAGE = "Calibration needed - restart"
 DATA_SATURATED_MESSAGE = "Data saturated - reduce gain"
 FRAME_DELAYED_MESSAGE = "Frame delayed"
 
 
@@ -104,18 +105,28 @@
         )
         _create_h5_string_dataset(
             file, "processor_config", self.shared_state.processor_config.to_json()
         )
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         self.shared_state.session_config = record.session_config
-        algo_group = record.get_algo_group(self.key)  # noqa: F841
-        self.shared_state.processor_config = self.get_processor_config_cls().from_json(
-            algo_group["processor_config"][()]
-        )
+        try:
+            algo_group = record.get_algo_group(self.key)  # noqa: F841
+        except KeyError:
+            self.shared_state.processor_config = self.get_processor_config_cls()()
+            self.callback(
+                StatusMessage(
+                    status="Could not load algo group. "
+                    + "Falling back to default processor config"
+                )
+            )
+        else:
+            self.shared_state.processor_config = self.get_processor_config_cls().from_json(
+                algo_group["processor_config"][()]
+            )
 
     @is_task
     def update_session_config(self, *, session_config: a121.SessionConfig) -> None:
         self.shared_state.session_config = session_config
         self.broadcast()
 
     @is_task
@@ -188,15 +199,15 @@
     @classmethod
     @abc.abstractmethod
     def get_default_sensor_config(cls) -> a121.SensorConfig:
         pass
 
     @staticmethod
     def _format_warning(s: str) -> str:
-        return f'<p style="color: #FD5200;"><b>Warning: {s}</b></p>'
+        return f'<b style="color: #FD5200;">Warning: {s}</b>'
 
 
 class ProcessorBackendPluginBase(
     GenericProcessorBackendPluginBase[a121.Result, ProcessorConfigT, ResultT, a121.Metadata]
 ):
     def _validate_session_config(self, session_config: a121.SessionConfig) -> None:
         if session_config.extended:
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,26 @@
         backend_plugin_state: Optional[
             ProcessorBackendPluginSharedState[ProcessorConfigT, a121.Metadata]
         ],
     ) -> None:
         if backend_plugin_state is None:
             self.session_config_editor.set_data(None)
             self.processor_config_editor.set_data(None)
-            self.metadata_view.update(None)
-            self.perf_calc_view.update()
+            self.metadata_view.set_data(None)
+            self.perf_calc_view.set_data()
         else:
             assert isinstance(backend_plugin_state, ProcessorBackendPluginSharedState)
             assert isinstance(
                 backend_plugin_state.processor_config, self.get_processor_config_cls()
             )
 
             self.session_config_editor.set_data(backend_plugin_state.session_config)
             self.processor_config_editor.set_data(backend_plugin_state.processor_config)
-            self.metadata_view.update(backend_plugin_state.metadata)
-            self.perf_calc_view.update(
+            self.metadata_view.set_data(backend_plugin_state.metadata)
+            self.perf_calc_view.set_data(
                 backend_plugin_state.session_config,
                 backend_plugin_state.metadata,
             )
 
             if backend_plugin_state.processor_config is not None:
                 results = (
                     backend_plugin_state.processor_config._collect_validation_results(
@@ -143,19 +143,15 @@
             app_model.is_ready_for_session()
             and app_model.backend_plugin_state is not None
             and app_model.backend_plugin_state.ready
             and self.session_config_editor.is_ready
             and self.processor_config_editor.is_ready
         )
 
-        if app_model.backend_plugin_state:
-            self.session_config_editor.set_selected_sensor(
-                app_model.backend_plugin_state.session_config.sensor_id,
-                self.app_model.connected_sensors,
-            )
+        self.session_config_editor.set_selectable_sensors(self.app_model.connected_sensors)
 
     @classmethod
     def supports_multiple_subsweeps(self) -> bool:
         return False
 
     @classmethod
     @abc.abstractmethod
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/_utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,32 +554,31 @@
             self.stop_button.setEnabled(False)
             self.defaults_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
             self.bilateration_config_editor.set_data(None)
             self.bilateration_config_editor.setEnabled(False)
-            self.two_sensor_id_editor.set_selected_sensors(None, [])
+            self.two_sensor_id_editor.setEnabled(False)
             self.message_box.setText("")
 
             return
 
         assert isinstance(state, SharedState)
 
         self.defaults_button.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
         self.bilateration_config_editor.setEnabled(
             app_model.plugin_state == PluginState.LOADED_IDLE
         )
         self.bilateration_config_editor.set_data(state.bilateration_config)
-        self.two_sensor_id_editor.set_selected_sensors(
-            state.sensor_ids, app_model.connected_sensors
-        )
+        self.two_sensor_id_editor.set_selectable_sensors(app_model.connected_sensors)
+        self.two_sensor_id_editor.set_data(state.sensor_ids)
         self.two_sensor_id_editor.setEnabled(app_model.plugin_state.is_steady)
 
         detector_status = Detector.get_detector_status(
             state.config, state.context, state.sensor_ids
         )
 
         self.message_box.setText(self.TEXT_MSG_MAP[detector_status.detector_state])
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 from scipy.signal import butter
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import (
     ENVELOPE_FWHM_M,
     AlgoParamEnum,
     AlgoProcessorConfigBase,
     ProcessorBase,
     exponential_smoothing_coefficient,
 )
@@ -67,20 +68,22 @@
             )
 
         return validation_results
 
 
 @attrs.frozen(kw_only=True)
 class BreathingProcessorExtraResult:
-    psd: npt.NDArray[np.float_]
-    frequencies: npt.NDArray[np.float_]
-    breathing_motion: npt.NDArray[np.float_]
-    time_vector: npt.NDArray[np.float_]
-    breathing_rate_history: npt.NDArray[np.float_]
-    all_breathing_rate_history: npt.NDArray[np.float_]
+    psd: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    frequencies: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    breathing_motion: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    time_vector: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    breathing_rate_history: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    all_breathing_rate_history: npt.NDArray[np.float_] = attrs.field(
+        eq=utils.attrs_ndarray_isclose
+    )
 
 
 @attrs.mutable(kw_only=True)
 class BreathingProcessorResult:
     breathing_rate: Optional[float] = attrs.field(default=None)
     """Estimated breathing rate. Breaths per minute."""
 
@@ -123,14 +126,15 @@
         lowest_breathing_rate_hz = processor_config.lowest_breathing_rate / self.SECONDS_IN_MINUTE
         highest_breathing_rate_hz = (
             processor_config.highest_breathing_rate / self.SECONDS_IN_MINUTE
         )
         self.frame_rate = sensor_config.frame_rate
         self.time_series_length_s = processor_config.time_series_length_s
         self.time_series_length = int(self.time_series_length_s * self.frame_rate)
+        self.padded_time_series_length = 2 ** (int(np.log2(self.time_series_length)) + 1)
         self.analysis_overlap = int(self.time_series_length / 2)
         self.num_points = sensor_config.num_points
 
         # Filter coefficients.
         self.b_static, self.a_static = butter(
             N=2, Wn=lowest_breathing_rate_hz, btype="lowpass", fs=self.frame_rate
         )
@@ -139,15 +143,15 @@
             Wn=[lowest_breathing_rate_hz, highest_breathing_rate_hz],
             btype="bandpass",
             fs=self.frame_rate,
         )
         self.sf = exponential_smoothing_coefficient(self.frame_rate, self.time_series_length_s)
 
         # PSD frequency vector.
-        self.frequencies = np.fft.rfftfreq(self.time_series_length, 1 / self.frame_rate)
+        self.frequencies = np.fft.rfftfreq(self.padded_time_series_length, 1 / self.frame_rate)
         self.time_vector = np.linspace(-self.HISTORY_S, 0, int(self.frame_rate * self.HISTORY_S))
 
         self.reinitialize_processor(0, self.num_points)
 
     def process(self, result: a121.Result) -> BreathingProcessorResult:
         frame = result.frame[:, self.start_point : self.end_point]
         mean_sweep = frame.mean(axis=0)
@@ -195,15 +199,17 @@
         self.breathing_motion_buffer = np.roll(self.breathing_motion_buffer, shift=-1, axis=0)
         self.breathing_motion_buffer[-1] = filt_angle
 
         # Calculate psd of signal.
         windowed_breathing_motion_buffer = (
             self.breathing_motion_buffer * np.hamming(self.time_series_length)[:, np.newaxis]
         )
-        psd = np.fft.rfft(windowed_breathing_motion_buffer, axis=0, n=self.time_series_length)
+        psd = np.fft.rfft(
+            windowed_breathing_motion_buffer, axis=0, n=self.padded_time_series_length
+        )
         # Omit **2 to reduce processing as it does not alter the result.
         psd = np.abs(psd)
         assert self.lp_filt_ampl is not None
         psd_weighted = np.sum(psd * self.lp_filt_ampl, axis=1) / np.sum(self.lp_filt_ampl)
 
         # Interpolate around peak to gain better resolution.
         # Wait until data of a full time series is available.
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_ref_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 
 @attrs.frozen(kw_only=True)
 class RefAppResult:
     app_state: AppState
     """Application state."""
 
-    distances_being_analyzed: Optional[tuple[int, int]] = None
+    distances_being_analyzed: Optional[Tuple[int, int]] = None
     """Range where breathing is being analyzed."""
 
     presence_result: PresenceProcessorResult
     """Presence processor result."""
 
     breathing_result: Optional[BreathingProcessorResult] = attrs.field(default=None)
     """Breathing processor result."""
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         self.blue_transparent_pen = pg.mkPen(f"{blue_color}50", width=2)
         self.orange_transparent_pen = pg.mkPen(f"{orange_color}50", width=2)
 
         brush_dot = et.utils.pg_brush_cycler(1)
         symbol_dot_kw = dict(symbol="o", symbolSize=10, symbolBrush=brush_dot, symbolPen="k")
 
         font = QFont()
-        font.setPixelSize(16.0)
+        font.setPixelSize(16)
 
         # Presence plot.
         self.presence_plot = win.addPlot(row=0, col=0)
         self.presence_plot.setMenuEnabled(False)
         self.presence_plot.showGrid(x=True, y=True)
         self.presence_plot.addLegend()
         self.presence_plot.setLabel("left", "Presence score")
@@ -692,15 +692,15 @@
             self.config_editor.setEnabled(False)
             self.sensor_config_editor.set_data(None)
             self.sensor_config_editor.setEnabled(False)
             self.breathing_config_editor.set_data(None)
             self.breathing_config_editor.setEnabled(False)
             self.presence_config_editor.set_data(None)
             self.presence_config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.sensor_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
@@ -708,15 +708,16 @@
         self.presence_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
         self.config_editor.set_data(state.config)
         self.sensor_config_editor.set_data(state.config)
         self.breathing_config_editor.set_data(state.config.breathing_config)
         self.presence_config_editor.set_data(state.config.presence_config)
 
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,32 +96,46 @@
                 context_dict[sensor_id] = SingleSensorContext.from_h5(group[key])
 
         return DetectorContext(single_sensor_contexts=context_dict)
 
 
 @attrs.mutable(kw_only=True)
 class SingleSensorExtraContext(AlgoBase):
-    offset_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(default=None)
-    noise_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(default=None)
-    close_range_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(default=None)
+    offset_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    noise_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    close_range_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     recorded_threshold_frames: Optional[List[List[npt.NDArray[np.complex_]]]] = attrs.field(
-        default=None
+        default=None, eq=utils.attrs_optional_ndarray_isclose
     )
 
 
 @attrs.mutable(kw_only=True)
 class SingleSensorContext(AlgoBase):
     loopback_peak_location_m: Optional[float] = attrs.field(default=None)
-    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(default=None)
-    phase_jitter_comp_reference: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    phase_jitter_comp_reference: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     recorded_thresholds_mean_sweep: Optional[List[npt.NDArray[np.float_]]] = attrs.field(
-        default=None
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    recorded_thresholds_noise_std: Optional[List[List[np.float_]]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    bg_noise_std: Optional[List[List[float]]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
     )
-    recorded_thresholds_noise_std: Optional[List[List[np.float_]]] = attrs.field(default=None)
-    bg_noise_std: Optional[List[List[float]]] = attrs.field(default=None)
     session_config_used_during_calibration: Optional[a121.SessionConfig] = attrs.field(
         default=None
     )
     reference_temperature: Optional[int] = attrs.field(default=None)
     sensor_calibration: Optional[a121.SensorCalibration] = attrs.field(default=None)
     extra_context: SingleSensorExtraContext = attrs.field(factory=SingleSensorExtraContext)
     # TODO: Make recorded_thresholds Optional[List[Optional[npt.NDArray[np.float_]]]]
@@ -383,18 +397,22 @@
             )
 
         return validation_results
 
 
 @attrs.frozen(kw_only=True)
 class DetectorResult:
-    distances: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    distances: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     """Estimated distances (m), sorted according to the selected peak sorting strategy."""
 
-    strengths: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    strengths: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     """Estimated reflector strengths corresponding to the peak amplitude of the estimated
     distances.
     """
 
     near_edge_status: Optional[bool] = attrs.field(default=None)
     """Boolean indicating an object close to the start edge, located outside of the
     measurement range.
@@ -409,18 +427,18 @@
     """
 
     temperature: Optional[int] = attrs.field(default=None)
     """Temperature in sensor during measurement (in degree Celsius). Notice that this has poor
     absolute accuracy.
     """
 
-    processor_results: list[ProcessorResult] = attrs.field()
+    processor_results: List[ProcessorResult] = attrs.field()
     """Processing result. Used for visualization in Exploration Tool."""
 
-    service_extended_result: list[dict[int, a121.Result]] = attrs.field()
+    service_extended_result: List[Dict[int, a121.Result]] = attrs.field()
     """Service extended result. Used for visualization in Exploration Tool."""
 
 
 class Detector(Controller[DetectorConfig, Dict[int, DetectorResult]]):
     """Distance detector
     :param client: Client
     :param sensor_id: Sensor id
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,15 +506,15 @@
             self.start_button.setEnabled(False)
             self.calibrate_detector_button.setEnabled(False)
             self.stop_button.setEnabled(False)
             self.defaults_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
             self.message_box.setText("")
 
             return
 
         assert isinstance(state, SharedState)
 
         try:
@@ -540,15 +540,16 @@
 
         self.defaults_button.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
 
         (sensor_id,) = state.sensor_ids
-        self.sensor_id_pidget.set_selected_sensor(sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         detector_status = Detector.get_detector_status(
             state.config, state.context, state.sensor_ids
         )
 
         self.message_box.setText(self.TEXT_MSG_MAP[detector_status.detector_state])
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 from scipy.signal import filtfilt
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import (
     APPROX_BASE_STEP_LENGTH_M,
     ENVELOPE_FWHM_M,
     AlgoParamEnum,
     AlgoProcessorConfigBase,
     ProcessorBase,
     find_peaks,
@@ -90,43 +91,65 @@
         self, config: Optional[a121.SessionConfig]
     ) -> list[a121.ValidationResult]:
         return []
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorContext:
-    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(default=None)
-    phase_jitter_comp_ref: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    recorded_threshold_mean_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    recorded_threshold_noise_std: Optional[List[np.float_]] = attrs.field(default=None)
+    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    phase_jitter_comp_ref: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    recorded_threshold_mean_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    recorded_threshold_noise_std: Optional[List[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     bg_noise_std: Optional[List[float]] = attrs.field(default=None)
     reference_temperature: Optional[int] = attrs.field(default=None)
     loopback_peak_location_m: Optional[float] = attrs.field(default=None)
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorExtraResult:
     """
     Contains information for visualization in ET.
     """
 
-    abs_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    used_threshold: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    distances_m: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    abs_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    used_threshold: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    distances_m: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
-    estimated_distances: Optional[list[float]] = attrs.field(default=None)
-    estimated_strengths: Optional[list[float]] = attrs.field(default=None)
+    estimated_distances: Optional[List[float]] = attrs.field(default=None)
+    estimated_strengths: Optional[List[float]] = attrs.field(default=None)
     near_edge_status: Optional[bool] = attrs.field(default=None)
-    recorded_threshold_mean_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    recorded_threshold_noise_std: Optional[list[np.float_]] = attrs.field(default=None)
-    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(default=None)
-    phase_jitter_comp_reference: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
+    recorded_threshold_mean_sweep: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    recorded_threshold_noise_std: Optional[List[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    direct_leakage: Optional[npt.NDArray[np.complex_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    phase_jitter_comp_reference: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
     extra_result: ProcessorExtraResult = attrs.field(factory=ProcessorExtraResult)
 
 
 class Processor(ProcessorBase[ProcessorConfig, ProcessorResult]):
     """Distance processor
 
     For all used subsweeps, the ``profile`` and ``step_length`` must be the same.
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import PERCEIVED_WAVELENGTH, AlgoProcessorConfigBase, ProcessorBase
 
 
 @attrs.mutable(kw_only=True)
 class ProcessorConfig(AlgoProcessorConfigBase):
     threshold: Optional[float] = attrs.field(default=25.0)
 
@@ -55,19 +56,19 @@
 @attrs.frozen(kw_only=True)
 class ProcessorContext:
     ...
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
-    lp_abs_sweep: npt.NDArray[np.float_]
-    angle_sweep: npt.NDArray[np.float_]
+    lp_abs_sweep: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    angle_sweep: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     threshold: Optional[float] = attrs.field(default=None)
-    rel_time_stamps: npt.NDArray[np.float_]
-    distance_history: npt.NDArray[np.float_]
+    rel_time_stamps: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    distance_history: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     peak_loc_m: Optional[float] = attrs.field(default=None)
 
 
 class Processor(ProcessorBase[ProcessorConfig, ProcessorResult]):
     estimated_distance: Optional[float]
     prev_peak_loc_m: Optional[float]
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import attrs
 import h5py
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core.entities.configs.config_enums import IdleState, Profile
-from acconeer.exptool.a121._core.utils import is_divisor_of, is_multiple_of
+from acconeer.exptool.a121._core.utils import attrs_ndarray_isclose, is_divisor_of, is_multiple_of
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo import (
     ENVELOPE_FWHM_M,
     AlgoBase,
     AlgoConfigBase,
     Controller,
     select_prf,
@@ -191,21 +191,21 @@
 
 
 @attrs.frozen(kw_only=True)
 class DetectorResult:
     intra_presence_score: float = attrs.field()
     """A measure of the amount of fast motion detected."""
 
-    intra_depthwise_scores: npt.NDArray[np.float_] = attrs.field()
+    intra_depthwise_scores: npt.NDArray[np.float_] = attrs.field(eq=attrs_ndarray_isclose)
     """The depthwise presence scores for fast motions."""
 
     inter_presence_score: float = attrs.field()
     """A measure of the amount of slow motion detected."""
 
-    inter_depthwise_scores: npt.NDArray[np.float_] = attrs.field()
+    inter_depthwise_scores: npt.NDArray[np.float_] = attrs.field(eq=attrs_ndarray_isclose)
     """The depthwise presence scores for slow motions."""
 
     presence_distance: float = attrs.field()
     """The distance, in meters, to the detected object."""
 
     presence_detected: bool = attrs.field()
     """True if presence was detected, False otherwise."""
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     PluginSpecBase,
     PluginState,
     icons,
     is_task,
     pidgets,
 )
 from acconeer.exptool.app.new.ui.plugin_components.pidgets.hooks import disable_if, parameter_is
+from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 from acconeer.exptool.app.new.ui.plugin_components.save_dialog import PresentationType
 
 from ._configs import (
     get_long_range_config,
     get_low_power_config,
     get_medium_range_config,
     get_short_range_config,
@@ -292,15 +293,15 @@
         self.intra_hist_plot.setLabel("left", "Score")
         self.intra_hist_plot.setXRange(-self.history_length_s, 0)
         self.intra_history_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
         self.intra_hist_plot.setYRange(0, 10)
         if not self.detector_config.intra_enable:
             intra_color = et.utils.color_cycler(1)
             intra_color = f"{intra_color}50"
-            intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.DashLine)
+            intra_dashed_pen = pg.mkPen(intra_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine)
             intra_pen = pg.mkPen(intra_color, width=2)
         else:
             intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
             intra_pen = et.utils.pg_pen_cycler(1)
 
         self.intra_hist_curve = self.intra_hist_plot.plot(pen=intra_pen)
         limit_line = pg.InfiniteLine(angle=0, pen=intra_dashed_pen)
@@ -325,15 +326,15 @@
         self.inter_hist_plot.setLabel("left", "Score")
         self.inter_hist_plot.setXRange(-self.history_length_s, 0)
         self.inter_history_smooth_max = et.utils.SmoothMax(self.detector_config.frame_rate)
         self.inter_hist_plot.setYRange(0, 10)
         if not self.detector_config.inter_enable:
             inter_color = et.utils.color_cycler(0)
             inter_color = f"{inter_color}50"
-            inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.DashLine)
+            inter_dashed_pen = pg.mkPen(inter_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine)
             inter_pen = pg.mkPen(inter_color, width=2)
         else:
             inter_pen = et.utils.pg_pen_cycler(0)
             inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
 
         self.inter_hist_curve = self.inter_hist_plot.plot(pen=inter_pen)
         limit_line = pg.InfiniteLine(angle=0, pen=inter_dashed_pen)
@@ -453,14 +454,17 @@
         self.sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(
             parent=sensor_selection_group
         )
         self.sensor_id_pidget.sig_update.connect(self._on_sensor_id_update)
         sensor_selection_group.layout().addWidget(self.sensor_id_pidget)
         scrolly_layout.addWidget(sensor_selection_group)
 
+        self.range_helper = RangeHelpView()
+        scrolly_layout.addWidget(self.range_helper)
+
         self.config_editor = AttrsConfigEditor(
             title="Detector parameters",
             factory_mapping=self._get_pidget_mapping(),
             config_type=DetectorConfig,
             extra_presenter=_set_config_presenter,
             parent=self.scrolly_widget,
         )
@@ -616,32 +620,37 @@
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
             assert not_handled == []
 
+            self.range_helper.set_data(
+                Detector._get_sensor_config(backend_plugin_state.config).subsweep
+            )
+
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import attrs
 import numpy as np
 import numpy.typing as npt
 from numpy import cos, pi, sqrt, square
 from scipy.special import binom
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import AlgoProcessorConfigBase, ProcessorBase
 from acconeer.exptool.a121.algo._utils import get_distances_m
 
 
 @attrs.mutable(kw_only=True)
 class ProcessorConfig(AlgoProcessorConfigBase):
     intra_enable: bool = attrs.field(default=True)
@@ -74,28 +75,28 @@
 
 @attrs.frozen(kw_only=True)
 class ProcessorExtraResult:
     """
     Contains information for visualization in ET.
     """
 
-    frame: npt.NDArray[np.complex_] = attrs.field()
-    abs_mean_sweep: npt.NDArray[np.float_] = attrs.field()
-    fast_lp_mean_sweep: npt.NDArray[np.float_] = attrs.field()
-    slow_lp_mean_sweep: npt.NDArray[np.float_] = attrs.field()
-    lp_noise: npt.NDArray[np.float_] = attrs.field()
+    frame: npt.NDArray[np.complex_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    abs_mean_sweep: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    fast_lp_mean_sweep: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    slow_lp_mean_sweep: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    lp_noise: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     presence_distance_index: int = attrs.field()
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
     intra_presence_score: float = attrs.field()
-    intra: npt.NDArray[np.float_] = attrs.field()
+    intra: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     inter_presence_score: float = attrs.field()
-    inter: npt.NDArray[np.float_] = attrs.field()
+    inter: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     presence_distance: float = attrs.field()
     presence_detected: bool = attrs.field()
     extra_result: ProcessorExtraResult = attrs.field()
 
 
 class Processor(ProcessorBase[ProcessorConfig, ProcessorResult]):
     # lp(f): low pass (filtered)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import attrs
 import h5py
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121._core.entities.configs.config_enums import IdleState, Profile
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo._base import AlgoBase, AlgoBaseT
 from acconeer.exptool.a121.algo._utils import estimate_frame_rate
 from acconeer.exptool.a121.algo.presence._detector import (
     AlgoConfigBase,
     Controller,
@@ -119,39 +120,39 @@
             )
 
         return cls(**d)
 
 
 @attrs.frozen(kw_only=True)
 class RefAppResult:
-    zone_limits: npt.NDArray[np.float_] = attrs.field()
+    zone_limits: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     "The upper limit for each zone."
 
     presence_detected: bool = attrs.field()
     """True if presence was detected, False otherwise."""
 
     max_presence_zone: Optional[int] = attrs.field()
     """The zone for maximum presence score if presence detected, else None."""
 
-    total_zone_detections: npt.NDArray[np.int_] = attrs.field()
+    total_zone_detections: npt.NDArray[np.int_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     """Detection result for all zones."""
 
     inter_presence_score: float = attrs.field()
     """A measure of the amount of slow motion detected."""
 
-    inter_zone_detections: npt.NDArray[np.int_] = attrs.field()
+    inter_zone_detections: npt.NDArray[np.int_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     """Slow motion presence detection result for all zones."""
 
     max_inter_zone: Optional[int] = attrs.field()
     """The zone for maximum slow motion presence score if slow presence detected, else None."""
 
     intra_presence_score: float = attrs.field()
     """A measure of the amount of fast motion detected."""
 
-    intra_zone_detections: npt.NDArray[np.int_] = attrs.field()
+    intra_zone_detections: npt.NDArray[np.int_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     """Fast motion presence detection result for all zones."""
 
     max_intra_zone: Optional[int] = attrs.field()
     """The zone for maximum fast motion presence score if fast presence detecte, else None."""
 
     used_config: _Mode = attrs.field()
     """The configuration used for the measurement."""
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 import pyqtgraph as pg
 
 import acconeer.exptool as et
 from acconeer.exptool import a121
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
-from acconeer.exptool.a121.algo._base import AlgoBase
 from acconeer.exptool.a121.algo._plugins import (
     DetectorBackendPluginBase,
     DetectorPlotPluginBase,
     DetectorViewPluginBase,
 )
 from acconeer.exptool.a121.algo.presence._detector import Detector
 from acconeer.exptool.a121.algo.presence._detector_plugin import ViewPlugin as PresenceViewPlugin
@@ -42,14 +41,15 @@
     PluginPresetBase,
     PluginSpecBase,
     PluginState,
     icons,
     is_task,
     pidgets,
 )
+from acconeer.exptool.app.new.ui.plugin_components.range_help_view import RangeHelpView
 
 from ._configs import (
     get_ceiling_config,
     get_long_range_config,
     get_low_power_config,
     get_medium_range_config,
     get_short_range_config,
@@ -63,23 +63,17 @@
     RefAppResult,
     _load_algo_data,
     _Mode,
 )
 
 
 @attrs.mutable(kw_only=True)
-class PlotConfig(AlgoBase):
-    show_all_detected_zones: bool = attrs.field(default=False)
-
-
-@attrs.mutable(kw_only=True)
 class SharedState:
     sensor_id: int = attrs.field(default=1)
     config: RefAppConfig = attrs.field(factory=RefAppConfig)
-    plot_config: PlotConfig = attrs.field(factory=PlotConfig)
     ref_app_context: Optional[RefAppContext] = attrs.field(default=None)
 
 
 class PluginPresetId(Enum):
     SHORT_RANGE = auto()
     MEDIUM_RANGE = auto()
     LONG_RANGE = auto()
@@ -106,34 +100,25 @@
         self._ref_app_instance: Optional[RefApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = RefAppConfig.from_json(file["config"][()])
-        self.shared_state.plot_config = PlotConfig.from_json(file["plot_config"][()])
-
-        show_all_detected_zones = self.shared_state.plot_config.show_all_detected_zones
-        self.shared_state.config.show_all_detected_zones = show_all_detected_zones
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState()
         self.broadcast()
 
     @is_task
     def update_sensor_id(self, *, sensor_id: int) -> None:
         self.shared_state.sensor_id = sensor_id
         self.broadcast()
 
-    @is_task
-    def update_plot_config(self, *, config: PlotConfig) -> None:
-        self.shared_state.plot_config = config
-        self.broadcast()
-
     def _sync_sensor_ids(self) -> None:
         if self.client is not None:
             sensor_ids = self.client.server_info.connected_sensors
 
             if len(sensor_ids) > 0 and self.shared_state.sensor_id not in sensor_ids:
                 self.shared_state.sensor_id = sensor_ids[0]
 
@@ -150,21 +135,19 @@
     @is_task
     def update_wake_up_config(self, *, config: PresenceWakeUpConfig) -> None:
         self.shared_state.config.wake_up_config = config
         self.broadcast()
 
     def save_to_cache(self, file: h5py.File) -> None:
         _create_h5_string_dataset(file, "config", self.shared_state.config.to_json())
-        _create_h5_string_dataset(file, "plot_config", self.shared_state.plot_config.to_json())
 
     @is_task
     def set_preset(self, preset_id: int) -> None:
         preset_config = self.PLUGIN_PRESETS[preset_id]
         self.shared_state.config = preset_config()
-        self.shared_state.plot_config = PlotConfig()
         self.broadcast()
 
     def load_from_record_setup(self, *, record: a121.H5Record) -> None:
         algo_group = record.get_algo_group(self.key)
         _, config, ref_app_context = _load_algo_data(algo_group)
         self.shared_state.config = config
         self.shared_state.ref_app_context = ref_app_context
@@ -196,15 +179,14 @@
         # self._ref_app_instance.ref_app_processor.zone_limits will always be for
         # wake_up_config if wake_up_mode is enabled
         self.callback(
             GeneralMessage(
                 name="setup",
                 kwargs=dict(
                     ref_app_config=self.shared_state.config,
-                    plot_config=self.shared_state.plot_config,
                     estimated_frame_rate=self._ref_app_instance.detector.estimated_frame_rate,
                     nominal_zone_limits=nominal_zone_limits,
                     wake_up_zone_limits=self._ref_app_instance.ref_app_processor.zone_limits,
                 ),
                 recipient="plot_plugin",
             )
         )
@@ -236,29 +218,29 @@
     def update_from_message(self, message: GeneralMessage) -> None:
         assert isinstance(message.data, RefAppResult)
         self.update(message.data)
 
     def setup(
         self,
         ref_app_config: RefAppConfig,
-        plot_config: PlotConfig,
         estimated_frame_rate: float,
         nominal_zone_limits: npt.NDArray[np.float_],
         wake_up_zone_limits: npt.NDArray[np.float_],
     ) -> None:
         self.ref_app_config = ref_app_config
         self.nominal_config = ref_app_config.nominal_config
         self.wake_up_config = ref_app_config.wake_up_config
 
-        self.show_all_detected_zones = plot_config.show_all_detected_zones
+        self.show_all_detected_zones = self.ref_app_config.show_all_detected_zones
 
         self.history_length_s = 5
         self.time_fifo: List[float] = []
         self.intra_fifo: List[float] = []
         self.inter_fifo: List[float] = []
+        self.switch_data: Optional[RefAppResult] = None
 
         win = self.plot_layout
 
         self.intra_limit_lines = []
         self.inter_limit_lines = []
 
         # Intra presence history plot
@@ -277,15 +259,15 @@
         self.intra_hist_plot.setXRange(-self.history_length_s, 0)
         self.intra_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
         self.intra_hist_plot.setYRange(0, 10)
         if not self.nominal_config.intra_enable:
             intra_color = et.utils.color_cycler(1)
             intra_color = f"{intra_color}50"
             self.nominal_intra_dashed_pen = pg.mkPen(
-                intra_color, width=2.5, style=QtCore.Qt.DashLine
+                intra_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine
             )
             self.nominal_intra_pen = pg.mkPen(intra_color, width=2)
         else:
             self.nominal_intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
             self.nominal_intra_pen = et.utils.pg_pen_cycler(1)
 
         self.intra_hist_curve = self.intra_hist_plot.plot(pen=self.nominal_intra_pen)
@@ -312,15 +294,15 @@
         self.inter_hist_plot.setXRange(-self.history_length_s, 0)
         self.inter_history_smooth_max = et.utils.SmoothMax(estimated_frame_rate)
         self.inter_hist_plot.setYRange(0, 10)
         if not self.nominal_config.inter_enable:
             inter_color = et.utils.color_cycler(0)
             inter_color = f"{inter_color}50"
             self.nominal_inter_dashed_pen = pg.mkPen(
-                inter_color, width=2.5, style=QtCore.Qt.DashLine
+                inter_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine
             )
             self.nominal_inter_pen = pg.mkPen(inter_color, width=2)
         else:
             self.nominal_inter_pen = et.utils.pg_pen_cycler(0)
             self.nominal_inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
 
         self.inter_hist_curve = self.inter_hist_plot.plot(pen=self.nominal_inter_pen)
@@ -376,26 +358,26 @@
             if self.wake_up_config.intra_enable:
                 self.wake_up_intra_dashed_pen = et.utils.pg_pen_cycler(1, width=2.5, style="--")
                 self.wake_up_intra_pen = et.utils.pg_pen_cycler(1)
             else:
                 intra_color = et.utils.color_cycler(1)
                 intra_color = f"{intra_color}50"
                 self.wake_up_intra_dashed_pen = pg.mkPen(
-                    intra_color, width=2.5, style=QtCore.Qt.DashLine
+                    intra_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine
                 )
                 self.wake_up_intra_pen = pg.mkPen(intra_color, width=2)
 
             if self.wake_up_config.inter_enable:
                 self.wake_up_inter_pen = et.utils.pg_pen_cycler(0)
                 self.wake_up_inter_dashed_pen = et.utils.pg_pen_cycler(0, width=2.5, style="--")
             else:
                 inter_color = et.utils.color_cycler(0)
                 inter_color = f"{inter_color}50"
                 self.wake_up_inter_dashed_pen = pg.mkPen(
-                    inter_color, width=2.5, style=QtCore.Qt.DashLine
+                    inter_color, width=2.5, style=QtCore.Qt.PenStyle.DashLine
                 )
                 self.wake_up_inter_pen = pg.mkPen(inter_color, width=2)
 
     @staticmethod
     def create_sector_plot(
         title: str, num_sectors: int, start_m: float, zone_limits: npt.NDArray[np.float_]
     ) -> Tuple[pg.PlotItem, List[pg.QtWidgets.QGraphicsEllipseItem]]:
@@ -559,15 +541,15 @@
 
             for sector in self.wake_up_sectors:
                 sector.setBrush(brush)
 
         if data.presence_detected:
             self.color_zones(data, show_all_zones, sectors)
             self.switch_data = data
-        elif data.switch_delay:
+        elif data.switch_delay and self.switch_data is not None:
             self.color_zones(self.switch_data, True, self.wake_up_sectors[1:])
 
         self.nominal_sectors[0].setPen(pg.mkPen(color_nominal, width=1))
         self.nominal_sectors[0].setBrush(pg.mkBrush(color_nominal))
 
         if self.ref_app_config.wake_up_mode:
             self.wake_up_sectors[0].setPen(pg.mkPen(color_wake_up, width=1))
@@ -639,54 +621,51 @@
         scrolly_layout.addWidget(sensor_selection_group)
 
         self.config_editor = AttrsConfigEditor(
             title="Ref App parameters",
             factory_mapping={
                 "wake_up_mode": pidgets.CheckboxPidgetFactory(
                     name_label_text="Switch config on wake up"
-                )
+                ),
+                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
+                    name_label_text="Show all detected zones",
+                ),
             },
             config_type=RefAppConfig,
             parent=self.scrolly_widget,
         )
         self.config_editor.sig_update.connect(self._on_config_update)
         scrolly_layout.addWidget(self.config_editor)
 
+        self.range_helper_wake_up = RangeHelpView()
+        self.range_helper_wake_up.setTitle("Wake up config, approx. selected range")
+        scrolly_layout.addWidget(self.range_helper_wake_up)
+
         self.wake_up_config_editor = AttrsConfigEditor(
             title="Wake up config parameters",
             factory_mapping=self._get_presence_wake_up_pidget_mapping(),
             config_type=PresenceWakeUpConfig,
             parent=self.scrolly_widget,
         )
         self.wake_up_config_editor.sig_update.connect(self._on_wake_up_config_update)
         scrolly_layout.addWidget(self.wake_up_config_editor)
 
+        self.range_helper_nominal = RangeHelpView()
+        self.range_helper_nominal.setTitle("Nominal config, approx. selected range")
+        scrolly_layout.addWidget(self.range_helper_nominal)
+
         self.nominal_config_editor = AttrsConfigEditor(
             title="Nominal config parameters",
             factory_mapping=self._get_presence_zone_pidget_mapping(),
             config_type=PresenceZoneConfig,
             parent=self.scrolly_widget,
         )
         self.nominal_config_editor.sig_update.connect(self._on_nominal_config_update)
         scrolly_layout.addWidget(self.nominal_config_editor)
 
-        self.plot_config_editor = AttrsConfigEditor(
-            title="Plot parameters",
-            factory_mapping={
-                "show_all_detected_zones": pidgets.CheckboxPidgetFactory(
-                    name_label_text="Show all detected zones",
-                )
-            },
-            config_type=PlotConfig,
-            save_load_buttons=False,
-            parent=self.scrolly_widget,
-        )
-        self.plot_config_editor.sig_update.connect(self._on_plot_config_update)
-        scrolly_layout.addWidget(self.plot_config_editor)
-
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     @classmethod
     def _get_presence_zone_pidget_mapping(cls) -> PidgetGroupFactoryMapping:
         presence_pidget_mapping = dict(PresenceViewPlugin._get_pidget_mapping())
         presence_pidget_mapping.update(
@@ -720,46 +699,57 @@
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.wake_up_config_editor.handle_validation_results(not_handled)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
+            assert not_handled == []
+
             self.wake_up_config_editor.setHidden(not backend_plugin_state.config.wake_up_mode)
 
-            assert not_handled == []
+            self.range_helper_wake_up.setHidden(not backend_plugin_state.config.wake_up_mode)
+            if backend_plugin_state.config.wake_up_config is not None:
+                self.range_helper_wake_up.set_data(
+                    Detector._get_sensor_config(
+                        backend_plugin_state.config.wake_up_config
+                    ).subsweep
+                )
+
+            self.range_helper_nominal.set_data(
+                Detector._get_sensor_config(backend_plugin_state.config.nominal_config).subsweep
+            )
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
             self.nominal_config_editor.set_data(None)
             self.nominal_config_editor.setEnabled(False)
             self.wake_up_config_editor.set_data(None)
             self.wake_up_config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
         self.nominal_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.nominal_config_editor.set_data(state.config.nominal_config)
         self.wake_up_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.wake_up_config_editor.set_data(state.config.wake_up_config)
-        self.plot_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
-        self.plot_config_editor.set_data(state.plot_config)
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
@@ -768,17 +758,14 @@
 
     def _on_nominal_config_update(self, config: PresenceZoneConfig) -> None:
         BackendPlugin.update_nominal_config.rpc(self.app_model.put_task, config=config)
 
     def _on_wake_up_config_update(self, config: PresenceWakeUpConfig) -> None:
         BackendPlugin.update_wake_up_config.rpc(self.app_model.put_task, config=config)
 
-    def _on_plot_config_update(self, config: PlotConfig) -> None:
-        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
-
     def _send_defaults_request(self) -> None:
         BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
         BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,189 @@
-# Copyright (c) Acconeer AB, 2022-2023
+# Copyright (c) Acconeer AB, 2023
 # All rights reserved
+
 from __future__ import annotations
 
-import json
-import typing as t
+import warnings
+from typing import Any, Dict, Optional, Tuple
 
+import attrs
 import h5py
-import numpy as np
-import numpy.typing as npt
 
-from acconeer.exptool.a121._core import complex_array_to_int16_complex
+from acconeer.exptool import a121
+from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
+from acconeer.exptool.a121.algo import Controller
+from acconeer.exptool.a121.algo.distance import (
+    Detector,
+    DetectorConfig,
+    DetectorContext,
+    DetectorResult,
+)
 
-from ._processor import SubsweepProcessorResult
+from ._processor import Processor, ProcessorConfig, ProcessorExtraResult, ProcessorLevelStatus
 
 
-S = t.TypeVar("S")
-T = t.TypeVar("T")
+@attrs.mutable(kw_only=True)
+class RefAppConfig(DetectorConfig):
+    start_m: float = attrs.field(default=0.03)
+    """Start of measurement range."""
+    end_m: float = attrs.field(default=0.5)
+    """End of measurement range."""
+    median_filter_length: int = attrs.field(default=5)
+    """Length of the median filter used to improve robustness of the result."""
+    num_medians_to_average: int = attrs.field(default=1)
+    """Number of medians averaged to obtain the final level."""
+
+    @start_m.validator
+    def _(self, _: Any, value: float) -> None:
+        if value < Detector.MIN_DIST_M:
+            raise ValueError(f"Cannot start measurements closer than {Detector.MIN_DIST_M}m")
+
+    @end_m.validator
+    def _(self, _: Any, value: float) -> None:
+        if value > Detector.MAX_DIST_M:
+            raise ValueError(f"Cannot measure further than {Detector.MAX_DIST_M}m")
+
+    def to_detector_config(self) -> DetectorConfig:
+        return DetectorConfig(
+            start_m=self.start_m - 0.015,
+            end_m=self.end_m * 1.05,
+            max_step_length=self.max_step_length,
+            max_profile=self.max_profile,
+            signal_quality=self.signal_quality,
+            threshold_method=self.threshold_method,
+            peaksorting_method=self.peaksorting_method,
+            reflector_shape=self.reflector_shape,
+            num_frames_in_recorded_threshold=self.num_frames_in_recorded_threshold,
+            fixed_threshold_value=self.fixed_threshold_value,
+            threshold_sensitivity=self.threshold_sensitivity,
+            update_rate=self.update_rate,
+        )
 
-_ALL_RESULT_FIELDS = (
-    "frame",
-    "distance_velocity_map",
-    "amplitudes",
-    "phases",
-)
 
+@attrs.frozen(kw_only=True)
+class RefAppExtraResult:
+    processor_extra_result: ProcessorExtraResult
+    detector_result: Dict[int, DetectorResult]
 
-_INCOMPLETE_SERIALIZATION_MSG = (
-    f"Group does not contains all fields {_ALL_RESULT_FIELDS}."
-    + "Use 'allow_missing_fields' to replace missing fields with None"
-)
 
+RefAppContext = DetectorContext
 
-def optional_apply(func: t.Callable[[S], T]) -> t.Callable[[t.Optional[S]], t.Optional[T]]:
-    def wrapper(arg: t.Optional[S]) -> t.Optional[T]:
-        if arg is None:
-            return None
-        else:
-            return func(arg)
-
-    return wrapper
-
-
-_maybe_ndarray = optional_apply(np.array)
-
-
-@optional_apply
-def _frame_preprocessing(json_frame: npt.NDArray[np.int_]) -> npt.NDArray[np.complex_]:
-    """
-    A "json_frame" has the ".real" & ".imag" in a 2-lenght-list in the innermost dimension.
-    """
-    return json_frame[..., 0] + 1j * json_frame[..., 1]  # type: ignore[no-any-return]
-
-
-class SubsweepProcessorResultJSONEncoder(json.JSONEncoder):
-    def __init__(self, *, fields: t.Sequence[str] = _ALL_RESULT_FIELDS, **kwargs: t.Any) -> None:
-        super().__init__(**kwargs)
-        self.fields = fields
-
-    def default(self, o: t.Any) -> t.Any:
-        if isinstance(o, SubsweepProcessorResult):
-            result = o
-            full_dict = dict(
-                frame=complex_array_to_int16_complex(result.frame).tolist(),
-                distance_velocity_map=result.distance_velocity_map.tolist(),
-                amplitudes=result.amplitudes.tolist(),
-                phases=result.phases.tolist(),
-            )
-            return {k: v for k, v in full_dict.items() if k in self.fields}
-
-        return super().default(o)
-
-
-class SubsweepProcessorResultJSONDecoder(json.JSONDecoder):
-    def __init__(self, *, allow_missing_fields: bool = False, **kwargs: t.Any) -> None:
-        super().__init__(object_hook=self.object_hook, **kwargs)
-        self.allow_missing_fields = allow_missing_fields
-
-    def object_hook(self, obj: dict[str, t.Any]) -> SubsweepProcessorResult:
-        frame = _frame_preprocessing(_maybe_ndarray(obj.get("frame")))
-        dvm = _maybe_ndarray(obj.get("distance_velocity_map"))
-        amplitudes = _maybe_ndarray(obj.get("amplitudes"))
-        phases = _maybe_ndarray(obj.get("phases"))
-
-        if not self.allow_missing_fields and (
-            frame is None or dvm is None or amplitudes is None or phases is None
-        ):
-            raise ValueError(_INCOMPLETE_SERIALIZATION_MSG)
-
-        return SubsweepProcessorResult(
-            frame=frame,  # type: ignore[arg-type]
-            distance_velocity_map=dvm,  # type: ignore[arg-type]
-            amplitudes=amplitudes,  # type: ignore[arg-type]
-            phases=phases,  # type: ignore[arg-type]
-        )
 
+@attrs.frozen(kw_only=True)
+class RefAppResult:
+    peak_detected: Optional[bool]
+    """True if a peak (level) is detected, False if no peak is
+    detected, or None if a result is not available."""
+    peak_status: Optional[ProcessorLevelStatus]
+    """Status assigned to the detected peak."""
+    level: Optional[float]
+    """Liquid level relative to the base of the tank."""
+    extra_result: RefAppExtraResult
+    """Extra result: Only used for the plots in the GUI."""
 
-class SubsweepProcessorResultJSONSerializer:
+
+class RefApp(Controller[RefAppConfig, RefAppResult]):
     def __init__(
-        self, fields: t.Sequence[str] = _ALL_RESULT_FIELDS, allow_missing_fields: bool = False
+        self,
+        *,
+        client: a121.Client,
+        sensor_id: int,
+        config: RefAppConfig,
+        context: Optional[RefAppContext] = None,
     ) -> None:
-        self.fields = fields
-        self.allow_missing_fields = allow_missing_fields
+        super().__init__(client=client, config=config)
+        self.sensor_id = sensor_id
 
-    def serialize(self, result: SubsweepProcessorResult) -> str:
-        return json.dumps(result, cls=SubsweepProcessorResultJSONEncoder, fields=self.fields)
+        detector_config = self.config.to_detector_config()
 
-    def deserialize(self, result: str) -> SubsweepProcessorResult:
-        return json.loads(  # type: ignore[no-any-return]
-            result,
-            cls=SubsweepProcessorResultJSONDecoder,
-            allow_missing_fields=self.allow_missing_fields,
+        self._detector = Detector(
+            client=self.client,
+            sensor_ids=[self.sensor_id],
+            detector_config=detector_config,
+            context=context,
         )
 
+        processor_config = ProcessorConfig(
+            median_filter_length=self.config.median_filter_length,
+            num_medians_to_average=self.config.num_medians_to_average,
+            tank_range_start_m=self.config.start_m,
+            tank_range_end_m=self.config.end_m,
+        )
 
-class SubsweepProcessorResultListH5Serializer:
-    """
-    Reads or writes a SparseIQ SubsweepProcessorResult from/to a given h5py.Group
-    """
+        self._processor = Processor(processor_config)
 
-    def __init__(
-        self,
-        group: h5py.Group,
-        fields: t.Sequence[str] = _ALL_RESULT_FIELDS,
-        allow_missing_fields: bool = False,
+        self.started = False
+
+    def calibrate(self) -> None:
+        self._detector.calibrate_detector()
+
+    def start(
+        self, recorder: Optional[a121.Recorder] = None, algo_group: Optional[h5py.Group] = None
     ) -> None:
-        """
-        :param destination: The H5 group that will have datasets read/written to it
-        :param fields: The fields to serialize. Has no effect on de-serialization
-        :param allow_missing_fields:
-            Whether it's acceptable to break type safety during de-serialization
-            by replacing missing fields by ``None``. Has no effect on serialization.
-        """
-        self.group = group
-        self.fields = fields
-        self.allow_missing_fields = allow_missing_fields
-
-    def serialize(self, results: t.List[SubsweepProcessorResult]) -> None:
-        if "frame" in self.fields:
-            self.group.create_dataset(
-                "frame",
-                dtype=complex,
-                data=np.stack([res.frame for res in results]),
-                track_times=False,
-            )
-
-        if "distance_velocity_map" in self.fields:
-            self.group.create_dataset(
-                "distance_velocity_map",
-                dtype=float,
-                data=np.stack([res.distance_velocity_map for res in results]),
-                track_times=False,
-            )
-
-        if "amplitudes" in self.fields:
-            self.group.create_dataset(
-                "amplitudes",
-                dtype=float,
-                data=np.stack([res.amplitudes for res in results]),
-                track_times=False,
-            )
-
-        if "phases" in self.fields:
-            self.group.create_dataset(
-                "phases",
-                dtype=float,
-                data=np.stack([res.phases for res in results]),
-                track_times=False,
-            )
-
-    def _deserialize_at_index(self, index: int) -> SubsweepProcessorResult:
-        frames = self.group.get("frame", None)
-        dvms = self.group.get("distance_velocity_map", None)
-        ampss = self.group.get("amplitudes", None)
-        phasess = self.group.get("phases", None)
-
-        if not self.allow_missing_fields and (
-            frames is None or dvms is None or ampss is None or phasess is None
-        ):
-            raise ValueError(_INCOMPLETE_SERIALIZATION_MSG)
-
-        frame = None if (frames is None) else frames[index]
-        dvm = None if (dvms is None) else dvms[index]
-        amps = None if (ampss is None) else ampss[index]
-        phases = None if (phasess is None) else phasess[index]
-
-        return SubsweepProcessorResult(
-            frame=frame,  # type: ignore[arg-type]
-            distance_velocity_map=dvm,  # type: ignore[arg-type]
-            amplitudes=amps,  # type: ignore[arg-type]
-            phases=phases,  # type: ignore[arg-type]
+        if self.started:
+            raise RuntimeError("Already started")
+
+        if recorder is not None:
+            if isinstance(recorder, a121.H5Recorder):
+                algo_group = recorder.require_algo_group("tank_level")
+                _record_algo_data(algo_group, self.sensor_id, self.config, self._detector.context)
+            else:
+                # Should never happen as we currently only have the H5Recorder
+                warnings.warn("Will not save algo data")
+
+        self._detector.start(recorder=recorder, _algo_group=algo_group)
+
+        self.started = True
+
+    def get_next(self) -> RefAppResult:
+        if not self.started:
+            raise RuntimeError("Not started")
+
+        result = self._detector.get_next()
+
+        processor_result = self._processor.process(result)
+
+        ref_app_extra_result = RefAppExtraResult(
+            processor_extra_result=processor_result.extra_result, detector_result=result
         )
 
-    def deserialize(self, _: None) -> t.List[SubsweepProcessorResult]:
-        optional_lens = set(
-            optional_apply(len)(series)
-            for series in [
-                self.group.get("frame", None),
-                self.group.get("distance_velocity_map", None),
-                self.group.get("amplitudes", None),
-                self.group.get("phases", None),
-            ]
+        return RefAppResult(
+            peak_detected=processor_result.peak_detected,
+            peak_status=processor_result.peak_status,
+            level=processor_result.filtered_level,
+            extra_result=ref_app_extra_result,
         )
-        lens = {l for l in optional_lens if l is not None}
 
-        (common_length,) = lens
+    def update_config(self, config: RefAppConfig) -> None:
+        raise NotImplementedError
+
+    def stop(self) -> Any:
+        if not self.started:
+            raise RuntimeError("Already stopped")
+
+        recorder_result = self._detector.stop()
+
+        self.started = False
+
+        return recorder_result
+
+
+def _record_algo_data(
+    algo_group: h5py.Group, sensor_id: int, config: RefAppConfig, context: RefAppContext
+) -> None:
+    algo_group.create_dataset("sensor_id", data=sensor_id, track_times=False)
+
+    _create_h5_string_dataset(algo_group, "config", config.to_json())
+
+    context_group = algo_group.create_group("tank_level_context")
+    context.to_h5(context_group)
+
+
+def _load_algo_data(algo_group: h5py.Group) -> Tuple[int, RefAppConfig, RefAppContext]:
+    sensor_id = int(algo_group["sensor_id"][()])
+    config = RefAppConfig.from_json(algo_group["config"][()])
+
+    context_group = algo_group["tank_level_context"]
+    tank_level_context = DetectorContext.from_h5(context_group)
 
-        return [self._deserialize_at_index(i) for i in range(int(common_length))]
+    return sensor_id, config, tank_level_context
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,36 +477,37 @@
             results = backend_plugin_state.config._collect_validation_results()
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
             sensor_config = Detector._get_sensor_config(backend_plugin_state.config)
-            self.range_help_view.update(sensor_config.subsweep)
+            self.range_help_view.set_data(sensor_config.subsweep)
             self.sensor_config_status.set_data(sensor_config)
             assert not_handled == []
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/speed/_processors.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/speed/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,16 +282,21 @@
 
         self.upper_std_history = np.roll(self.upper_std_history, -1)
         self.upper_std_history[-1] = (
             example_app_result.velocity - 0.5 * processor_extra_result.peak_width
         )
         self.upper_std_curve.setData(xs, self.upper_std_history)
 
-        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
-        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
+        low_lim = np.minimum(
+            np.min(processor_extra_result.psd_threshold), np.min(processor_extra_result.psd)
+        )
+        high_lim = self.psd_smooth_max.update(
+            np.maximum(processor_extra_result.psd_threshold, processor_extra_result.psd)
+        )
+        self.psd_plot.setYRange(np.log10(low_lim), np.log10(high_lim))
         self.psd_plot.setXRange(
             processor_extra_result.max_bin_vertical_vs[0],
             processor_extra_result.max_bin_vertical_vs[-1],
         )
         self.psd_curve.setData(
             processor_extra_result.vertical_velocities, processor_extra_result.psd
         )
@@ -380,15 +385,15 @@
     @classmethod
     def _get_pidget_mapping(cls) -> PidgetFactoryMapping:
         return {
             "surface_distance": pidgets.FloatPidgetFactory(
                 name_label_text="Surface distance",
                 suffix=" m",
                 decimals=2,
-                limits=(0.1, 3),
+                limits=(0.1, None),
             ),
             "sensor_angle": pidgets.FloatPidgetFactory(
                 name_label_text="Sensor angle",
                 suffix=" degrees",
                 decimals=1,
                 limits=(0, 89),
             ),
@@ -503,36 +508,37 @@
 
             not_handled = self.config_editor.handle_validation_results(results)
 
             not_handled = self.misc_error_view.handle_validation_results(not_handled)
 
             assert not_handled == []
 
-            self.range_helper.update(
+            self.range_helper.set_data(
                 ExampleApp._get_sensor_config(backend_plugin_state.config).subsweep
             )
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         state = app_model.backend_plugin_state
 
         if state is None:
             self.start_button.setEnabled(False)
             self.stop_button.setEnabled(False)
 
             self.config_editor.set_data(None)
             self.config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
 
             return
 
         assert isinstance(state, SharedState)
 
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.set_data(state.config)
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import attrs
 import numpy as np
 import numpy.typing as npt
 import scipy
 from scipy.signal import welch
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import AlgoProcessorConfigBase, ProcessorBase
 from acconeer.exptool.a121.algo._utils import (
     APPROX_BASE_STEP_LENGTH_M,
     PERCEIVED_WAVELENGTH,
     find_peaks,
     get_distances_m,
 )
@@ -75,21 +76,21 @@
 
 @attrs.frozen(kw_only=True)
 class ProcessorExtraResult:
     """
     Contains information for visualization in ET.
     """
 
-    max_bin_vertical_vs: npt.NDArray[np.float_] = attrs.field()
+    max_bin_vertical_vs: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     peak_width: float = attrs.field()
 
-    vertical_velocities: npt.NDArray[np.float_] = attrs.field()
-    psd: npt.NDArray[np.float_] = attrs.field()
+    vertical_velocities: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
+    psd: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     peak_idx: Optional[np.int_] = attrs.field()
-    psd_threshold: npt.NDArray[np.float_] = attrs.field()
+    psd_threshold: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
     estimated_v: float = attrs.field()
     distance_m: float = attrs.field()
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,27 +632,28 @@
             self.start_button.setEnabled(False)
             self.calibrate_detector_button.setEnabled(False)
             self.stop_button.setEnabled(False)
             self.defaults_button.setEnabled(False)
 
             self.config_editor.setEnabled(False)
             self.tank_level_config_editor.setEnabled(False)
-            self.sensor_id_pidget.set_selected_sensor(None, [])
+            self.sensor_id_pidget.setEnabled(False)
             self.message_box.setText("")
 
             return
 
         assert isinstance(state, SharedState)
 
         self.defaults_button.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
         self.tank_level_config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
         self.config_editor.setEnabled(app_model.plugin_state == PluginState.LOADED_IDLE)
 
-        self.sensor_id_pidget.set_selected_sensor(state.sensor_id, app_model.connected_sensors)
+        self.sensor_id_pidget.set_selectable_sensors(app_model.connected_sensors)
+        self.sensor_id_pidget.set_data(state.sensor_id)
         self.sensor_id_pidget.setEnabled(app_model.plugin_state.is_steady)
 
         detector_status = Detector.get_detector_status(
             state.config.to_detector_config(), state.context, [state.sensor_id]
         )
 
         self.message_box.setText(self.TEXT_MSG_MAP[detector_status.detector_state])
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Dict, List, Optional
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import AlgoProcessorConfigBase
 from acconeer.exptool.a121.algo.distance import DetectorResult
 
 
 TIME_HISTORY_S = 30
 UPDATES_PER_SECOND = 4
 
@@ -30,15 +31,17 @@
 
 @attrs.frozen(kw_only=True)
 class ProcessorExtraResult:
     """
     Contains information for visualization in ET.
     """
 
-    level_and_time_for_plotting: dict[str, npt.NDArray[np.float_]]
+    level_and_time_for_plotting: Dict[str, npt.NDArray[np.float_]] = attrs.field(
+        eq=utils.attrs_dict_ndarray_isclose
+    )
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
     """Processor results"""
 
     peak_detected: Optional[bool]
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
+from acconeer.exptool.a121._core import utils
 from acconeer.exptool.a121.algo import (
     APPROX_BASE_STEP_LENGTH_M,
     AlgoProcessorConfigBase,
     ProcessorBase,
     double_buffering_frame_filter,
 )
 
@@ -80,17 +81,21 @@
 class ProcessorContext:
     ...
 
 
 @attrs.frozen(kw_only=True)
 class ProcessorResult:
     result_available: bool
-    time_series: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    lp_z_abs_db: Optional[npt.NDArray[np.float_]] = attrs.field(default=None)
-    freqs: npt.NDArray[np.float_]
+    time_series: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    lp_z_abs_db: Optional[npt.NDArray[np.float_]] = attrs.field(
+        default=None, eq=utils.attrs_optional_ndarray_isclose
+    )
+    freqs: npt.NDArray[np.float_] = attrs.field(eq=utils.attrs_ndarray_isclose)
     max_amplitude: float
     amplitude_threshold: float
     max_psd_ampl: Optional[float] = attrs.field(default=None)
     max_psd_ampl_freq: Optional[float] = attrs.field(default=None)
 
 
 class Processor(ProcessorBase[ProcessorConfig, ProcessorResult]):
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 import ctypes
 import importlib.resources
 import sys
+import typing as t
 
 import qdarktheme
 
 from PySide6 import QtCore, QtGui
 from PySide6.QtWidgets import QApplication
 
 import pyqtgraph as pg
@@ -37,17 +38,16 @@
     if sys.platform == "win32" or sys.platform == "cygwin":
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID("acconeer.exptool")
 
     QApplication.setHighDpiScaleFactorRoundingPolicy(
         QtCore.Qt.HighDpiScaleFactorRoundingPolicy.PassThrough,
     )
 
-    app = QApplication.instance()
-    if app is None:
-        app = QApplication(sys.argv)
+    # The cast necessitated of a miss in the typing stubs.
+    app: QApplication = t.cast(QApplication, QApplication.instance()) or QApplication(sys.argv)
 
     app.setStyleSheet(qdarktheme.load_stylesheet("light"))
     app.setAttribute(QtCore.Qt.ApplicationAttribute.AA_UseHighDpiPixmaps)
 
     backend = Backend()
     backend.start()
 
@@ -77,25 +77,25 @@
     backend.stop()
 
 
 def _pixmap_to_icon(pixmap: QtGui.QPixmap) -> QtGui.QIcon:
     size = max(pixmap.size().height(), pixmap.size().width())
 
     square_pixmap = QtGui.QPixmap(size, size)
-    square_pixmap.fill(QtGui.Qt.transparent)
+    square_pixmap.fill(QtGui.QRgba64.fromRgba(0, 0, 0, 0))
 
     painter = QtGui.QPainter(square_pixmap)
     painter.drawPixmap(
         (square_pixmap.size().width() - pixmap.size().width()) // 2,
         (square_pixmap.size().height() - pixmap.size().height()) // 2,
         pixmap,
     )
     painter.end()
 
     scaled_pixmap = square_pixmap.scaled(
         256,
         256,
-        aspectMode=QtGui.Qt.KeepAspectRatio,
-        mode=QtGui.Qt.SmoothTransformation,
+        aspectMode=QtCore.Qt.AspectRatioMode.KeepAspectRatio,
+        mode=QtGui.Qt.TransformationMode.SmoothTransformation,
     )
 
     return QtGui.QIcon(scaled_pixmap)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,15 +602,16 @@
 
     def is_ready_for_session(self) -> bool:
         """
         Returns True if the plugin is ready for a new session.
         Additional conditions can be added in respective plugin.
         """
         return (
-            self.plugin_state == PluginState.LOADED_IDLE
+            self.backend_plugin_state is not None
+            and self.plugin_state == PluginState.LOADED_IDLE
             and self.connection_state == ConnectionState.CONNECTED
             and bool(self.connected_sensors)
         )
 
     def _failed_autoconnect(
         self, exception: Exception, traceback_format_exc: Optional[str] = None
     ) -> None:
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from PySide6.QtCore import QObject, QThread, QTimerEvent, Signal, Slot
@@ -16,19 +16,19 @@
     sig_update = Signal(object, object)
 
     class Worker(QObject):
         sig_update = Signal(object, object)
         serial_devices: Any = None
         usb_devices: Any = None
 
-        @Slot()  # type: ignore[misc]
+        @Slot()
         def start(self) -> None:
             self.timer_id = self.startTimer(500)
 
-        @Slot()  # type: ignore[misc]
+        @Slot()
         def stop(self) -> None:
             self.killTimer(self.timer_id)
 
         def timerEvent(self, event: QTimerEvent) -> None:
             serial_devices = get_serial_devices()  # type: ignore[name-defined]
             usb_devices = get_usb_devices()  # type: ignore[name-defined]
 
@@ -36,29 +36,29 @@
                 self.serial_devices = serial_devices
                 self.usb_devices = usb_devices
                 self.sig_update.emit(serial_devices, usb_devices)
 
     def __init__(self, parent: QObject) -> None:
         super().__init__(parent)
 
-        self.thread = QThread(self)
+        self._thread = QThread(self)
         self.worker = self.Worker()
-        self.thread.started.connect(self.worker.start)
-        self.thread.finished.connect(self.worker.stop)
+        self._thread.started.connect(self.worker.start)
+        self._thread.finished.connect(self.worker.stop)
         self.worker.sig_update.connect(self._on_update)
-        self.worker.moveToThread(self.thread)
+        self.worker.moveToThread(self._thread)
         self.signalling = False
 
     def start(self) -> None:
-        self.thread.start()
+        self._thread.start()
         self.signalling = True
 
     def stop(self) -> None:
-        self.thread.quit()
-        self.thread.wait()
+        self._thread.quit()
+        self._thread.wait()
         self.signalling = False
 
     def pause(self) -> None:
         self.signalling = False
 
     def resume(self) -> None:
         self.signalling = True
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/backend/_tasks.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/backend/_tasks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,30 +48,32 @@
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setWindowTitle("Flash tool")
         self.setMinimumWidth(250)
 
         vbox = QVBoxLayout(self)
-        vbox.setAlignment(Qt.AlignCenter)
+        vbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.loading = QLabel()
-        self.loading.setAlignment(Qt.AlignCenter)
+        self.loading.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         loader_gif = None
         with importlib.resources.path(resources, "loader.gif") as path:
             loader_gif = path
 
         self.flash_movie = QMovie(str(loader_gif))
         self.loading.setMovie(self.flash_movie)
         vbox.addWidget(self.loading)
 
         self.flash_label = QLabel(self)
-        self.flash_label.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.MinimumExpanding)
-        self.flash_label.setAlignment(Qt.AlignCenter)
+        self.flash_label.setSizePolicy(
+            QSizePolicy.Policy.Preferred, QSizePolicy.Policy.MinimumExpanding
+        )
+        self.flash_label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         vbox.addWidget(self.flash_label)
 
         self.ok_button = QPushButton(self)
         self.ok_button.setText("OK")
         self.ok_button.setHidden(True)
         self.ok_button.clicked.connect(self._on_ok_click)
         vbox.addWidget(self.ok_button)
@@ -198,17 +200,18 @@
         if self.usr_edit.text() == "" or self.pwd_edit.text() == "":
             self.login_button.setEnabled(False)
         else:
             self.login_button.setEnabled(True)
 
     def _on_remember_me_checked(self) -> None:
         if self.remember_me_box.isChecked() and not self.cookies_accepted:
-            self.cookies_accepted = CookieConsentDialog(self).exec()
+            exit_code = CookieConsentDialog(self).exec()
+            self.cookies_accepted = exit_code == 0
             if not self.cookies_accepted:
-                self.remember_me_box.setCheckState(Qt.Unchecked)
+                self.remember_me_box.setCheckState(Qt.CheckState.Unchecked)
 
     def _handle_login(self) -> None:
         self.login_status_label.setHidden(True)
 
         usr = self.usr_edit.text()
         pwd = self.pwd_edit.text()
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import traceback
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Optional, Tuple
+from typing import Optional
 
 from requests import Response, Session
 from requests.cookies import RequestsCookieJar
 
 from PySide6.QtCore import QThread, Signal
 
 from acconeer.exptool.app.new._exceptions import HandledException
@@ -64,15 +64,15 @@
             log.error(str(e))
             self.flash_failed.emit(HandledException(e), traceback.format_exc())
 
 
 class AuthThread(QThread):
     license_loaded = Signal(DevLicense)
     auth_failed = Signal()
-    auth_done = Signal((RequestsCookieJar, Tuple[bool, Session, Response]))
+    auth_done = Signal(tuple)  # (RequestsCookieJar, Tuple[bool, Session, Response]))
 
     def __init__(
         self,
         usr: Optional[str] = "",
         pwd: Optional[str] = "",
         do_login: bool = False,
         dev_license: DevLicense = None,
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,20 +336,14 @@
         self.flash_button.setEnabled(
             not self.authenticating
             and not self.downloading_firmware
             and self.flash_device is not None
             and self.bin_file is not None
         )
 
-    def exec(self) -> None:
-        if self.app_model.connection_interface == ConnectionInterface.SOCKET:
-            self.app_model.set_connection_interface(ConnectionInterface.USB)
-
-        super().exec()
-
     def closeEvent(self, event: QCloseEvent) -> None:
         if self.authenticating:
             self.auth_thread.terminate()
             self.auth_thread.wait()
 
         if self.downloading_firmware:
             self.download_thread.terminate()
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,13 +117,13 @@
                     (HELP(), "Help", HelpMainWidget(self)),
                 ],
             )
         )
 
         self.setStatusBar(StatusBar(app_model, self))
         self.setWindowTitle("Acconeer Exploration Tool")
-        self.moveEvent = lambda _: self.saveGeometry()
+        self.moveEvent = lambda _: self.saveGeometry()  # type: ignore[method-assign,assignment]
 
         app_model.sig_error.connect(self.on_app_model_error)
 
     def on_app_model_error(self, exception: Exception, traceback_str: t.Optional[str]) -> None:
         ExceptionWidget(self, exc=exception, traceback_str=traceback_str).exec()
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         *,
         exc: Exception,
         traceback_str: Optional[str] = None,
         title: str = "Error",
     ) -> None:
         super().__init__(parent)
 
-        self.setIcon(QMessageBox.Warning)
-        self.setStandardButtons(QMessageBox.Ok)
+        self.setIcon(QMessageBox.Icon.Warning)
+        self.setStandardButtons(QMessageBox.StandardButton.Ok)
 
         self.setWindowTitle(title)
         self.setText(str(exc))
 
         try:
             raise exc
         except HandledException:
@@ -62,9 +62,9 @@
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setLayout(QHBoxLayout(self))
         self.layout().setContentsMargins(5, 5, 5, 5)
 
         frame = QFrame(self)
-        frame.setFrameShape(QFrame.VLine)
+        frame.setFrameShape(QFrame.Shape.VLine)
         self.layout().addWidget(frame)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from PySide6.QtWidgets import QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121._core import Criticality
 
 from .data_editor import DataEditor
 from .json_save_load_buttons import JsonPresentable, JsonSaveLoadButtons
-from .pidgets import FlatPidgetGroup, Pidget, PidgetGroup, PidgetGroupHook, PidgetHook
+from .pidgets import FlatPidgetGroup, Pidget, PidgetGroup, PidgetHook, WidgetHook
 from .save_dialog import PresenterFunc
 from .types import PidgetFactoryMapping, PidgetGroupFactoryMapping
 from .utils import GroupBox
 
 
 T = TypeVar("T", bound=JsonPresentable)
 
@@ -68,29 +68,30 @@
         parent: Optional[QWidget] = None,
     ) -> None:
         super().__init__(parent=parent)
         self._config = None
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().setSpacing(11)
+
         group_box = GroupBox.vertical(
             title,
             right_header=(
-                JsonSaveLoadButtons.from_editor_and_config_type(self, config_type, extra_presenter)
+                JsonSaveLoadButtons.from_editor_and_config_type(self, config_type, extra_presenter)  # type: ignore[arg-type]
                 if save_load_buttons
                 else None
             ),
             parent=self,
         )
         self.layout().addWidget(group_box)
 
         self._pidget_mapping: dict[str, Pidget] = {}
         self._pidget_hooks: dict[str, Sequence[PidgetHook]] = {}
         self._group_widgets: list[QWidget] = []
-        self._group_hooks: list[Sequence[PidgetGroupHook]] = []
+        self._group_hooks: list[Sequence[WidgetHook]] = []
         self._erroneous_aspects = set()
 
         for pidget_group, factory_mapping in _to_group_factory_mapping(factory_mapping).items():
             pidgets = []
             for aspect, factory in factory_mapping.items():
                 pidget = factory.create(group_box)
                 pidget.sig_update.connect(partial(self._update_config_aspect, aspect))
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     def __init__(self, label: str, widget: QWidget, parent: t.Optional[QWidget] = None) -> None:
         super().__init__(parent)
 
         self.widget = widget
         self.widget.setVisible(False)
 
         self.arrow_button = QToolButton()
-        self.arrow_button.setToolButtonStyle(QtCore.Qt.ToolButtonTextBesideIcon)
+        self.arrow_button.setToolButtonStyle(QtCore.Qt.ToolButtonStyle.ToolButtonTextBesideIcon)
         self.arrow_button.setText(label)
-        self.arrow_button.setArrowType(QtCore.Qt.RightArrow)
+        self.arrow_button.setArrowType(QtCore.Qt.ArrowType.RightArrow)
         self.arrow_button.setCheckable(True)
         self.arrow_button.setChecked(False)
         self.arrow_button.toggled.connect(self._on_toggle)
 
         self.setLayout(QVBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         self.layout().addWidget(self.arrow_button)
         self.layout().addWidget(self.widget)
 
     def set_collapsed(self, collapsed: bool) -> None:
         self.widget.setVisible(not collapsed)
-        self.arrow_button.setArrowType(QtCore.Qt.RightArrow if collapsed else QtCore.Qt.DownArrow)
+        self.arrow_button.setArrowType(
+            QtCore.Qt.ArrowType.RightArrow if collapsed else QtCore.Qt.ArrowType.DownArrow
+        )
 
     def _on_toggle(self, checked: bool) -> None:
         self.set_collapsed(not checked)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/json_save_load_buttons.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,19 @@
     return None
 
 
 class JsonSaveLoadButtons(QWidget):
     _ICON_SIZE = QSize(20, 20)
     _BUTTON_SIZE = QSize(35, 25)
     _ICON_TRANSIENT_CHECKMARK_DURATION_MS = 2000
-    _FILE_DIALOG_OPTIONS = dict(
-        filter="JSON (*.json)",
-        options=QFileDialog.Option.DontUseNativeDialog,
-    )
+    _FILE_DIALOG_FILTER = "JSON (*.json)"
 
     def __init__(
         self,
-        getter: t.Callable[[], JsonPresentable],
+        getter: t.Callable[[], t.Optional[JsonPresentable]],
         setter: t.Callable[[JsonPresentable], t.Any],
         encoder: t.Callable[[JsonPresentable], str],
         decoder: t.Callable[[str], JsonPresentable],
         extra_presenter: PresenterFunc,
         parent: t.Optional[QWidget] = None,
     ) -> None:
         super().__init__(parent=parent)
@@ -117,15 +114,15 @@
         self.layout().setContentsMargins(5, 5, 5, 8)
         self.layout().addWidget(self._save)
         self.layout().addWidget(self._load)
 
     @classmethod
     def from_editor_and_config_type(
         cls,
-        editor: DataEditor[JsonPresentable],
+        editor: DataEditor[t.Optional[JsonPresentable]],
         config_type: t.Type[JsonPresentable],
         extra_presenter: PresenterFunc = lambda i, t: None,
     ) -> JsonSaveLoadButtons:
         """
         Creates a JsonSaveLoadButtons instance with a built-in JSON preview
 
         :param editor: The editor to bind the save/load buttons to
@@ -142,32 +139,40 @@
             extra_presenter,
         )
         editor.sig_update.connect(lambda model: buttons._save.setEnabled(model is not None))
         return buttons
 
     def _save_to_selected_file(self) -> None:
         model = self._getter()
+
+        if model is None:
+            raise RuntimeError
+
         filename = SaveDialogWithPreview.get_save_file_name(
             caption="Save to file",
             model=model,
             presenter=_none_coalescing_chain(
                 _json_presentation,
                 set_config_presenter,
                 self._extra_presenter,
             ),
-            **self._FILE_DIALOG_OPTIONS,
+            filter=self._FILE_DIALOG_FILTER,
+            parent=self,
         )
 
         if filename:
             Path(filename).with_suffix(".json").write_text(self._encoder(model))
             self._show_transient_checkmark(self._save)
 
     def _load_and_set_selected_file(self) -> None:
         filename, _ = QFileDialog.getOpenFileName(
-            caption="Load from file", **self._FILE_DIALOG_OPTIONS
+            self,
+            caption="Load from file",
+            filter=self._FILE_DIALOG_FILTER,
+            options=QFileDialog.Option.DontUseNativeDialog,
         )
 
         if filename:
             self._setter(self._decoder(Path(filename).read_text()))
             self._show_transient_checkmark(self._load)
 
     @classmethod
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         self.setLayout(self._layout)
 
         self._metadata_view = MetadataView(self)
         self._extended_metadata_view = ExtendedMetadataView(self)
         self._layout.addWidget(self._metadata_view)
         self._layout.addWidget(self._extended_metadata_view)
 
-    def update(
+    def set_data(
         self,
         metadata: Optional[Union[a121.Metadata, list[dict[int, a121.Metadata]]]] = None,
     ) -> None:
         if isinstance(metadata, list):
             self._metadata_view.setHidden(True)
             self._extended_metadata_view.setHidden(False)
-            self._extended_metadata_view.update(metadata)
+            self._extended_metadata_view.set_data(metadata)
         else:
             self._metadata_view.setHidden(False)
             self._extended_metadata_view.setHidden(True)
-            self._metadata_view.update(metadata)
+            self._metadata_view.set_data(metadata)
 
 
 class ExtendedMetadataView(QWidget):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
         self.setLayout(QVBoxLayout(self))
 
@@ -82,82 +82,85 @@
             subwidget.setTitle("")
             self._tab_widget.addTab(subwidget, "-")
 
     def _remove_unnecessary_tabs(self, needed_widgets: int) -> None:
         while self._tab_widget.count() > needed_widgets:
             self._tab_widget.removeTab(0)
 
-    def update(self, extended_metadata: Optional[list[dict[int, a121.Metadata]]]) -> None:
+    def set_data(self, extended_metadata: Optional[list[dict[int, a121.Metadata]]]) -> None:
         if extended_metadata is None:
             self._represent_none()
             return
 
         tabs_needed = _core.utils.extended_structure_entry_count(extended_metadata)
         self._add_needed_tabs(tabs_needed)
         self._remove_unnecessary_tabs(tabs_needed)
 
         for i, (group_id, sensor_id, metadata) in enumerate(
             _core.utils.iterate_extended_structure(extended_metadata)
         ):
             self._tab_widget.setTabText(i, f"G{group_id}:S{sensor_id}")
             metadata_view = self._tab_widget.widget(i)
             if isinstance(metadata_view, MetadataView):
-                metadata_view.update(metadata)
+                metadata_view.set_data(metadata)
             else:
                 raise RuntimeError(
                     "ExtendedMetadataView contains child widgets that are not MetadataViews."
                 )
 
 
 class MetadataView(QGroupBox):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setTitle("Metadata")
-        self.setLayout(QGridLayout(self))
+        layout = QGridLayout(self)
 
         row = 0
 
         self.frame_data_length = MetadataValueWidget(self)
-        self.layout().addWidget(self.frame_data_length, row, 1)
+        layout.addWidget(self.frame_data_length, row, 1)
 
         frame_data_length_label = QLabel("Frame data length", self)
-        frame_data_length_label.setToolTip(a121.Metadata.frame_data_length.__doc__)
-        self.layout().addWidget(frame_data_length_label, row, 0)
+        frame_data_length_label.setToolTip(a121.Metadata.frame_data_length.__doc__ or "")
+        layout.addWidget(frame_data_length_label, row, 0)
 
         row += 1
 
         self.calibration_temperature = MetadataValueWidget(self)
-        self.layout().addWidget(self.calibration_temperature, row, 1)
+        layout.addWidget(self.calibration_temperature, row, 1)
 
         calibration_temperature_label = QLabel("Calibration temperature", self)
-        calibration_temperature_label.setToolTip(a121.Metadata.calibration_temperature.__doc__)
-        self.layout().addWidget(calibration_temperature_label, row, 0)
+        calibration_temperature_label.setToolTip(
+            a121.Metadata.calibration_temperature.__doc__ or ""
+        )
+        layout.addWidget(calibration_temperature_label, row, 0)
 
         row += 1
 
         self.max_sweep_rate = MetadataValueWidget(self)
-        self.layout().addWidget(self.max_sweep_rate, row, 1)
+        layout.addWidget(self.max_sweep_rate, row, 1)
 
         max_sweep_rate_label = QLabel("Max sweep rate", self)
-        max_sweep_rate_label.setToolTip(a121.Metadata.max_sweep_rate.__doc__)
-        self.layout().addWidget(max_sweep_rate_label, row, 0)
+        max_sweep_rate_label.setToolTip(a121.Metadata.max_sweep_rate.__doc__ or "")
+        layout.addWidget(max_sweep_rate_label, row, 0)
 
         row += 1
 
         self.high_speed_mode = MetadataValueWidget(self)
-        self.layout().addWidget(self.high_speed_mode, row, 1)
+        layout.addWidget(self.high_speed_mode, row, 1)
 
         high_speed_mode_label = QLabel("High speed mode", self)
-        high_speed_mode_label.setToolTip(a121.Metadata.high_speed_mode.__doc__)
-        self.layout().addWidget(high_speed_mode_label, row, 0)
+        high_speed_mode_label.setToolTip(a121.Metadata.high_speed_mode.__doc__ or "")
+        layout.addWidget(high_speed_mode_label, row, 0)
 
-        self.update(None)
+        self.setLayout(layout)
+        self.set_data(None)
 
-    def update(self, metadata: Optional[a121.Metadata]) -> None:
+    def set_data(self, metadata: Optional[a121.Metadata]) -> None:
         self.frame_data_length.setText(f"{metadata.frame_data_length}" if metadata else "-")
         self.calibration_temperature.setText(
             f"{metadata.calibration_temperature}" if metadata else "-"
         )
 
         if metadata:
             if metadata.max_sweep_rate:
@@ -175,11 +178,11 @@
             else "-"
         )
 
 
 class MetadataValueWidget(QLineEdit):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
-        self.setAlignment(QtCore.Qt.AlignRight)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
         self.setFixedWidth(_WIDGET_WIDTH)
         self.setReadOnly(True)
-        self.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,37 +32,37 @@
         self.setLayout(self._layout)
 
         self._perf_calc_view = PerfCalcView(self)
         self._extended_perf_calc_view = ExtendedPerfCalcView(self)
         self._layout.addWidget(self._perf_calc_view)
         self._layout.addWidget(self._extended_perf_calc_view)
 
-    def update(
+    def set_data(
         self,
         session_config: Optional[a121.SessionConfig] = None,
         metadata: Optional[Union[a121.Metadata, list[dict[int, a121.Metadata]]]] = None,
     ) -> None:
         if isinstance(metadata, list):
             self._layout.setCurrentIndex(1)
-            self._extended_perf_calc_view.update(session_config, metadata)
+            self._extended_perf_calc_view.set_data(session_config, metadata)
         else:
             self._layout.setCurrentIndex(0)
-            self._perf_calc_view.update(session_config, metadata)
+            self._perf_calc_view.set_data(session_config, metadata)
 
 
-class ExtendedPerfCalcView(GroupBox):
+class ExtendedPerfCalcView(GroupBox[QVBoxLayout]):
     def __init__(self, parent: QWidget) -> None:
         super().__init__("Performance calculations", QVBoxLayout, parent=parent)
 
         label = QLabel("No estimates available", self)
         label.setEnabled(False)
-        label.setAlignment(QtCore.Qt.AlignCenter)
+        label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.layout().addWidget(label)
 
-    def update(
+    def set_data(
         self,
         session_config: Optional[a121.SessionConfig] = None,
         extended_metadata: Optional[list[dict[int, a121.Metadata]]] = None,
     ) -> None:
         pass
 
 
@@ -82,17 +82,17 @@
 
         self.average_current = PerfCalcValueWidget(self)
         layout.addWidget(self.average_current, 0, 1)
         average_current_label = QLabel("Estimated avg. current", self)
         average_current_label.setToolTip(tooltip)
         layout.addWidget(average_current_label, 0, 0)
 
-        self.update(None)
+        self.set_data(None)
 
-    def update(
+    def set_data(
         self,
         session_config: Optional[a121.SessionConfig] = None,
         metadata: Optional[a121.Metadata] = None,
     ) -> None:
         try:
             self._update(session_config, metadata)
         except Exception:
@@ -116,11 +116,11 @@
 
         self.average_current.setText(f"{pc.average_current * 1e3:.0f} mA")
 
 
 class PerfCalcValueWidget(QLineEdit):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
-        self.setAlignment(QtCore.Qt.AlignRight)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
         self.setFixedWidth(_WIDGET_WIDTH)
         self.setReadOnly(True)
-        self.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Acconeer AB, 2023
 # All rights reserved
 
 from . import hooks
-from .pidget_groups import CollapsiblePidgetGroup, FlatPidgetGroup, PidgetGroup, PidgetGroupHook
+from .pidget_groups import CollapsiblePidgetGroup, FlatPidgetGroup, PidgetGroup, WidgetHook
 from .pidgets import (
     CheckboxPidget,
     CheckboxPidgetFactory,
     ComboboxPidget,
     ComboboxPidgetFactory,
     EnumPidget,
     EnumPidgetFactory,
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 It's still possible to use any function that adheres to respective type.
 
 The definitions of these hooks are placed in ``pidget_groups.py`` and
 ``pidgets.py``, respectively.
 
 .. code-block:: python
-    PidgetGroupHook = t.Callable[
+    WidgetHook = t.Callable[
         [QWidget, t.Mapping[str, Pidget]], None
     ]
     PidgetHook = Callable[
         ["Pidget", Mapping[str, "Pidget"]], None
     ]
 
-A ``PidgetGroupHook`` is a function that accepts a ``QWidget`` instance
+A ``WidgetHook`` is a function that accepts a ``QWidget`` instance
 and a ``Mapping[str, Pidget]`` and returns nothing.
 The ``QWidget`` instance is the container widget returned by the
 ``get_container`` function of the ``PidgetGroup``.
 
 .. code-block:: python
     def my_hook(pg: QWidget, mapping: Mapping[str, Pidget]) -> None:
         print(pg)  # pg will be the "a" variable below
 
     a = PidgetGroup(
         hooks=my_hook,
         # or hooks=[my_hook]
         # or hooks=(my_hook,)
     )
 
-The second argument of a ``PidgetGroupHook`` is the ``PidgetMapping`` kept
+The second argument of a ``WidgetHook`` is the ``PidgetMapping`` kept
 internally in ``AttrsConfigEditor``;
 
 .. code-block:: python
     def my_hook(pg: QWidget, mapping: Mapping[str, Pidget]) -> None:
         print(mapping)
         # mapping will be:
         # {
@@ -65,20 +65,19 @@
 """
 from __future__ import annotations
 
 import typing as t
 
 from PySide6.QtWidgets import QWidget
 
-from .pidget_groups import PidgetGroupHook
-from .pidgets import Pidget, PidgetHook
+from .pidget_groups import WidgetHook
+from .pidgets import Pidget
 
 
 PidgetMapping = t.Mapping[str, Pidget]
-GeneralHook = t.Union[PidgetHook, PidgetGroupHook]
 
 PidgetMappingPredicate = t.Callable[[PidgetMapping], bool]
 
 
 def parameter_equals(aspect: str, value: t.Any) -> PidgetMappingPredicate:
     """Checks whether the parameter of the pidget assigned to aspect is equal to value"""
 
@@ -105,23 +104,23 @@
     def inner(mapping: PidgetMapping) -> bool:
         lower, higher = range
         return bool(lower < mapping[aspect].get_data() < higher)
 
     return inner
 
 
-def enable_if(predicate: PidgetMappingPredicate) -> GeneralHook:
+def enable_if(predicate: PidgetMappingPredicate) -> WidgetHook:
     """Enables the instance this hook is assigned to if the predicate evaluates to "True" """
 
     def inner(inst: QWidget, mapping: PidgetMapping) -> None:
         inst.setEnabled(predicate(mapping))
 
     return inner
 
 
-def disable_if(predicate: PidgetMappingPredicate) -> GeneralHook:
+def disable_if(predicate: PidgetMappingPredicate) -> WidgetHook:
     """Negation of "enable_if" """
 
     def inner(inst: QWidget, mapping: PidgetMapping) -> None:
         inst.setEnabled(not predicate(mapping))
 
     return inner
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 from acconeer.exptool.app.new.ui.plugin_components.collapsible_widget import CollapsibleWidget
 
 from .common import MaybeIterable, as_sequence
 from .pidgets import Pidget
 
 
-PidgetGroupHook = t.Callable[[QWidget, t.Mapping[str, Pidget]], None]
+WidgetHook = t.Callable[[QWidget, t.Mapping[str, Pidget]], None]
 
 
-def _hooks_converter(a: MaybeIterable[PidgetGroupHook]) -> t.Sequence[PidgetGroupHook]:
+def _hooks_converter(a: MaybeIterable[WidgetHook]) -> t.Sequence[WidgetHook]:
     return as_sequence(a)
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class PidgetGroup(abc.ABC):
     """The base pidget group."""
 
     _instance_id: uuid.UUID = attrs.field(factory=uuid.uuid4, init=False)
     """Unique ID for each instance. Enables using otherwise equal instances as hash keys"""
 
-    hooks: t.Sequence[PidgetGroupHook] = attrs.field(factory=tuple, converter=_hooks_converter)
+    hooks: t.Sequence[WidgetHook] = attrs.field(factory=tuple, converter=_hooks_converter)
     """Sequence of hooks for this instance"""
 
     @abc.abstractmethod
     def get_container(self, pidgets: t.Iterable[Pidget]) -> QWidget:
         """Wraps given pidgets in a container that is specified in each subclass"""
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,33 +208,33 @@
     limit_texts: Optional[Tuple[Optional[str], Optional[str]]] = None
 
     def __attrs_post_init__(self) -> None:
         if self.log_scale:
             if self.limits[0] <= 0:
                 raise ValueError("Lower limit must be > 0 when using log scale")
 
-    def create(self, parent: QWidget) -> FloatSliderPidget:
+    def create(self, parent: QWidget) -> FloatSliderPidget:  # type: ignore[override]
         return FloatSliderPidget(self, parent)
 
 
 class FloatSliderPidget(Pidget):
     def __init__(self, factory: FloatSliderPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
         self.__spin_box = _PidgetDoubleSpinBox(
             self._body_widget,
             limits=factory.limits,
             suffix=factory.suffix,
             decimals=factory.decimals,
         )
         self.__spin_box.valueChanged.connect(self.__on_spin_box_changed)
-        self._body_layout.addWidget(self.__spin_box, 0, 1)
+        self._body_layout.addWidget(self.__spin_box, 0, 1)  # type: ignore[call-arg]
 
         slider_widget = QWidget(self._body_widget)
-        self._body_layout.addWidget(slider_widget, 1, 0, 1, -1)
+        self._body_layout.addWidget(slider_widget, 1, 0, 1, -1)  # type: ignore[call-arg]
         slider_widget.setLayout(QHBoxLayout(slider_widget))
         slider_widget.layout().setContentsMargins(11, 6, 11, 0)
 
         lower_limit, upper_limit = factory.limits
         if factory.show_limit_values:
             slider_widget.layout().addWidget(QLabel(str(lower_limit), slider_widget))
 
@@ -248,26 +248,26 @@
         slider_widget.layout().addWidget(self._slider)
 
         if factory.show_limit_values:
             slider_widget.layout().addWidget(QLabel(str(upper_limit), slider_widget))
 
         if factory.limit_texts is not None:
             label_text_widget = QWidget(self._body_widget)
-            self._body_layout.addWidget(label_text_widget, 2, 0, 1, -1)
+            self._body_layout.addWidget(label_text_widget, 2, 0, 1, -1)  # type: ignore[call-arg]
             label_text_widget.setLayout(QHBoxLayout(label_text_widget))
             label_text_widget.layout().setContentsMargins(11, 0, 11, 0)
             label_text_widget.layout().setSpacing(0)
 
             left, right = factory.limit_texts
 
             if left is not None:
                 label = QLabel(left, label_text_widget)
                 label_text_widget.layout().addWidget(label)
 
-            label_text_widget.layout().addStretch(1)
+            label_text_widget.layout().addStretch(1)  # type: ignore[attr-defined]
 
             if right is not None:
                 label = QLabel(right, label_text_widget)
                 label_text_widget.layout().addWidget(label)
 
     def _create_body_layout(self, note_label_widget: QWidget) -> QLayout:
         """Called by Pidget.__init__"""
@@ -339,15 +339,15 @@
         pass
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalIntPidgetFactory(OptionalPidgetFactory, IntPidgetFactory):
     init_set_value: Optional[int] = None
 
-    def create(self, parent: QWidget) -> OptionalIntPidget:
+    def create(self, parent: QWidget) -> OptionalIntPidget:  # type: ignore[override]
         return OptionalIntPidget(self, parent)
 
 
 class OptionalIntPidget(OptionalPidget):
     def __init__(self, factory: OptionalIntPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
 
@@ -397,15 +397,15 @@
 
     placeholder_text: Optional[str] = None
     """
     Text that will be displayed when the checkbox is unchecked (and data is None).
     placeholder_text = None disables the placeholder text entierly
     """
 
-    def create(self, parent: QWidget) -> OptionalFloatPidget:
+    def create(self, parent: QWidget) -> OptionalFloatPidget:  # type: ignore[override]
         return OptionalFloatPidget(self, parent)
 
 
 class OptionalFloatPidget(OptionalPidget):
     _SPINBOX_INDEX = 0
     _DUMMY_INDEX = 1
 
@@ -523,17 +523,17 @@
 
         self._combobox = _PidgetComboBox(self._body_widget)
         self._body_layout.addWidget(self._combobox)
 
         for displayed_text, user_data in factory.items:
             self._combobox.addItem(displayed_text, user_data)
 
-        self._combobox.currentIndexChanged.connect(self.__emit_data_of_combobox_item)
+        self._combobox.currentIndexChanged.connect(self._emit_data_of_combobox_item)
 
-    def __emit_data_of_combobox_item(self, index: int) -> None:
+    def _emit_data_of_combobox_item(self, index: int) -> None:
         data = self._combobox.itemData(index)
         self.sig_update.emit(data)
 
     def set_data(self, param: Any) -> None:
         with QtCore.QSignalBlocker(self):
             index = self._combobox.findData(param)
             if index == -1:
@@ -550,40 +550,52 @@
     name_label_tooltip: str = attrs.field(default="The sensor to use in session")
 
     def create(self, parent: QWidget) -> SensorIdPidget:
         return SensorIdPidget(self, parent)
 
 
 class SensorIdPidget(ComboboxPidget[int]):
-    _sensor_list: list[int]
-
     def __init__(self, factory: SensorIdPidgetFactory, parent: QWidget) -> None:
         super().__init__(factory, parent)
-        self._sensor_list = []
+        self._sensor_id = 1
+        self.set_data(self._sensor_id)
+
+    def _emit_data_of_combobox_item(self, index: int) -> None:
+        data = self._combobox.itemData(index)
+
+        if data is None:
+            return
 
-    def _update_items(self, items: list[tuple[str, int]]) -> None:
-        with QtCore.QSignalBlocker(
-            self
-        ):  # Does not take into account when selected item is removed
+        self._sensor_id = data
+        self.sig_update.emit(data)
+
+    def set_selectable_sensors(self, sensor_list: list[int]) -> None:
+        with QtCore.QSignalBlocker(self):
             self._combobox.clear()
 
-            for displayed_text, user_data in items:
-                self._combobox.addItem(displayed_text, user_data)
+            for sensor_id in sensor_list:
+                self._combobox.addItem(str(sensor_id), sensor_id)
 
-    def set_selected_sensor(self, sensor_id: Optional[int], sensor_list: list[int]) -> None:
-        if sensor_list != self._sensor_list:
-            self._sensor_list = sensor_list
-            self._update_items([(str(i), i) for i in sensor_list])
+            self.set_data(self._sensor_id)
+
+        self.setEnabled(len(sensor_list) > 0)
+
+    def set_data(self, sensor_id: int) -> None:
+        self._sensor_id = sensor_id
 
         try:
             super().set_data(sensor_id)
         except ValueError:
-            self.setEnabled(False)
-        else:
-            self.setEnabled(True)
+            with QtCore.QSignalBlocker(self):
+                self._combobox.setCurrentIndex(-1)
+
+            self._combobox.setPlaceholderText(f"{self._sensor_id} (unavailable)")
+
+    def get_data(self) -> int:
+        return self._sensor_id
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class EnumPidgetFactory(ComboboxPidgetFactory[EnumT]):
     enum_type: Type[EnumT] = attrs.field()
     label_mapping: dict[EnumT, str] = attrs.field()
 
@@ -609,15 +621,15 @@
 class EnumPidget(ComboboxPidget[EnumT]):
     def __init__(self, factory: EnumPidgetFactory[EnumT], parent: QWidget) -> None:
         super().__init__(factory, parent)
 
 
 @attrs.frozen(kw_only=True, slots=False)
 class OptionalEnumPidgetFactory(OptionalPidgetFactory, EnumPidgetFactory[EnumT]):
-    def create(self, parent: QWidget) -> OptionalEnumPidget:
+    def create(self, parent: QWidget) -> OptionalEnumPidget:  # type: ignore[override]
         return OptionalEnumPidget(self, parent)
 
 
 class OptionalEnumPidget(OptionalPidget):
     def __init__(self, factory: OptionalEnumPidgetFactory[EnumT], parent: QWidget) -> None:
         super().__init__(factory, parent)
 
@@ -689,15 +701,15 @@
         init_set_value: Optional[int] = None,
         suffix: Optional[str] = None,
     ) -> None:
         super().__init__(parent)
 
         self.setKeyboardTracking(False)
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
-        self.setAlignment(QtCore.Qt.AlignRight)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
         self.setFixedWidth(_WIDGET_WIDTH)
 
         self.setRange(*_convert_int_limits_to_qt_range(limits))
 
         if suffix:
             self.setSuffix(f" {suffix}")
 
@@ -721,15 +733,15 @@
         decimals: int = 1,
         suffix: Optional[str] = None,
     ) -> None:
         super().__init__(parent)
 
         self.setKeyboardTracking(False)
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
-        self.setAlignment(QtCore.Qt.AlignRight)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
         self.setFixedWidth(_WIDGET_WIDTH)
 
         self.setRange(*_convert_float_limits_to_qt_range(limits))
         self.setDecimals(decimals)
         self.setSingleStep(10 ** (-decimals))
 
         if suffix:
@@ -766,15 +778,15 @@
         self,
         parent: QWidget,
         *,
         limits: Tuple[float, float],
         decimals: int,
         log_scale: bool,
     ) -> None:
-        super().__init__(QtCore.Qt.Horizontal, parent)
+        super().__init__(QtCore.Qt.Orientation.Horizontal, parent)
 
         self.limits = limits
         self.decimals = decimals
         self.log_scale = log_scale
 
         self.setRange(0, self.NUM_STEPS)
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         layout.addWidget(QLabel("End", self), 0, 1)
         layout.addWidget(self._end, 1, 1)
 
         self._step = RangeHelpViewValueWidget(self)
         layout.addWidget(QLabel("Step", self), 0, 2)
         layout.addWidget(self._step, 1, 2)
 
-        self.update(None)
+        self.set_data(None)
 
-    def update(self, subsweep_config: Optional[a121.SubsweepConfig]) -> None:
+    def set_data(self, subsweep_config: Optional[a121.SubsweepConfig]) -> None:
         if subsweep_config:
             end_point = (
                 subsweep_config.start_point
                 + (subsweep_config.num_points - 1) * subsweep_config.step_length
             )
             start_m = subsweep_config.start_point * self.APPROX_BASE_STEP_LENGTH_M
             end_m = end_point * self.APPROX_BASE_STEP_LENGTH_M
@@ -55,8 +55,8 @@
             self._end.clear()
 
 
 class RangeHelpViewValueWidget(QLineEdit):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
         self.setEnabled(False)
-        self.setAlignment(QtCore.Qt.AlignRight)
+        self.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     @classmethod
     def get_save_file_name(
         cls,
         model: t.Any,
         presenter: PresenterFunc,
         caption: str = "",
         filter: str = "All (*)",
-        options: QFileDialog.Option = QFileDialog.Option(),
+        options: QFileDialog.Option = QFileDialog.Option.DontUseNativeDialog,
         parent: t.Optional[QWidget] = None,
     ) -> t.Optional[str]:
         dialog = QFileDialog(caption=caption)
         dialog.setAcceptMode(QFileDialog.AcceptMode.AcceptSave)
         dialog.setNameFilter(filter)
         dialog.setOptions(options)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/preview.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/save_dialog/set_config_presenter.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self._update_rate_erroneous = False
 
         self.setLayout(QVBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         self.session_group_box = GroupBox.vertical(
             "Session parameters",
-            JsonSaveLoadButtons.from_editor_and_config_type(self, a121.SessionConfig),
+            JsonSaveLoadButtons.from_editor_and_config_type(self, a121.SessionConfig),  # type: ignore[arg-type]
             parent=self,
         )
         self.session_group_box.layout().setSpacing(self.SPACING)
         self.layout().addWidget(self.session_group_box)
 
         self._sensor_id_pidget = pidgets.SensorIdPidgetFactory(items=[]).create(self)
         self._sensor_id_pidget.sig_update.connect(self._update_sole_sensor_id)
@@ -75,16 +75,16 @@
         self._update_rate_pidget.sig_update.connect(self._update_update_rate)
         self.session_group_box.layout().addWidget(self._update_rate_pidget)
 
         self._sensor_config_editor = SensorConfigEditor(supports_multiple_subsweeps, self)
         self._sensor_config_editor.sig_update.connect(self._update_sole_sensor_config)
         self.layout().addWidget(self._sensor_config_editor)
 
-    def set_selected_sensor(self, sensor_id: Optional[int], sensor_list: list[int]) -> None:
-        self._sensor_id_pidget.set_selected_sensor(sensor_id, sensor_list)
+    def set_selectable_sensors(self, sensor_list: list[int]) -> None:
+        self._sensor_id_pidget.set_selectable_sensors(sensor_list)
 
     def set_read_only(self, read_only: bool) -> None:
         self._sensor_id_pidget.setEnabled(not read_only)
         self._update_rate_pidget.setEnabled(not read_only)
         self._sensor_config_editor.set_read_only(read_only)
 
     def set_data(self, session_config: Optional[a121.SessionConfig]) -> None:
@@ -94,14 +94,15 @@
         self._session_config = session_config
         self.setEnabled(session_config is not None)
 
         if self._session_config is None:
             log.debug("could not update ui as SessionConfig is None")
             return
 
+        self._sensor_id_pidget.set_data(self._session_config.sensor_id)
         self._update_rate_pidget.set_data(self._session_config.update_rate)
         self._sensor_config_editor.set_data(self._session_config.sensor_config)
 
     def get_data(self) -> Optional[a121.SessionConfig]:
         return copy.deepcopy(self._session_config)
 
     def handle_validation_results(
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         for pidget in self._subsweep_config_pidgets.values():
             pidget.setEnabled(not read_only)
 
     def set_data(self, subsweep_config: Optional[a121.SubsweepConfig]) -> None:
         if self._subsweep_config == subsweep_config:
             return
 
-        self.range_help_view.update(subsweep_config)
+        self.range_help_view.set_data(subsweep_config)
         self._subsweep_config = subsweep_config
 
         self.setEnabled(self._subsweep_config is not None)
         if self._subsweep_config is None:
             log.debug("could not update ui as SubsweepConfig is None")
             return
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
-import typing as t
-
 from PySide6.QtCore import Signal
 from PySide6.QtWidgets import QHBoxLayout, QWidget
 
 from . import pidgets
 
 
 class TwoSensorIdsEditor(QWidget):
 
     sig_update = Signal(object)
-    sensor_ids: t.Optional[list[int]]
 
     def __init__(self, name_label_texts: list[str]):
         super().__init__()
 
         self._sensor_id_pidget_1 = pidgets.SensorIdPidgetFactory(
             name_label_text=name_label_texts[0], items=[]
         ).create(self)
@@ -28,28 +25,25 @@
 
         self.setLayout(QHBoxLayout(self))
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         self.layout().addWidget(self._sensor_id_pidget_1)
         self.layout().addWidget(self._sensor_id_pidget_2)
 
-        self._sensor_id_pidget_1.sig_update.connect(
-            lambda sensor_id: self.handle_pidget_signal(sensor_id, sensor_id_position=0)
-        )
-        self._sensor_id_pidget_2.sig_update.connect(
-            lambda sensor_id: self.handle_pidget_signal(sensor_id, sensor_id_position=1)
-        )
-        self.sensor_ids = None
-
-    def set_selected_sensors(
-        self, sensor_ids: t.Optional[list[int]], sensor_list: list[int]
-    ) -> None:
-        if sensor_ids:
-            assert len(sensor_ids) == 2
-            self.sensor_ids = sensor_ids
-            self._sensor_id_pidget_1.set_selected_sensor(sensor_ids[0], sensor_list)
-            self._sensor_id_pidget_2.set_selected_sensor(sensor_ids[1], sensor_list)
-
-    def handle_pidget_signal(self, sensor_id: int, sensor_id_position: int) -> None:
-        if self.sensor_ids is not None:
-            self.sensor_ids[sensor_id_position] = sensor_id
-            self.sig_update.emit(self.sensor_ids)
+        self._sensor_id_pidget_1.sig_update.connect(lambda: self.sig_update.emit(self.sensor_ids))
+        self._sensor_id_pidget_2.sig_update.connect(lambda: self.sig_update.emit(self.sensor_ids))
+
+    @property
+    def sensor_ids(self) -> list[int]:
+        return [
+            self._sensor_id_pidget_1.get_data(),
+            self._sensor_id_pidget_2.get_data(),
+        ]
+
+    def set_data(self, sensor_ids: list[int]) -> None:
+        assert len(sensor_ids) == 2
+        self._sensor_id_pidget_1.set_data(sensor_ids[0])
+        self._sensor_id_pidget_2.set_data(sensor_ids[1])
+
+    def set_selectable_sensors(self, sensor_list: list[int]) -> None:
+        self._sensor_id_pidget_1.set_selectable_sensors(sensor_list)
+        self._sensor_id_pidget_2.set_selectable_sensors(sensor_list)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/plugin_components/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/plugin_components/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 import typing as t
 
 from PySide6.QtCore import QPoint, QRect
 from PySide6.QtGui import QResizeEvent
 from PySide6.QtWidgets import QFrame, QGridLayout, QLabel, QLayout, QVBoxLayout, QWidget
 
 
-class GroupBox(QWidget):
+_T = t.TypeVar("_T", bound=QLayout)
+
+
+class GroupBox(QWidget, t.Generic[_T]):
     _HORIZONTAL_HEADER_MARGIN = 7
     _EXTRA_MARGIN_TO_AVOID_CLIPPING = 2
 
     class _Position(enum.Enum):
         LEFT = enum.auto()
         RIGHT = enum.auto()
 
     def __init__(
         self,
         left_header: t.Union[QWidget, str],
-        layout_type: t.Type[QLayout],
+        layout_type: t.Type[_T],
         right_header: t.Optional[QWidget] = None,
         *,
         parent: t.Optional[QWidget] = None,
     ) -> None:
         super().__init__()
         self.setLayout(QVBoxLayout())
 
@@ -50,30 +53,30 @@
     @classmethod
     def vertical(
         cls,
         left_header: t.Union[QWidget, str],
         right_header: t.Optional[QWidget] = None,
         *,
         parent: t.Optional[QWidget] = None,
-    ) -> GroupBox:
-        return cls(left_header, QVBoxLayout, right_header=right_header, parent=parent)
+    ) -> GroupBox[QVBoxLayout]:
+        return cls(left_header, QVBoxLayout, right_header=right_header, parent=parent)  # type: ignore[return-value,arg-type]
 
     @classmethod
     def grid(
         cls,
         left_header: t.Union[QWidget, str],
         right_header: t.Optional[QWidget] = None,
         *,
         parent: t.Optional[QWidget] = None,
-    ) -> GroupBox:
-        return cls(left_header, QGridLayout, right_header=None, parent=parent)
+    ) -> GroupBox[QGridLayout]:
+        return cls(left_header, QGridLayout, right_header=None, parent=parent)  # type: ignore[return-value,arg-type]
 
-    def layout(self) -> QLayout:
+    def layout(self) -> _T:
         """Returns the layout of the internal QFrame"""
-        return self._frame.layout()
+        return self._frame.layout()  # type: ignore[return-value]
 
     @staticmethod
     def _wrap_in_frame(widget: QWidget, frame_parent: t.Optional[QWidget] = None) -> QFrame:
         """
         Header widgets are wrapped in a frame to
         make sure the header widgets have an opaque background
         """
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import itertools
 import threading
-from typing import Optional
+from typing import Iterator, Optional
 
 import numpy as np
-import qtawesome as qta
 
 from PySide6 import QtCore
-from PySide6.QtGui import QPainter, QPaintEvent, QTextDocument
+from PySide6.QtGui import QTextDocument
 from PySide6.QtWidgets import (
-    QHBoxLayout,
+    QDialog,
     QLabel,
-    QMainWindow,
+    QPushButton,
     QStatusBar,
-    QStyle,
-    QStyleOption,
     QTextBrowser,
+    QVBoxLayout,
     QWidget,
 )
 
 import acconeer.exptool
 from acconeer.exptool.app.new import check_package_outdated, get_latest_changelog
 from acconeer.exptool.app.new.app_model import AppModel
 from acconeer.exptool.utils import get_module_version  # type: ignore[import]
@@ -164,135 +163,135 @@
                 tooltip = ""
 
         self.setToolTip(tooltip)
         self.setStyleSheet(f"QWidget{{{css}}}")
         self.setText(text)
 
 
-class VersionLabel(QWidget):
-    sig_version_outdated = QtCore.Signal()
+class VersionButton(QPushButton):
+    sig_payload = QtCore.Signal(
+        tuple
+    )  # tuple[changelog (str), latest version (str), outdated? (bool)]
 
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
-        self.parent = parent
-        h_layout = QHBoxLayout()
-        self.setLayout(h_layout)
-        h_layout.setContentsMargins(0, 0, 0, 0)
-        h_layout.setSpacing(0)
-
         et_version = get_module_version(acconeer.exptool)
-        et_version_text = f"ET: {et_version}"
-        et_version_label = QLabel(et_version_text, self)
-        h_layout.addWidget(et_version_label)
-
-        def version_check(et_version: str) -> None:
-            version_outdated, latest_v = check_package_outdated("acconeer-exptool", et_version)
-            self.changelog = None
-
-            if version_outdated:
-                self.changelog = get_latest_changelog()
-                self.setStyleSheet(
-                    f"QWidget{{background-color: {BUTTON_ICON_COLOR}; color: #e2e2e2}}"
-                )
-
-                self.setToolTip(
-                    "There is a new software version available!\n"
-                    f"The latest version is: {latest_v}. \n"
-                    "Click to view changelog."
-                )
-                self.sig_version_outdated.emit()
-                self.mousePressEvent = self._toggle_changelog
-
-        self.sig_version_outdated.connect(self._create_changelog_window)
-        self.sig_version_outdated.connect(lambda: self._add_icon_to_version_label(self))
-
-        version_thread = threading.Thread(target=lambda: version_check(et_version))
-        version_thread.start()
-
-    def _create_changelog_window(self) -> None:
-        if self.changelog is not None:
-            self.cl_window = ChangelogWindow(self)
-            self.cl_window.set_text(self.changelog)
-
-    def _add_icon_to_version_label(self, version_widget: QWidget) -> None:
-        layout = version_widget.layout()
-        icon_widget = qta.IconWidget()
-        icon_widget.setIcon(REFRESH(color="#e2e2e2"))
-        layout.addWidget(icon_widget)
-
-    def _toggle_changelog(self, label: QLabel) -> None:
-        if self.changelog is not None:
-            self.cl_window.setVisible(not self.cl_window.isVisible())
-
-    def paintEvent(self, pe: QPaintEvent) -> None:
-        o = QStyleOption()
-        o.initFrom(self)
-        p = QPainter(self)
-        self.style().drawPrimitive(QStyle.PE_Widget, o, p, self)
+        self._changelog_text: Optional[str] = None
+
+        self.setFlat(True)
+        self.setText(f"ET: {et_version}")
+
+        self.clicked.connect(self._on_click)
+        self.sig_payload.connect(self._handle_payload)
+
+        self._version_thread = threading.Thread(target=lambda: self._get_payload(et_version))
+        self._version_thread.start()
+
+    def _on_click(self) -> None:
+        if self._changelog_text is None:
+            return
+
+        ChangelogDialog(markdown_text=self._changelog_text).exec()
+
+    def _handle_payload(self, payload: tuple[str, str, bool]) -> None:
+        (changelog_text, latest_version, is_outdated) = payload
+
+        if not is_outdated:
+            return
+
+        self._changelog_text = changelog_text
+
+        self.setIcon(REFRESH(color="#e2e2e2"))
+        self.setStyleSheet(
+            f"QPushButton{{ background-color: {BUTTON_ICON_COLOR}; color: #e2e2e2; }}"
+        )
+        self.setToolTip(
+            "There is a new software version available!\n"
+            f"The latest version is: {latest_version}. \n"
+            "Click to view changelog."
+        )
+
+    def _get_payload(self, et_version: str) -> None:
+        is_outdated, latest_version = check_package_outdated("acconeer-exptool", et_version)
+        self.sig_payload.emit((get_latest_changelog(), latest_version, is_outdated))
 
 
 class StatusBar(QStatusBar):
+    MAX_DISPLAY_TIME_MS = 3000
+
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(parent)
 
-        self.parent = parent
+        self._status_messages: list[str] = []
 
-        app_model.sig_status_message.connect(self._on_app_model_status_message)
+        app_model.sig_status_message.connect(lambda m: self._status_messages.append(m))
+        app_model.sig_status_message.connect(self._trigger_display)
 
         self.message_timer = QtCore.QTimer(self)
-        self.message_timer.setInterval(3000)
+        self.message_timer.setInterval(self.MAX_DISPLAY_TIME_MS)
         self.message_timer.setSingleShot(True)
-        self.message_timer.timeout.connect(self._on_timer)
+        self.message_timer.timeout.connect(self._trigger_display)
 
         self.message_widget = QLabel(self)
         self.addWidget(self.message_widget)
 
         self.addPermanentWidget(FrameCountLabel(app_model, self))
         self.addPermanentWidget(RateStatsLabel(app_model, self))
         self.addPermanentWidget(JitterStatsLabel(app_model, self))
         self.addPermanentWidget(BackendCPUPercentLabel(app_model, self))
         self.addPermanentWidget(RSSVersionLabel(app_model, self))
-        self.addPermanentWidget(VersionLabel(app_model, self))
+        self.addPermanentWidget(VersionButton(app_model, self))
 
         font_families = [
             "Consolas",  # Windows
             "Droid Sans Mono",  # Ubuntu
             "DejaVu Sans Mono",  # Ubuntu, backup
             "SF Mono",  # Mac
         ]
         font_family = ", ".join(f'"{ff}"' for ff in font_families)
         self.setStyleSheet(f"QWidget{{font-family: {font_family};}}")
 
-    def _on_app_model_status_message(self, message: Optional[str]) -> None:
-        self.message_timer.stop()
+    def _trigger_display(self) -> None:
+        if self.message_timer.isActive():
+            return
 
-        if message:
-            self.message_widget.setText(message)
-            self.message_timer.start()
+        if self._status_messages:
+            (message, occurances) = next(self._rle_status_messages)
+
+            if occurances > 1:
+                self.message_widget.setText(f"{message} (x{occurances})")
+            else:
+                self.message_widget.setText(message)
+
+            self._status_messages = self._status_messages[occurances:]
+            self.message_timer.start(self._message_display_time)
         else:
             self.message_widget.clear()
 
-    def _on_timer(self) -> None:
-        self.message_widget.clear()
-
+    @property
+    def _rle_status_messages(self) -> Iterator[tuple[str, int]]:
+        return (
+            (message, len(list(group)))
+            for message, group in itertools.groupby(self._status_messages)
+        )
+
+    @property
+    def _message_display_time(self) -> int:
+        num_messages = len(list(self._rle_status_messages))
+        return int(self.MAX_DISPLAY_TIME_MS / (1 + 2 ** (num_messages - 5)))
 
-class ChangelogWindow(QMainWindow):
-    def __init__(self, parent: QWidget = None) -> None:
-        super().__init__()
 
-        self.setWindowTitle("Changelog")
-        self.text_browser = QTextBrowser()
-        self.setCentralWidget(self.text_browser)
-        self.set_center(parent.parent.parent)
-        self.showEvent = lambda _: self.set_center(parent.parent.parent)
+class ChangelogDialog(QDialog):
+    def __init__(self, markdown_text: str, parent: Optional[QWidget] = None) -> None:
+        super().__init__(parent)
 
-    def set_text(self, text: str) -> None:
         document = QTextDocument()
-        document.setMarkdown(text)
-        self.text_browser.setDocument(document)
+        document.setMarkdown(markdown_text)
+
+        text_browser = QTextBrowser(self)
+        text_browser.setDocument(document)
+        text_browser.setMinimumWidth(round(document.idealWidth() * 1.1))
+        text_browser.setMinimumHeight(500)
 
-    def set_center(self, main_window: QMainWindow) -> None:
-        fg = self.frameGeometry()
-        fg.moveCenter(main_window.geometry().center())
-        self.move(fg.topLeft())
-        self.resize(500, 400)
+        self.setLayout(QVBoxLayout())
+        self.layout().addWidget(text_browser)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         self.layout().setContentsMargins(0, 0, 0, 0)
 
         self.layout().addWidget(SerialPortComboBox(app_model, self))
 
 
 class _ConnectSettingsButton(QPushButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
-        super().__init__(parent, flat=True)
+        super().__init__(parent)
+        self.setFlat(True)
         self.app_model = app_model
 
         self.setIcon(COG())
         self.setToolTip("Advanced settings")
 
         self.settings_dialog = _ConnectSettingsDialog(app_model, self)
 
@@ -214,41 +215,42 @@
 
 class ClientConnectionWidget(AppModelAwareWidget):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(app_model, parent)
 
         self.app_model = app_model
 
-        self.setLayout(QHBoxLayout(self))
-        self.layout().setContentsMargins(0, 0, 0, 0)
+        layout = QHBoxLayout(self)
+        layout.setContentsMargins(0, 0, 0, 0)
 
         self.interface_dd = QComboBox(self)
         self.interface_dd.setMinimumWidth(110)
 
-        self.layout().addWidget(self.interface_dd)
+        layout.addWidget(self.interface_dd)
 
         self.interface_dd.addItem("Socket", userData=ConnectionInterface.SOCKET)
         self.interface_dd.addItem("Serial", userData=ConnectionInterface.SERIAL)
         self.interface_dd.addItem("USB", userData=ConnectionInterface.USB)
         self.interface_dd.addItem("Simulated", userData=ConnectionInterface.SIMULATED)
 
         self.interface_dd.currentIndexChanged.connect(self._on_interface_dd_change)
 
         self.stacked = QStackedWidget(self)
         self.stacked.setStyleSheet("QStackedWidget {background-color: transparent;}")
         self.stacked.addWidget(_SocketConnectionWidget(app_model, self.stacked))
         self.stacked.addWidget(_SerialConnectionWidget(app_model, self.stacked))
         self.stacked.addWidget(USBDeviceComboBox(app_model, self.stacked))
         self.stacked.addWidget(_SimulatedConnectionWidget(app_model, self.stacked))
-        self.layout().addWidget(self.stacked)
+        layout.addWidget(self.stacked)
 
-        self.layout().addWidget(_ConnectSettingsButton(app_model, self))
-        self.layout().addWidget(_ConnectAndDisconnectButton(app_model, self))
+        layout.addWidget(_ConnectSettingsButton(app_model, self))
+        layout.addWidget(_ConnectAndDisconnectButton(app_model, self))
 
-        self.layout().addStretch(1)
+        layout.addStretch(1)
+        self.setLayout(layout)
 
     def _on_interface_dd_change(self) -> None:
         self.app_model.set_connection_interface(self.interface_dd.currentData())
 
     def on_app_model_update(self, app_model: AppModel) -> None:
         self.stacked.setEnabled(
             app_model.connection_state == ConnectionState.DISCONNECTED,
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,27 +59,24 @@
 
 class PluginSelectionButtonGroup(QButtonGroup):
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
 
         self.setExclusive(True)
 
-    def addButton(self, button: PluginSelectionButton) -> None:
-        super().addButton(button)
-
     def checkedButton(self) -> PluginSelectionButton:
         button = super().checkedButton()
         assert isinstance(button, PluginSelectionButton)
         return button
 
-    def buttons(self) -> list[PluginSelectionButton]:
+    def buttons(self) -> list[PluginSelectionButton]:  # type: ignore[override]
         buttons = super().buttons()
         assert isinstance(buttons, list)
         assert all(isinstance(e, PluginSelectionButton) for e in buttons)
-        return buttons
+        return buttons  # type: ignore[return-value]
 
 
 class PluginPresetButton(QPushButton):
     def __init__(self, plugin_preset: PluginPresetSpec, default: bool, parent: QWidget) -> None:
         super().__init__(parent)
 
         if default:
@@ -172,14 +169,17 @@
 
             if plugin.description:
                 label = QLabel(group_box)
                 label.setText(plugin.description)
                 label.setWordWrap(True)
                 group_box.layout().addWidget(label)
 
+    def layout(self) -> QVBoxLayout:
+        return super().layout()  # type: ignore[return-value]
+
     def _on_load_click(self) -> None:
         self.layout().addStretch(1)
 
         plugin = self.button_group.checkedButton().plugin
         self.app_model.load_plugin(plugin)
 
     def _on_app_model_update(self, app_model: AppModel) -> None:
@@ -211,44 +211,47 @@
         self.layout().addWidget(PluginPresetPlaceholder(app_model, self))
 
 
 class PlotPlaceholder(QWidget):
     def __init__(self, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
 
-        self.setLayout(QVBoxLayout(self))
-        self.layout().addStretch(1)
-        self.layout().addLayout(self._select_module_text())
-        self.layout().addWidget(self._teaser_text())
-        self.layout().addStretch(1)
+        layout = QVBoxLayout(self)
+
+        layout.addStretch(1)
+        layout.addLayout(self._select_module_text())
+        layout.addWidget(self._teaser_text())
+        layout.addStretch(1)
+
+        self.setLayout(layout)
 
     def _select_module_text(self) -> QHBoxLayout:
         h_box = QHBoxLayout()
         h_box.addStretch(1)
 
         icon_widget = qta.IconWidget()
         icon_widget.setIconSize(QtCore.QSize(36, 36))
         icon_widget.setIcon(ARROW_LEFT_BOLD(color="#4d5157"))
 
         label = QLabel("Select a module to begin", self)
         label.setStyleSheet("font-size: 20px;")
-        label.setAlignment(QtCore.Qt.AlignCenter)
+        label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
         h_box.addWidget(icon_widget)
         h_box.addWidget(label)
         h_box.addStretch(1)
 
         return h_box
 
     def _teaser_text(self) -> QLabel:
         teaser_label = QLabel(
             "More detectors and example applications will\nbe released continuously.", self
         )
         teaser_label.setStyleSheet("font-size: 16px;")
-        teaser_label.setAlignment(QtCore.Qt.AlignCenter)
+        teaser_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
         return teaser_label
 
 
 class PluginPlotArea(QFrame):
     _FPS = 60
 
@@ -293,15 +296,15 @@
 
         if plugin is None:
             self.child_widget = PlotPlaceholder()
         else:
             self.child_widget = pg.GraphicsLayoutWidget()
             self.plot_plugin = plugin.create_plot_plugin(
                 app_model=self.app_model,
-                plot_layout=self.child_widget.ci,
+                plot_layout=self.child_widget.ci,  # type: ignore[attr-defined]
             )
 
         self.layout().addWidget(self.child_widget)
 
 
 class ControlPlaceholder(QWidget):
     def __init__(self, parent: Optional[QWidget] = None) -> None:
@@ -309,15 +312,15 @@
 
         self.setLayout(QGridLayout(self))
 
         with importlib.resources.path(resources, "icon-black.svg") as path:
             icon = QSvgWidget(str(path), self)
 
         icon.setMaximumSize(60, 60)
-        icon.renderer().setAspectRatioMode(QtCore.Qt.KeepAspectRatio)
+        icon.renderer().setAspectRatioMode(QtCore.Qt.AspectRatioMode.KeepAspectRatio)
         effect = QGraphicsOpacityEffect(icon)
         effect.setOpacity(0.1)
         icon.setGraphicsEffect(effect)
 
         self.layout().addWidget(icon)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 
     def _on_app_model_update(self, app_model: AppModel) -> None:
         self.setChecked(app_model.recording_enabled)
         self.setEnabled(app_model.plugin_state.is_steady)
 
 
 class FileButton(QPushButton):
+    """A practically abstract class (cannot be abstract due to meta class conflict)"""
+
     def __init__(
         self,
         app_model: AppModel,
         text: str,
         icon: QtGui.QIcon,
         shortcut: Optional[str],
         tooltip: Optional[str],
@@ -74,14 +76,17 @@
         if tooltip is not None:
             self.setToolTip(tooltip)
 
         self.clicked.connect(self._on_click)
 
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
+    def _on_click(self) -> None:
+        raise NotImplementedError
+
 
 class LoadFileButton(FileButton):
     def __init__(self, app_model: AppModel, parent: QWidget) -> None:
         super().__init__(
             app_model,
             "Load from file",
             FOLDER_OPEN(),
@@ -95,15 +100,15 @@
         self.setEnabled(app_model.plugin_state.is_steady)
 
     def _on_click(self) -> None:
         filename, _ = QFileDialog.getOpenFileName(
             self,
             caption="Load from file",
             filter=_file_suffix_to_filter(".h5", ".npz"),
-            options=QFileDialog.DontUseNativeDialog,
+            options=QFileDialog.Option.DontUseNativeDialog,
         )
 
         if not filename:
             return
 
         self.app_model.load_from_file(Path(filename))
 
@@ -127,15 +132,15 @@
         if self.app_model.saveable_file is None:
             raise RuntimeError
 
         filename, _ = QFileDialog.getSaveFileName(
             self,
             caption="Save to file",
             filter=_file_suffix_to_filter(self.app_model.saveable_file.suffix),
-            options=QFileDialog.DontUseNativeDialog,
+            options=QFileDialog.Option.DontUseNativeDialog,
         )
 
         if not filename:
             return
 
         path = Path(filename)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 class ScrollAreaDecorator(QScrollArea):
     def __init__(self, decoratee: QWidget) -> None:
         """Puts `decoratee` in a frameless QScrollArea with no horizontal scroll."""
         super().__init__()
 
         self.setWidgetResizable(True)
-        self.setFrameShape(QFrame.NoFrame)
-        self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.setFrameShape(QFrame.Shape.NoFrame)
+        self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.horizontalScrollBar().setEnabled(False)
 
         self.setWidget(decoratee)
 
 
 class TopAlignDecorator(QWidget):
     def __init__(self, decoratee: QWidget) -> None:
@@ -39,8 +39,8 @@
         super().__init__()
         self.setLayout(wrappee)
 
 
 class HorizontalSeparator(QFrame):
     def __init__(self, parent: Optional[QWidget] = None) -> None:
         super().__init__(parent)
-        self.setFrameShape(QFrame.HLine)
+        self.setFrameShape(QFrame.Shape.HLine)
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.2.1/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.2.1/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.2.1/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.2.0
+Version: 7.2.1
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
@@ -65,14 +65,15 @@
 ## News
 
 * v6.0.0 released. See the [Changelog](https://docs.acconeer.com/en/latest/changelog.html).
 
 ## Setting up your evaluation kit
 
 * [XC120 + XE121 (A121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xc120_xe121.html)
+* [Raspberry Pi (A121 on XE121)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a121_xe121.html)
 * [Raspberry Pi (A111 on XC111+XR111 or XC112+XR112)](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/raspberry_a111.html)
 * [XM112](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm112.html)
 * [XM122](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm122.html)
 * [XM132](https://docs.acconeer.com/en/latest/exploration_tool/evk_setup/xm132.html)
 
 For additional resources, head over to the [Acconeer developer page](https://developer.acconeer.com/). There you will find both a getting started guide and a video showing you how to set up your evaluation kit. There you will also find the SDK download.
```

### Comparing `acconeer-exptool-7.2.0/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.2.1/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -298,66 +298,59 @@
 src/acconeer/exptool/a121/algo/bilateration/_plugin.py
 src/acconeer/exptool/a121/algo/bilateration/_processor.py
 src/acconeer/exptool/a121/algo/breathing/__init__.py
 src/acconeer/exptool/a121/algo/breathing/_configs.py
 src/acconeer/exptool/a121/algo/breathing/_processor.py
 src/acconeer/exptool/a121/algo/breathing/_ref_app.py
 src/acconeer/exptool/a121/algo/breathing/_ref_app_plugin.py
-src/acconeer/exptool/a121/algo/breathing/_serializer.py
 src/acconeer/exptool/a121/algo/distance/__init__.py
 src/acconeer/exptool/a121/algo/distance/__main__.py
 src/acconeer/exptool/a121/algo/distance/_aggregator.py
 src/acconeer/exptool/a121/algo/distance/_configs.py
 src/acconeer/exptool/a121/algo/distance/_detector.py
 src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
 src/acconeer/exptool/a121/algo/distance/_processors.py
-src/acconeer/exptool/a121/algo/distance/_serializers.py
 src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
 src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
 src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
 src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
 src/acconeer/exptool/a121/algo/presence/__init__.py
 src/acconeer/exptool/a121/algo/presence/_configs.py
 src/acconeer/exptool/a121/algo/presence/_detector.py
 src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
 src/acconeer/exptool/a121/algo/presence/_processors.py
-src/acconeer/exptool/a121/algo/presence/_serializers.py
 src/acconeer/exptool/a121/algo/smart_presence/__init__.py
 src/acconeer/exptool/a121/algo/smart_presence/_configs.py
 src/acconeer/exptool/a121/algo/smart_presence/_processor.py
 src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
 src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
-src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
 src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
 src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
 src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
 src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
-src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
 src/acconeer/exptool/a121/algo/speed/__init__.py
 src/acconeer/exptool/a121/algo/speed/_configs.py
 src/acconeer/exptool/a121/algo/speed/_detector.py
 src/acconeer/exptool/a121/algo/speed/_detector_plugin.py
 src/acconeer/exptool/a121/algo/speed/_processors.py
 src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
 src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
 src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
 src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
 src/acconeer/exptool/a121/algo/tank_level/__init__.py
 src/acconeer/exptool/a121/algo/tank_level/_configs.py
 src/acconeer/exptool/a121/algo/tank_level/_plugin.py
 src/acconeer/exptool/a121/algo/tank_level/_processor.py
 src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
-src/acconeer/exptool/a121/algo/tank_level/_serializer.py
 src/acconeer/exptool/a121/algo/touchless_button/__init__.py
 src/acconeer/exptool/a121/algo/touchless_button/__main__.py
 src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
 src/acconeer/exptool/a121/algo/touchless_button/_configs.py
 src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
 src/acconeer/exptool/a121/algo/touchless_button/_processor.py
-src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
 src/acconeer/exptool/a121/algo/vibration/__init__.py
 src/acconeer/exptool/a121/algo/vibration/__main__,py
 src/acconeer/exptool/a121/algo/vibration/_plugin.py
 src/acconeer/exptool/a121/algo/vibration/_processor.py
 src/acconeer/exptool/app/__init__.py
 src/acconeer/exptool/app/__main__.py
 src/acconeer/exptool/app/launcher.py
@@ -469,14 +462,21 @@
 src/acconeer/exptool/flash/_stm32uart/__init__.py
 src/acconeer/exptool/flash/_stm32uart/_meta.py
 src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
 src/acconeer/exptool/flash/_xc120/__init__.py
 src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
 src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
 src/acconeer/exptool/flash/_xc120/_meta.py
+src/acconeer/exptool/opser/__init__.py
+src/acconeer/exptool/opser/api.py
+src/acconeer/exptool/opser/builtin_persistors.py
+src/acconeer/exptool/opser/core.py
+src/acconeer/exptool/opser/optimizing_persistors.py
+src/acconeer/exptool/opser/py.typed
+src/acconeer/exptool/opser/registry_persistor.py
 src/acconeer/exptool/setup/__init__.py
 src/acconeer/exptool/setup/__main__.py
 src/acconeer/exptool/setup/py.typed
 src/acconeer/exptool/setup/base/__init__.py
 src/acconeer/exptool/setup/base/platform_install.py
 src/acconeer/exptool/setup/base/prompts.py
 src/acconeer/exptool/setup/base/setup_group.py
```

### Comparing `acconeer-exptool-7.2.0/tools/check_changelog.py` & `acconeer-exptool-7.2.1/tools/check_changelog.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/check_copyright.py` & `acconeer-exptool-7.2.1/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/check_line_length.py` & `acconeer-exptool-7.2.1/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/check_permissions.py` & `acconeer-exptool-7.2.1/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/check_sdk_mentions.py` & `acconeer-exptool-7.2.1/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/check_whitespace.py` & `acconeer-exptool-7.2.1/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/tools/update_regmap.py` & `acconeer-exptool-7.2.1/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.2.0/utils/convert_to_csv.py` & `acconeer-exptool-7.2.1/utils/convert_to_csv.py`

 * *Files identical despite different names*

