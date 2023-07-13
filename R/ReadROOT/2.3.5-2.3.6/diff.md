# Comparing `tmp/ReadROOT-2.3.5.tar.gz` & `tmp/ReadROOT-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadROOT-2.3.5.tar", last modified: Wed Jul 12 20:54:32 2023, max compression
+gzip compressed data, was "ReadROOT-2.3.6.tar", last modified: Thu Jul 13 15:06:44 2023, max compression
```

## Comparing `ReadROOT-2.3.5.tar` & `ReadROOT-2.3.6.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:32.316802 ReadROOT-2.3.5/
--rw-rw-rw-   0        0        0    16128 2023-02-15 23:51:19.000000 ReadROOT-2.3.5/ErrorPropagation.py
--rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.3.5/IOClasses.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:31.492792 ReadROOT-2.3.5/Images/
--rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Calculate.png
--rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Clear.png
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:31.823802 ReadROOT-2.3.5/Images/CoMPASS/
--rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.3.5/Images/CoMPASS/Coincidence.png
--rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.3.5/Images/CoMPASS/Discriminator.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.3.5/Images/CoMPASS/EnergyCalibration.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.3.5/Images/CoMPASS/Input.png
--rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.3.5/Images/CoMPASS/Misc.png
--rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/CoMPASS/OpenGraph.png
--rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.3.5/Images/CoMPASS/QDC.png
--rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.3.5/Images/CoMPASS/Rejections.png
--rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.3.5/Images/CoMPASS/Spectra.png
--rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.3.5/Images/CoMPASS/Sync.png
--rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/CoMPASS/icon64x64.ico
--rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.3.5/Images/CoMPASS/icon64x64.png
--rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.3.5/Images/CompClear.png
--rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.3.5/Images/Disabled0.png
--rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.3.5/Images/Disabled1.png
--rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.3.5/Images/Disabled2.png
--rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.3.5/Images/Disabled3.png
--rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.3.5/Images/DisabledSelect.png
--rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.3.5/Images/DisabledSelectROI.png
--rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/EnergyHist.png
--rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.3.5/Images/EnergyvsEnergyHist.png
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:32.152797 ReadROOT-2.3.5/Images/Log/
--rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.3.5/Images/Log/0.png
--rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.3.5/Images/Log/1.png
--rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.3.5/Images/Log/2.png
--rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.3.5/Images/Log/3.png
--rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.3.5/Images/Log/4.png
--rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.3.5/Images/Log/5.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.3.5/Images/Log/6.png
--rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.3.5/Images/Log/7.png
--rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.3.5/Images/Log/8.png
--rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.3.5/Images/Log/9+.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.3.5/Images/Log/9.png
--rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/MCS Graph.png
--rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Off0.png
--rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Off1.png
--rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Off2.png
--rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Off3.png
--rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.3.5/Images/OffSelect.png
--rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/OffSelectROI.png
--rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/On0.png
--rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/On1.png
--rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/On2.png
--rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/On3.png
--rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.3.5/Images/OnSelect.png
--rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/OnSelectROI.png
--rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/OpenFolder.png
--rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/OpenFolderCompass.png
--rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/PSDHist.png
--rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/PSDvsEnergyHist.png
--rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/Plot.png
--rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/PlotCompass.png
--rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.3.5/Images/SaveCompass.png
--rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/SaveImage.png
--rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/TOFHist.png
--rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.3.5/Images/TOFvsEnergyHist.png
--rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/Images/TimeHist.png
--rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.3.5/Images/axis.png
--rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.3.5/Images/collapsed.png
--rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.3.5/Images/delete.png
--rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.3.5/Images/expanded.png
--rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.3.5/Images/file_config.png
--rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.3.5/Images/grid.png
--rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.3.5/Images/histogram.png
--rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.3.5/Images/info.png
--rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.3.5/Images/line.png
--rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.3.5/Images/save.png
--rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.3.5/Images/settings.png
--rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.3.5/Images/start.png
--rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.3.5/Images/stop.png
--rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.3.5/Images/time.png
--rw-rw-rw-   0        0        0      481 2023-07-12 20:54:32.313799 ReadROOT-2.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    10478 2023-07-05 16:18:23.000000 ReadROOT-2.3.5/QtClasses.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:32.226816 ReadROOT-2.3.5/ReadROOT.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-12 20:54:29.000000 ReadROOT-2.3.5/ReadROOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2100 2023-07-12 20:54:30.000000 ReadROOT-2.3.5/ReadROOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:54:29.000000 ReadROOT-2.3.5/ReadROOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-07-12 20:54:29.000000 ReadROOT-2.3.5/ReadROOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 20:54:29.000000 ReadROOT-2.3.5/ReadROOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11944 2023-07-10 20:03:24.000000 ReadROOT-2.3.5/XML_Parser.py
--rw-rw-rw-   0        0        0     2497 2023-07-11 14:33:41.000000 ReadROOT-2.3.5/__init__.py
--rw-rw-rw-   0        0        0      881 2023-07-05 19:59:51.000000 ReadROOT-2.3.5/config.json
--rw-rw-rw-   0        0        0     7798 2022-12-02 19:45:45.000000 ReadROOT-2.3.5/funcs.cpp
--rw-rw-rw-   0        0        0     1624 2023-06-28 16:56:46.000000 ReadROOT-2.3.5/funcs.hpp
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:32.269803 ReadROOT-2.3.5/merge/
--rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.3.5/merge/__init__.py
--rw-rw-rw-   0        0        0     5715 2023-07-03 16:23:21.000000 ReadROOT-2.3.5/merge/merge_root_files.py
--rw-rw-rw-   0        0        0    31747 2023-07-03 15:57:45.000000 ReadROOT-2.3.5/read_root.py
--rw-rw-rw-   0        0        0    79395 2023-06-14 15:45:35.000000 ReadROOT-2.3.5/read_root_gui.py
--rw-rw-rw-   0        0        0    88671 2023-07-12 20:53:30.000000 ReadROOT-2.3.5/read_root_gui_v2.py
--rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.3.5/root_plotter.py
--rw-rw-rw-   0        0        0       42 2023-07-12 20:54:32.317806 ReadROOT-2.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1473 2023-07-12 20:53:40.000000 ReadROOT-2.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:54:32.307801 ReadROOT-2.3.5/test/
--rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.3.5/test/test.py
--rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.3.5/test/test_cpp.py
--rw-rw-rw-   0        0        0      356 2023-06-28 16:56:46.000000 ReadROOT-2.3.5/wrap.cpp
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.620422 ReadROOT-2.3.6/
+-rw-rw-rw-   0        0        0    16128 2023-02-15 23:51:19.000000 ReadROOT-2.3.6/ErrorPropagation.py
+-rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.3.6/IOClasses.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:43.957427 ReadROOT-2.3.6/Images/
+-rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Calculate.png
+-rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Clear.png
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.236437 ReadROOT-2.3.6/Images/CoMPASS/
+-rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.3.6/Images/CoMPASS/Coincidence.png
+-rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.3.6/Images/CoMPASS/Discriminator.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.3.6/Images/CoMPASS/EnergyCalibration.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.3.6/Images/CoMPASS/Input.png
+-rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.3.6/Images/CoMPASS/Misc.png
+-rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/CoMPASS/OpenGraph.png
+-rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.3.6/Images/CoMPASS/QDC.png
+-rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.3.6/Images/CoMPASS/Rejections.png
+-rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.3.6/Images/CoMPASS/Spectra.png
+-rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.3.6/Images/CoMPASS/Sync.png
+-rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/CoMPASS/icon64x64.ico
+-rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.3.6/Images/CoMPASS/icon64x64.png
+-rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.3.6/Images/CompClear.png
+-rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.3.6/Images/Disabled0.png
+-rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.3.6/Images/Disabled1.png
+-rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.3.6/Images/Disabled2.png
+-rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.3.6/Images/Disabled3.png
+-rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.3.6/Images/DisabledSelect.png
+-rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.3.6/Images/DisabledSelectROI.png
+-rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/EnergyHist.png
+-rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.3.6/Images/EnergyvsEnergyHist.png
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.490419 ReadROOT-2.3.6/Images/Log/
+-rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.3.6/Images/Log/0.png
+-rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.3.6/Images/Log/1.png
+-rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.3.6/Images/Log/2.png
+-rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.3.6/Images/Log/3.png
+-rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.3.6/Images/Log/4.png
+-rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.3.6/Images/Log/5.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.3.6/Images/Log/6.png
+-rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.3.6/Images/Log/7.png
+-rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.3.6/Images/Log/8.png
+-rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.3.6/Images/Log/9+.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.3.6/Images/Log/9.png
+-rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/MCS Graph.png
+-rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Off0.png
+-rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Off1.png
+-rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Off2.png
+-rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Off3.png
+-rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.3.6/Images/OffSelect.png
+-rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/OffSelectROI.png
+-rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/On0.png
+-rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/On1.png
+-rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/On2.png
+-rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/On3.png
+-rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.3.6/Images/OnSelect.png
+-rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/OnSelectROI.png
+-rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/OpenFolder.png
+-rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/OpenFolderCompass.png
+-rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/PSDHist.png
+-rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/PSDvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/Plot.png
+-rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/PlotCompass.png
+-rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.3.6/Images/SaveCompass.png
+-rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/SaveImage.png
+-rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/TOFHist.png
+-rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.3.6/Images/TOFvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/Images/TimeHist.png
+-rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.3.6/Images/axis.png
+-rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.3.6/Images/collapsed.png
+-rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.3.6/Images/delete.png
+-rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.3.6/Images/expanded.png
+-rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.3.6/Images/file_config.png
+-rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.3.6/Images/grid.png
+-rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.3.6/Images/histogram.png
+-rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.3.6/Images/info.png
+-rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.3.6/Images/line.png
+-rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.3.6/Images/save.png
+-rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.3.6/Images/settings.png
+-rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.3.6/Images/start.png
+-rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.3.6/Images/stop.png
+-rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.3.6/Images/time.png
+-rw-rw-rw-   0        0        0      481 2023-07-13 15:06:44.618427 ReadROOT-2.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10478 2023-07-05 16:18:23.000000 ReadROOT-2.3.6/QtClasses.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.546423 ReadROOT-2.3.6/ReadROOT.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-13 15:06:42.000000 ReadROOT-2.3.6/ReadROOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2100 2023-07-13 15:06:43.000000 ReadROOT-2.3.6/ReadROOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 15:06:42.000000 ReadROOT-2.3.6/ReadROOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-07-13 15:06:42.000000 ReadROOT-2.3.6/ReadROOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 15:06:42.000000 ReadROOT-2.3.6/ReadROOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11944 2023-07-10 20:03:24.000000 ReadROOT-2.3.6/XML_Parser.py
+-rw-rw-rw-   0        0        0     2497 2023-07-11 14:33:41.000000 ReadROOT-2.3.6/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-07-05 19:59:51.000000 ReadROOT-2.3.6/config.json
+-rw-rw-rw-   0        0        0     7798 2022-12-02 19:45:45.000000 ReadROOT-2.3.6/funcs.cpp
+-rw-rw-rw-   0        0        0     1624 2023-06-28 16:56:46.000000 ReadROOT-2.3.6/funcs.hpp
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.582423 ReadROOT-2.3.6/merge/
+-rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.3.6/merge/__init__.py
+-rw-rw-rw-   0        0        0     5738 2023-07-13 15:06:11.000000 ReadROOT-2.3.6/merge/merge_root_files.py
+-rw-rw-rw-   0        0        0    31747 2023-07-03 15:57:45.000000 ReadROOT-2.3.6/read_root.py
+-rw-rw-rw-   0        0        0    79395 2023-06-14 15:45:35.000000 ReadROOT-2.3.6/read_root_gui.py
+-rw-rw-rw-   0        0        0    88671 2023-07-12 20:53:30.000000 ReadROOT-2.3.6/read_root_gui_v2.py
+-rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.3.6/root_plotter.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 15:06:44.620422 ReadROOT-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2023-07-13 15:04:45.000000 ReadROOT-2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 15:06:44.614421 ReadROOT-2.3.6/test/
+-rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.3.6/test/test.py
+-rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.3.6/test/test_cpp.py
+-rw-rw-rw-   0        0        0      356 2023-06-28 16:56:46.000000 ReadROOT-2.3.6/wrap.cpp
```

### Comparing `ReadROOT-2.3.5/ErrorPropagation.py` & `ReadROOT-2.3.6/ErrorPropagation.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/IOClasses.py` & `ReadROOT-2.3.6/IOClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Calculate.png` & `ReadROOT-2.3.6/Images/Calculate.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Clear.png` & `ReadROOT-2.3.6/Images/Clear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Coincidence.png` & `ReadROOT-2.3.6/Images/CoMPASS/Coincidence.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Discriminator.png` & `ReadROOT-2.3.6/Images/CoMPASS/Discriminator.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/EnergyCalibration.png` & `ReadROOT-2.3.6/Images/CoMPASS/EnergyCalibration.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Input.png` & `ReadROOT-2.3.6/Images/CoMPASS/Input.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Misc.png` & `ReadROOT-2.3.6/Images/CoMPASS/Misc.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/OpenGraph.png` & `ReadROOT-2.3.6/Images/CoMPASS/OpenGraph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/QDC.png` & `ReadROOT-2.3.6/Images/CoMPASS/QDC.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Rejections.png` & `ReadROOT-2.3.6/Images/CoMPASS/Rejections.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Spectra.png` & `ReadROOT-2.3.6/Images/CoMPASS/Spectra.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/Sync.png` & `ReadROOT-2.3.6/Images/CoMPASS/Sync.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/icon64x64.ico` & `ReadROOT-2.3.6/Images/CoMPASS/icon64x64.ico`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CoMPASS/icon64x64.png` & `ReadROOT-2.3.6/Images/CoMPASS/icon64x64.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/CompClear.png` & `ReadROOT-2.3.6/Images/CompClear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Disabled0.png` & `ReadROOT-2.3.6/Images/Disabled0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Disabled1.png` & `ReadROOT-2.3.6/Images/Disabled1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Disabled2.png` & `ReadROOT-2.3.6/Images/Disabled2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Disabled3.png` & `ReadROOT-2.3.6/Images/Disabled3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/DisabledSelect.png` & `ReadROOT-2.3.6/Images/DisabledSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/DisabledSelectROI.png` & `ReadROOT-2.3.6/Images/DisabledSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/EnergyHist.png` & `ReadROOT-2.3.6/Images/EnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/EnergyvsEnergyHist.png` & `ReadROOT-2.3.6/Images/EnergyvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/0.png` & `ReadROOT-2.3.6/Images/Log/0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/2.png` & `ReadROOT-2.3.6/Images/Log/2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/3.png` & `ReadROOT-2.3.6/Images/Log/3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/4.png` & `ReadROOT-2.3.6/Images/Log/4.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/5.png` & `ReadROOT-2.3.6/Images/Log/5.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/6.png` & `ReadROOT-2.3.6/Images/Log/6.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/7.png` & `ReadROOT-2.3.6/Images/Log/7.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/8.png` & `ReadROOT-2.3.6/Images/Log/8.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/9+.png` & `ReadROOT-2.3.6/Images/Log/9+.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Log/9.png` & `ReadROOT-2.3.6/Images/Log/9.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/MCS Graph.png` & `ReadROOT-2.3.6/Images/MCS Graph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Off0.png` & `ReadROOT-2.3.6/Images/Off0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Off1.png` & `ReadROOT-2.3.6/Images/Off1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Off2.png` & `ReadROOT-2.3.6/Images/Off2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Off3.png` & `ReadROOT-2.3.6/Images/Off3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OffSelect.png` & `ReadROOT-2.3.6/Images/OffSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OffSelectROI.png` & `ReadROOT-2.3.6/Images/OffSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/On0.png` & `ReadROOT-2.3.6/Images/On0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/On1.png` & `ReadROOT-2.3.6/Images/On1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/On2.png` & `ReadROOT-2.3.6/Images/On2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/On3.png` & `ReadROOT-2.3.6/Images/On3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OnSelect.png` & `ReadROOT-2.3.6/Images/OnSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OnSelectROI.png` & `ReadROOT-2.3.6/Images/OnSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OpenFolder.png` & `ReadROOT-2.3.6/Images/OpenFolder.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/OpenFolderCompass.png` & `ReadROOT-2.3.6/Images/OpenFolderCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/PSDHist.png` & `ReadROOT-2.3.6/Images/PSDHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/PSDvsEnergyHist.png` & `ReadROOT-2.3.6/Images/PSDvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/Plot.png` & `ReadROOT-2.3.6/Images/Plot.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/PlotCompass.png` & `ReadROOT-2.3.6/Images/PlotCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/SaveCompass.png` & `ReadROOT-2.3.6/Images/SaveCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/SaveImage.png` & `ReadROOT-2.3.6/Images/SaveImage.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/TOFHist.png` & `ReadROOT-2.3.6/Images/TOFHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/TOFvsEnergyHist.png` & `ReadROOT-2.3.6/Images/TOFvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/TimeHist.png` & `ReadROOT-2.3.6/Images/TimeHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/axis.png` & `ReadROOT-2.3.6/Images/axis.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/delete.png` & `ReadROOT-2.3.6/Images/delete.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/file_config.png` & `ReadROOT-2.3.6/Images/file_config.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/grid.png` & `ReadROOT-2.3.6/Images/grid.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/histogram.png` & `ReadROOT-2.3.6/Images/histogram.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/info.png` & `ReadROOT-2.3.6/Images/info.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/save.png` & `ReadROOT-2.3.6/Images/save.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/settings.png` & `ReadROOT-2.3.6/Images/settings.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/start.png` & `ReadROOT-2.3.6/Images/start.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/stop.png` & `ReadROOT-2.3.6/Images/stop.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/Images/time.png` & `ReadROOT-2.3.6/Images/time.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/QtClasses.py` & `ReadROOT-2.3.6/QtClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/ReadROOT.egg-info/SOURCES.txt` & `ReadROOT-2.3.6/ReadROOT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/XML_Parser.py` & `ReadROOT-2.3.6/XML_Parser.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/__init__.py` & `ReadROOT-2.3.6/__init__.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/config.json` & `ReadROOT-2.3.6/config.json`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/funcs.cpp` & `ReadROOT-2.3.6/funcs.cpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/funcs.hpp` & `ReadROOT-2.3.6/funcs.hpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/merge/merge_root_files.py` & `ReadROOT-2.3.6/merge/merge_root_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,31 +30,31 @@
 
 class Merger(QtCore.QObject):
     """Merger Class.
     The start file is considered #1 and stop file, #0.
 
     Parameters
     ----------
-    file_ch0 : Path
+    stop_file : Path
         Root file containing the stop events
-    file_ch1 : Path
+    start_file : Path
         Root file containing the start events
     window : U64, optional
         Maximum time for the events to coincide, by default 0
     tree : str, optional
         TTree key for the root files, by default "Data_R"
     """
     cuts_enabled = False
     unfilter_data = False
     finished = QtCore.pyqtSignal(list)
 
-    def __init__(self, file_ch0: Path, file_ch1: Path, window: U64 = 0, tree: str = "Data_R") -> None:
+    def __init__(self, stop_file: Path, start_file: Path, window: U64 = 0, tree: str = "Data_R") -> None:
         super(Merger, self).__init__()
-        self.file_ch0__: Path = file_ch0
-        self.file_ch1__: Path = file_ch1
+        self.file_ch0__: Path = stop_file
+        self.file_ch1__: Path = start_file
         self.window : U64 = window
         self.tree = tree
         self.cuts = {0:[],1:[]}
 
     def select_cuts(self, start: U16, stop: U16, file: int):
         if self.cuts.get(file) is not None:
             self.cuts[file] = [start, stop]
@@ -95,15 +95,15 @@
         iter_e1 = np.nditer(filtered_root_file1["Energy"])
        
         t0 = next(iter_t0)
         e0 = next(iter_e0)
         t1 = next(iter_t1) 
         e1 = next(iter_e1)
         while t0 != 0 and t1 != 0:
-            delta, sign = uint64_diff(t0, t1)
+            delta, sign = uint64_diff(t0, t1) # Doing t0-t1
             if delta <= threshold:
                 result.append(ConsolidatedData(t0, t1, e0, e1))
                 
                 t0 = next(iter_t0, 0)
                 e0 = next(iter_e0, 0)
                 
                 t1 = next(iter_t1, 0)
```

### Comparing `ReadROOT-2.3.5/read_root.py` & `ReadROOT-2.3.6/read_root.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/read_root_gui.py` & `ReadROOT-2.3.6/read_root_gui.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/read_root_gui_v2.py` & `ReadROOT-2.3.6/read_root_gui_v2.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/root_plotter.py` & `ReadROOT-2.3.6/root_plotter.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.3.5/setup.py` & `ReadROOT-2.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.5"
+__version__ = "2.3.6"
 
 from setuptools import setup
 
 setup(
     name = "ReadROOT",
     version = __version__,
     description = "Easy GUI made to read ROOT files created by the CoMPASS software distribued by CAEN.",
```

### Comparing `ReadROOT-2.3.5/test/test_cpp.py` & `ReadROOT-2.3.6/test/test_cpp.py`

 * *Files identical despite different names*

