# Comparing `tmp/darfix-0.9.7.tar.gz` & `tmp/darfix-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/darfix-0.9.7.tar", last modified: Wed Mar  1 17:09:12 2023, max compression
+gzip compressed data, was "dist/darfix-0.9.8.tar", last modified: Wed May 10 15:43:31 2023, max compression
```

## Comparing `darfix-0.9.7.tar` & `darfix-0.9.8.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-03-01 13:15:22.000000 darfix-0.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      752 2023-03-01 17:09:12.000000 darfix-0.9.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-03-01 13:15:22.000000 darfix-0.9.7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-01 13:15:22.000000 darfix-0.9.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1895 2023-03-01 17:09:12.000000 darfix-0.9.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-01 13:15:22.000000 darfix-0.9.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-03-01 17:04:30.000000 darfix-0.9.7/src/darfix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2655 2023-03-01 16:33:36.000000 darfix-0.9.7/src/darfix/app/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/core/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/autofocus.py
--rw-rw-rw-   0 root         (0) root         (0)     9947 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/componentsMatching.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/data_selection.py
--rw-rw-rw-   0 root         (0) root         (0)    95197 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9180 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     7361 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/geneticShiftDetection.py
--rw-rw-rw-   0 root         (0) root         (0)     6945 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/imageOperations.py
--rw-rw-rw-   0 root         (0) root         (0)    11397 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/imageRegistration.py
--rw-rw-rw-   0 root         (0) root         (0)    18358 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/mapping.py
--rw-rw-rw-   0 root         (0) root         (0)    14412 2023-03-01 15:22:25.000000 darfix-0.9.7/src/darfix/core/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/roi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/core/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/core/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_components_matching.py
--rw-rw-rw-   0 root         (0) root         (0)    29321 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    15632 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_dimension.py
--rw-rw-rw-   0 root         (0) root         (0)     4119 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_ga.py
--rw-rw-rw-   0 root         (0) root         (0)     7141 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_image_operations.py
--rw-rw-rw-   0 root         (0) root         (0)    15895 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_image_registration.py
--rw-rw-rw-   0 root         (0) root         (0)     3753 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     3501 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_roi.py
--rw-rw-rw-   0 root         (0) root         (0)     3499 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/test/test_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)      950 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/decomposition/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6589 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10534 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/ipca.py
--rw-rw-rw-   0 root         (0) root         (0)     3997 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/nica.py
--rw-rw-rw-   0 root         (0) root         (0)     4463 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/nmf.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/decomposition/test/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/test_ipca.py
--rw-rw-rw-   0 root         (0) root         (0)     4709 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/test_nica.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/test_nmf.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/decomposition/test/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1949 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/PCAWidget.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/binningWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     7120 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/blindSourceSeparationWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     5817 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/dataPartitionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    10086 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/datasetSelectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    25314 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/dimensionsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    13147 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/displayComponentsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    19878 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/grainPlotWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/lineProfileWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     8001 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/linkComponentsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6603 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/magnificationWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/metadataWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    20787 2023-03-01 15:22:25.000000 darfix-0.9.7/src/darfix/gui/noiseRemovalWidget.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/operationThread.py
--rw-rw-rw-   0 root         (0) root         (0)     4095 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/projectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    22642 2023-03-01 15:22:25.000000 darfix-0.9.7/src/darfix/gui/rockingCurvesWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     9368 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/roiSelectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/rsmHistogramWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/rsmWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    13665 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/shiftCorrectionWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/showStackWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6278 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/gui/zSumWidget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/io/dataset_io.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/io/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/resources/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/resources/gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/resources/gui/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/resources/gui/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/curves.png
--rw-rw-rw-   0 root         (0) root         (0)     6830 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/curves.svg
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/resize.png
--rw-rw-rw-   0 root         (0) root         (0)     8233 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/resize.svg
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/scatter.png
--rw-rw-rw-   0 root         (0) root         (0)    20421 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/resources/gui/icons/scatter.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/darfix/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4724 2023-03-01 13:15:22.000000 darfix-0.9.7/src/darfix/test/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6558 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      243 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-01 17:09:12.000000 darfix-0.9.7/src/darfix.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/darfix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/orangecontrib/darfix/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/darfix/test/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/test/orangeWorkflowTest.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/test/test_ewoks.py
--rw-rw-rw-   0 root         (0) root         (0)     2608 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/test/test_widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7661 2023-03-01 16:33:36.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/darfix_example1.ows
--rw-rw-rw-   0 root         (0) root         (0)     5116 2023-03-01 16:33:36.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/darfix_example2.ows
--rw-rw-rw-   0 root         (0) root         (0)  8391680 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/strain_0000.edf
--rw-rw-rw-   0 root         (0) root         (0)  8403250 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/tutorials/strain_0001.edf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/binning.py
--rw-rw-rw-   0 root         (0) root         (0)     1958 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/blindsourceseparation.py
--rw-rw-rw-   0 root         (0) root         (0)     1137 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/datacopy.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/datapartition.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-03-01 16:33:36.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/dataselection.py
--rw-rw-rw-   0 root         (0) root         (0)     3884 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-03-01 15:16:13.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/flash.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/grainplot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 17:09:12.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 17:09:05.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/axes.png
--rw-rw-rw-   0 root         (0) root         (0)     5038 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/axes.svg
--rw-rw-rw-   0 root         (0) root         (0)     3212 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/bss.png
--rw-rw-rw-   0 root         (0) root         (0)     4986 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/bss.svg
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     8068 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/copy.svg
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/curves.png
--rw-rw-rw-   0 root         (0) root         (0)    51435 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/curves.svg
--rw-rw-rw-   0 root         (0) root         (0)   233309 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon.png
--rw-rw-rw-   0 root         (0) root         (0)    35611 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg
--rw-rw-rw-   0 root         (0) root         (0)   236860 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/filter.png
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/filter.svg
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/flash.svg
--rw-rw-rw-   0 root         (0) root         (0)    22180 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/grainplot.png
--rw-rw-rw-   0 root         (0) root         (0)  2409867 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/grainplot.svg
--rw-rw-rw-   0 root         (0) root         (0)    64642 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/image-select-box.svg
--rw-rw-rw-   0 root         (0) root         (0)    16836 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/line_profile.png
--rw-rw-rw-   0 root         (0) root         (0)   132131 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/line_profile.svg
--rw-rw-rw-   0 root         (0) root         (0)     9458 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/link.png
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/link.svg
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/metadata.png
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/metadata.svg
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/mywidget.svg
--rw-rw-rw-   0 root         (0) root         (0)     6218 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal.png
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal.svg
--rw-rw-rw-   0 root         (0) root         (0)     6897 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg
--rw-rw-rw-   0 root         (0) root         (0)     3583 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/param_dims.png
--rw-rw-rw-   0 root         (0) root         (0)     9708 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/param_dims.svg
--rw-rw-rw-   0 root         (0) root         (0)     4325 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/pca.png
--rw-rw-rw-   0 root         (0) root         (0)    21388 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/pca.svg
--rw-rw-rw-   0 root         (0) root         (0)     2140 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/random.svg
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/resize.png
--rw-rw-rw-   0 root         (0) root         (0)     6668 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/roi.png
--rw-rw-rw-   0 root         (0) root         (0)    66544 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/roi.svg
--rw-rw-rw-   0 root         (0) root         (0)     3260 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/save.svg
--rw-rw-rw-   0 root         (0) root         (0)     8108 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/shift_correction.svg
--rw-rw-rw-   0 root         (0) root         (0)     4978 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/upload.svg
--rw-rw-rw-   0 root         (0) root         (0)     2853 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/zsum.svg
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/lineprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/linkcomponents.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-03-01 15:16:13.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/noiseremoval.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/pca.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/projection.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/rockingcurves.py
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/roiselection.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/rsmhistogram.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/shiftcorrection.py
--rw-rw-rw-   0 root         (0) root         (0)     4619 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-03-01 13:15:22.000000 darfix-0.9.7/src/orangecontrib/darfix/widgets/zsum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-10 05:03:44.000000 darfix-0.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-10 15:43:31.000000 darfix-0.9.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-05-10 05:03:44.000000 darfix-0.9.8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-05-10 05:03:44.000000 darfix-0.9.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2023-05-10 15:43:31.000000 darfix-0.9.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-10 05:03:44.000000 darfix-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-10 15:33:24.000000 darfix-0.9.8/src/darfix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/app/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/core/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/autofocus.py
+-rw-rw-rw-   0 root         (0) root         (0)     9947 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/componentsMatching.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/data_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    95197 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     9180 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)     7361 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/geneticShiftDetection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6945 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/imageOperations.py
+-rw-rw-rw-   0 root         (0) root         (0)    11397 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/imageRegistration.py
+-rw-rw-rw-   0 root         (0) root         (0)    18358 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)    14389 2023-05-10 14:50:18.000000 darfix-0.9.8/src/darfix/core/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/roi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/core/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/core/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_components_matching.py
+-rw-rw-rw-   0 root         (0) root         (0)    29321 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    15632 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_dimension.py
+-rw-rw-rw-   0 root         (0) root         (0)     4119 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_ga.py
+-rw-rw-rw-   0 root         (0) root         (0)     7141 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_image_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)    15895 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_image_registration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3753 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     3501 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3499 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/test/test_workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      950 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/decomposition/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10534 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/ipca.py
+-rw-rw-rw-   0 root         (0) root         (0)     3997 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/nica.py
+-rw-rw-rw-   0 root         (0) root         (0)     4463 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/nmf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/decomposition/test/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/test_ipca.py
+-rw-rw-rw-   0 root         (0) root         (0)     4709 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/test_nica.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/test_nmf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/decomposition/test/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/PCAWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/binningWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/blindSourceSeparationWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5817 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/dataPartitionWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    10086 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/datasetSelectionWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    25314 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/dimensionsWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    13147 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/displayComponentsWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    19878 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/grainPlotWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/lineProfileWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     8001 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/linkComponentsWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6603 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/magnificationWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/metadataWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    20787 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/noiseRemovalWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/operationThread.py
+-rw-rw-rw-   0 root         (0) root         (0)     4095 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/projectionWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    22642 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/rockingCurvesWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     9368 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/roiSelectionWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/rsmHistogramWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/rsmWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    13665 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/shiftCorrectionWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/showStackWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6278 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/gui/zSumWidget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/io/dataset_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    10758 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/io/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/resources/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/resources/gui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/resources/gui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/resources/gui/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/curves.png
+-rw-rw-rw-   0 root         (0) root         (0)     6830 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/curves.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/resize.png
+-rw-rw-rw-   0 root         (0) root         (0)     8233 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/resize.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/scatter.png
+-rw-rw-rw-   0 root         (0) root         (0)    20421 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/resources/gui/icons/scatter.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/darfix/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4724 2023-05-10 05:03:44.000000 darfix-0.9.8/src/darfix/test/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6558 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      730 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 15:43:31.000000 darfix-0.9.8/src/darfix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/darfix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/orangecontrib/darfix/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/darfix/test/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/test/orangeWorkflowTest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/test/test_ewoks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/test/test_widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7661 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/darfix_example1.ows
+-rw-rw-rw-   0 root         (0) root         (0)     5116 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/darfix_example2.ows
+-rw-rw-rw-   0 root         (0) root         (0)  8391680 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/strain_0000.edf
+-rw-rw-rw-   0 root         (0) root         (0)  8403250 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/tutorials/strain_0001.edf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/binning.py
+-rw-rw-rw-   0 root         (0) root         (0)     1958 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/blindsourceseparation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/datacopy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/datapartition.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/dataselection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3884 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/flash.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/grainplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 15:43:31.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 15:43:25.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/axes.png
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/axes.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/bss.png
+-rw-rw-rw-   0 root         (0) root         (0)     4986 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/bss.svg
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8068 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/curves.png
+-rw-rw-rw-   0 root         (0) root         (0)    51435 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/curves.svg
+-rw-rw-rw-   0 root         (0) root         (0)   233309 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    35611 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)   236860 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/filter.png
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/filter.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/flash.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22180 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/grainplot.png
+-rw-rw-rw-   0 root         (0) root         (0)  2409867 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/grainplot.svg
+-rw-rw-rw-   0 root         (0) root         (0)    64642 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/image-select-box.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16836 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/line_profile.png
+-rw-rw-rw-   0 root         (0) root         (0)   132131 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/line_profile.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9458 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/link.png
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/link.svg
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/metadata.png
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/metadata.svg
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/mywidget.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6218 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal.png
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6897 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3583 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/param_dims.png
+-rw-rw-rw-   0 root         (0) root         (0)     9708 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/param_dims.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/pca.png
+-rw-rw-rw-   0 root         (0) root         (0)    21388 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/pca.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/random.svg
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/resize.png
+-rw-rw-rw-   0 root         (0) root         (0)     6668 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/roi.png
+-rw-rw-rw-   0 root         (0) root         (0)    66544 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/roi.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/save.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8108 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/shift_correction.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4978 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/upload.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/zsum.svg
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/lineprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/linkcomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/noiseremoval.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/pca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/projection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/rockingcurves.py
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/roiselection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/rsmhistogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     2269 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/shiftcorrection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4619 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-10 05:03:44.000000 darfix-0.9.8/src/orangecontrib/darfix/widgets/zsum.py
```

### Comparing `darfix-0.9.7/LICENSE` & `darfix-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/PKG-INFO` & `darfix-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darfix
-Version: 0.9.7
+Version: 0.9.8
 Summary: Computer vision software for the interpretation of diffraction images
 Home-page: https://gitlab.esrf.fr/XRD/darfix
 Author: J.Garriga
 Author-email: julia.garriga@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/XRD/darfix/
 Project-URL: Documentation, http://www.edna-site.org/pub/doc/darfix/latest
```

### Comparing `darfix-0.9.7/README.rst` & `darfix-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/setup.cfg` & `darfix-0.9.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -79,19 +79,14 @@
 exclude = 
 	.eggs
 
 [flake8_nb]
 ignore = E501, E203, W503, E402
 max-line-length = 88
 
-[build_sphinx]
-project = darfix
-version = attr: darfix.__version__
-source-dir = ./doc
-
 [coverage:run]
 omit = 
 	setup.py
 	darfix/tests/*
 	orangecontrib/tests/*
 
 [egg_info]
```

### Comparing `darfix-0.9.7/src/darfix/__init__.py` & `darfix-0.9.8/src/darfix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 - silx.io: Functions for input/output operations
 - silx.utils: Miscellaneous convenient functions
 """
 
 __authors__ = ["J. Garriga"]
 __license__ = "MIT"
 __date__ = "16/12/2019"
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 from ._config import Config as _Config
 
 config = _Config()
 """Global configuration shared with the whole library"""
```

### Comparing `darfix-0.9.7/src/darfix/_config.py` & `darfix-0.9.8/src/darfix/_config.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/app/__main__.py` & `darfix-0.9.8/src/darfix/app/__main__.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/componentsMatching.py` & `darfix-0.9.8/src/darfix/core/componentsMatching.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/data_selection.py` & `darfix-0.9.8/src/darfix/core/data_selection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/dataset.py` & `darfix-0.9.8/src/darfix/core/dataset.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/dimension.py` & `darfix-0.9.8/src/darfix/core/dimension.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/geneticShiftDetection.py` & `darfix-0.9.8/src/darfix/core/geneticShiftDetection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/imageOperations.py` & `darfix-0.9.8/src/darfix/core/imageOperations.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/imageRegistration.py` & `darfix-0.9.8/src/darfix/core/imageRegistration.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/mapping.py` & `darfix-0.9.8/src/darfix/core/mapping.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/process.py` & `darfix-0.9.8/src/darfix/core/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 __authors__ = ["J. Garriga"]
 __license__ = "MIT"
 __date__ = "16/07/2021"
 
 
 import os
-from collections import Mapping
-from typing import Iterable, Union, Optional
+from typing import Iterable, Union, Optional, Mapping
 from ewoksutils.import_utils import qualname
 import numpy
 import copy
 
 from silx.gui import qt
 from darfix.core import utils
 from darfix.gui.blindSourceSeparationWidget import Method
```

### Comparing `darfix-0.9.7/src/darfix/core/roi.py` & `darfix-0.9.8/src/darfix/core/roi.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_components_matching.py` & `darfix-0.9.8/src/darfix/core/test/test_components_matching.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_dataset.py` & `darfix-0.9.8/src/darfix/core/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_dimension.py` & `darfix-0.9.8/src/darfix/core/test/test_dimension.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_ga.py` & `darfix-0.9.8/src/darfix/core/test/test_ga.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_image_operations.py` & `darfix-0.9.8/src/darfix/core/test/test_image_operations.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_image_registration.py` & `darfix-0.9.8/src/darfix/core/test/test_image_registration.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_mapping.py` & `darfix-0.9.8/src/darfix/core/test/test_mapping.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_roi.py` & `darfix-0.9.8/src/darfix/core/test/test_roi.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/test/test_workflow.py` & `darfix-0.9.8/src/darfix/core/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/core/utils.py` & `darfix-0.9.8/src/darfix/core/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/base.py` & `darfix-0.9.8/src/darfix/decomposition/base.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/ipca.py` & `darfix-0.9.8/src/darfix/decomposition/ipca.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/nica.py` & `darfix-0.9.8/src/darfix/decomposition/nica.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/nmf.py` & `darfix-0.9.8/src/darfix/decomposition/nmf.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/pca.py` & `darfix-0.9.8/src/darfix/decomposition/pca.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/test/test_base.py` & `darfix-0.9.8/src/darfix/decomposition/test/test_base.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/test/test_ipca.py` & `darfix-0.9.8/src/darfix/decomposition/test/test_ipca.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/test/test_nica.py` & `darfix-0.9.8/src/darfix/decomposition/test/test_nica.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/test/test_nmf.py` & `darfix-0.9.8/src/darfix/decomposition/test/test_nmf.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/decomposition/test/utils.py` & `darfix-0.9.8/src/darfix/decomposition/test/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/PCAWidget.py` & `darfix-0.9.8/src/darfix/gui/PCAWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/binningWidget.py` & `darfix-0.9.8/src/darfix/gui/binningWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/blindSourceSeparationWidget.py` & `darfix-0.9.8/src/darfix/gui/blindSourceSeparationWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/dataPartitionWidget.py` & `darfix-0.9.8/src/darfix/gui/dataPartitionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/datasetSelectionWidget.py` & `darfix-0.9.8/src/darfix/gui/datasetSelectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/dimensionsWidget.py` & `darfix-0.9.8/src/darfix/gui/dimensionsWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/displayComponentsWidget.py` & `darfix-0.9.8/src/darfix/gui/displayComponentsWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/grainPlotWidget.py` & `darfix-0.9.8/src/darfix/gui/grainPlotWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/lineProfileWidget.py` & `darfix-0.9.8/src/darfix/gui/lineProfileWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/linkComponentsWidget.py` & `darfix-0.9.8/src/darfix/gui/linkComponentsWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/magnificationWidget.py` & `darfix-0.9.8/src/darfix/gui/magnificationWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/metadataWidget.py` & `darfix-0.9.8/src/darfix/gui/metadataWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/noiseRemovalWidget.py` & `darfix-0.9.8/src/darfix/gui/noiseRemovalWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/operationThread.py` & `darfix-0.9.8/src/darfix/gui/operationThread.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/projectionWidget.py` & `darfix-0.9.8/src/darfix/gui/projectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/rockingCurvesWidget.py` & `darfix-0.9.8/src/darfix/gui/rockingCurvesWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/roiSelectionWidget.py` & `darfix-0.9.8/src/darfix/gui/roiSelectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/rsmHistogramWidget.py` & `darfix-0.9.8/src/darfix/gui/rsmHistogramWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/rsmWidget.py` & `darfix-0.9.8/src/darfix/gui/rsmWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/shiftCorrectionWidget.py` & `darfix-0.9.8/src/darfix/gui/shiftCorrectionWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/showStackWidget.py` & `darfix-0.9.8/src/darfix/gui/showStackWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/utils.py` & `darfix-0.9.8/src/darfix/gui/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/gui/zSumWidget.py` & `darfix-0.9.8/src/darfix/gui/zSumWidget.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/io/dataset_io.py` & `darfix-0.9.8/src/darfix/io/dataset_io.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/io/utils.py` & `darfix-0.9.8/src/darfix/io/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/curves.png` & `darfix-0.9.8/src/darfix/resources/gui/icons/curves.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/curves.svg` & `darfix-0.9.8/src/darfix/resources/gui/icons/curves.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/resize.png` & `darfix-0.9.8/src/darfix/resources/gui/icons/resize.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/resize.svg` & `darfix-0.9.8/src/darfix/resources/gui/icons/resize.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/scatter.png` & `darfix-0.9.8/src/darfix/resources/gui/icons/scatter.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/resources/gui/icons/scatter.svg` & `darfix-0.9.8/src/darfix/resources/gui/icons/scatter.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix/test/utils.py` & `darfix-0.9.8/src/darfix/test/utils.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix.egg-info/PKG-INFO` & `darfix-0.9.8/src/darfix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darfix
-Version: 0.9.7
+Version: 0.9.8
 Summary: Computer vision software for the interpretation of diffraction images
 Home-page: https://gitlab.esrf.fr/XRD/darfix
 Author: J.Garriga
 Author-email: julia.garriga@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/XRD/darfix/
 Project-URL: Documentation, http://www.edna-site.org/pub/doc/darfix/latest
```

### Comparing `darfix-0.9.7/src/darfix.egg-info/SOURCES.txt` & `darfix-0.9.8/src/darfix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/darfix.egg-info/requires.txt` & `darfix-0.9.8/src/darfix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/test/orangeWorkflowTest.py` & `darfix-0.9.8/src/orangecontrib/darfix/test/orangeWorkflowTest.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/test/test_ewoks.py` & `darfix-0.9.8/src/orangecontrib/darfix/test/test_ewoks.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/test/test_widgets.py` & `darfix-0.9.8/src/orangecontrib/darfix/test/test_widgets.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/tutorials/darfix_example1.ows` & `darfix-0.9.8/src/orangecontrib/darfix/tutorials/darfix_example1.ows`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/tutorials/darfix_example2.ows` & `darfix-0.9.8/src/orangecontrib/darfix/tutorials/darfix_example2.ows`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/tutorials/strain_0000.edf` & `darfix-0.9.8/src/orangecontrib/darfix/tutorials/strain_0000.edf`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/tutorials/strain_0001.edf` & `darfix-0.9.8/src/orangecontrib/darfix/tutorials/strain_0001.edf`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/__init__.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/binning.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/binning.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/blindsourceseparation.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/blindsourceseparation.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/datacopy.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/datacopy.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/datapartition.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/datapartition.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/dataselection.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/dataselection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/dimensions.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/dimensions.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/flash.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/flash.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/grainplot.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/grainplot.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/axes.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/axes.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/axes.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/axes.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/bss.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/bss.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/bss.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/bss.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/copy.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/copy.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/curves.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/curves.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/curves.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/curves.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/darfix_icon8.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/filter.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/filter.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/filter.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/filter.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/flash.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/flash.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/grainplot.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/grainplot.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/grainplot.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/grainplot.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/image-select-box.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/image-select-box.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/line_profile.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/line_profile.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/line_profile.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/line_profile.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/link.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/link.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/link.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/link.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/metadata.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/metadata.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/metadata.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/metadata.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/mywidget.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/noise_removal_backup.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/param_dims.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/param_dims.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/param_dims.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/param_dims.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/pca.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/pca.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/pca.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/pca.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/random.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/random.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/resize.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/resize.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/roi.png` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/roi.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/roi.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/save.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/save.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/shift_correction.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/shift_correction.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/upload.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/upload.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/icons/zsum.svg` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/icons/zsum.svg`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/lineprofile.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/lineprofile.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/linkcomponents.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/linkcomponents.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/metadata.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/metadata.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/noiseremoval.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/noiseremoval.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/pca.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/pca.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/projection.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/projection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/rockingcurves.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/rockingcurves.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/roiselection.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/roiselection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/rsmhistogram.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/rsmhistogram.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/shiftcorrection.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/shiftcorrection.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/transformation.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/transformation.py`

 * *Files identical despite different names*

### Comparing `darfix-0.9.7/src/orangecontrib/darfix/widgets/zsum.py` & `darfix-0.9.8/src/orangecontrib/darfix/widgets/zsum.py`

 * *Files identical despite different names*

