# Comparing `tmp/ifiscripts-2023.7.3.1.tar.gz` & `tmp/ifiscripts-2023.7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifiscripts-2023.7.3.1.tar", last modified: Mon Jul  3 06:52:16 2023, max compression
+gzip compressed data, was "ifiscripts-2023.7.3.2.tar", last modified: Mon Jul  3 09:35:33 2023, max compression
```

## Comparing `ifiscripts-2023.7.3.1.tar` & `ifiscripts-2023.7.3.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:52:16.597474 ifiscripts-2023.7.3.1/
--rw-rw-rw-   0        0        0  1006250 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/26_XYZ-22_Rec709.cube
--rw-rw-rw-   0        0        0     1137 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       72 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1188 2023-07-03 06:52:16.595582 ifiscripts-2023.7.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4589 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/README.rst
--rw-rw-rw-   0        0        0     5015 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/film_scan_aip_documentation.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 06:52:16.274714 ifiscripts-2023.7.3.1/ifiscripts.egg-info/
--rw-rw-rw-   0        0        0     1188 2023-07-03 06:52:15.000000 ifiscripts-2023.7.3.1/ifiscripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2023-07-03 06:52:15.000000 ifiscripts-2023.7.3.1/ifiscripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:52:15.000000 ifiscripts-2023.7.3.1/ifiscripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-03 06:52:15.000000 ifiscripts-2023.7.3.1/ifiscripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-03 06:52:15.000000 ifiscripts-2023.7.3.1/ifiscripts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 06:52:16.369044 ifiscripts-2023.7.3.1/legacy_scripts/
--rw-rw-rw-   0        0        0     2960 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/batchfixity.py
--rw-rw-rw-   0        0        0     1639 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/db_cleaning.py
--rw-rw-rw-   0        0        0    11445 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/dpxonly.py
--rw-rw-rw-   0        0        0     5145 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/dvsip.py
--rw-rw-rw-   0        0        0     1054 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/giffer.py
--rw-rw-rw-   0        0        0     1023 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/loopline.py
--rw-rw-rw-   0        0        0    11758 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/makedpx.py
--rw-rw-rw-   0        0        0      883 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/mezzaninecheck.py
--rw-rw-rw-   0        0        0     1769 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/oeremove.py
--rw-rw-rw-   0        0        0     3905 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/pg.py
--rw-rw-rw-   0        0        0     3145 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/playerseq.py
--rw-rw-rw-   0        0        0    22350 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/premisgui.py
--rw-rw-rw-   0        0        0     2730 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/qctools.py
--rw-rw-rw-   0        0        0    16007 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/rawbatch.py
--rw-rw-rw-   0        0        0      440 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/renumber.py
--rw-rw-rw-   0        0        0    67528 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/legacy_scripts/revtmd.py
--rw-rw-rw-   0        0        0     1359 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/legacy_scripts/sha512deep.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:52:16.588475 ifiscripts-2023.7.3.1/scripts/
--rw-rw-rw-   0        0        0   126723 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/Objects.py
--rw-rw-rw-   0        0        0     3729 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/accession_register.py
--rw-rw-rw-   0        0        0    12517 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/aipcreator.py
--rw-rw-rw-   0        0        0     9815 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/as11fixity.py
--rw-rw-rw-   0        0        0    16950 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/batchaipcreator.py
--rw-rw-rw-   0        0        0     6149 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/batchdiff_framemd5.py
--rw-rw-rw-   0        0        0     3618 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/batchmakeshell.py
--rw-rw-rw-   0        0        0     6148 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/batchsipcreator.py
--rw-rw-rw-   0        0        0     9679 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/bitc.py
--rw-rw-rw-   0        0        0    10725 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/concat.py
--rw-rw-rw-   0        0        0    33418 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/copyit.py
--rw-rw-rw-   0        0        0    23661 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/dcpaccess.py
--rw-rw-rw-   0        0        0    14055 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/dcpfixity.py
--rw-rw-rw-   0        0        0     4814 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/deletefiles.py
--rw-rw-rw-   0        0        0    70345 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/dfxml.py
--rw-rw-rw-   0        0        0      832 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/durationcheck.py
--rw-rw-rw-   0        0        0     7524 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/ffv1mkvvalidate.py
--rw-rw-rw-   0        0        0     1946 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/framemd5.py
--rw-rw-rw-   0        0        0    77085 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/ififuncs.py
--rw-rw-rw-   0        0        0    12425 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/loopline_repackage.py
--rw-rw-rw-   0        0        0     3738 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/make_mediaconch.py
--rw-rw-rw-   0        0        0     1691 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/makedfxml.py
--rw-rw-rw-   0        0        0     3761 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/makedip.py
--rw-rw-rw-   0        0        0    12425 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/makeffv1.py
--rw-rw-rw-   0        0        0    32016 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/makepbcore.py
--rw-rw-rw-   0        0        0      317 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/makeuuid.py
--rw-rw-rw-   0        0        0     3512 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/makezip.py
--rw-rw-rw-   0        0        0     7111 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/manifest.py
--rw-rw-rw-   0        0        0     5859 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/masscopy.py
--rw-rw-rw-   0        0        0      971 2022-11-10 10:42:35.000000 ifiscripts-2023.7.3.1/scripts/massqc.py
--rw-rw-rw-   0        0        0      757 2023-06-08 06:23:40.000000 ifiscripts-2023.7.3.1/scripts/mergepbcore.py
--rw-rw-rw-   0        0        0     2049 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/multicopy.py
--rw-rw-rw-   0        0        0    10808 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/normalise.py
--rw-rw-rw-   0        0        0     2689 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/order.py
--rw-rw-rw-   0        0        0     6820 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/package_update.py
--rw-rw-rw-   0        0        0     3968 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/packagecheck.py
--rw-rw-rw-   0        0        0     4935 2023-02-09 14:47:17.000000 ifiscripts-2023.7.3.1/scripts/prores.py
--rw-rw-rw-   0        0        0    15431 2023-05-23 20:55:54.000000 ifiscripts-2023.7.3.1/scripts/seq2ffv1.py
--rw-rw-rw-   0        0        0    28617 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.1/scripts/sipcreator.py
--rw-rw-rw-   0        0        0     8138 2023-06-16 14:14:33.000000 ifiscripts-2023.7.3.1/scripts/strongbox_fixity.py
--rw-rw-rw-   0        0        0     2750 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/subfolders.py
--rw-rw-rw-   0        0        0     4030 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/testfiles.py
--rw-rw-rw-   0        0        0    10083 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/validate.py
--rw-rw-rw-   0        0        0     7359 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.1/scripts/walk_to_dfxml.py
--rw-rw-rw-   0        0        0       42 2023-07-03 06:52:16.598476 ifiscripts-2023.7.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3152 2023-07-03 06:51:36.000000 ifiscripts-2023.7.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:35:33.009033 ifiscripts-2023.7.3.2/
+-rw-rw-rw-   0        0        0  1006250 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/26_XYZ-22_Rec709.cube
+-rw-rw-rw-   0        0        0     1137 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       72 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1188 2023-07-03 09:35:33.008039 ifiscripts-2023.7.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4589 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/README.rst
+-rw-rw-rw-   0        0        0     5015 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/film_scan_aip_documentation.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 09:35:32.634060 ifiscripts-2023.7.3.2/ifiscripts.egg-info/
+-rw-rw-rw-   0        0        0     1188 2023-07-03 09:35:31.000000 ifiscripts-2023.7.3.2/ifiscripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-07-03 09:35:32.000000 ifiscripts-2023.7.3.2/ifiscripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:35:32.000000 ifiscripts-2023.7.3.2/ifiscripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-03 09:35:32.000000 ifiscripts-2023.7.3.2/ifiscripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-03 09:35:32.000000 ifiscripts-2023.7.3.2/ifiscripts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 09:35:32.773666 ifiscripts-2023.7.3.2/legacy_scripts/
+-rw-rw-rw-   0        0        0     2960 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/batchfixity.py
+-rw-rw-rw-   0        0        0     1639 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/db_cleaning.py
+-rw-rw-rw-   0        0        0    11445 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/dpxonly.py
+-rw-rw-rw-   0        0        0     5145 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/dvsip.py
+-rw-rw-rw-   0        0        0     1054 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/giffer.py
+-rw-rw-rw-   0        0        0     1023 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/loopline.py
+-rw-rw-rw-   0        0        0    11758 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/makedpx.py
+-rw-rw-rw-   0        0        0      883 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/mezzaninecheck.py
+-rw-rw-rw-   0        0        0     1769 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/oeremove.py
+-rw-rw-rw-   0        0        0     3905 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/pg.py
+-rw-rw-rw-   0        0        0     3145 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/playerseq.py
+-rw-rw-rw-   0        0        0    22350 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/premisgui.py
+-rw-rw-rw-   0        0        0     2730 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/qctools.py
+-rw-rw-rw-   0        0        0    16007 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/rawbatch.py
+-rw-rw-rw-   0        0        0      440 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/renumber.py
+-rw-rw-rw-   0        0        0    67528 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/legacy_scripts/revtmd.py
+-rw-rw-rw-   0        0        0     1359 2022-10-18 09:35:53.000000 ifiscripts-2023.7.3.2/legacy_scripts/sha512deep.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:35:33.000038 ifiscripts-2023.7.3.2/scripts/
+-rw-rw-rw-   0        0        0   123258 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/Objects.py
+-rw-rw-rw-   0        0        0     3729 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/accession_register.py
+-rw-rw-rw-   0        0        0    12517 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/aipcreator.py
+-rw-rw-rw-   0        0        0     9815 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/as11fixity.py
+-rw-rw-rw-   0        0        0    16950 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/batchaipcreator.py
+-rw-rw-rw-   0        0        0     6149 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/batchdiff_framemd5.py
+-rw-rw-rw-   0        0        0     3618 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/batchmakeshell.py
+-rw-rw-rw-   0        0        0     6005 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/batchsipcreator.py
+-rw-rw-rw-   0        0        0     9396 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/bitc.py
+-rw-rw-rw-   0        0        0    10479 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/concat.py
+-rw-rw-rw-   0        0        0    32639 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/copyit.py
+-rw-rw-rw-   0        0        0    23142 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/dcpaccess.py
+-rw-rw-rw-   0        0        0    13705 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/dcpfixity.py
+-rw-rw-rw-   0        0        0     4814 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/deletefiles.py
+-rw-rw-rw-   0        0        0    68625 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/dfxml.py
+-rw-rw-rw-   0        0        0      804 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/durationcheck.py
+-rw-rw-rw-   0        0        0     7327 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/ffv1mkvvalidate.py
+-rw-rw-rw-   0        0        0     1946 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/framemd5.py
+-rw-rw-rw-   0        0        0    77085 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/ififuncs.py
+-rw-rw-rw-   0        0        0    12425 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/loopline_repackage.py
+-rw-rw-rw-   0        0        0     3668 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/make_mediaconch.py
+-rw-rw-rw-   0        0        0     1628 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/makedfxml.py
+-rw-rw-rw-   0        0        0     3680 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/makedip.py
+-rw-rw-rw-   0        0        0    12126 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/makeffv1.py
+-rw-rw-rw-   0        0        0    32016 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/makepbcore.py
+-rw-rw-rw-   0        0        0      300 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/makeuuid.py
+-rw-rw-rw-   0        0        0     3414 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/makezip.py
+-rw-rw-rw-   0        0        0     6947 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/manifest.py
+-rw-rw-rw-   0        0        0     5708 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/masscopy.py
+-rw-rw-rw-   0        0        0      971 2022-11-10 10:42:35.000000 ifiscripts-2023.7.3.2/scripts/massqc.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 06:23:40.000000 ifiscripts-2023.7.3.2/scripts/mergepbcore.py
+-rw-rw-rw-   0        0        0     1983 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/multicopy.py
+-rw-rw-rw-   0        0        0    10584 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/normalise.py
+-rw-rw-rw-   0        0        0     2689 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/order.py
+-rw-rw-rw-   0        0        0     6649 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/package_update.py
+-rw-rw-rw-   0        0        0     3853 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/packagecheck.py
+-rw-rw-rw-   0        0        0     4935 2023-02-09 14:47:17.000000 ifiscripts-2023.7.3.2/scripts/prores.py
+-rw-rw-rw-   0        0        0    15431 2023-05-23 20:55:54.000000 ifiscripts-2023.7.3.2/scripts/seq2ffv1.py
+-rw-rw-rw-   0        0        0    28617 2023-07-03 06:45:18.000000 ifiscripts-2023.7.3.2/scripts/sipcreator.py
+-rw-rw-rw-   0        0        0     8138 2023-06-16 14:14:33.000000 ifiscripts-2023.7.3.2/scripts/strongbox_fixity.py
+-rw-rw-rw-   0        0        0     2682 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/subfolders.py
+-rw-rw-rw-   0        0        0     3927 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/testfiles.py
+-rw-rw-rw-   0        0        0     9842 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/validate.py
+-rw-rw-rw-   0        0        0     7154 2023-07-03 09:33:40.000000 ifiscripts-2023.7.3.2/scripts/walk_to_dfxml.py
+-rw-rw-rw-   0        0        0       42 2023-07-03 09:35:33.010034 ifiscripts-2023.7.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3152 2023-07-03 09:34:26.000000 ifiscripts-2023.7.3.2/setup.py
```

### Comparing `ifiscripts-2023.7.3.1/26_XYZ-22_Rec709.cube` & `ifiscripts-2023.7.3.2/26_XYZ-22_Rec709.cube`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/LICENSE.txt` & `ifiscripts-2023.7.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/PKG-INFO` & `ifiscripts-2023.7.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.7.3.1
+Version: 2023.7.3.2
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
 Maintainer: Yazhou He
 Maintainer-email: yhe@irishfilm.ie
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ifiscripts-2023.7.3.1/README.rst` & `ifiscripts-2023.7.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/film_scan_aip_documentation.txt` & `ifiscripts-2023.7.3.2/film_scan_aip_documentation.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/ifiscripts.egg-info/PKG-INFO` & `ifiscripts-2023.7.3.2/ifiscripts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifiscripts
-Version: 2023.7.3.1
+Version: 2023.7.3.2
 Summary: Scripts for processing moving image material in the Irish Film Institute/Irish Film Archive
 Author: Kieran O'Leary
 Author-email: kieran.o.leary@gmail.com
 Maintainer: Yazhou He
 Maintainer-email: yhe@irishfilm.ie
 License: MIT
 Requires-Python: >=3.8
```

### Comparing `ifiscripts-2023.7.3.1/ifiscripts.egg-info/SOURCES.txt` & `ifiscripts-2023.7.3.2/ifiscripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/batchfixity.py` & `ifiscripts-2023.7.3.2/legacy_scripts/batchfixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/db_cleaning.py` & `ifiscripts-2023.7.3.2/legacy_scripts/db_cleaning.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/dpxonly.py` & `ifiscripts-2023.7.3.2/legacy_scripts/dpxonly.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/dvsip.py` & `ifiscripts-2023.7.3.2/legacy_scripts/dvsip.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/giffer.py` & `ifiscripts-2023.7.3.2/legacy_scripts/giffer.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/loopline.py` & `ifiscripts-2023.7.3.2/legacy_scripts/loopline.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/makedpx.py` & `ifiscripts-2023.7.3.2/legacy_scripts/makedpx.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/mezzaninecheck.py` & `ifiscripts-2023.7.3.2/legacy_scripts/mezzaninecheck.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/oeremove.py` & `ifiscripts-2023.7.3.2/legacy_scripts/oeremove.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/pg.py` & `ifiscripts-2023.7.3.2/legacy_scripts/pg.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/playerseq.py` & `ifiscripts-2023.7.3.2/legacy_scripts/playerseq.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/premisgui.py` & `ifiscripts-2023.7.3.2/legacy_scripts/premisgui.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/qctools.py` & `ifiscripts-2023.7.3.2/legacy_scripts/qctools.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/rawbatch.py` & `ifiscripts-2023.7.3.2/legacy_scripts/rawbatch.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/revtmd.py` & `ifiscripts-2023.7.3.2/legacy_scripts/revtmd.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/legacy_scripts/sha512deep.py` & `ifiscripts-2023.7.3.2/legacy_scripts/sha512deep.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/Objects.py` & `ifiscripts-2023.7.3.2/scripts/Objects.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,3465 +1,3465 @@
-
-# This software was developed at the National Institute of Standards
-# and Technology in whole or in part by employees of the Federal
-# Government in the course of their official duties. Pursuant to
-# title 17 Section 105 of the United States Code portions of this
-# software authored by NIST employees are not subject to copyright
-# protection and are in the public domain. For portions not authored
-# by NIST employees, NIST has been granted unlimited rights. NIST
-# assumes no responsibility whatsoever for its use by other parties,
-# and makes no guarantees, expressed or implied, about its quality,
-# reliability, or any other characteristic.
-#
-# We would appreciate acknowledgement if the software is used.
-
-"""
-This file re-creates the major DFXML classes with an emphasis on type safety, serializability, and de-serializability.
-
-With this module, reading disk images or DFXML files is done with the parse or iterparse functions.  Writing DFXML files can be done with the DFXMLObject.print_dfxml function.
-"""
-
-__version__ = "0.7.2"
-
-#Remaining roadmap to 1.0.0:
-# * Documentation.
-# * User testing.
-# * Compatibility with the DFXML schema, version >1.1.1.
-
-import logging
-import re
-import copy
-import xml.etree.ElementTree as ET
-import subprocess
-import dfxml
-import os
-import sys
-import struct
-import platform
-
-_logger = logging.getLogger(os.path.basename(__file__))
-
-#Contains: (namespace, local name) qualified XML element name pairs
-_warned_elements = set([])
-_warned_byterun_attribs = set([])
-
-#Contains: Unexpected 'facet' values on byte_runs elements.
-_warned_byterun_facets = set([])
-
-#Issue some log statements only once per program invocation.
-_nagged_alloc = False
-_warned_byterun_badtypecomp = False
-_nagged_volume_error_impldrift = False
-_nagged_volume_error_standin = False
-
-XMLNS_REGXML = "http://www.forensicswiki.org/wiki/RegXML"
-
-def _ET_tostring(e):
-    """Between Python v2 and v3, there are some differences in the ElementTree library's tostring() behavior.  One, the method balks at the "unicode" encoding in v2.  Two, in 2, the XML prototypes output with every invocation.  This method serves as a wrapper to deal with those issues, plus another issue where ET.tostring prints repeated xmlns declarations (observed on reading and writing a DFXML file twice in the same process).  The repeated prints appear to be from a lack of inspection of existing namespace declarations in the attributes dictionary."""
-    retval = None
-    if sys.version_info[0] < 3:
-        tmp = ET.tostring(e, encoding="UTF-8")
-        if tmp[0:2] == "<?":
-            #Trim away first line; it's an XML prototype.  This only appears in Python 2's ElementTree output.
-            retval = tmp[ tmp.find("?>\n")+3 : ]
-        else:
-            retval = tmp
-    else:
-        retval = ET.tostring(e, encoding="unicode")
-    container_end = retval.index(">")
-    for (uri, prefix) in list(ET._namespace_map.items()):
-        if prefix == "":
-            xmlns_attr_name = "xmlns"
-        else:
-            xmlns_attr_name = "xmlns:" + prefix
-        xmlns_attr_string = '%s="%s"' % (xmlns_attr_name, uri)
-        xmlns_attr_tally = retval.count(xmlns_attr_string, 0, container_end)
-        if xmlns_attr_tally > 1:
-            _logger.warning("ET.tostring() printed a repeated xmlns declaration: %r.  Trimming %d repetition(s)." % (xmlns_attr_string, xmlns_attr_tally-1))
-            container_string = retval[ : container_end+1 ]
-            retval = container_string.replace(xmlns_attr_string, "", xmlns_attr_tally-1) + retval[ container_end+1 : ]
-    return retval
-
-def _boolcast(val):
-    """Takes Boolean values, and 0 or 1 in string or integer form, and casts them all to Boolean.  Preserves nulls.  Balks at everything else."""
-    if val is None:
-        return None
-    if val in [True, False]:
-        return val
-
-    _val = val
-    if val in ["0", "1"]:
-        _val = int(val)
-    if _val in [0, 1]:
-        return _val == 1
-
-    _logger.debug("val = " + repr(val))
-    raise ValueError("Received a not-straightforwardly-Boolean value.  Expected some form of 0, 1, True, or False.")
-
-def _bytecast(val):
-    """Casts a value as a byte string.  If a character string, assumes a UTF-8 encoding."""
-    if val is None:
-        return None
-    if isinstance(val, bytes):
-        return val
-    return _strcast(val).encode("utf-8")
-
-def _intcast(val):
-    """Casts input integer or string to integer.  Preserves nulls.  Balks at everything else."""
-    if val is None:
-        return None
-    if sys.version_info[0] < 3:
-       if isinstance(val, long):
-           return val
-    if isinstance(val, int):
-        return val
-
-    if isinstance(val, str):
-        if val[0] == "-":
-            if val[1:].isdigit():
-                return int(val)
-        else:
-            if val.isdigit():
-                return int(val)
-
-    _logger.debug("val = " + repr(val))
-    raise ValueError("Received a non-int-castable value.  Expected an integer or an integer as a string.")
-
-def _read_differential_annotations(annodict, element, annoset):
-    """
-    Uses the shorthand-to-attribute mappings of annodict to translate attributes of element into annoset.
-    """
-    #_logger.debug("annoset, before: %r." % annoset)
-    #Start with inverting the dictionary
-    _d = { annodict[k].replace("delta:",""):k for k in annodict }
-    #_logger.debug("Inverted dictionary: _d = %r" % _d)
-    for attr in element.attrib:
-        #_logger.debug("Looking for differential annotations: %r" % element.attrib)
-        (ns, an) = _qsplit(attr)
-        if an in _d and ns == dfxml.XMLNS_DELTA:
-            #_logger.debug("Found; adding %r." % _d[an])
-            annoset.add(_d[an])
-    #_logger.debug("annoset, after: %r." % annoset)
-
-def _qsplit(tagname):
-    """Requires string input.  Returns namespace and local tag name as a pair.  I could've sworn this was a basic implementation gimme, but ET.QName ain't it."""
-    _typecheck(tagname, str)
-    if tagname[0] == "{":
-        i = tagname.rfind("}")
-        return ( tagname[1:i], tagname[i+1:] )
-    else:
-        return (None, tagname)
-
-def _strcast(val):
-    if val is None:
-        return None
-    return str(val)
-
-def _typecheck(obj, classinfo):
-    if not isinstance(obj, classinfo):
-        _logger.info("obj = " + repr(obj))
-        if isinstance(classinfo, tuple):
-            raise TypeError("Expecting object to be one of the types %r." % (classinfo,))
-        else:
-            raise TypeError("Expecting object to be of type %r." % classinfo)
-
-class DFXMLObject(object):
-    def __init__(self, *args, **kwargs):
-        self.command_line = kwargs.get("command_line")
-        self.program = kwargs.get("program")
-        self.program_version = kwargs.get("program_version")
-        self.version = kwargs.get("version")
-        self.sources = kwargs.get("sources", [])
-        self.dc = kwargs.get("dc", dict())
-        self.externals = kwargs.get("externals", OtherNSElementList())
-        self.diff_file_ignores = kwargs.get("diff_file_ignores", set())
-
-        self._namespaces = dict()
-        self._volumes = []
-        self._files = []
-
-        self._build_libraries = []
-        self._creator_libraries = []
-
-        input_volumes = kwargs.get("volumes") or []
-        input_files = kwargs.get("files") or []
-        for v in input_volumes:
-            self.append(v)
-        for f in input_files:
-            self.append(f)
-
-        #Add default namespaces
-        self.add_namespace("", dfxml.XMLNS_DFXML)
-        self.add_namespace("dc", dfxml.XMLNS_DC)
-
-    def __iter__(self):
-        """Yields all VolumeObjects, recursively their FileObjects, and the FileObjects directly attached to this DFXMLObject, in that order."""
-        for v in self._volumes:
-            yield v
-            for f in v:
-                yield f
-        for f in self._files:
-            yield f
-
-    def _add_library(self, target_list, *args, **kwargs):
-        #_logger.debug("_add_library:args = %r." % (args,))
-        _library = None
-        if len(args) == 1 and isinstance(args[0], LibraryObject):
-            _library = args[0]
-        elif len(args) > 1 and isinstance(args[0], str) and isinstance(args[1], str):
-            _library = LibraryObject(args[0], args[1])
-        else:
-            raise ValueError("Unexpected arguments format (expecting (string, string) or a LibraryObject): %r." % (args,))
-        #_logger.debug("_library = %r." % _library)
-        if not _library is None:
-            target_list.append(_library)
-
-    def add_build_library(self, *args, **kwargs):
-        self._add_library(self.build_libraries, *args, **kwargs)
-
-    def add_creator_library(self, *args, **kwargs):
-        self._add_library(self.creator_libraries, *args, **kwargs)
-
-    def add_namespace(self, prefix, url):
-        """In case of conflicting namespace definitions, first definition wins."""
-        #_logger.debug("self._namespaces.keys() = %r." % self._namespaces.keys())
-        if prefix not in self._namespaces.keys():
-            #_logger.debug("Registering namespace: %r, %r." % (prefix, url))
-            self._namespaces[prefix] = url
-            ET.register_namespace(prefix, url)
-            #_logger.debug("ET namespaces after registration: %r." % ET._namespace_map)
-
-    def append(self, value):
-        if isinstance(value, VolumeObject):
-            self._volumes.append(value)
-        elif isinstance(value, FileObject):
-            self._files.append(value)
-        else:
-            _logger.debug("value = %r" % value)
-            raise TypeError("Expecting a VolumeObject or a FileObject.  Got instead this type: %r." % type(value))
-
-    def iter_namespaces(self):
-        """Yields (prefix, url) pairs of each namespace registered in this DFXMLObject."""
-        for prefix in sorted(self._namespaces.keys()):
-            yield (prefix, self._namespaces[prefix])
-
-    def populate_from_Element(self, e):
-        if "version" in e.attrib:
-            self.version = e.attrib["version"]
-
-        for ce in e.findall(".//*"):
-            (cns, cln) = _qsplit(ce.tag)
-            if cln == "program":
-                self.program = ce.text
-            elif cln == "version":
-                self.program_version = ce.text
-            elif cln == "command_line":
-                self.command_line = ce.text
-            elif cln == "image_filename":
-                self.sources.append(ce.text)
-            elif cln in ("creator", "build_environment"):
-                for cce in ce.findall(".//*"):
-                    if _qsplit(cce.tag)[1] != "library":
-                        continue
-                    lobj = LibraryObject()
-                    lobj.populate_from_Element(cce)
-                    if cln == "build_environment":
-                        self.add_build_library(lobj)
-                    elif cln == "creator":
-                        self.add_creator_library(lobj)
-            elif (cns, cln) == (dfxml.XMLNS_DELTA, "file_ignore"):
-                self.diff_file_ignores.add(ce.text)
-            elif cns not in [dfxml.XMLNS_DFXML, ""]:
-                #Put all non-DFXML-namespace elements into the externals list.
-                self.externals.append(ce)
-
-    def print_dfxml(self, output_fh=sys.stdout):
-        """Memory-efficient DFXML document printer.  However, it assumes the whole element tree is already constructed."""
-        pe = self.to_partial_Element()
-        dfxml_wrapper = _ET_tostring(pe)
-        #_logger.debug("print_dfxml:dfxml_wrapper = %r." % dfxml_wrapper)
-        dfxml_foot = "</dfxml>"
-        #Check for an empty element
-        if dfxml_wrapper.strip()[-3:] == " />":
-            dfxml_head = dfxml_wrapper.strip()[:-3] + ">"
-        elif dfxml_wrapper.strip()[-2:] == "/>":
-            dfxml_head = dfxml_wrapper.strip()[:-2] + ">"
-        else:
-            dfxml_head = dfxml_wrapper.strip()[:-len(dfxml_foot)]
-
-        output_fh.write("""<?xml version="1.0"?>\n""")
-        output_fh.write(dfxml_head)
-        output_fh.write("\n")
-        _logger.debug("Writing %d volume objects." % len(self._volumes))
-        for v in self._volumes:
-            v.print_dfxml(output_fh)
-            output_fh.write("\n")
-        _logger.debug("Writing %d file objects." % len(self._files))
-        for f in self._files:
-            e = f.to_Element()
-            output_fh.write(_ET_tostring(e))
-            output_fh.write("\n")
-        output_fh.write(dfxml_foot)
-        output_fh.write("\n")
-
-    def to_Element(self):
-        outel = self.to_partial_Element()
-        for v in self._volumes:
-            tmpel = v.to_Element()
-            outel.append(tmpel)
-        for f in self._files:
-            tmpel = f.to_Element()
-            outel.append(tmpel)
-        return outel
-
-    def to_dfxml(self):
-        """Serializes the entire DFXML document tree into a string.  Then returns that string.  RAM-intensive.  Most will want to use print_dfxml() instead"""
-        return _ET_tostring(self.to_Element())
-
-    def to_partial_Element(self):
-        outel = ET.Element("dfxml")
-
-        _logger.debug("self.diff_file_ignores = %r." % self.diff_file_ignores)
-        for diff_file_ignore in sorted(self.diff_file_ignores):
-            self.add_namespace("delta", dfxml.XMLNS_DELTA)
-            tmpel0 = ET.Element("delta:file_ignore")
-            tmpel0.text = diff_file_ignore
-            outel.append(tmpel0)
-
-        for e in self.externals:
-            outel.append(e)
-
-        tmpel0 = ET.Element("metadata")
-        for key in sorted(self.dc):
-            _typecheck(key, str)
-            if ":" in key:
-                raise ValueError("Dublin Core key-value entries should have keys without the colon character.  If this causes an interesting namespace issue for you, please report it as a bug.")
-            tmpel1 = ET.Element("dc:" + key)
-            tmpel1.text = self.dc[key]
-            tmpel0.append(tmpel1)
-        outel.append(tmpel0)
-
-        if self.command_line or \
-          self.program or \
-          self.program_version or \
-          0 < len(self.build_libraries) or \
-          0 < len(self.creator_libraries):
-            tmpel0 = ET.Element("creator")
-            if self.program:
-                tmpel1 = ET.Element("program")
-                tmpel1.text = self.program
-                tmpel0.append(tmpel1)
-            if self.program_version:
-                tmpel1 = ET.Element("version")
-                tmpel1.text = self.program_version
-                tmpel0.append(tmpel1)
-            if 0 < len(self.build_libraries):
-                tmpel1 = ET.Element("build_environment")
-                for library in self._build_libraries:
-                    tmpel2 = library.to_Element()
-                    tmpel1.append(tmpel2)
-                tmpel0.append(tmpel1)
-            if self.command_line:
-                tmpel1 = ET.Element("execution_environment")
-                tmpel2 = ET.Element("command_line")
-                tmpel2.text = self.command_line
-                tmpel1.append(tmpel2)
-                tmpel0.append(tmpel1)
-            for library in self.creator_libraries:
-                tmpel1 = library.to_Element()
-                tmpel0.append(tmpel1)
-            outel.append(tmpel0)
-
-        if len(self.sources) > 0:
-            tmpel0 = ET.Element("source")
-            for source in self.sources:
-                tmpel1 = ET.Element("image_filename")
-                tmpel1.text = source
-                tmpel0.append(tmpel1)
-            outel.append(tmpel0)
-
-        if self.version:
-            outel.attrib["version"] = self.version
-
-        #Apparently, namespace setting is only available with the write() function, which is memory-impractical for significant uses of DFXML.
-        #Ref: http://docs.python.org/3.3/library/xml.etree.elementtree.html#xml.etree.ElementTree.ElementTree.write
-        for (prefix, url) in self.iter_namespaces():
-            if prefix == "":
-                attrib_name = "xmlns"
-            else:
-                attrib_name = "xmlns:" + prefix
-            outel.attrib[attrib_name] = url
-        #_logger.debug("ET namespaces at outel generation: %r." % ET._namespace_map)
-        #_logger.debug("outel.attrib = %r." % outel.attrib)
-
-        return outel
-
-    @property
-    def command_line(self):
-        return self._command_line
-
-    @command_line.setter
-    def command_line(self, value):
-        self._command_line = _strcast(value)
-
-    @property
-    def build_libraries(self):
-        return self._build_libraries
-
-    @property
-    def creator_libraries(self):
-        return self._creator_libraries
-
-    @property
-    def dc(self):
-        """The Dublin Core dictionary of key-value pairs for this document.  Typically, "type" is  "Hash List", or "Disk Image".  Keys should be strings not containing colons, values should be strings.  If this causes an issue for you, please report it as a bug."""
-        return self._dc
-
-    @dc.setter
-    def dc(self, value):
-        _typecheck(value, dict)
-        self._dc = value
-
-    @property
-    def diff_file_ignores(self):
-        """A set of DFXML file properties that are excluded from being flagged as differences.  An example of when one may want to use this is when comparing two file system trees in the same file system: inodes are likely to be a differing factor, best excluded to inspect other changes."""
-        return self._diff_file_ignores
-
-    @diff_file_ignores.setter
-    def diff_file_ignores(self, value):
-        _typecheck(value, set)
-        self._diff_file_ignores = value
-
-    @property
-    def externals(self):
-        """(This property behaves the same as FileObject.externals.)"""
-        return self._externals
-
-    @externals.setter
-    def externals(self, val):
-        _typecheck(val, OtherNSElementList)
-        self._externals = val
-
-    @property
-    def files(self):
-        """List of file objects directly attached to this DFXMLObject.  No setter for now."""
-        return self._files
-
-    @property
-    def namespaces(self):
-        raise AttributeError("The namespaces dictionary should not be directly accessed; instead, use .iter_namespaces().")
-
-    @property
-    def program(self):
-        """This property becomes the element at dfxml/creator/program."""
-        return self._program
-
-    @program.setter
-    def program(self, value):
-        self._program = _strcast(value)
-
-    @property
-    def program_version(self):
-        """This property becomes the element at dfxml/creator/version."""
-        return self._program_version
-
-    @program_version.setter
-    def program_version(self, value):
-        self._program_version = _strcast(value)
-
-    @property
-    def sources(self):
-        return self._sources
-
-    @sources.setter
-    def sources(self, value):
-        if not value is None:
-            _typecheck(value, list)
-        self._sources = value
-
-    @property
-    def version(self):
-        return self._version
-
-    @version.setter
-    def version(self, value):
-        self._version = _strcast(value)
-
-    @property
-    def volumes(self):
-        """List of volume objects directly attached to this DFXMLObject.  No setter for now."""
-        return self._volumes
-
-class LibraryObject(object):
-    def __init__(self, *args, **kwargs):
-        self.name = None
-        self.version = None
-
-        if len(args) >= 1:
-            self.name = args[0]
-        if len(args) >= 2:
-            self.version = args[1]
-
-    def __eq__(self, other):
-        """
-        This equality function tests the name and version values strictly.  For less-strict testing, like allowing matching on missing versions, use relaxed_eq.
-        This function can compare against another LibraryObject.
-        """
-        if not isinstance(other, LibraryObject):
-            return False
-        return self.name == other.name and \
-          self.version == other.version
-
-    def __repr__(self):
-        parts = []
-        if self.name:
-            parts.append("name=%r" % self.name)
-        if self.version:
-            parts.append("version=%r" % self.version)
-        return "LibraryObject(" + ", ".join(parts) + ")"
-
-    def populate_from_Element(self, e):
-        if "name" in e.attrib:
-            self.name = e.attrib["name"]
-        if "version" in e.attrib:
-            self.version = e.attrib["version"]
-
-    def relaxed_eq(self, other):
-        """
-        This function can compare against another LibraryObject.
-        """
-        if not isinstance(other, LibraryObject):
-            return False
-        if self.name != other.name:
-            return False
-        if self.version is None or other.version is None:
-            return True
-        return self.version == other.version
-
-    def to_Element(self):
-        outel = ET.Element("library")
-        if not self.name is None:
-            outel.attrib["name"] = self.name
-        if not self.version is None:
-            outel.attrib["version"] = self.version
-        return outel
-
-    @property
-    def name(self):
-        return self._name
-
-    @name.setter
-    def name(self, value):
-        self._name = _strcast(value)
-
-    @property
-    def version(self):
-        return self._version
-
-    @version.setter
-    def version(self, value):
-        self._version = _strcast(value)
-
-class RegXMLObject(object):
-    def __init__(self, *args, **kwargs):
-        self.command_line = kwargs.get("command_line")
-        self.interpreter = kwargs.get("interpreter")
-        self.metadata = kwargs.get("metadata")
-        self.program = kwargs.get("program")
-        self.program_version = kwargs.get("program_version")
-        self.sources = kwargs.get("sources", [])
-        self.version = kwargs.get("version")
-        self._hives = []
-        self._cells = []
-        self._namespaces = dict()
-        input_hives = kwargs.get("hives") or [] # In case kwargs["hives"] = None.
-        input_cells = kwargs.get("cells") or []
-        for hive in input_hives:
-            self.append(hive)
-        for cell in input_cells:
-            self.append(cells)
-
-        #Add default namespaces
-        #TODO This will cause a problem when the Objects bindings are used for a DFXML document and RegXML document in the same program.
-        self.add_namespace("", XMLNS_REGXML)
-
-    def __iter__(self):
-        """Yields all HiveObjects, recursively their CellObjects, and the CellObjects directly attached to this RegXMLObject, in that order."""
-        for h in self._hives:
-            yield h
-            for c in h:
-                yield c
-        for c in self._cells:
-            yield c
-
-    def add_namespace(self, prefix, url):
-        self._namespaces[prefix] = url
-        ET.register_namespace(prefix, url)
-
-    def append(self, value):
-        if isinstance(value, HiveObject):
-            self._hives.append(value)
-        elif isinstance(value, CellObject):
-            self._cells.append(value)
-        else:
-            _logger.debug("value = %r" % value)
-            raise TypeError("Expecting a HiveObject or a CellObject.  Got instead this type: %r." % type(value))
-
-    def print_regxml(self, output_fh=sys.stdout):
-        """Serializes and prints the entire object, without constructing the whole tree."""
-        regxml_wrapper = _ET_tostring(self.to_partial_Element())
-        #_logger.debug("regxml_wrapper = %r." % regxml_wrapper)
-        regxml_foot = "</regxml>"
-        #Check for an empty element
-        if regxml_wrapper.strip()[-3:] == " />":
-            regxml_head = regxml_wrapper.strip()[:-3] + ">"
-        elif regxml_wrapper.strip()[-2:] == "/>":
-            regxml_head = regxml_wrapper.strip()[:-2] + ">"
-        else:
-            regxml_head = regxml_wrapper.strip()[:-len(regxml_foot)]
-
-        output_fh.write(regxml_head)
-        output_fh.write("\n")
-        for hive in self._hives:
-            hive.print_regxml(output_fh)
-        output_fh.write(regxml_foot)
-        output_fh.write("\n")
-
-    def to_Element(self):
-        outel = self.to_partial_Element()
-
-        for hive in self._hives:
-            tmpel = hive.to_Element()
-            outel.append(tmpel)
-
-        for cell in self._cells:
-            tmpel = cell.to_Element()
-            outel.append(tmpel)
-
-        return outel
-
-    def to_partial_Element(self):
-        """
-        Creates the wrapping RegXML element.  No hives, no cells.  Saves on creating an entire Element tree in memory.
-        """
-        outel = ET.Element("regxml")
-
-        if self.version:
-            outel.attrib["version"] = self.version
-
-        if self.program or self.program_version:
-            tmpel0 = ET.Element("creator")
-            if self.program:
-                tmpel1 = ET.Element("program")
-                tmpel1.text = self.program
-                tmpel0.append(tmpel1)
-            if self.program_version:
-                tmpel1 = ET.Element("version")
-                tmpel1.text = self.program_version
-                tmpel0.append(tmpel1)
-            outel.append(tmpel0)
-
-        if self.command_line:
-            tmpel0 = ET.Element("execution_environment")
-
-            if self.interpreter:
-                tmpel1 = ET.Element("interpreter")
-                tmpel1.text = self.interpreter
-
-            tmpel1 = ET.Element("command_line")
-            tmpel1.text = self.command_line
-            tmpel0.append(tmpel1)
-
-            #TODO Note libraries used at run-time
-
-            outel.append(tmpel0)
-
-        if len(self.sources) > 0:
-            tmpel0 = ET.Element("source")
-            for source in self.sources:
-                tmpel1 = ET.Element("image_filename")
-                tmpel1.text = source
-                tmpel0.append(tmpel1)
-            outel.append(tmpel0)
-
-        #Apparently, namespace setting is only available with the write() function, which is memory-impractical for significant uses of RegXML.
-        #Ref: http://docs.python.org/3.3/library/xml.etree.elementtree.html#xml.etree.ElementTree.ElementTree.write
-        for prefix in sorted(self._namespaces.keys()):
-            if prefix == "":
-                attrib_name = "xmlns"
-            else:
-                attrib_name += "xmlns:" + prefix
-            outel.attrib[attrib_name] = self._namespaces[prefix]
-
-        return outel
-
-    def to_regxml(self):
-        """Serializes the entire RegXML document tree into a string.  Returns that string.  RAM-intensive.  Most will want to use print_regxml() instead."""
-        return _ET_tostring(self.to_Element())
-
-
-class VolumeObject(object):
-
-    _all_properties = set([
-      "annos",
-      "allocated_only",
-      "block_count",
-      "block_size",
-      "byte_runs",
-      "error",
-      "externals",
-      "first_block",
-      "ftype",
-      "ftype_str",
-      "last_block",
-      "partition_offset",
-      "original_volume",
-      "sector_size"
-    ])
-
-    _diff_attr_names = {
-      "new":"delta:new_volume",
-      "deleted":"delta:deleted_volume",
-      "modified":"delta:modified_volume",
-      "matched":"delta:matched"
-    }
-
-    #TODO There may be need in the future to compare the annotations as well.  It complicates make_differential_dfxml too much for now.
-    _incomparable_properties = set([
-      "annos"
-    ])
-
-    def __init__(self, *args, **kwargs):
-        self._files = []
-        self._annos = set()
-        self._diffs = set()
-
-        for prop in VolumeObject._all_properties:
-            if prop in ["annos", "files"]:
-                continue
-            elif prop == "externals":
-                setattr(self, prop, kwargs.get(prop, OtherNSElementList()))
-            else:
-                setattr(self, prop, kwargs.get(prop))
-
-    def __iter__(self):
-        """Yields all FileObjects directly attached to this VolumeObject."""
-        for f in self._files:
-            yield f
-
-    def __repr__(self):
-        parts = []
-        for prop in VolumeObject._all_properties:
-            #Skip outputting the files list.
-            if prop == "files":
-                continue
-            val = getattr(self, prop)
-            if not val is None:
-                parts.append("%s=%r" % (prop, val))
-        return "VolumeObject(" + ", ".join(parts) + ")"
-
-    def append(self, value):
-        _typecheck(value, FileObject)
-        self._files.append(value)
-
-    def compare_to_original(self):
-        self._diffs = self.compare_to_other(self.original_volume, True)
-
-    def compare_to_other(self, other, ignore_original=False):
-        """Returns a set of all the properties found to differ."""
-        _typecheck(other, VolumeObject)
-        diffs = set()
-        for prop in VolumeObject._all_properties:
-            if prop in VolumeObject._incomparable_properties:
-                continue
-            if ignore_original and prop == "original_volume":
-                continue
-
-            #_logger.debug("getattr(self, %r) = %r" % (prop, getattr(self, prop)))
-            #_logger.debug("getattr(other, %r) = %r" % (prop, getattr(other, prop)))
-
-            #Allow file system type to be case-insensitive
-            if prop == "ftype_str":
-                o = getattr(other, prop)
-                if o: o = o.lower()
-                s = getattr(self, prop)
-                if s: s = s.lower()
-                if s != o:
-                    diffs.add(prop)
-            else:
-                if getattr(self, prop) != getattr(other, prop):
-                    diffs.add(prop)
-        return diffs
-
-    def populate_from_Element(self, e):
-        global _warned_elements
-        _typecheck(e, (ET.Element, ET.ElementTree))
-        #_logger.debug("e = %r" % e)
-
-        #Read differential annotations
-        _read_differential_annotations(VolumeObject._diff_attr_names, e, self.annos)
-
-        #Split into namespace and tagname
-        (ns, tn) = _qsplit(e.tag)
-        assert tn in ["volume", "original_volume"]
-
-        #Look through direct-child elements to populate run array
-        for ce in e.findall("./*"):
-            #_logger.debug("ce = %r" % ce)
-            (cns, ctn) = _qsplit(ce.tag)
-            #_logger.debug("cns = %r" % cns)
-            #_logger.debug("ctn = %r" % ctn)
-            if ctn == "byte_runs":
-                self.byte_runs = ByteRuns()
-                self.byte_runs.populate_from_Element(ce)
-            elif ctn == "byte_run":
-                #byte_runs' block recursively handles this element.
-                continue
-            elif ctn == "original_volume":
-                self.original_volume = VolumeObject()
-                self.original_volume.populate_from_Element(ce)
-            elif ctn in VolumeObject._all_properties:
-                #_logger.debug("ce.text = %r" % ce.text)
-                setattr(self, ctn, ce.text)
-                #_logger.debug("getattr(self, %r) = %r" % (ctn, getattr(self, ctn)))
-            elif cns not in [dfxml.XMLNS_DFXML, ""]:
-                #Put all non-DFXML-namespace elements into the externals list.
-                self.externals.append(ce)
-            else:
-                if (cns, ctn) not in _warned_elements:
-                    _warned_elements.add((cns, ctn))
-                    _logger.warning("Unsure what to do with this element in a VolumeObject: %r" % ce)
-
-    def print_dfxml(self, output_fh=sys.stdout):
-        pe = self.to_partial_Element()
-        dfxml_wrapper = _ET_tostring(pe)
-
-        if len(pe) == 0 and len(self._files) == 0:
-            output_fh.write(dfxml_wrapper)
-            return
-
-        dfxml_foot = "</volume>"
-
-        #Deal with an empty element being printed as <elem/>
-        if len(pe) == 0:
-            replaced_dfxml_wrapper = dfxml_wrapper.replace(" />", ">")
-            dfxml_head = replaced_dfxml_wrapper
-        else:
-            dfxml_head = dfxml_wrapper.strip()[:-len(dfxml_foot)]
-
-        output_fh.write(dfxml_head)
-        output_fh.write("\n")
-        _logger.debug("Writing %d file objects for this volume." % len(self._files))
-        for f in self._files:
-            e = f.to_Element()
-            output_fh.write(_ET_tostring(e))
-            output_fh.write("\n")
-        output_fh.write(dfxml_foot)
-        output_fh.write("\n")
-
-    def to_Element(self):
-        outel = self.to_partial_Element()
-        #If there is an error reported on this volume, pop the element off of the partial element's end.
-        errorel = None
-        if not (self.error is None or self.error == ""):
-            if len(outel) == 0:
-                raise ValueError("Partial volume element has no children, but at least the error property was set.")
-            if _qsplit(outel[-1].tag)[1] == "error":
-                #(ET.Element does not have pop().)
-                errorel = outel[-1]
-                del(outel[-1])
-            else:
-                if outel.find("error"):
-                    global _nagged_volume_error_impldrift
-                    if not _nagged_volume_error_impldrift:
-                        _logger.error("Implementation drift - when this code was initially written, the error element was the last to be appended to the partial element.  Leaving the found error element in place for now, but this may fail validation against the schema because of child ordering.")
-                        _nagged_volume_error_impldrift = True
-                else:
-                    global _nagged_volume_error_standin
-                    if not _nagged_volume_error_standin:
-                        _logger.warning("Could not find 'error' child on partial volume element.  Creating a replacement.")
-                        _nagged_volume_error_standin = True
-                    errorel = ET.Element("error")
-                    errorel.text = str(self.error)
-        for f in self._files:
-            tmpel = f.to_Element()
-            outel.append(tmpel)
-        #The error element comes after the fileobject list in the schema.
-        if not errorel is None:
-            outel.append(errorel)
-        return outel
-
-    def to_partial_Element(self):
-        """Returns the volume element with its properties, except for the child fileobjects.  Properties are appended in DFXML schema order."""
-        outel = ET.Element("volume")
-
-        annos_whittle_set = copy.deepcopy(self.annos)
-        diffs_whittle_set = copy.deepcopy(self.diffs)
-
-        #Add differential annotations
-        for annodiff in VolumeObject._diff_attr_names:
-            if annodiff in annos_whittle_set:
-                outel.attrib[VolumeObject._diff_attr_names[annodiff]] = "1"
-                annos_whittle_set.remove(annodiff)
-        if len(annos_whittle_set) > 0:
-            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
-
-        for e in self.externals:
-            outel.append(e)
-
-        if self.byte_runs:
-            outel.append(self.byte_runs.to_Element())
-
-        def _append_el(prop, value):
-            tmpel = ET.Element(prop)
-            _keep = False
-            if not value is None:
-                tmpel.text = str(value)
-                _keep = True
-            if prop in self.diffs:
-                tmpel.attrib["delta:changed_property"] = "1"
-                diffs_whittle_set.remove(prop)
-                _keep = True
-            if _keep:
-                outel.append(tmpel)
-
-        def _append_str(prop):
-            value = getattr(self, prop)
-            _append_el(prop, value)
-
-        def _append_bool(prop):
-            value = getattr(self, prop)
-            if not value is None:
-                value = "1" if value else "0"
-            _append_el(prop, value)
-
-        for prop in [
-          "partition_offset",
-          "sector_size",
-          "block_size",
-          "ftype",
-          "ftype_str",
-          "block_count",
-          "first_block",
-          "last_block"
-        ]:
-            _append_str(prop)
-
-        #Output the one Boolean property
-        _append_bool("allocated_only")
-
-        #Output the original volume's properties
-        if not self.original_volume is None or "original_volume" in diffs_whittle_set:
-            #Skip FileObject list, if any
-            if self.original_volume is None:
-                tmpel = ET.Element("delta:original_volume")
-            else:
-                tmpel = self.original_volume.to_partial_Element()
-                tmpel.tag = "delta:original_volume"
-
-            if "original_volume" in diffs_whittle_set:
-                tmpel.attrib["delta:changed_property"] = "1"
-
-            outel.append(tmpel)
-
-        #Output the error property (which will be popped and re-appended after the file list in to_Element)
-        #The error should come last because of the two spots extended elements can be placed; this is to simplify the file-listing VolumeObject.to_Element() method.
-        _append_str("error")
-
-        if len(diffs_whittle_set) > 0:
-            _logger.warning("Did not annotate all of the differing properties of this volume.  Remaining properties:  %r." % diffs_whittle_set)
-
-        return outel
-
-    @property
-    def allocated_only(self):
-        return self._allocated_only
-
-    @allocated_only.setter
-    def allocated_only(self, val):
-        self._allocated_only = _boolcast(val)
-
-    @property
-    def annos(self):
-        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
-        return self._annos
-
-    @annos.setter
-    def annos(self, val):
-        _typecheck(val, set)
-        self._annos = val
-
-    @property
-    def block_count(self):
-        return self._block_count
-
-    @block_count.setter
-    def block_count(self, val):
-        self._block_count = _intcast(val)
-
-    @property
-    def block_size(self):
-        return self._block_size
-
-    @block_size.setter
-    def block_size(self, val):
-        self._block_size = _intcast(val)
-
-    @property
-    def diffs(self):
-        return self._diffs
-
-    @property
-    def error(self):
-        return self._error
-
-    @error.setter
-    def error(self, val):
-        self._error = _strcast(val)
-
-    @property
-    def externals(self):
-        """(This property behaves the same as FileObject.externals.)"""
-        return self._externals
-
-    @externals.setter
-    def externals(self, val):
-        _typecheck(val, OtherNSElementList)
-        self._externals = val
-
-    @property
-    def files(self):
-        """List of file objects directly attached to this VolumeObject.  No setter for now."""
-        return self._files
-
-    @property
-    def first_block(self):
-        return self._first_block
-
-    @first_block.setter
-    def first_block(self, val):
-        self._first_block = _intcast(val)
-
-    @property
-    def ftype(self):
-        return self._ftype
-
-    @ftype.setter
-    def ftype(self, val):
-        self._ftype = _intcast(val)
-
-    @property
-    def ftype_str(self):
-        return self._ftype_str
-
-    @ftype_str.setter
-    def ftype_str(self, val):
-        self._ftype_str = _strcast(val)
-
-    @property
-    def last_block(self):
-        return self._last_block
-
-    @last_block.setter
-    def last_block(self, val):
-        self._last_block = _intcast(val)
-
-    @property
-    def original_volume(self):
-        return self._original_volume
-
-    @original_volume.setter
-    def original_volume(self, val):
-        if not val is None:
-            _typecheck(val, VolumeObject)
-        self._original_volume= val
-
-    @property
-    def partition_offset(self):
-        return self._partition_offset
-
-    @partition_offset.setter
-    def partition_offset(self, val):
-        self._partition_offset = _intcast(val)
-
-    @property
-    def sector_size(self):
-        return self._sector_size
-
-    @sector_size.setter
-    def sector_size(self, val):
-        self._sector_size = _intcast(val)
-
-class HiveObject(object):
-
-    _all_properties = set([
-      "annos",
-      "mtime",
-      "filename",
-      "original_fileobject",
-      "original_hive"
-    ])
-
-    _diff_attr_names = {
-      "new":"delta:new_hive",
-      "deleted":"delta:deleted_hive",
-      "modified":"delta:modified_hive",
-      "matched":"delta:matched"
-    }
-
-    _incomparable_properties = set([
-      "annos"
-    ])
-
-    def __init__(self, *args, **kwargs):
-        self._cells = []
-        self._annos = set()
-        self._diffs = set()
-
-        for prop in HiveObject._all_properties:
-            if prop in ["annos", "cells"]:
-                continue
-            setattr(self, prop, kwargs.get(prop))
-
-    def __iter__(self):
-        """Yields all CellObjects directly attached to this HiveObject."""
-        for c in self._cells:
-            yield c
-
-    def append(self, value):
-        _typecheck(value, CellObject)
-        self._cells.append(value)
-
-    def compare_to_original(self):
-        self._diffs = self.compare_to_other(self.original_hive, True)
-
-    def compare_to_other(self, other, ignore_original=False):
-        """Returns a set of all the properties found to differ."""
-        _typecheck(other, HiveObject)
-        diffs = set()
-        for prop in HiveObject._all_properties:
-            if prop in HiveObject._incomparable_properties:
-                continue
-            if ignore_original and prop == "original_hive":
-                continue
-
-            #Allow file system type to be case-insensitive
-            if getattr(self, prop) != getattr(other, prop):
-                diffs.add(prop)
-        return diffs
-
-    def print_regxml(self, output_fh=sys.stdout):
-        pe = self.to_partial_Element()
-        xml_wrapper = _ET_tostring(pe)
-        xml_foot = "</hive>"
-        #Check for an empty element
-        if xml_wrapper.strip()[-3:] == " />":
-            xml_head = xml_wrapper.strip()[:-3] + ">"
-        elif xml_wrapper.strip()[-2:] == "/>":
-            xml_head = xml_wrapper.strip()[:-2] + ">"
-        else:
-            xml_head = xml_wrapper.strip()[:-len(xml_foot)]
-
-        output_fh.write(xml_head)
-        output_fh.write("\n")
-
-        for cell in self._cells:
-            output_fh.write(cell.to_regxml())
-            output_fh.write("\n")
-
-        output_fh.write(xml_foot)
-        output_fh.write("\n")
-
-    def to_Element(self):
-        outel = self.to_partial_Element()
-        for cell in self._cells:
-            tmpel = cell.to_Element()
-            outel.append(tmpel)
-        return outel
-
-    def to_partial_Element(self):
-        outel = ET.Element("hive")
-
-        if self.filename:
-            tmpel = ET.Element("filename")
-            tmpel.text = self.filename
-            outel.append(tmpel)
-
-        if self.mtime:
-            tmpel = self.mtime.to_Element()
-            outel.append(tmpel)
-
-        if self.original_fileobject:
-            tmpel = self.original_fileobject.to_Element()
-            #NOTE: "delta" namespace intentionally omitted.
-            tmpel.tag = "original_fileobject"
-            outel.append(tmpel)
-
-        return outel
-
-    @property
-    def annos(self):
-        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
-        return self._annos
-
-    @annos.setter
-    def annos(self, val):
-        _typecheck(val, set)
-        self._annos = val
-
-    @property
-    def filename(self):
-        """Path of the hive file within the parent file system."""
-        return self._filename
-
-    @filename.setter
-    def filename(self, val):
-        self._filename = _strcast(val)
-
-    @property
-    def mtime(self):
-        return self._mtime
-
-    @mtime.setter
-    def mtime(self, val):
-        if val is None:
-            self._mtime = None
-        elif isinstance(val, TimestampObject):
-            self._mtime = val
-        else:
-            checked_val = TimestampObject(val, name="mtime")
-            self._mtime = checked_val
-
-    @property
-    def original_fileobject(self):
-        return self._original_fileobject
-
-    @original_fileobject.setter
-    def original_fileobject(self, val):
-        if not val is None:
-            _typecheck(val, FileObject)
-        self._original_fileobject = val
-
-    @property
-    def original_hive(self):
-        return self._original_hive
-
-    @original_hive.setter
-    def original_hive(self, val):
-        if not val is None:
-            _typecheck(val, HiveObject)
-        self._original_hive = val
-
-class ByteRun(object):
-
-    _all_properties = set([
-      "img_offset",
-      "fs_offset",
-      "file_offset",
-      "fill",
-      "len",
-      "type",
-      "uncompressed_len"
-    ])
-
-    def __init__(self, *args, **kwargs):
-        for prop in ByteRun._all_properties:
-            setattr(self, prop, kwargs.get(prop))
-
-    def __add__(self, other):
-        """
-        Joins two ByteRun objects into a single run if possible.  Returns a new object of the concatenation if successful, None if not.
-        """
-        _typecheck(other, ByteRun)
-        #Don't glom fills of different values
-        if self.fill != other.fill:
-            return None
-
-        #Don't glom typed byte runs (particularly since type has been observed to be 'resident')
-        if self.type != other.type:
-            return None
-
-        #Don't glom compressed runs
-        if not self.uncompressed_len is None or not other.uncompressed_len is None:
-            return None
-
-        if None in [self.len, other.len]:
-            return None
-
-        for prop in ["img_offset", "fs_offset", "file_offset"]:
-            if None in [getattr(self, prop), getattr(other, prop)]:
-                continue
-            if getattr(self, prop) + self.len == getattr(other, prop):
-                retval = copy.deepcopy(self)
-                retval.len += other.len
-                return retval
-        return None
-
-    def __eq__(self, other):
-        #Check type
-        if other is None:
-            return False
-        if not isinstance(other, ByteRun):
-            if not _warned_byterun_badtypecomp:
-                _logger.warning("A ByteRun comparison was called against a non-ByteRun object: " + repr(other) + ".")
-                _warned_byterun_badtypecomp = True
-            return False
-
-        #Check values
-        return \
-          self.img_offset == other.img_offset and \
-          self.fs_offset == other.fs_offset and \
-          self.file_offset == other.file_offset and \
-          self.fill == other.fill and \
-          self.len == other.len and \
-          self.type == other.type and \
-          self.uncompressed_len == other.uncompressed_len
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        parts = []
-        for prop in ByteRun._all_properties:
-            val = getattr(self, prop)
-            if not val is None:
-                parts.append("%s=%r" % (prop, val))
-        return "ByteRun(" + ", ".join(parts) + ")"
-
-    def populate_from_Element(self, e):
-        _typecheck(e, (ET.Element, ET.ElementTree))
-
-        #Split into namespace and tagname
-        (ns, tn) = _qsplit(e.tag)
-        assert tn == "byte_run"
-
-        copied_attrib = copy.deepcopy(e.attrib)
-
-        #Populate run properties from element attributes
-        for prop in ByteRun._all_properties:
-            if prop in copied_attrib:
-                val = copied_attrib.get(prop)
-                if not val is None:
-                    setattr(self, prop, val)
-                del copied_attrib[prop]
-        #Note remaining properties
-        for prop in copied_attrib:
-            if prop not in _warned_byterun_attribs:
-                _warned_byterun_attribs.add(prop)
-                _logger.warning("No instructions present for processing this attribute found on a byte run: %r." % prop)
-
-    def to_Element(self):
-        outel = ET.Element("byte_run")
-        for prop in ByteRun._all_properties:
-            val = getattr(self, prop)
-            #Skip null properties
-            if val is None:
-                continue
-
-            if isinstance(val, bytes):
-                outel.attrib[prop] = str(struct.unpack("b", val)[0])
-            else:
-                outel.attrib[prop] = str(val)
-
-        return outel
-
-    @property
-    def file_offset(self):
-        return self._file_offset
-
-    @file_offset.setter
-    def file_offset(self, val):
-        self._file_offset = _intcast(val)
-
-    @property
-    def fill(self):
-        """
-        At the moment, the fill value is assumed to be a single byte.  The value you receive from this property wll be None or a byte.  Setting fill to the string "0" will return the null byte when retrieved later.
-
-        For now, setting to any digital string (e.g. "41") will return a byte representing the integer casting string (e.g. the number 41), but this is subject to change pending some discussion.
-        """
-        return self._fill
-
-    @fill.setter
-    def fill(self, val):
-        if val is None:
-            self._fill = val
-        elif val == "0":
-            self._fill = b'\x00'
-        elif isinstance(val, bytes):
-            if len(val) != 1:
-                raise NotImplementedError("Received a %d-length fill byte string for a byte run.  Only 1-byte fill strings are accepted for now, pending further discussion.")
-            self._fill = val
-        elif isinstance(val, int):
-            #This is the easiest way between Python 2 and 3.  int.to_bytes would be better, but that is only in >=3.2.
-            self._fill = struct.pack("b", val)
-        elif isinstance(val, str) and val.isdigit():
-            #Recurse, changing type
-            self.fill = int(val)
-
-    @property
-    def fs_offset(self):
-        return self._fs_offset
-
-    @fs_offset.setter
-    def fs_offset(self, val):
-        self._fs_offset = _intcast(val)
-
-    @property
-    def img_offset(self):
-        return self._img_offset
-
-    @img_offset.setter
-    def img_offset(self, val):
-        self._img_offset = _intcast(val)
-
-    @property
-    def len(self):
-        return self._len
-
-    @len.setter
-    def len(self, val):
-        self._len = _intcast(val)
-
-    @property
-    def type(self):
-        return self._type
-
-    @type.setter
-    def type(self, val):
-        self._type = _strcast(val)
-
-    @property
-    def uncompressed_len(self):
-        return self._uncompressed_len
-
-    @uncompressed_len.setter
-    def uncompressed_len(self, val):
-        self._uncompressed_len = _intcast(val)
-
-class ByteRuns(object):
-    """
-    A list-like object for ByteRun objects.
-    """
-    #Must define these methods to adhere to the list protocol:
-    #__len__
-    #__getitem__
-    #__setitem__
-    #__delitem__
-    #__iter__
-    #append
-    #
-    #Refs:
-    #http://www.rafekettler.com/magicmethods.html
-    #http://stackoverflow.com/a/8841520
-
-    _facet_values = [None, "data", "inode", "name"]
-
-    def __init__(self, run_list=None, **kwargs):
-        self._facet = kwargs.get("facet")
-        self._listdata = []
-        if isinstance(run_list, list):
-            for run in run_list:
-                self.append(run)
-
-    def __delitem__(self, key):
-        del self._listdata[key]
-
-    def __eq__(self, other):
-        """Compares the byte run lists and the facet (allowing a null facet to match "data")."""
-        #Check type
-        if other is None:
-            return False
-        _typecheck(other, ByteRuns)
-
-        if self.facet != other.facet:
-            if set([self.facet, other.facet]) != set([None, "data"]):
-                return False
-        if len(self) != len(other):
-            #_logger.debug("len(self) = %d" % len(self))
-            #_logger.debug("len(other) = %d" % len(other))
-            return False
-        for (sbr_index, sbr) in enumerate(self):
-            obr = other[sbr_index]
-            #_logger.debug("sbr_index = %d" % sbr_index)
-            #_logger.debug("sbr = %r" % sbr)
-            #_logger.debug("obr = %r" % obr)
-            if sbr != obr:
-                return False
-        return True
-
-    def __getitem__(self, key):
-        return self._listdata.__getitem__(key)
-
-    def __iter__(self):
-        return iter(self._listdata)
-
-    def __len__(self):
-        return self._listdata.__len__()
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        parts = []
-        for run in self:
-            parts.append(repr(run))
-        maybe_facet = ""
-        if self.facet:
-            maybe_facet = "facet=%r, " % self.facet
-        return "ByteRuns(" + maybe_facet + "run_list=[" + ", ".join(parts) + "])"
-
-    def __setitem__(self, key, value):
-        _typecheck(value, ByteRun)
-        self._listdata[key] = value
-
-    def append(self, value):
-        """
-        Appends a ByteRun object to this container's list.
-        """
-        _typecheck(value, ByteRun)
-        self._listdata.append(value)
-
-    def glom(self, value):
-        """
-        Appends a ByteRun object to this container's list, after attempting to join the run with the last run already stored.
-        """
-        _typecheck(value, ByteRun)
-        if len(self._listdata) == 0:
-            self.append(value)
-        else:
-            last_run = self._listdata[-1]
-            maybe_new_run = last_run + value
-            if maybe_new_run is None:
-                self.append(value)
-            else:
-                self._listdata[-1] = maybe_new_run
-
-    def iter_contents(self, raw_image, buffer_size=1048576, sector_size=512, errlog=None, statlog=None):
-        """
-        Generator.  Yields contents, as byte strings one block at a time, given a backing raw image path.  Relies on The SleuthKit's img_cat, so contents can be extracted from any disk image type that TSK supports.
-        @param buffer_size The maximum size of the byte strings yielded.
-        @param sector_size The size of a disk sector in the raw image.  Required by img_cat.
-        """
-        if not isinstance(raw_image, str):
-            raise TypeError("iter_contents needs the string path to the image file.  Received: %r." % raw_image)
-
-        stderr_fh = None
-        if not errlog is None:
-            stderr_fh = open(errlog, "wb")
-
-        status_fh = None
-        if not statlog is None:
-            status_fh = open(errlog, "wb")
-
-        #The exit status of the last img_cat.
-        last_status = None
-
-        try:
-            for run in self:
-                if run.len is None:
-                    raise AttributeError("Byte runs can't be extracted if a run length is undefined.")
-
-                len_to_read = run.len
-
-                #If we have a fill character, just pump out that character
-                if not run.fill is None and len(run.fill) > 0:
-                    while len_to_read > 0:
-                        #This multiplication and slice should handle multi-byte fill characters, in case that ever comes up.
-                        yield (run.fill * buffer_size)[ : min(len_to_read, buffer_size)]
-                        len_to_read -= buffer_size
-                    #Next byte run
-                    continue
-
-                if run.img_offset is None:
-                    raise AttributeError("Byte runs can't be extracted if missing a fill character and image offset.")
-
-                cmd = ["img_cat"]
-                cmd.append("-b")
-                cmd.append(str(sector_size))
-                cmd.append("-s")
-                cmd.append(str(run.img_offset//sector_size))
-                cmd.append("-e")
-                cmd.append(str( (run.img_offset + run.len)//sector_size))
-                cmd.append(raw_image)
-                p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=stderr_fh)
-
-                #Do the buffered read
-                while len_to_read > 0:
-                    buffer_data = p.stdout.read(buffer_size)
-                    yield_data = buffer_data[ : min(len_to_read, buffer_size)]
-                    if len(yield_data) > 0:
-                        yield yield_data
-                    else:
-                        #Let the subprocess terminate so we can see the exit status
-                        p.wait()
-                        last_status = p.returncode
-                        if last_status != 0:
-                            raise subprocess.CalledProcessError(last_status, " ".join(cmd), "img_cat failed.")
-                    len_to_read -= buffer_size
-        except Exception as e:
-            #Cleanup in an exception
-            if not stderr_fh is None:
-                stderr_fh.close()
-
-            if not status_fh is None:
-                if isinstance(e, subprocess.CalledProcessError):
-                    status_fh.write(e.returncode)
-                else:
-                    status_fh.write("1")
-                status_fh.close()
-            raise e
-
-        #Cleanup when all's gone well.
-        if not status_fh is None:
-            if not last_status is None:
-                status_fh.write(last_status)
-            status_fh.close()
-        if not stderr_fh is None:
-            stderr_fh.close()
-
-    def populate_from_Element(self, e):
-        _typecheck(e, (ET.Element, ET.ElementTree))
-
-        #Split into namespace and tagname
-        (ns, tn) = _qsplit(e.tag)
-        assert tn == "byte_runs"
-
-        if "facet" in e.attrib:
-            self.facet = e.attrib["facet"]
-
-        #Look through direct-child elements to populate run array
-        for ce in e.findall("./*"):
-            (cns, ctn) = _qsplit(ce.tag)
-            if ctn == "byte_run":
-                nbr = ByteRun()
-                nbr.populate_from_Element(ce)
-                self.append(nbr)
-
-    def to_Element(self):
-        outel = ET.Element("byte_runs")
-        for run in self:
-            tmpel = run.to_Element()
-            outel.append(tmpel)
-        if self.facet:
-            outel.attrib["facet"] = self.facet
-        return outel
-
-    @property
-    def facet(self):
-        """Expected to be null, "data", "inode", or "name".  See FileObject.data_brs, FileObject.inode_brs, and FileObject.name_brs."""
-        return self._facet
-
-    @facet.setter
-    def facet(self, val):
-        if not val is None:
-            _typecheck(val, str)
-        if val not in ByteRuns._facet_values:
-            raise ValueError("A ByteRuns facet must be one of these: %r.  Received: %r." % (ByteRuns._facet_values, val))
-        self._facet = val
-
-re_precision = re.compile(r"(?P<num>\d+)(?P<unit>(|m|n)s|d)?")
-class TimestampObject(object):
-    """
-    Encodes the "dftime" type.  Wraps around dfxml.dftime, closely enough that this might just get folded into that class.
-
-    TimestampObjects implement a vs-null comparison workaround as in the SAS family of products:  Null, for ordering purposes, is considered to be a value less than negative infinity.
-    """
-
-    timestamp_name_list = ["mtime", "atime", "ctime", "crtime", "dtime", "bkup_time"]
-
-    def __init__(self, *args, **kwargs):
-        self.name = kwargs.get("name")
-        self.prec = kwargs.get("prec")
-        #_logger.debug("type(args) = %r" % type(args))
-        #_logger.debug("args = %r" % (args,))
-        if len(args) == 0:
-            self.time = None
-        elif len(args) == 1:
-            self.time = args[0]
-        else:
-            raise ValueError("Unexpected arguments.  Whole args tuple: %r." % (args,))
-
-        self._timestamp = None
-
-    def __eq__(self, other):
-        #Check type
-        if other is None:
-            return False
-        _typecheck(other, TimestampObject)
-
-        if self.name != other.name:
-            return False
-        if self.prec != other.prec:
-            return False
-        if self.time != other.time:
-            return False
-        return True
-
-    def __ge__(self, other):
-        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
-        if other is None:
-            return False
-        else:
-            self._comparison_sanity_check(other)
-        return self.time.__ge__(other.time)
-
-    def __gt__(self, other):
-        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
-        if other is None:
-            return False
-        else:
-            self._comparison_sanity_check(other)
-        return self.time.__gt__(other.time)
-
-    def __le__(self, other):
-        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
-        if other is None:
-            return True
-        else:
-            self._comparison_sanity_check(other)
-        return self.time.__le__(other.time)
-
-    def __lt__(self, other):
-        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
-        if other is None:
-            return True
-        else:
-            self._comparison_sanity_check(other)
-        return self.time.__lt__(other.time)
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        parts = []
-        if self.name:
-            parts.append("name=%r" % self.name)
-        if self.prec:
-            parts.append("prec=%r" % (self.prec,))
-        if self.time:
-            parts.append("%r" % self.time)
-        return "TimestampObject(" + ", ".join(parts) + ")"
-
-    def __str__(self):
-        if self.time:
-            return str(self.time)
-        else:
-            return self.__repr__()
-
-    def _comparison_sanity_check(self, other):
-        if None in (self.time, other.time):
-            raise ValueError("Can't compare TimestampObjects: %r, %r." % self, other)
-
-    def populate_from_Element(self, e):
-        _typecheck(e, (ET.Element, ET.ElementTree))
-        if "prec" in e.attrib:
-            self.prec = e.attrib["prec"]
-        self.time = e.text
-        (ns, tn) = _qsplit(e.tag)
-        self.name = tn
-
-    def to_Element(self):
-        _typecheck(self.name, str)
-        outel = ET.Element(self.name)
-        if self.prec:
-            outel.attrib["prec"] = "%d%s" % self.prec
-        if self.time:
-            outel.text = str(self.time)
-        return outel
-
-    @property
-    def name(self):
-        """The type of timestamp - modified (mtime), accessed (atime), etc."""
-        return self._name
-
-    @name.setter
-    def name(self, value):
-        if not value is None:
-            if not value in TimestampObject.timestamp_name_list:
-                raise ValueError("The timestamp name must be in this list: %r.  Received: %r." % (TimestampObject.timestamp_name_list, value))
-        self._name = value
-
-    @property
-    def prec(self):
-        """
-        A pair, (resolution, unit); unit is a second (s), millisecond, nanosecond, or day (d).  The default unit is "s".  Can be passed as a string or a duple.
-        """
-        return self._prec
-
-    @prec.setter
-    def prec(self, value):
-        if value is None:
-            self._prec = None
-            return self._prec
-        elif isinstance(value, tuple) and \
-          len(value) == 2 and \
-          isinstance(value[0], int) and \
-          isinstance(value[1], str):
-            self._prec = value
-            return self._prec
-
-        m = re_precision.match(value)
-        md = m.groupdict()
-        tup = (int(md["num"]), md.get("unit") or "s")
-        #_logger.debug("tup = %r" % (tup,))
-        self._prec = tup
-
-    @property
-    def time(self):
-        """
-        The actual timestamp.  A dfxml.dftime object.  This class might be superfluous and end up collapsing into that...
-        """
-        return self._time
-
-    @time.setter
-    def time(self, value):
-        if value is None:
-            self._time = None
-        else:
-            checked_value = dfxml.dftime(value)
-            #_logger.debug("checked_value.timestamp() = %r" % checked_value.timestamp())
-            self._time = checked_value
-            #Propagate timestamp value to other formats
-            self._timestamp = self._time.timestamp()
-
-    @property
-    def timestamp(self):
-        """A Unix floating-point timestamp, as time.mktime returns.  Currently, there is no setter for this property."""
-        return self._timestamp
-
-
-class FileObject(object):
-    """
-    This class provides property accesses, an XML serializer (ElementTree-based), and a deserializer.
-    The properties interface is NOT function calls, but simple accesses.  That is, the old _fileobject_ style:
-
-        assert isinstance(fi, dfxml.fileobject)
-        fi.mtime()
-
-    is now replaced with:
-
-        assert isinstance(fi, Objects.FileObject)
-        fi.mtime
-    """
-
-    _all_properties = set([
-      "alloc",
-      "alloc_inode",
-      "alloc_name",
-      "annos",
-      "atime",
-      "bkup_time",
-      "byte_runs",
-      "compressed",
-      "crtime",
-      "ctime",
-      "data_brs",
-      "dtime",
-      "error",
-      "externals",
-      "filename",
-      "filesize",
-      "gid",
-      "id",
-      "inode",
-      "inode_brs",
-      "link_target",
-      "libmagic",
-      "md5",
-      "meta_type",
-      "mode",
-      "mtime",
-      "name_brs",
-      "name_type",
-      "nlink",
-      "original_fileobject",
-      "orphan",
-      "parent_object",
-      "partition",
-      "seq",
-      "sha1",
-      "sha256",
-      "sha512",
-      "uid",
-      "unalloc",
-      "unused",
-      "used"
-    ])
-
-    _br_facet_to_property = {
-      "data":"data_brs",
-      "inode":"inode_brs",
-      "name":"name_brs"
-    }
-
-    #TODO There may be need in the future to compare the annotations as well.  It complicates make_differential_dfxml too much for now.
-    _incomparable_properties = set([
-      "annos",
-      "byte_runs",
-      "id",
-      "unalloc",
-      "unused"
-    ])
-
-    _diff_attr_names = {
-      "new":"delta:new_file",
-      "deleted":"delta:deleted_file",
-      "renamed":"delta:renamed_file",
-      "changed":"delta:changed_file",
-      "modified":"delta:modified_file",
-      "matched":"delta:matched"
-    }
-
-    def __init__(self, *args, **kwargs):
-        #Prime all the properties
-        for prop in FileObject._all_properties:
-            if prop == "annos":
-                continue
-            elif prop == "externals":
-                setattr(self, prop, kwargs.get(prop, OtherNSElementList()))
-            else:
-                setattr(self, prop, kwargs.get(prop))
-        self._annos = set()
-        self._diffs = set()
-
-    def __eq__(self, other):
-        if other is None:
-            return False
-        _typecheck(other, FileObject)
-        for prop in FileObject._all_properties:
-            if prop in FileObject._incomparable_properties:
-                continue
-            if getattr(self, prop) != getattr(other, prop):
-                return False
-        return True
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        parts = []
-
-        for prop in sorted(FileObject._all_properties):
-            #Save data byte runs for the end, as theirs lists can get really long.
-            if prop not in ["byte_runs", "data_brs"]:
-                value = getattr(self, prop)
-                if not value is None:
-                    parts.append("%s=%r" % (prop, value))
-
-        if self.data_brs:
-            parts.append("data_brs=%r" % self.byte_runs)
-
-        return "FileObject(" + ", ".join(parts) + ")"
-
-    def compare_to_original(self, **kwargs):
-        file_ignores = kwargs.get("file_ignores", set())
-        self._diffs = self.compare_to_other(self.original_fileobject, True, file_ignores)
-
-    def compare_to_other(self, other, ignore_original=False, file_ignores=set()):
-        _typecheck(other, FileObject)
-
-        diffs = set()
-
-        for propname in FileObject._all_properties:
-            if propname in file_ignores:
-                continue
-            if propname in FileObject._incomparable_properties:
-                continue
-            if ignore_original and propname == "original_fileobject":
-                continue
-            oval = getattr(other, propname)
-            sval = getattr(self, propname)
-            if oval is None and sval is None:
-                continue
-            if oval != sval:
-                #_logger.debug("propname, oval, sval: %r, %r, %r" % (propname, oval, sval))
-                diffs.add(propname)
-
-        return diffs
-
-    def extract_facet(self, facet, image_path=None, buffer_size=1048576, partition_offset=None, sector_size=512, errlog=None, statlog=None, icat_threshold = 268435456):
-        """
-        Generator.  Extracts the facet with a SleuthKit tool, yielding chunks of the data.
-
-        @param buffer_size The facet data is yielded in chunks of at most this parameter's size. Default 1MiB.
-        @param partition_offset The offset of the file's containing partition, in bytes.  Needed for icat.  If not given, the FileObject's VolumeObject will be used.  If that's also absent, icat can't be used, and img_cat will instead be tried as a fallback (which means byte runs must be in the DFXML).
-        @param icat_threshold icat incurs extensive, non-sequential IO overhead to walk the filesystem to reach the facet's byte runs.  img_cat can be called on each byte run reported in the DFXML file, but on fragmented files this incurs overhead in process spawning.  Facets larger than this threshold are extracted with icat.  Default 256MiB.  Force icat by setting this to -1; force img_cat with infinity (float("inf")).
-        """
-
-        _image_path = image_path
-        if _image_path is None:
-            raise ValueError("The backing image path must be supplied.")
-
-        _partition_offset = partition_offset
-        if _partition_offset is None:
-            if self.volume_object:
-                _partition_offset = self.volume_object.partition_offset
-
-        #Try using icat; needs inode number and volume offset.  We're additionally requiring the filesize be known.
-        #TODO The icat needs a little more experimentation.
-        if False and facet == "content" and \
-          not self.filesize is None and \
-          self.filesize >= icat_threshold and \
-          not self.inode is None and \
-          not _partition_offset is None:
-            _logger.debug("Extracting with icat: %r." % self)
-
-            #Set up logging if desired
-            stderr_fh = sys.stderr
-            if not errlog is None:
-                stderr_fh = open(errlog, "wb")
-
-            status_fh = None
-            if not statlog is None:
-                status_fh = open(errlog, "w")
-
-            #Set up icat process
-            cmd = ["icat"]
-            cmd.append("-b")
-            cmd.append(str(sector_size))
-            cmd.append("-o")
-            cmd.append(str(self.volume_object.partition_offset//sector_size))
-            if not self.volume_object.ftype_str is None:
-                cmd.append("-f")
-                cmd.append(self.volume_object.ftype_str)
-            cmd.append(image_path)
-            cmd.append(str(self.inode))
-            p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=stderr_fh)
-
-            #Do a buffered read
-            len_to_read = self.filesize
-            while len_to_read > 0:
-                buffer_data = p.stdout.read(buffer_size)
-                yield_data = buffer_data[ : min(len_to_read, buffer_size)]
-                if len(yield_data) > 0:
-                    yield yield_data
-                else:
-                    #Let the subprocess terminate so we can see the exit status
-                    p.wait()
-                    last_status = p.returncode
-
-                    #Log the status if requested
-                    if not status_fh is None:
-                        status_fh.write(last_status)
-
-                    #Act on a bad status
-                    if last_status != 0:
-                        raise subprocess.CalledProcessError(last_status, " ".join(cmd), "icat failed.")
-                len_to_read -= buffer_size
-
-            #Clean up file handles
-            if status_fh: status_fh.close()
-            if stderr_fh: stderr_fh.close()
-
-        elif not self.byte_runs is None:
-            for chunk in self.byte_runs.iter_contents(_image_path, buffer_size, sector_size, errlog, statlog):
-                yield chunk
-
-    def is_allocated(self):
-        """Collapse potentially-partial allocation information into a yes, no, or unknown answer."""
-        if self.alloc_inode == True and self.alloc_name == True:
-            return True
-        if self.alloc_inode is None and self.alloc_name is None:
-            if self.alloc is None:
-                return None
-            else:
-                return self.alloc
-        #Partial allocation information at this point is assumed False.  In some file systems, like FAT, we only need one of alloc_inode and alloc_name for allocation status.  Guidelines on which should win out haven't been set yet, though, so wait on this.
-        return False
-
-    def populate_from_Element(self, e):
-        """Populates this FileObject's properties from an ElementTree Element.  The Element need not be retained."""
-        global _warned_elements
-        _typecheck(e, (ET.Element, ET.ElementTree))
-
-        #_logger.debug("FileObject.populate_from_Element(%r)" % e)
-
-        #Split into namespace and tagname
-        (ns, tn) = _qsplit(e.tag)
-        assert tn in ["fileobject", "original_fileobject", "parent_object"]
-
-        #Map "delta:" attributes of <fileobject>s into the self.annos set
-        #_logger.debug("self.annos, before: %r." % self.annos)
-        _read_differential_annotations(FileObject._diff_attr_names, e, self.annos)
-        #_logger.debug("self.annos, after: %r." % self.annos)
-
-        #Look through direct-child elements for other properties
-        for ce in e.findall("./*"):
-            (cns, ctn) = _qsplit(ce.tag)
-            #_logger.debug("Populating from child element: %r." % ce.tag)
-
-            #Inherit any marked changes
-            for attr in ce.attrib:
-                #_logger.debug("Inspecting attr for diff. annos: %r." % attr)
-                (ns, an) = _qsplit(attr)
-                if an == "changed_property" and ns == dfxml.XMLNS_DELTA:
-                    #_logger.debug("Identified changed property: %r." % ctn)
-                    #TODO There may be a more elegant way of handling the hashes and any other attribute-dependent element-to-property mapping.  Probably involving XPath.
-                    if ctn == "hashdigest":
-                        if "type" not in ce.attrib:
-                            raise AttributeError("Attribute 'type' not found.  Every hashdigest element should have a 'type' attribute to identify the hash type.")
-                        self.diffs.add(ce.attrib["type"].lower())
-                    elif ctn == "byte_runs":
-                        facet = ce.attrib.get("facet")
-                        prop = FileObject._br_facet_to_property.get(facet, "data_brs")
-                        self.diffs.add(prop)
-                    else:
-                        self.diffs.add(ctn)
-
-            if ctn == "byte_runs":
-                #byte_runs might be for file contents, the inode/MFT entry, or the directory entry naming the file.  Use the facet attribute to determine which.  If facet is absent, assume they're data byte runs.
-                if "facet" in ce.attrib:
-                    if ce.attrib["facet"] not in FileObject._br_facet_to_property:
-                        if not ce.attrib["facet"] in _warned_byterun_facets:
-                            _warned_byterun_facets.add(ce.attrib["facet"])
-                            _logger.warning("byte_runs facet %r was unexpected.  Will not interpret this element.")
-                    else:
-                        brs = ByteRuns()
-                        brs.populate_from_Element(ce)
-                        brs.facet = ce.attrib["facet"]
-                        setattr(self, FileObject._br_facet_to_property[brs.facet], brs)
-                else:
-                    self.byte_runs = ByteRuns()
-                    self.byte_runs.populate_from_Element(ce)
-            elif ctn == "hashdigest":
-                if ce.attrib["type"].lower() == "md5":
-                    self.md5 = ce.text
-                elif ce.attrib["type"].lower() == "sha1":
-                    self.sha1 = ce.text
-                elif ce.attrib["type"].lower() == "sha256":
-                    self.sha256 = ce.text
-                elif ce.attrib["type"].lower() == "sha512":
-                    self.sha512 = ce.text
-            elif ctn == "original_fileobject":
-                self.original_fileobject = FileObject()
-                self.original_fileobject.populate_from_Element(ce)
-            elif ctn == "parent_object":
-                self.parent_object = FileObject()
-                self.parent_object.populate_from_Element(ce)
-            elif ctn in ["atime", "bkup_time", "crtime", "ctime", "dtime", "mtime"]:
-                setattr(self, ctn, TimestampObject())
-                getattr(self, ctn).populate_from_Element(ce)
-            elif ctn in FileObject._all_properties:
-                setattr(self, ctn, ce.text)
-            elif cns not in [dfxml.XMLNS_DFXML, ""]:
-                #Put all non-DFXML-namespace elements into the externals list.
-                self.externals.append(ce)
-            else:
-                if (cns, ctn) not in _warned_elements:
-                    _warned_elements.add((cns, ctn))
-                    _logger.warning("Uncertain what to do with this element: %r" % ce)
-
-    def populate_from_stat(self, s):
-        """Populates FileObject fields from a stat() call."""
-        import os
-        _typecheck(s, os.stat_result)
-
-        self.mode = s.st_mode
-        self.nlink = s.st_nlink
-        self.uid = s.st_uid
-        self.gid = s.st_gid
-        self.filesize = s.st_size
-        #s.st_dev is ignored for now.
-        if platform.system() == "Windows":
-            # On Windows, Python 2 reports 0L.  Treat this as absent information.
-            # On Windows, Python 3 reports the "File ID" ( see "nFileIndexLow" remark at: https://msdn.microsoft.com/en-us/library/aa363788 ).  Record this as the inode number for now.  NOTE: in the future this may become a Windows-namespaced property "fileindex"; it may be prudent to later file a follow-on to Python Issue 32878 ( https://bugs.python.org/issue32878 ).
-            if sys.version_info[0] >= 3:
-                self.inode = s.st_ino
-        else:
-            self.inode = s.st_ino
-
-        if "st_mtime" in dir(s):
-            self.mtime = s.st_mtime
-
-        if "st_atime" in dir(s):
-            self.atime = s.st_atime
-
-        if "st_ctime" in dir(s):
-            self.ctime = s.st_ctime
-
-        if "st_birthtime" in dir(s):
-            self.crtime = s.st_birthtime
-
-    def to_Element(self):
-        """Creates an ElementTree Element with elements in DFXML schema order."""
-        outel = ET.Element("fileobject")
-
-        annos_whittle_set = copy.deepcopy(self.annos)
-        diffs_whittle_set = copy.deepcopy(self.diffs)
-
-        for annodiff in FileObject._diff_attr_names:
-            if annodiff in annos_whittle_set:
-                outel.attrib[FileObject._diff_attr_names[annodiff]] = "1"
-                annos_whittle_set.remove(annodiff)
-        if len(annos_whittle_set) > 0:
-            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
-
-        def _anno_change(el):
-            if el.tag in self.diffs:
-                el.attrib["delta:changed_property"] = "1"
-                diffs_whittle_set.remove(el.tag)
-
-        def _anno_hash(el):
-            if el.attrib["type"] in self.diffs:
-                el.attrib["delta:changed_property"] = "1"
-                diffs_whittle_set.remove(el.attrib["type"])
-
-        def _anno_byte_runs(el):
-            if "facet" in el.attrib:
-                prop = FileObject._br_facet_to_property[el.attrib["facet"]]
-            else:
-                prop = "data_brs"
-            if prop in self.diffs:
-                el.attrib["delta:changed_property"] = "1"
-                #_logger.debug("diffs_whittle_set = %r." % diffs_whittle_set)
-                diffs_whittle_set.remove(prop)
-
-        #Recall that Element text must be a string
-        def _append_str(name, value):
-            """Note that empty elements should be created if the element was removed."""
-            if not value is None or name in diffs_whittle_set:
-                tmpel = ET.Element(name)
-                if not value is None:
-                    tmpel.text = str(value)
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        def _append_time(name, value):
-            """Note that empty elements should be created if the element was removed."""
-            if not value is None or name in diffs_whittle_set:
-                if not value is None and value.time:
-                    tmpel = value.to_Element()
-                else:
-                    tmpel = ET.Element(name)
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        def _append_bool(name, value):
-            """Note that empty elements should be created if the element was removed."""
-            if not value is None or name in diffs_whittle_set:
-                tmpel = ET.Element(name)
-                if not value is None:
-                    tmpel.text = str(1 if value else 0)
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        _using_facets = False
-        def _append_byte_runs(name, value):
-            """The complicated part here is setting the "data" facet on the byte runs, because we assume that no facet definitions means that for this file, there's only the one byte_runs list for data."""
-            #_logger.debug("_append_byte_runs(%r, %r)" % (name, value))
-            if value or name in diffs_whittle_set:
-                if value:
-                    tmpel = value.to_Element()
-                    if "facet" in tmpel.attrib:
-                        _using_facets = True
-                else:
-                    tmpel = ET.Element("byte_runs")
-                    propname_to_facet = {
-                      "data_brs": "data",
-                      "inode_brs": "inode",
-                      "name_brs": "name"
-                    }
-                    if name in propname_to_facet:
-                        _using_facets = True
-                        tmpel.attrib["facet"] = propname_to_facet[name]
-                    elif _using_facets:
-                        tmpel.attrib["facet"] = propname_to_facet["data_brs"]
-                _anno_byte_runs(tmpel)
-                outel.append(tmpel)
-
-        def _append_externals():
-            for e in self.externals:
-                outel.append(e)
-
-        def _append_object(name, value, namespace_prefix=None):
-            """name must be the name of a property that has a to_Element() method.  namespace_prefix will be prepended as-is to the element tag."""
-            obj = value
-            if obj or name in diffs_whittle_set:
-                if obj:
-                    tmpel = obj.to_Element()
-                else:
-                    tmpel = ET.Element(name)
-                #Set the tag name here for properties like parent_object, a FileObject without being wholly a FileObject.
-                if namespace_prefix:
-                    tmpel.tag = namespace_prefix + name
-                else:
-                    tmpel.tag = name
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        def _append_hash(name, value):
-            if not value is None or name in diffs_whittle_set:
-                tmpel = ET.Element("hashdigest")
-                tmpel.attrib["type"] = name
-                if not value is None:
-                    tmpel.text = value
-                _anno_hash(tmpel)
-                outel.append(tmpel)
-
-        #The parent object is a one-off.  Duplicating the whole parent is wasteful, so create a shadow object that just outputs the important bits.
-        if not self.parent_object is None:
-            parent_object_shadow = FileObject()
-            parent_object_shadow.inode = self.parent_object.inode
-            _append_object("parent_object", parent_object_shadow)
-
-        _append_str("filename", self.filename)
-        _append_str("error", self.error)
-        _append_str("partition", self.partition)
-        _append_str("id", self.id)
-        _append_str("name_type", self.name_type)
-        _append_str("filesize", self.filesize)
-        #TODO Define a better flag for if we're going to output <alloc> elements.
-        if self.alloc_name is None and self.alloc_inode is None:
-            _append_bool("alloc", self.alloc)
-        else:
-            _append_bool("alloc_inode", self.alloc_inode)
-            _append_bool("alloc_name", self.alloc_name)
-        _append_bool("used", self.used)
-        _append_bool("orphan", self.orphan)
-        _append_bool("compressed", self.compressed)
-        _append_str("inode", self.inode)
-        _append_str("meta_type", self.meta_type)
-        _append_str("mode", self.mode)
-        _append_str("nlink", self.nlink)
-        _append_str("uid", self.uid)
-        _append_str("gid", self.gid)
-        _append_time("mtime", self.mtime)
-        _append_time("ctime", self.ctime)
-        _append_time("atime", self.atime)
-        _append_time("crtime", self.crtime)
-        _append_str("seq", self.seq)
-        _append_time("dtime", self.dtime)
-        _append_time("bkup_time", self.bkup_time)
-        _append_str("link_target", self.link_target)
-        _append_str("libmagic", self.libmagic)
-        _append_externals()
-        _append_byte_runs("inode_brs", self.inode_brs)
-        _append_byte_runs("name_brs", self.name_brs)
-        _append_byte_runs("data_brs", self.data_brs)
-        _append_hash("md5", self.md5)
-        _append_hash("sha1", self.sha1)
-        _append_hash("sha256", self.sha256)
-        _append_hash("sha512", self.sha512)
-        _append_object("original_fileobject", self.original_fileobject, "delta:")
-
-        if len(diffs_whittle_set) > 0:
-            _logger.warning("Did not annotate all of the differing properties of this file.  Remaining properties:  %r." % diffs_whittle_set)
-
-        return outel
-
-    def to_dfxml(self):
-        return _ET_tostring(self.to_Element())
-
-    @property
-    def alloc(self):
-        """Note that setting .alloc will affect the value of .unalloc, and vice versa.  The last one to set wins."""
-        global _nagged_alloc
-        if not _nagged_alloc:
-            #alloc isn't deprecated yet.
-            #_logger.warning("The FileObject.alloc property is deprecated.  Use .alloc_inode and/or .alloc_name instead.  .alloc is proxied as True if alloc_inode and alloc_name are both True.")
-            _nagged_alloc = True
-        if self.alloc_inode and self.alloc_name:
-            return True
-        else:
-            return self._alloc
-
-    @alloc.setter
-    def alloc(self, val):
-        self._alloc = _boolcast(val)
-        if not self._alloc is None:
-            self._unalloc = not self._alloc
-
-    @property
-    def alloc_inode(self):
-        return self._alloc_inode
-
-    @alloc_inode.setter
-    def alloc_inode(self, val):
-        self._alloc_inode = _boolcast(val)
-
-    @property
-    def alloc_name(self):
-        return self._alloc_name
-
-    @alloc_name.setter
-    def alloc_name(self, val):
-        self._alloc_name = _boolcast(val)
-
-    @property
-    def annos(self):
-        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
-        return self._annos
-
-    @annos.setter
-    def annos(self, val):
-        _typecheck(val, set)
-        self._annos = val
-
-    @property
-    def atime(self):
-        return self._atime
-
-    @atime.setter
-    def atime(self, val):
-        if val is None:
-            self._atime = None
-        elif isinstance(val, TimestampObject):
-            self._atime = val
-        else:
-            checked_val = TimestampObject(val, name="atime")
-            self._atime = checked_val
-
-    @property
-    def bkup_time(self):
-        return self._bkup_time
-
-    @bkup_time.setter
-    def bkup_time(self, val):
-        if val is None:
-            self._bkup_time = None
-        elif isinstance(val, TimestampObject):
-            self._bkup_time = val
-        else:
-            checked_val = TimestampObject(val, name="bkup_time")
-            self._bkup_time = checked_val
-
-    @property
-    def byte_runs(self):
-        """This property is now a synonym for the data byte runs (.data_brs)."""
-        return self.data_brs
-
-    @byte_runs.setter
-    def byte_runs(self, val):
-        self.data_brs = val
-
-    @property
-    def compressed(self):
-        return self._compressed
-
-    @compressed.setter
-    def compressed(self, val):
-        self._compressed = _boolcast(val)
-
-    @property
-    def ctime(self):
-        return self._ctime
-
-    @ctime.setter
-    def ctime(self, val):
-        if val is None:
-            self._ctime = None
-        elif isinstance(val, TimestampObject):
-            self._ctime = val
-        else:
-            checked_val = TimestampObject(val, name="ctime")
-            self._ctime = checked_val
-
-    @property
-    def crtime(self):
-        return self._crtime
-
-    @crtime.setter
-    def crtime(self, val):
-        if val is None:
-            self._crtime = None
-        elif isinstance(val, TimestampObject):
-            self._crtime = val
-        else:
-            checked_val = TimestampObject(val, name="crtime")
-            self._crtime = checked_val
-
-    @property
-    def data_brs(self):
-        """The byte runs that store the file's content."""
-        return self._data_brs
-
-    @data_brs.setter
-    def data_brs(self, val):
-        if not val is None:
-            _typecheck(val, ByteRuns)
-        self._data_brs = val
-
-    @property
-    def diffs(self):
-        """This property intentionally has no setter.  To populate, call compare_to_original() after assigning an original_fileobject."""
-        return self._diffs
-
-    @property
-    def dtime(self):
-        return self._dtime
-
-    @dtime.setter
-    def dtime(self, val):
-        if val is None:
-            self._dtime = None
-        elif isinstance(val, TimestampObject):
-            self._dtime = val
-        else:
-            checked_val = TimestampObject(val, name="dtime")
-            self._dtime = checked_val
-
-    @property
-    def error(self):
-        return self._error
-
-    @error.setter
-    def error(self, val):
-        self._error = _strcast(val)
-
-    @property
-    def filename(self):
-        return self._filename
-
-    @filename.setter
-    def filename(self, val):
-        self._filename = _strcast(val)
-    @property
-    def externals(self):
-        """
-        This property exposes XML elements of other namespaces.  Since these elements can be of arbitrary complexity, this list is solely comprised ofxml.etree.ElementTree.Element objects.  The tags must be a fully-qualified namespace (of the pattern {URI}localname).  If generating the Elements with a script instead of de-serializing from XML, you should issue an ElementTree register_namespace call with your namespace abbreviation prefix.
-        NOTE:  Diffs are currently NOT computed for external elements.
-        NOTE:  This property should be considered unstable, as the interface is in an early design phase.  Please notify the maintainers of this library (see the Git history for the Objects.py file) if you are using this interface and wish to be notified of updates."""
-        return self._externals
-
-    @externals.setter
-    def externals(self, val):
-        _typecheck(val, OtherNSElementList)
-        self._externals = val
-
-    @property
-    def filesize(self):
-        return self._filesize
-
-    @filesize.setter
-    def filesize(self, val):
-        self._filesize = _intcast(val)
-
-    @property
-    def gid(self):
-        return self._gid
-
-    @gid.setter
-    def gid(self, val):
-        self._gid = _strcast(val)
-
-    @property
-    def id(self):
-        return self._id
-
-    @id.setter
-    def id(self, val):
-        self._id = _intcast(val)
-
-    @property
-    def inode(self):
-        return self._inode
-
-    @inode.setter
-    def inode(self, val):
-        self._inode = _intcast(val)
-
-    @property
-    def libmagic(self):
-        return self._libmagic
-
-    @libmagic.setter
-    def libmagic(self, val):
-        self._libmagic = _strcast(val)
-
-    @property
-    def inode_brs(self):
-        """The byte run(s) that represents the file's metadata object (the inode or the MFT entry).  In file systems that do not distinguish between inode and directory entry, e.g. FAT, .inode_brs should be equivalent to .name_brs, if both fields are present."""
-        return self._inode_brs
-
-    @inode_brs.setter
-    def inode_brs(self, val):
-        if not val is None:
-            _typecheck(val, ByteRuns)
-        self._inode_brs = val
-
-    @property
-    def md5(self):
-        return self._md5
-
-    @md5.setter
-    def md5(self, val):
-        self._md5 = _strcast(val)
-
-    @property
-    def meta_type(self):
-        return self._meta_type
-
-    @meta_type.setter
-    def meta_type(self, val):
-        self._meta_type = _intcast(val)
-
-    @property
-    def mode(self):
-        """The security mode is represented in the FileObject as a base-10 integer.  It is also serialized as a decimal integer."""
-        return self._mode
-
-    @mode.setter
-    def mode(self, val):
-        self._mode = _intcast(val)
-
-    @property
-    def mtime(self):
-        return self._mtime
-
-    @mtime.setter
-    def mtime(self, val):
-        if val is None:
-            self._mtime = None
-        elif isinstance(val, TimestampObject):
-            self._mtime = val
-        else:
-            checked_val = TimestampObject(val, name="mtime")
-            self._mtime = checked_val
-
-    @property
-    def name_brs(self):
-        """The byte run(s) that represents the file's name object (the directory entry).  In file systems that do not distinguish between inode and directory entry, e.g. FAT, .inode_brs should be equivalent to .name_brs, if both fields are present."""
-        return self._name_brs
-
-    @name_brs.setter
-    def name_brs(self, val):
-        if not val is None:
-            _typecheck(val, ByteRuns)
-        self._name_brs = val
-
-    @property
-    def name_type(self):
-        return self._name_type
-
-    @name_type.setter
-    def name_type(self, val):
-        if val is None:
-            self._name_type = val
-        else:
-            cast_val = _strcast(val)
-            if cast_val not in ["-", "V", "b", "c", "d", "h", "l", "p", "r", "s", "v", "w"]:
-                raise ValueError("Unexpected name_type received: %r (casted to %r)." % (val, cast_val))
-            self._name_type = cast_val
-
-    @property
-    def nlink(self):
-        return self._nlink
-
-    @nlink.setter
-    def nlink(self, val):
-        self._nlink = _intcast(val)
-
-    @property
-    def orphan(self):
-        return self._orphan
-
-    @orphan.setter
-    def orphan(self, val):
-        self._orphan = _boolcast(val)
-
-    @property
-    def original_fileobject(self):
-        return self._original_fileobject
-
-    @original_fileobject.setter
-    def original_fileobject(self, val):
-        if not val is None:
-            _typecheck(val, FileObject)
-        self._original_fileobject = val
-
-    @property
-    def partition(self):
-        return self._partition
-
-    @partition.setter
-    def partition(self, val):
-        self._partition = _intcast(val)
-
-    @property
-    def parent_object(self):
-        """This object is an extremely sparse FileObject, containing just identifying information.  Alternately, it can be an entire object reference to the parent Object, though uniqueness should be checked."""
-        return self._parent_object
-
-    @parent_object.setter
-    def parent_object(self, val):
-        if not val is None:
-            _typecheck(val, FileObject)
-        self._parent_object = val
-
-    @property
-    def seq(self):
-        return self._seq
-
-    @seq.setter
-    def seq(self, val):
-        self._seq = _intcast(val)
-
-    @property
-    def sha1(self):
-        return self._sha1
-
-    @sha1.setter
-    def sha1(self, val):
-        self._sha1 = _strcast(val)
-
-    @property
-    def sha256(self):
-        return self._sha256
-
-    @sha256.setter
-    def sha256(self, val):
-        self._sha256 = _strcast(val)
-    
-    @property
-    def sha512(self):
-        return self._sha512
-        
-    @sha512.setter
-    def sha512(self, val):
-        self._sha512 = _strcast(val)
-
-    @property
-    def uid(self):
-        return self._uid
-
-    @uid.setter
-    def uid(self, val):
-        self._uid = _strcast(val)
-
-    @property
-    def unalloc(self):
-        """Note that setting .unalloc will affect the value of .alloc, and vice versa.  The last one to set wins."""
-        return self._unalloc
-
-    @unalloc.setter
-    def unalloc(self, val):
-        self._unalloc = _boolcast(val)
-        if not self._unalloc is None:
-            self._alloc = not self._unalloc
-
-    @property
-    def unused(self):
-        return self._used
-
-    @unused.setter
-    def unused(self, val):
-        self._unused = _intcast(val)
-        if not self._unused is None:
-            self._used = not self._unused
-
-    @property
-    def used(self):
-        return self._used
-
-    @used.setter
-    def used(self, val):
-        self._used = _intcast(val)
-        if not self._used is None:
-            self._unused = not self._used
-
-    @property
-    def volume_object(self):
-        """Reference to the containing volume object.  Not meant to be propagated with __repr__ or to_Element()."""
-        return self._volume_object
-
-    @volume_object.setter
-    def volume_object(self, val):
-        if not val is None:
-            _typecheck(val, VolumeObject)
-        self._volume_object = val
-
-class OtherNSElementList(list):
-    #Note that super() must be called with arguments to work in Python 2.
-
-    @classmethod
-    def _check_qname(cls, tagname):
-        (ns, ln) = _qsplit(tagname)
-        if ns == dfxml.XMLNS_DFXML:
-            raise ValueError("'External' elements must be a non-DFXML namespace.")
-        #Register qname for later output
-        #TODO Devise a module-level interface for namespace abreviations.
-
-    def __repr__(self):
-        #Unwrap the string representation of this class's type name (necessary because we don't necessarily know if it'll be Objects.Other... or just Other...).
-        _typestr = str(type(self))[ len("<class '") : -len("'>") ]
-        return _typestr + "(" + super(OtherNSElementList, self).__repr__() + ")"
-
-    def __setitem__(self, idx, value):
-        _typecheck(value, ET.Element)
-        OtherNSElementList._check_qname(value.tag)
-        super(OtherNSElementList, self).__setitem__(idx, value)
-
-    def append(self, value):
-        _typecheck(value, ET.Element)
-        OtherNSElementList._check_qname(value.tag)
-        super(OtherNSElementList, self).append(value)
-
-class CellObject(object):
-
-    _all_properties = set([
-      "alloc",
-      "annos",
-      "basename",
-      "byte_runs",
-      "cellpath",
-      "data",
-      "data_conversions",
-      "data_encoding",
-      "data_type",
-      "error",
-      "mtime",
-      "name_type",
-      "original_cellobject",
-      "parent_object",
-      "root"
-    ])
-
-    _diff_attr_names = {
-      "new":"delta:new_cell",
-      "deleted":"delta:deleted_cell",
-      "changed":"delta:changed_cell",
-      "modified":"delta:modified_cell",
-      "matched":"delta:matched"
-    }
-
-    #TODO There may be need in the future to compare the annotations as well.
-    _incomparable_properties = set([
-      "annos"
-    ])
-
-    def __init__(self, *args, **kwargs):
-        #These properties must be assigned first for sanity check dependencies
-        self.name_type = kwargs.get("name_type")
-
-        for prop in CellObject._all_properties:
-            if prop == "annos":
-                setattr(self, prop, kwargs.get(prop, set()))
-            else:
-                setattr(self, prop, kwargs.get(prop))
-
-        self._diffs = set()
-
-    def __eq__(self, other):
-        if other is None:
-            return False
-        _typecheck(other, CellObject)
-        for prop in CellObject._all_properties:
-            if prop in CellObject._incomparable_properties:
-                continue
-            if getattr(self, prop) != getattr(other, prop):
-                return False
-        return True
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __repr__(self):
-        parts = []
-
-        for prop in sorted(list(CellObject._all_properties)):
-            if not getattr(self, prop) is None:
-                parts.append("%s=%r" % (prop, getattr(self, prop)))
-
-        return "CellObject(" + ", ".join(parts) + ")"
-
-    def compare_to_original(self):
-        self._diffs = self.compare_to_other(self.original_cellobject, True)
-
-    def compare_to_other(self, other, ignore_original=False):
-        _typecheck(other, CellObject)
-
-        diffs = set()
-
-        for propname in CellObject._all_properties:
-            if propname in CellObject._incomparable_properties:
-                continue
-            if ignore_original and propname == "original_cellobject":
-                continue
-            oval = getattr(other, propname)
-            sval = getattr(self, propname)
-            if oval is None and sval is None:
-                continue
-            if oval != sval:
-                #_logger.debug("propname, oval, sval: %r, %r, %r" % (propname, oval, sval))
-                diffs.add(propname)
-
-        return diffs
-
-    def populate_from_Element(self, e):
-        """Populates this CellObject's properties from an ElementTree Element.  The Element need not be retained."""
-        global _warned_elements
-        _typecheck(e, (ET.Element, ET.ElementTree))
-
-        _read_differential_annotations(CellObject._diff_attr_names, e, self.annos)
-
-        #Split into namespace and tagname
-        (ns, tn) = _qsplit(e.tag)
-        assert tn in ["cellobject", "original_cellobject", "parent_object"]
-
-        if e.attrib.get("root"):
-            self.root = e.attrib["root"]
-
-        #Look through direct-child elements for other properties
-        for ce in e.findall("./*"):
-            (cns, ctn) = _qsplit(ce.tag)
-            if ctn == "alloc":
-                self.alloc = ce.text
-            elif ctn == "basename":
-                self.basename = ce.text
-            elif ctn == "byte_runs":
-                self.byte_runs = ByteRuns()
-                self.byte_runs.populate_from_Element(ce)
-            elif ctn == "cellpath":
-                self.cellpath = ce.text
-            elif ctn == "data":
-                self.data = ce.text
-                if ce.attrib.get("encoding"):
-                    self.data_encoding = ce.attrib["encoding"]
-            elif ctn == "data_conversions":
-                self.data_conversions = dict()
-                for cce in ce:
-                    if cce.tag == "int":
-                        self.data_conversions["int"] = int()
-                    elif cce.tag == "string":
-                        self.data_conversions["string"] = cce.text
-                    elif cce.tag == "string_list":
-                        self.data_conversions["string_list"] = []
-                        for ccce in cce:
-                            self.data_conversions["string_list"].append(ccce.text)
-            elif ctn == "data_type":
-                self.data_type = ce.text
-            elif ctn == "error":
-                self.error = ce.text
-            elif ctn == "mtime":
-                self.mtime = TimestampObject()
-                self.mtime.populate_from_Element(ce)
-            elif ctn == "name_type":
-                self.name_type = ce.text
-            elif ctn == "original_cellobject":
-                self.original_cellobject = CellObject()
-                self.original_cellobject.populate_from_Element(ce)
-            elif ctn == "parent_object":
-                self.parent_object = CellObject()
-                self.parent_object.populate_from_Element(ce)
-            else:
-                if (cns, ctn) not in _warned_elements:
-                    _warned_elements.add((cns, ctn))
-                    _logger.warning("Uncertain what to do with this element: %r" % ce)
-
-        self.sanity_check()
-
-    def sanity_check(self):
-        if self.name_type and self.name_type != "k":
-            if self.mtime:
-                _logger.info("Error occurred sanity-checking this CellObject: %r." % self)
-                raise ValueError("A Registry Key (node) is the only kind of CellObject that can have a timestamp.")
-            if self.root:
-                _logger.info("Error occurred sanity-checking this CellObject: %r." % self)
-                raise ValueError("A Registry Key (node) is the only kind of CellObject that can have the 'root' attribute.")
-
-    def to_Element(self):
-        self.sanity_check()
-
-        outel = ET.Element("cellobject")
-
-        annos_whittle_set = copy.deepcopy(self.annos)
-        diffs_whittle_set = copy.deepcopy(self.diffs)
-
-        for annodiff in CellObject._diff_attr_names:
-            if annodiff in annos_whittle_set:
-                outel.attrib[CellObject._diff_attr_names[annodiff]] = "1"
-                annos_whittle_set.remove(annodiff)
-        if len(annos_whittle_set) > 0:
-            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
-
-        def _anno_change(el):
-            if el.tag in self.diffs:
-                el.attrib["delta:changed_property"] = "1"
-                diffs_whittle_set.remove(el.tag)
-            #Do an additional check for data_encoding, which is serialized as an attribute.
-            if el.tag == "data" and "data_encoding" in self.diffs:
-                el.attrib["delta:changed_property"] = "1"
-                diffs_whittle_set.remove("data_encoding")
-
-        def _append_bool(name, value):
-            if not value is None or name in diffs_whittle_set:
-                tmpel = ET.Element(name)
-                if not value is None:
-                    tmpel.text = "1" if value else "0"
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        #Recall that Element text must be a string
-        def _append_str(name, value):
-            if not value is None or name in diffs_whittle_set:
-                tmpel = ET.Element(name)
-                if not value is None:
-                    tmpel.text = str(value)
-                _anno_change(tmpel)
-
-                if name == "data" and not self.data_encoding is None:
-                    tmpel.attrib["encoding"] = self.data_encoding
-
-                outel.append(tmpel)
-
-        def _append_object(name, value):
-            if not value is None or name in diffs_whittle_set:
-                if value is None:
-                    tmpel = ET.Element(name)
-                else:
-                    tmpel = value.to_Element()
-                _anno_change(tmpel)
-                outel.append(tmpel)
-
-        #TODO root should be an element too.  Revise schema.
-        if self.root:
-            outel.attrib["root"] = str(self.root)
-
-        _append_str("cellpath", self.cellpath)
-        _append_str("basename", self.basename)
-        _append_str("error", self.error)
-        _append_str("name_type", self.name_type)
-        _append_bool("alloc", self.alloc)
-        _append_object("mtime", self.mtime)
-        _append_str("data_type", self.data_type)
-        _append_str("data", self.data)
-
-        #The experimental conversions element needs its own code
-        if not self.data_conversions is None or "data_conversions" in diffs_whittle_set:
-            tmpel = ET.Element("data_conversions")
-            if not self.data_conversions is None:
-                if "int" in self.data_conversions:
-                    tmpcel = ET.Element("int")
-                    tmpcel.text = str(self.data_conversions["int"])
-                    tmpel.append(tmpcel)
-                if "string" in self.data_conversions:
-                    tmpcel = ET.Element("string")
-                    tmpcel.text = str(self.data_conversions["string"])
-                    tmpel.append(tmpcel)
-                if "string_list" in self.data_conversions:
-                    tmpcel = ET.Element("string_list")
-                    for s in self.data_conversions["string"]:
-                        tmpccel = ET.Element("string")
-                        tmpccel.text = s
-                        tmpcel.append(tmpccel)
-                    tmpel.append(tmpcel)
-
-            _anno_change(tmpel)
-            outel.append(tmpel)
-
-        _append_object("byte_runs", self.byte_runs)
-        _append_object("original_cellobject", self.original_cellobject)
-
-        if len(diffs_whittle_set) > 0:
-            _logger.warning("Did not annotate all of the differing properties of this file.  Remaining properties:  %r." % diffs_whittle_set)
-
-        return outel
-
-    def to_regxml(self):
-        return _ET_tostring(self.to_Element())
-
-    @property
-    def alloc(self):
-        return self._alloc
-
-    @alloc.setter
-    def alloc(self, val):
-        self._alloc = _boolcast(val)
-
-    @property
-    def annos(self):
-        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
-        return self._annos
-
-    @annos.setter
-    def annos(self, val):
-        _typecheck(val, set)
-        self._annos = val
-
-    @property
-    def basename(self):
-        return self._basename
-
-    @basename.setter
-    def basename(self, val):
-        if not val is None:
-            _typecheck(val, str)
-        self._basename = val
-
-    @property
-    def byte_runs(self):
-        return self._byte_runs
-
-    @byte_runs.setter
-    def byte_runs(self, val):
-        if not val is None:
-            _typecheck(val, ByteRuns)
-        self._byte_runs = val
-
-    @property
-    def cellpath(self):
-        return self._cellpath
-
-    @cellpath.setter
-    def cellpath(self, val):
-        if not val is None:
-            _typecheck(val, str)
-        self._cellpath = val
-
-    @property
-    def data(self):
-        """Expecting a base64-encoded string.  See conversions (according to the Hive parser's library) in data_conversions property."""
-        return self._data
-
-    @data.setter
-    def data(self, val):
-        if not val is None:
-            _typecheck(val, str)
-        self._data = val
-
-    @property
-    def data_conversions(self):
-        return self._data_conversions
-
-    @data_conversions.setter
-    def data_conversions(self, val):
-        if not val is None:
-            _typecheck(val, dict)
-        self._data_conversions = val
-
-    @property
-    def data_encoding(self):
-        """Expecting a string, typically 'base64'."""
-        return self._data_encoding
-
-    @data_encoding.setter
-    def data_encoding(self, val):
-        if not val is None:
-            _typecheck(val, str)
-        self._data_encoding = val
-
-    @property
-    def data_type(self):
-        """Expecting a string, e.g. "REG_MULTI_SZ", or an int, because value type is known to be overloaded as an integer storage field in some cells."""
-        return self._data_type
-
-    @data_type.setter
-    def data_type(self, val):
-        if not val in [
-          None,
-          "REG_NONE",
-          "REG_SZ",
-          "REG_EXPAND_SZ",
-          "REG_BINARY",
-          "REG_DWORD",
-          "REG_DWORD_BIG_ENDIAN",
-          "REG_LINK",
-          "REG_MULTI_SZ",
-          "REG_RESOURCE_LIST",
-          "REG_FULL_RESOURCE_DESCRIPTOR",
-          "REG_RESOURCE_REQUIREMENTS_LIST",
-          "REG_QWORD"
-        ]:
-            if not isinstance(val, int) or (isinstance(val, str) and val.isdigit()):
-                raise ValueError("Unexpected value data type received: %r, type %r." % (val, type(val)))
-        self._data_type = val
-
-    @property
-    def diffs(self):
-        return self._diffs
-
-    @diffs.setter
-    def diffs(self, value):
-        _typecheck(value, set)
-        self._diffs = value
-
-    @property
-    def error(self):
-        return self._error
-
-    @error.setter
-    def error(self, value):
-        if not value is None:
-            _typecheck(value, str)
-        self._error = value
-
-    @property
-    def hive_object(self):
-        """Reference to the containing hive object.  Not meant to be propagated with __repr__ or to_Element()."""
-        return self._hive_object
-
-    @hive_object.setter
-    def hive_object(self, val):
-        if not val is None:
-            _typecheck(val, HiveObject)
-        self._hive_object = val
-
-    @property
-    def mtime(self):
-        return self._mtime
-
-    @mtime.setter
-    def mtime(self, val):
-        if val is None:
-            self._mtime = None
-        elif isinstance(val, TimestampObject):
-            self._mtime = val
-        else:
-            self._mtime = TimestampObject(val, name="mtime")
-            self.sanity_check()
-
-    @property
-    def name_type(self):
-        return self._name_type
-
-    @name_type.setter
-    def name_type(self, val):
-        if not val is None:
-            assert val in ["k", "v"]
-        self._name_type = val
-
-    @property
-    def original_cellobject(self):
-        return self._original_cellobject
-
-    @original_cellobject.setter
-    def original_cellobject(self, val):
-        if not val is None:
-            _typecheck(val, CellObject)
-        self._original_cellobject = val
-
-    @property
-    def parent_object(self):
-        """This object is an extremely sparse CellObject, containing just identifying information.  Alternately, it can be an entire object reference to the parent Object, though uniqueness should be checked."""
-        return self._parent_object
-
-    @parent_object.setter
-    def parent_object(self, val):
-        if not val is None:
-            _typecheck(val, CellObject)
-        self._parent_object = val
-
-    @property
-    def root(self):
-        return self._root
-
-    @root.setter
-    def root(self, val):
-        self._root = _boolcast(val)
-
-
-def iterparse(filename, events=("start","end"), **kwargs):
-    """
-    Generator.  Yields a stream of populated DFXMLObjects, VolumeObjects and FileObjects, paired with an event type ("start" or "end").  The DFXMLObject and VolumeObjects do NOT have their child lists populated with this method - that is left to the calling program.
-
-    The event type interface is meant to match the interface of ElementTree's iterparse; this is simply for familiarity's sake.  DFXMLObjects and VolumeObjects are yielded with "start" when the stream of VolumeObject or FileObjects begins - that is, they are yielded after being fully constructed up to the potentially-lengthy child object stream.  FileObjects are yielded only with "end".
-
-    @param filename: A string
-    @param events: Events.  Optional.  A tuple of strings, containing "start" and/or "end".
-    @param dfxmlobject: A DFXMLObject document.  Optional.  A DFXMLObject is created and yielded in the object stream if this argument is not supplied.
-    @param fiwalk: Optional.  Path to a particular fiwalk build you want to run.
-    """
-
-    #The DFXML stream file handle.
-    fh = None
-    subp = None
-    fiwalk_path = kwargs.get("fiwalk", "fiwalk")
-    subp_command = [fiwalk_path, "-x", filename]
-    if filename.endswith("xml"):
-        fh = open(filename, "rb")
-    else:
-        subp = subprocess.Popen(subp_command, stdout=subprocess.PIPE)
-        fh = subp.stdout
-
-    _events = set()
-    for e in events:
-        if not e in ("start","end"):
-            raise ValueError("Unexpected event type: %r.  Expecting 'start', 'end'." % e)
-        _events.add(e)
-
-    dobj = kwargs.get("dfxmlobject", DFXMLObject())
-
-    #The only way to efficiently populate VolumeObjects is to populate the object when the stream has hit its first FileObject.
-    vobj = None
-
-    #It doesn't seem ElementTree allows fetching parents of Elements that are incomplete (just hit the "start" event).  So, build a volume Element when we've hit "<volume ... >", glomming all elements until the first fileobject is hit.
-    #Likewise with the Element for the DFXMLObject.
-    dfxml_proxy = None
-    volume_proxy = None
-
-    #State machine, used to track when the first fileobject of a volume is encountered.
-    READING_START = 0
-    READING_PRESTREAM = 1 #DFXML metadata, pre-Object stream
-    READING_VOLUMES = 2
-    READING_FILES = 3
-    READING_POSTSTREAM = 4 #DFXML metadata, post-Object stream (typically the <rusage> element)
-    _state = READING_START
-
-    for (ETevent, elem) in ET.iterparse(fh, events=("start-ns", "start", "end")):
-        #View the object event stream in debug mode
-        #_logger.debug("(event, elem) = (%r, %r)" % (ETevent, elem))
-        #if ETevent in ("start", "end"):
-        #    _logger.debug("_ET_tostring(elem) = %r" % _ET_tostring(elem))
-
-        #Track namespaces
-        if ETevent == "start-ns":
-            dobj.add_namespace(*elem)
-            ET.register_namespace(*elem)
-            continue
-
-        #Split tag name into namespace and local name
-        (ns, ln) = _qsplit(elem.tag)
-
-        if ETevent == "start":
-            if ln == "dfxml":
-                if _state != READING_START:
-                    raise ValueError("Encountered a <dfxml> element, but the parser isn't in its start state.  Recursive <dfxml> declarations aren't supported at this time.")
-                dfxml_proxy = ET.Element(elem.tag)
-                for k in elem.attrib:
-                    #Note that xmlns declarations don't appear in elem.attrib.
-                    dfxml_proxy.attrib[k] = elem.attrib[k]
-                _state = READING_PRESTREAM
-            elif ln == "volume":
-                if _state == READING_PRESTREAM:
-                    #Cut; yield DFXMLObject now.
-                    dobj.populate_from_Element(dfxml_proxy)
-                    if "start" in _events:
-                        yield ("start", dobj)
-                #Start populating a new Volume proxy.
-                volume_proxy = ET.Element(elem.tag)
-                for k in elem.attrib:
-                    volume_proxy.attrib[k] = elem.attrib[k]
-                _state = READING_VOLUMES
-            elif ln == "fileobject":
-                if _state == READING_PRESTREAM:
-                    #Cut; yield DFXMLObject now.
-                    dobj.populate_from_Element(dfxml_proxy)
-                    if "start" in _events:
-                        yield ("start", dobj)
-                elif _state == READING_VOLUMES:
-                    #_logger.debug("Encountered a fileobject while reading volume properties.  Yielding volume now.")
-                    #Cut; yield VolumeObject now.
-                    if volume_proxy is not None:
-                        vobj = VolumeObject()
-                        vobj.populate_from_Element(volume_proxy)
-                        if "start" in _events:
-                            yield ("start", vobj)
-                        #Reset
-                        volume_proxy.clear()
-                        volume_proxy = None
-                _state = READING_FILES
-        elif ETevent == "end":
-            if ln == "fileobject":
-                if _state in (READING_PRESTREAM, READING_POSTSTREAM):
-                    #This particular branch can be reached if there are trailing fileobject elements after the volume element.  This would happen if a tool needed to represent files (likely reassembled fragments) found outside all the partitions.
-                    #More frequently, we hit this point when there are no volume groupings.
-                    vobj = None
-                fi = FileObject()
-                fi.populate_from_Element(elem)
-                fi.volume_object = vobj
-                #_logger.debug("fi = %r" % fi)
-                if "end" in _events:
-                    yield ("end", fi)
-                #Reset
-                elem.clear()
-            elif ln == "dfxml":
-                if "end" in _events:
-                    #_logger.debug("end, dfxml, _state=%r" % _state)
-                    if _state == READING_PRESTREAM:
-                        #This DFXML document contains no volumes or files, but may contain other metadata.  Populate (which would normally be done before starting a child Object stream) and yield.
-                        dobj.populate_from_Element(dfxml_proxy)
-                        yield ("end", dobj)
-            elif ln == "volume":
-                if _state == READING_VOLUMES:
-                    #Create and yield VolumeObject now (because there were no file objects to trigger it in the "start" ElementTree events branch above)
-                    vobj = VolumeObject()
-                    vobj.populate_from_Element(volume_proxy)
-                    if "start" in _events:
-                        yield ("start", vobj)
-                if "end" in _events:
-                    yield ("end", vobj)
-                _state = READING_POSTSTREAM
-            elif _state == READING_VOLUMES:
-                #This is a volume property; glom onto the proxy.
-                if volume_proxy is not None:
-                    volume_proxy.append(elem)
-            elif _state == READING_PRESTREAM:
-                if ln in ["metadata", "creator", "source"] or ns != dfxml.XMLNS_DFXML:
-                    #This is a direct child of the DFXML document property; glom onto the proxy.
-                    if dfxml_proxy is not None:
-                        dfxml_proxy.append(elem)
-
-    #If we called Fiwalk, double-check that it exited successfully.
-    if not subp is None:
-        _logger.debug("Calling wait() to let the Fiwalk subprocess terminate...") #Just reading from subp.stdout doesn't let the process terminate; it only finishes working.
-        subp.wait()
-        if subp.returncode != 0:
-            e = subprocess.CalledProcessError("There was an error running Fiwalk.")
-            e.returncode = subp.returncode
-            e.cmd = subp_command
-            raise e
-        _logger.debug("...Done.")
-
-def parse(filename):
-    """Returns a DFXMLObject populated from the contents of the (string) filename argument."""
-    retval = None
-    appender = None
-    for (event, obj) in iterparse(filename):
-        if event == "start":
-            if isinstance(obj, DFXMLObject):
-                retval = obj
-                appender = obj
-            elif isinstance(obj, VolumeObject):
-                retval.append(obj)
-                appender = obj
-        elif event == "end":
-            if isinstance(obj, DFXMLObject):
-                if retval is None:
-                    retval = obj
-                appender = obj
-            if isinstance(obj, VolumeObject):
-                appender = retval
-            elif isinstance(obj, FileObject):
-                appender.append(obj)
-    return retval
-
-if __name__ == "__main__":
-    import argparse
-    parser = argparse.ArgumentParser()
-
-    logging.basicConfig(level=logging.DEBUG)
-    #Run unit tests
-
-    assert _intcast(-1) == -1
-    assert _intcast("-1") == -1
-    assert _qsplit("{http://www.w3.org/2001/XMLSchema}all") == ("http://www.w3.org/2001/XMLSchema","all")
-    assert _qsplit("http://www.w3.org/2001/XMLSchema}all") == (None, "http://www.w3.org/2001/XMLSchema}all")
-
-
-    fi = FileObject()
-
-    #Check property setting
-    fi.mtime = "1999-12-31T23:59:59Z"
-    _logger.debug("fi = %r" % fi)
-
-    #Check bad property setting
-    failed = None
-    try:
-        fi.mtime = "Not a timestamp"
-        failed = False
-    except:
-        failed = True
-    _logger.debug("fi = %r" % fi)
-    _logger.debug("failed = %r" % failed)
-    assert failed
-
-    t0 = TimestampObject(prec="100ns", name="mtime")
-    _logger.debug("t0 = %r" % t0)
-    assert t0.prec[0] == 100
-    assert t0.prec[1] == "ns"
-    t1 = TimestampObject("2009-01-23T01:23:45Z", prec="2", name="atime")
-    _logger.debug("t1 = %r" % t1)
-    assert t1.prec[0] == 2
-    assert t1.prec[1] == "s"
-
-    print("Unit tests passed.")
+
+# This software was developed at the National Institute of Standards
+# and Technology in whole or in part by employees of the Federal
+# Government in the course of their official duties. Pursuant to
+# title 17 Section 105 of the United States Code portions of this
+# software authored by NIST employees are not subject to copyright
+# protection and are in the public domain. For portions not authored
+# by NIST employees, NIST has been granted unlimited rights. NIST
+# assumes no responsibility whatsoever for its use by other parties,
+# and makes no guarantees, expressed or implied, about its quality,
+# reliability, or any other characteristic.
+#
+# We would appreciate acknowledgement if the software is used.
+
+"""
+This file re-creates the major DFXML classes with an emphasis on type safety, serializability, and de-serializability.
+
+With this module, reading disk images or DFXML files is done with the parse or iterparse functions.  Writing DFXML files can be done with the DFXMLObject.print_dfxml function.
+"""
+
+__version__ = "0.7.2"
+
+#Remaining roadmap to 1.0.0:
+# * Documentation.
+# * User testing.
+# * Compatibility with the DFXML schema, version >1.1.1.
+
+import logging
+import re
+import copy
+import xml.etree.ElementTree as ET
+import subprocess
+import dfxml
+import os
+import sys
+import struct
+import platform
+
+_logger = logging.getLogger(os.path.basename(__file__))
+
+#Contains: (namespace, local name) qualified XML element name pairs
+_warned_elements = set([])
+_warned_byterun_attribs = set([])
+
+#Contains: Unexpected 'facet' values on byte_runs elements.
+_warned_byterun_facets = set([])
+
+#Issue some log statements only once per program invocation.
+_nagged_alloc = False
+_warned_byterun_badtypecomp = False
+_nagged_volume_error_impldrift = False
+_nagged_volume_error_standin = False
+
+XMLNS_REGXML = "http://www.forensicswiki.org/wiki/RegXML"
+
+def _ET_tostring(e):
+    """Between Python v2 and v3, there are some differences in the ElementTree library's tostring() behavior.  One, the method balks at the "unicode" encoding in v2.  Two, in 2, the XML prototypes output with every invocation.  This method serves as a wrapper to deal with those issues, plus another issue where ET.tostring prints repeated xmlns declarations (observed on reading and writing a DFXML file twice in the same process).  The repeated prints appear to be from a lack of inspection of existing namespace declarations in the attributes dictionary."""
+    retval = None
+    if sys.version_info[0] < 3:
+        tmp = ET.tostring(e, encoding="UTF-8")
+        if tmp[0:2] == "<?":
+            #Trim away first line; it's an XML prototype.  This only appears in Python 2's ElementTree output.
+            retval = tmp[ tmp.find("?>\n")+3 : ]
+        else:
+            retval = tmp
+    else:
+        retval = ET.tostring(e, encoding="unicode")
+    container_end = retval.index(">")
+    for (uri, prefix) in list(ET._namespace_map.items()):
+        if prefix == "":
+            xmlns_attr_name = "xmlns"
+        else:
+            xmlns_attr_name = "xmlns:" + prefix
+        xmlns_attr_string = '%s="%s"' % (xmlns_attr_name, uri)
+        xmlns_attr_tally = retval.count(xmlns_attr_string, 0, container_end)
+        if xmlns_attr_tally > 1:
+            _logger.warning("ET.tostring() printed a repeated xmlns declaration: %r.  Trimming %d repetition(s)." % (xmlns_attr_string, xmlns_attr_tally-1))
+            container_string = retval[ : container_end+1 ]
+            retval = container_string.replace(xmlns_attr_string, "", xmlns_attr_tally-1) + retval[ container_end+1 : ]
+    return retval
+
+def _boolcast(val):
+    """Takes Boolean values, and 0 or 1 in string or integer form, and casts them all to Boolean.  Preserves nulls.  Balks at everything else."""
+    if val is None:
+        return None
+    if val in [True, False]:
+        return val
+
+    _val = val
+    if val in ["0", "1"]:
+        _val = int(val)
+    if _val in [0, 1]:
+        return _val == 1
+
+    _logger.debug("val = " + repr(val))
+    raise ValueError("Received a not-straightforwardly-Boolean value.  Expected some form of 0, 1, True, or False.")
+
+def _bytecast(val):
+    """Casts a value as a byte string.  If a character string, assumes a UTF-8 encoding."""
+    if val is None:
+        return None
+    if isinstance(val, bytes):
+        return val
+    return _strcast(val).encode("utf-8")
+
+def _intcast(val):
+    """Casts input integer or string to integer.  Preserves nulls.  Balks at everything else."""
+    if val is None:
+        return None
+    if sys.version_info[0] < 3:
+       if isinstance(val, long):
+           return val
+    if isinstance(val, int):
+        return val
+
+    if isinstance(val, str):
+        if val[0] == "-":
+            if val[1:].isdigit():
+                return int(val)
+        else:
+            if val.isdigit():
+                return int(val)
+
+    _logger.debug("val = " + repr(val))
+    raise ValueError("Received a non-int-castable value.  Expected an integer or an integer as a string.")
+
+def _read_differential_annotations(annodict, element, annoset):
+    """
+    Uses the shorthand-to-attribute mappings of annodict to translate attributes of element into annoset.
+    """
+    #_logger.debug("annoset, before: %r." % annoset)
+    #Start with inverting the dictionary
+    _d = { annodict[k].replace("delta:",""):k for k in annodict }
+    #_logger.debug("Inverted dictionary: _d = %r" % _d)
+    for attr in element.attrib:
+        #_logger.debug("Looking for differential annotations: %r" % element.attrib)
+        (ns, an) = _qsplit(attr)
+        if an in _d and ns == dfxml.XMLNS_DELTA:
+            #_logger.debug("Found; adding %r." % _d[an])
+            annoset.add(_d[an])
+    #_logger.debug("annoset, after: %r." % annoset)
+
+def _qsplit(tagname):
+    """Requires string input.  Returns namespace and local tag name as a pair.  I could've sworn this was a basic implementation gimme, but ET.QName ain't it."""
+    _typecheck(tagname, str)
+    if tagname[0] == "{":
+        i = tagname.rfind("}")
+        return ( tagname[1:i], tagname[i+1:] )
+    else:
+        return (None, tagname)
+
+def _strcast(val):
+    if val is None:
+        return None
+    return str(val)
+
+def _typecheck(obj, classinfo):
+    if not isinstance(obj, classinfo):
+        _logger.info("obj = " + repr(obj))
+        if isinstance(classinfo, tuple):
+            raise TypeError("Expecting object to be one of the types %r." % (classinfo,))
+        else:
+            raise TypeError("Expecting object to be of type %r." % classinfo)
+
+class DFXMLObject(object):
+    def __init__(self, *args, **kwargs):
+        self.command_line = kwargs.get("command_line")
+        self.program = kwargs.get("program")
+        self.program_version = kwargs.get("program_version")
+        self.version = kwargs.get("version")
+        self.sources = kwargs.get("sources", [])
+        self.dc = kwargs.get("dc", dict())
+        self.externals = kwargs.get("externals", OtherNSElementList())
+        self.diff_file_ignores = kwargs.get("diff_file_ignores", set())
+
+        self._namespaces = dict()
+        self._volumes = []
+        self._files = []
+
+        self._build_libraries = []
+        self._creator_libraries = []
+
+        input_volumes = kwargs.get("volumes") or []
+        input_files = kwargs.get("files") or []
+        for v in input_volumes:
+            self.append(v)
+        for f in input_files:
+            self.append(f)
+
+        #Add default namespaces
+        self.add_namespace("", dfxml.XMLNS_DFXML)
+        self.add_namespace("dc", dfxml.XMLNS_DC)
+
+    def __iter__(self):
+        """Yields all VolumeObjects, recursively their FileObjects, and the FileObjects directly attached to this DFXMLObject, in that order."""
+        for v in self._volumes:
+            yield v
+            for f in v:
+                yield f
+        for f in self._files:
+            yield f
+
+    def _add_library(self, target_list, *args, **kwargs):
+        #_logger.debug("_add_library:args = %r." % (args,))
+        _library = None
+        if len(args) == 1 and isinstance(args[0], LibraryObject):
+            _library = args[0]
+        elif len(args) > 1 and isinstance(args[0], str) and isinstance(args[1], str):
+            _library = LibraryObject(args[0], args[1])
+        else:
+            raise ValueError("Unexpected arguments format (expecting (string, string) or a LibraryObject): %r." % (args,))
+        #_logger.debug("_library = %r." % _library)
+        if not _library is None:
+            target_list.append(_library)
+
+    def add_build_library(self, *args, **kwargs):
+        self._add_library(self.build_libraries, *args, **kwargs)
+
+    def add_creator_library(self, *args, **kwargs):
+        self._add_library(self.creator_libraries, *args, **kwargs)
+
+    def add_namespace(self, prefix, url):
+        """In case of conflicting namespace definitions, first definition wins."""
+        #_logger.debug("self._namespaces.keys() = %r." % self._namespaces.keys())
+        if prefix not in self._namespaces.keys():
+            #_logger.debug("Registering namespace: %r, %r." % (prefix, url))
+            self._namespaces[prefix] = url
+            ET.register_namespace(prefix, url)
+            #_logger.debug("ET namespaces after registration: %r." % ET._namespace_map)
+
+    def append(self, value):
+        if isinstance(value, VolumeObject):
+            self._volumes.append(value)
+        elif isinstance(value, FileObject):
+            self._files.append(value)
+        else:
+            _logger.debug("value = %r" % value)
+            raise TypeError("Expecting a VolumeObject or a FileObject.  Got instead this type: %r." % type(value))
+
+    def iter_namespaces(self):
+        """Yields (prefix, url) pairs of each namespace registered in this DFXMLObject."""
+        for prefix in sorted(self._namespaces.keys()):
+            yield (prefix, self._namespaces[prefix])
+
+    def populate_from_Element(self, e):
+        if "version" in e.attrib:
+            self.version = e.attrib["version"]
+
+        for ce in e.findall(".//*"):
+            (cns, cln) = _qsplit(ce.tag)
+            if cln == "program":
+                self.program = ce.text
+            elif cln == "version":
+                self.program_version = ce.text
+            elif cln == "command_line":
+                self.command_line = ce.text
+            elif cln == "image_filename":
+                self.sources.append(ce.text)
+            elif cln in ("creator", "build_environment"):
+                for cce in ce.findall(".//*"):
+                    if _qsplit(cce.tag)[1] != "library":
+                        continue
+                    lobj = LibraryObject()
+                    lobj.populate_from_Element(cce)
+                    if cln == "build_environment":
+                        self.add_build_library(lobj)
+                    elif cln == "creator":
+                        self.add_creator_library(lobj)
+            elif (cns, cln) == (dfxml.XMLNS_DELTA, "file_ignore"):
+                self.diff_file_ignores.add(ce.text)
+            elif cns not in [dfxml.XMLNS_DFXML, ""]:
+                #Put all non-DFXML-namespace elements into the externals list.
+                self.externals.append(ce)
+
+    def print_dfxml(self, output_fh=sys.stdout):
+        """Memory-efficient DFXML document printer.  However, it assumes the whole element tree is already constructed."""
+        pe = self.to_partial_Element()
+        dfxml_wrapper = _ET_tostring(pe)
+        #_logger.debug("print_dfxml:dfxml_wrapper = %r." % dfxml_wrapper)
+        dfxml_foot = "</dfxml>"
+        #Check for an empty element
+        if dfxml_wrapper.strip()[-3:] == " />":
+            dfxml_head = dfxml_wrapper.strip()[:-3] + ">"
+        elif dfxml_wrapper.strip()[-2:] == "/>":
+            dfxml_head = dfxml_wrapper.strip()[:-2] + ">"
+        else:
+            dfxml_head = dfxml_wrapper.strip()[:-len(dfxml_foot)]
+
+        output_fh.write("""<?xml version="1.0"?>\n""")
+        output_fh.write(dfxml_head)
+        output_fh.write("\n")
+        _logger.debug("Writing %d volume objects." % len(self._volumes))
+        for v in self._volumes:
+            v.print_dfxml(output_fh)
+            output_fh.write("\n")
+        _logger.debug("Writing %d file objects." % len(self._files))
+        for f in self._files:
+            e = f.to_Element()
+            output_fh.write(_ET_tostring(e))
+            output_fh.write("\n")
+        output_fh.write(dfxml_foot)
+        output_fh.write("\n")
+
+    def to_Element(self):
+        outel = self.to_partial_Element()
+        for v in self._volumes:
+            tmpel = v.to_Element()
+            outel.append(tmpel)
+        for f in self._files:
+            tmpel = f.to_Element()
+            outel.append(tmpel)
+        return outel
+
+    def to_dfxml(self):
+        """Serializes the entire DFXML document tree into a string.  Then returns that string.  RAM-intensive.  Most will want to use print_dfxml() instead"""
+        return _ET_tostring(self.to_Element())
+
+    def to_partial_Element(self):
+        outel = ET.Element("dfxml")
+
+        _logger.debug("self.diff_file_ignores = %r." % self.diff_file_ignores)
+        for diff_file_ignore in sorted(self.diff_file_ignores):
+            self.add_namespace("delta", dfxml.XMLNS_DELTA)
+            tmpel0 = ET.Element("delta:file_ignore")
+            tmpel0.text = diff_file_ignore
+            outel.append(tmpel0)
+
+        for e in self.externals:
+            outel.append(e)
+
+        tmpel0 = ET.Element("metadata")
+        for key in sorted(self.dc):
+            _typecheck(key, str)
+            if ":" in key:
+                raise ValueError("Dublin Core key-value entries should have keys without the colon character.  If this causes an interesting namespace issue for you, please report it as a bug.")
+            tmpel1 = ET.Element("dc:" + key)
+            tmpel1.text = self.dc[key]
+            tmpel0.append(tmpel1)
+        outel.append(tmpel0)
+
+        if self.command_line or \
+          self.program or \
+          self.program_version or \
+          0 < len(self.build_libraries) or \
+          0 < len(self.creator_libraries):
+            tmpel0 = ET.Element("creator")
+            if self.program:
+                tmpel1 = ET.Element("program")
+                tmpel1.text = self.program
+                tmpel0.append(tmpel1)
+            if self.program_version:
+                tmpel1 = ET.Element("version")
+                tmpel1.text = self.program_version
+                tmpel0.append(tmpel1)
+            if 0 < len(self.build_libraries):
+                tmpel1 = ET.Element("build_environment")
+                for library in self._build_libraries:
+                    tmpel2 = library.to_Element()
+                    tmpel1.append(tmpel2)
+                tmpel0.append(tmpel1)
+            if self.command_line:
+                tmpel1 = ET.Element("execution_environment")
+                tmpel2 = ET.Element("command_line")
+                tmpel2.text = self.command_line
+                tmpel1.append(tmpel2)
+                tmpel0.append(tmpel1)
+            for library in self.creator_libraries:
+                tmpel1 = library.to_Element()
+                tmpel0.append(tmpel1)
+            outel.append(tmpel0)
+
+        if len(self.sources) > 0:
+            tmpel0 = ET.Element("source")
+            for source in self.sources:
+                tmpel1 = ET.Element("image_filename")
+                tmpel1.text = source
+                tmpel0.append(tmpel1)
+            outel.append(tmpel0)
+
+        if self.version:
+            outel.attrib["version"] = self.version
+
+        #Apparently, namespace setting is only available with the write() function, which is memory-impractical for significant uses of DFXML.
+        #Ref: http://docs.python.org/3.3/library/xml.etree.elementtree.html#xml.etree.ElementTree.ElementTree.write
+        for (prefix, url) in self.iter_namespaces():
+            if prefix == "":
+                attrib_name = "xmlns"
+            else:
+                attrib_name = "xmlns:" + prefix
+            outel.attrib[attrib_name] = url
+        #_logger.debug("ET namespaces at outel generation: %r." % ET._namespace_map)
+        #_logger.debug("outel.attrib = %r." % outel.attrib)
+
+        return outel
+
+    @property
+    def command_line(self):
+        return self._command_line
+
+    @command_line.setter
+    def command_line(self, value):
+        self._command_line = _strcast(value)
+
+    @property
+    def build_libraries(self):
+        return self._build_libraries
+
+    @property
+    def creator_libraries(self):
+        return self._creator_libraries
+
+    @property
+    def dc(self):
+        """The Dublin Core dictionary of key-value pairs for this document.  Typically, "type" is  "Hash List", or "Disk Image".  Keys should be strings not containing colons, values should be strings.  If this causes an issue for you, please report it as a bug."""
+        return self._dc
+
+    @dc.setter
+    def dc(self, value):
+        _typecheck(value, dict)
+        self._dc = value
+
+    @property
+    def diff_file_ignores(self):
+        """A set of DFXML file properties that are excluded from being flagged as differences.  An example of when one may want to use this is when comparing two file system trees in the same file system: inodes are likely to be a differing factor, best excluded to inspect other changes."""
+        return self._diff_file_ignores
+
+    @diff_file_ignores.setter
+    def diff_file_ignores(self, value):
+        _typecheck(value, set)
+        self._diff_file_ignores = value
+
+    @property
+    def externals(self):
+        """(This property behaves the same as FileObject.externals.)"""
+        return self._externals
+
+    @externals.setter
+    def externals(self, val):
+        _typecheck(val, OtherNSElementList)
+        self._externals = val
+
+    @property
+    def files(self):
+        """List of file objects directly attached to this DFXMLObject.  No setter for now."""
+        return self._files
+
+    @property
+    def namespaces(self):
+        raise AttributeError("The namespaces dictionary should not be directly accessed; instead, use .iter_namespaces().")
+
+    @property
+    def program(self):
+        """This property becomes the element at dfxml/creator/program."""
+        return self._program
+
+    @program.setter
+    def program(self, value):
+        self._program = _strcast(value)
+
+    @property
+    def program_version(self):
+        """This property becomes the element at dfxml/creator/version."""
+        return self._program_version
+
+    @program_version.setter
+    def program_version(self, value):
+        self._program_version = _strcast(value)
+
+    @property
+    def sources(self):
+        return self._sources
+
+    @sources.setter
+    def sources(self, value):
+        if not value is None:
+            _typecheck(value, list)
+        self._sources = value
+
+    @property
+    def version(self):
+        return self._version
+
+    @version.setter
+    def version(self, value):
+        self._version = _strcast(value)
+
+    @property
+    def volumes(self):
+        """List of volume objects directly attached to this DFXMLObject.  No setter for now."""
+        return self._volumes
+
+class LibraryObject(object):
+    def __init__(self, *args, **kwargs):
+        self.name = None
+        self.version = None
+
+        if len(args) >= 1:
+            self.name = args[0]
+        if len(args) >= 2:
+            self.version = args[1]
+
+    def __eq__(self, other):
+        """
+        This equality function tests the name and version values strictly.  For less-strict testing, like allowing matching on missing versions, use relaxed_eq.
+        This function can compare against another LibraryObject.
+        """
+        if not isinstance(other, LibraryObject):
+            return False
+        return self.name == other.name and \
+          self.version == other.version
+
+    def __repr__(self):
+        parts = []
+        if self.name:
+            parts.append("name=%r" % self.name)
+        if self.version:
+            parts.append("version=%r" % self.version)
+        return "LibraryObject(" + ", ".join(parts) + ")"
+
+    def populate_from_Element(self, e):
+        if "name" in e.attrib:
+            self.name = e.attrib["name"]
+        if "version" in e.attrib:
+            self.version = e.attrib["version"]
+
+    def relaxed_eq(self, other):
+        """
+        This function can compare against another LibraryObject.
+        """
+        if not isinstance(other, LibraryObject):
+            return False
+        if self.name != other.name:
+            return False
+        if self.version is None or other.version is None:
+            return True
+        return self.version == other.version
+
+    def to_Element(self):
+        outel = ET.Element("library")
+        if not self.name is None:
+            outel.attrib["name"] = self.name
+        if not self.version is None:
+            outel.attrib["version"] = self.version
+        return outel
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = _strcast(value)
+
+    @property
+    def version(self):
+        return self._version
+
+    @version.setter
+    def version(self, value):
+        self._version = _strcast(value)
+
+class RegXMLObject(object):
+    def __init__(self, *args, **kwargs):
+        self.command_line = kwargs.get("command_line")
+        self.interpreter = kwargs.get("interpreter")
+        self.metadata = kwargs.get("metadata")
+        self.program = kwargs.get("program")
+        self.program_version = kwargs.get("program_version")
+        self.sources = kwargs.get("sources", [])
+        self.version = kwargs.get("version")
+        self._hives = []
+        self._cells = []
+        self._namespaces = dict()
+        input_hives = kwargs.get("hives") or [] # In case kwargs["hives"] = None.
+        input_cells = kwargs.get("cells") or []
+        for hive in input_hives:
+            self.append(hive)
+        for cell in input_cells:
+            self.append(cells)
+
+        #Add default namespaces
+        #TODO This will cause a problem when the Objects bindings are used for a DFXML document and RegXML document in the same program.
+        self.add_namespace("", XMLNS_REGXML)
+
+    def __iter__(self):
+        """Yields all HiveObjects, recursively their CellObjects, and the CellObjects directly attached to this RegXMLObject, in that order."""
+        for h in self._hives:
+            yield h
+            for c in h:
+                yield c
+        for c in self._cells:
+            yield c
+
+    def add_namespace(self, prefix, url):
+        self._namespaces[prefix] = url
+        ET.register_namespace(prefix, url)
+
+    def append(self, value):
+        if isinstance(value, HiveObject):
+            self._hives.append(value)
+        elif isinstance(value, CellObject):
+            self._cells.append(value)
+        else:
+            _logger.debug("value = %r" % value)
+            raise TypeError("Expecting a HiveObject or a CellObject.  Got instead this type: %r." % type(value))
+
+    def print_regxml(self, output_fh=sys.stdout):
+        """Serializes and prints the entire object, without constructing the whole tree."""
+        regxml_wrapper = _ET_tostring(self.to_partial_Element())
+        #_logger.debug("regxml_wrapper = %r." % regxml_wrapper)
+        regxml_foot = "</regxml>"
+        #Check for an empty element
+        if regxml_wrapper.strip()[-3:] == " />":
+            regxml_head = regxml_wrapper.strip()[:-3] + ">"
+        elif regxml_wrapper.strip()[-2:] == "/>":
+            regxml_head = regxml_wrapper.strip()[:-2] + ">"
+        else:
+            regxml_head = regxml_wrapper.strip()[:-len(regxml_foot)]
+
+        output_fh.write(regxml_head)
+        output_fh.write("\n")
+        for hive in self._hives:
+            hive.print_regxml(output_fh)
+        output_fh.write(regxml_foot)
+        output_fh.write("\n")
+
+    def to_Element(self):
+        outel = self.to_partial_Element()
+
+        for hive in self._hives:
+            tmpel = hive.to_Element()
+            outel.append(tmpel)
+
+        for cell in self._cells:
+            tmpel = cell.to_Element()
+            outel.append(tmpel)
+
+        return outel
+
+    def to_partial_Element(self):
+        """
+        Creates the wrapping RegXML element.  No hives, no cells.  Saves on creating an entire Element tree in memory.
+        """
+        outel = ET.Element("regxml")
+
+        if self.version:
+            outel.attrib["version"] = self.version
+
+        if self.program or self.program_version:
+            tmpel0 = ET.Element("creator")
+            if self.program:
+                tmpel1 = ET.Element("program")
+                tmpel1.text = self.program
+                tmpel0.append(tmpel1)
+            if self.program_version:
+                tmpel1 = ET.Element("version")
+                tmpel1.text = self.program_version
+                tmpel0.append(tmpel1)
+            outel.append(tmpel0)
+
+        if self.command_line:
+            tmpel0 = ET.Element("execution_environment")
+
+            if self.interpreter:
+                tmpel1 = ET.Element("interpreter")
+                tmpel1.text = self.interpreter
+
+            tmpel1 = ET.Element("command_line")
+            tmpel1.text = self.command_line
+            tmpel0.append(tmpel1)
+
+            #TODO Note libraries used at run-time
+
+            outel.append(tmpel0)
+
+        if len(self.sources) > 0:
+            tmpel0 = ET.Element("source")
+            for source in self.sources:
+                tmpel1 = ET.Element("image_filename")
+                tmpel1.text = source
+                tmpel0.append(tmpel1)
+            outel.append(tmpel0)
+
+        #Apparently, namespace setting is only available with the write() function, which is memory-impractical for significant uses of RegXML.
+        #Ref: http://docs.python.org/3.3/library/xml.etree.elementtree.html#xml.etree.ElementTree.ElementTree.write
+        for prefix in sorted(self._namespaces.keys()):
+            if prefix == "":
+                attrib_name = "xmlns"
+            else:
+                attrib_name += "xmlns:" + prefix
+            outel.attrib[attrib_name] = self._namespaces[prefix]
+
+        return outel
+
+    def to_regxml(self):
+        """Serializes the entire RegXML document tree into a string.  Returns that string.  RAM-intensive.  Most will want to use print_regxml() instead."""
+        return _ET_tostring(self.to_Element())
+
+
+class VolumeObject(object):
+
+    _all_properties = set([
+      "annos",
+      "allocated_only",
+      "block_count",
+      "block_size",
+      "byte_runs",
+      "error",
+      "externals",
+      "first_block",
+      "ftype",
+      "ftype_str",
+      "last_block",
+      "partition_offset",
+      "original_volume",
+      "sector_size"
+    ])
+
+    _diff_attr_names = {
+      "new":"delta:new_volume",
+      "deleted":"delta:deleted_volume",
+      "modified":"delta:modified_volume",
+      "matched":"delta:matched"
+    }
+
+    #TODO There may be need in the future to compare the annotations as well.  It complicates make_differential_dfxml too much for now.
+    _incomparable_properties = set([
+      "annos"
+    ])
+
+    def __init__(self, *args, **kwargs):
+        self._files = []
+        self._annos = set()
+        self._diffs = set()
+
+        for prop in VolumeObject._all_properties:
+            if prop in ["annos", "files"]:
+                continue
+            elif prop == "externals":
+                setattr(self, prop, kwargs.get(prop, OtherNSElementList()))
+            else:
+                setattr(self, prop, kwargs.get(prop))
+
+    def __iter__(self):
+        """Yields all FileObjects directly attached to this VolumeObject."""
+        for f in self._files:
+            yield f
+
+    def __repr__(self):
+        parts = []
+        for prop in VolumeObject._all_properties:
+            #Skip outputting the files list.
+            if prop == "files":
+                continue
+            val = getattr(self, prop)
+            if not val is None:
+                parts.append("%s=%r" % (prop, val))
+        return "VolumeObject(" + ", ".join(parts) + ")"
+
+    def append(self, value):
+        _typecheck(value, FileObject)
+        self._files.append(value)
+
+    def compare_to_original(self):
+        self._diffs = self.compare_to_other(self.original_volume, True)
+
+    def compare_to_other(self, other, ignore_original=False):
+        """Returns a set of all the properties found to differ."""
+        _typecheck(other, VolumeObject)
+        diffs = set()
+        for prop in VolumeObject._all_properties:
+            if prop in VolumeObject._incomparable_properties:
+                continue
+            if ignore_original and prop == "original_volume":
+                continue
+
+            #_logger.debug("getattr(self, %r) = %r" % (prop, getattr(self, prop)))
+            #_logger.debug("getattr(other, %r) = %r" % (prop, getattr(other, prop)))
+
+            #Allow file system type to be case-insensitive
+            if prop == "ftype_str":
+                o = getattr(other, prop)
+                if o: o = o.lower()
+                s = getattr(self, prop)
+                if s: s = s.lower()
+                if s != o:
+                    diffs.add(prop)
+            else:
+                if getattr(self, prop) != getattr(other, prop):
+                    diffs.add(prop)
+        return diffs
+
+    def populate_from_Element(self, e):
+        global _warned_elements
+        _typecheck(e, (ET.Element, ET.ElementTree))
+        #_logger.debug("e = %r" % e)
+
+        #Read differential annotations
+        _read_differential_annotations(VolumeObject._diff_attr_names, e, self.annos)
+
+        #Split into namespace and tagname
+        (ns, tn) = _qsplit(e.tag)
+        assert tn in ["volume", "original_volume"]
+
+        #Look through direct-child elements to populate run array
+        for ce in e.findall("./*"):
+            #_logger.debug("ce = %r" % ce)
+            (cns, ctn) = _qsplit(ce.tag)
+            #_logger.debug("cns = %r" % cns)
+            #_logger.debug("ctn = %r" % ctn)
+            if ctn == "byte_runs":
+                self.byte_runs = ByteRuns()
+                self.byte_runs.populate_from_Element(ce)
+            elif ctn == "byte_run":
+                #byte_runs' block recursively handles this element.
+                continue
+            elif ctn == "original_volume":
+                self.original_volume = VolumeObject()
+                self.original_volume.populate_from_Element(ce)
+            elif ctn in VolumeObject._all_properties:
+                #_logger.debug("ce.text = %r" % ce.text)
+                setattr(self, ctn, ce.text)
+                #_logger.debug("getattr(self, %r) = %r" % (ctn, getattr(self, ctn)))
+            elif cns not in [dfxml.XMLNS_DFXML, ""]:
+                #Put all non-DFXML-namespace elements into the externals list.
+                self.externals.append(ce)
+            else:
+                if (cns, ctn) not in _warned_elements:
+                    _warned_elements.add((cns, ctn))
+                    _logger.warning("Unsure what to do with this element in a VolumeObject: %r" % ce)
+
+    def print_dfxml(self, output_fh=sys.stdout):
+        pe = self.to_partial_Element()
+        dfxml_wrapper = _ET_tostring(pe)
+
+        if len(pe) == 0 and len(self._files) == 0:
+            output_fh.write(dfxml_wrapper)
+            return
+
+        dfxml_foot = "</volume>"
+
+        #Deal with an empty element being printed as <elem/>
+        if len(pe) == 0:
+            replaced_dfxml_wrapper = dfxml_wrapper.replace(" />", ">")
+            dfxml_head = replaced_dfxml_wrapper
+        else:
+            dfxml_head = dfxml_wrapper.strip()[:-len(dfxml_foot)]
+
+        output_fh.write(dfxml_head)
+        output_fh.write("\n")
+        _logger.debug("Writing %d file objects for this volume." % len(self._files))
+        for f in self._files:
+            e = f.to_Element()
+            output_fh.write(_ET_tostring(e))
+            output_fh.write("\n")
+        output_fh.write(dfxml_foot)
+        output_fh.write("\n")
+
+    def to_Element(self):
+        outel = self.to_partial_Element()
+        #If there is an error reported on this volume, pop the element off of the partial element's end.
+        errorel = None
+        if not (self.error is None or self.error == ""):
+            if len(outel) == 0:
+                raise ValueError("Partial volume element has no children, but at least the error property was set.")
+            if _qsplit(outel[-1].tag)[1] == "error":
+                #(ET.Element does not have pop().)
+                errorel = outel[-1]
+                del(outel[-1])
+            else:
+                if outel.find("error"):
+                    global _nagged_volume_error_impldrift
+                    if not _nagged_volume_error_impldrift:
+                        _logger.error("Implementation drift - when this code was initially written, the error element was the last to be appended to the partial element.  Leaving the found error element in place for now, but this may fail validation against the schema because of child ordering.")
+                        _nagged_volume_error_impldrift = True
+                else:
+                    global _nagged_volume_error_standin
+                    if not _nagged_volume_error_standin:
+                        _logger.warning("Could not find 'error' child on partial volume element.  Creating a replacement.")
+                        _nagged_volume_error_standin = True
+                    errorel = ET.Element("error")
+                    errorel.text = str(self.error)
+        for f in self._files:
+            tmpel = f.to_Element()
+            outel.append(tmpel)
+        #The error element comes after the fileobject list in the schema.
+        if not errorel is None:
+            outel.append(errorel)
+        return outel
+
+    def to_partial_Element(self):
+        """Returns the volume element with its properties, except for the child fileobjects.  Properties are appended in DFXML schema order."""
+        outel = ET.Element("volume")
+
+        annos_whittle_set = copy.deepcopy(self.annos)
+        diffs_whittle_set = copy.deepcopy(self.diffs)
+
+        #Add differential annotations
+        for annodiff in VolumeObject._diff_attr_names:
+            if annodiff in annos_whittle_set:
+                outel.attrib[VolumeObject._diff_attr_names[annodiff]] = "1"
+                annos_whittle_set.remove(annodiff)
+        if len(annos_whittle_set) > 0:
+            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
+
+        for e in self.externals:
+            outel.append(e)
+
+        if self.byte_runs:
+            outel.append(self.byte_runs.to_Element())
+
+        def _append_el(prop, value):
+            tmpel = ET.Element(prop)
+            _keep = False
+            if not value is None:
+                tmpel.text = str(value)
+                _keep = True
+            if prop in self.diffs:
+                tmpel.attrib["delta:changed_property"] = "1"
+                diffs_whittle_set.remove(prop)
+                _keep = True
+            if _keep:
+                outel.append(tmpel)
+
+        def _append_str(prop):
+            value = getattr(self, prop)
+            _append_el(prop, value)
+
+        def _append_bool(prop):
+            value = getattr(self, prop)
+            if not value is None:
+                value = "1" if value else "0"
+            _append_el(prop, value)
+
+        for prop in [
+          "partition_offset",
+          "sector_size",
+          "block_size",
+          "ftype",
+          "ftype_str",
+          "block_count",
+          "first_block",
+          "last_block"
+        ]:
+            _append_str(prop)
+
+        #Output the one Boolean property
+        _append_bool("allocated_only")
+
+        #Output the original volume's properties
+        if not self.original_volume is None or "original_volume" in diffs_whittle_set:
+            #Skip FileObject list, if any
+            if self.original_volume is None:
+                tmpel = ET.Element("delta:original_volume")
+            else:
+                tmpel = self.original_volume.to_partial_Element()
+                tmpel.tag = "delta:original_volume"
+
+            if "original_volume" in diffs_whittle_set:
+                tmpel.attrib["delta:changed_property"] = "1"
+
+            outel.append(tmpel)
+
+        #Output the error property (which will be popped and re-appended after the file list in to_Element)
+        #The error should come last because of the two spots extended elements can be placed; this is to simplify the file-listing VolumeObject.to_Element() method.
+        _append_str("error")
+
+        if len(diffs_whittle_set) > 0:
+            _logger.warning("Did not annotate all of the differing properties of this volume.  Remaining properties:  %r." % diffs_whittle_set)
+
+        return outel
+
+    @property
+    def allocated_only(self):
+        return self._allocated_only
+
+    @allocated_only.setter
+    def allocated_only(self, val):
+        self._allocated_only = _boolcast(val)
+
+    @property
+    def annos(self):
+        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
+        return self._annos
+
+    @annos.setter
+    def annos(self, val):
+        _typecheck(val, set)
+        self._annos = val
+
+    @property
+    def block_count(self):
+        return self._block_count
+
+    @block_count.setter
+    def block_count(self, val):
+        self._block_count = _intcast(val)
+
+    @property
+    def block_size(self):
+        return self._block_size
+
+    @block_size.setter
+    def block_size(self, val):
+        self._block_size = _intcast(val)
+
+    @property
+    def diffs(self):
+        return self._diffs
+
+    @property
+    def error(self):
+        return self._error
+
+    @error.setter
+    def error(self, val):
+        self._error = _strcast(val)
+
+    @property
+    def externals(self):
+        """(This property behaves the same as FileObject.externals.)"""
+        return self._externals
+
+    @externals.setter
+    def externals(self, val):
+        _typecheck(val, OtherNSElementList)
+        self._externals = val
+
+    @property
+    def files(self):
+        """List of file objects directly attached to this VolumeObject.  No setter for now."""
+        return self._files
+
+    @property
+    def first_block(self):
+        return self._first_block
+
+    @first_block.setter
+    def first_block(self, val):
+        self._first_block = _intcast(val)
+
+    @property
+    def ftype(self):
+        return self._ftype
+
+    @ftype.setter
+    def ftype(self, val):
+        self._ftype = _intcast(val)
+
+    @property
+    def ftype_str(self):
+        return self._ftype_str
+
+    @ftype_str.setter
+    def ftype_str(self, val):
+        self._ftype_str = _strcast(val)
+
+    @property
+    def last_block(self):
+        return self._last_block
+
+    @last_block.setter
+    def last_block(self, val):
+        self._last_block = _intcast(val)
+
+    @property
+    def original_volume(self):
+        return self._original_volume
+
+    @original_volume.setter
+    def original_volume(self, val):
+        if not val is None:
+            _typecheck(val, VolumeObject)
+        self._original_volume= val
+
+    @property
+    def partition_offset(self):
+        return self._partition_offset
+
+    @partition_offset.setter
+    def partition_offset(self, val):
+        self._partition_offset = _intcast(val)
+
+    @property
+    def sector_size(self):
+        return self._sector_size
+
+    @sector_size.setter
+    def sector_size(self, val):
+        self._sector_size = _intcast(val)
+
+class HiveObject(object):
+
+    _all_properties = set([
+      "annos",
+      "mtime",
+      "filename",
+      "original_fileobject",
+      "original_hive"
+    ])
+
+    _diff_attr_names = {
+      "new":"delta:new_hive",
+      "deleted":"delta:deleted_hive",
+      "modified":"delta:modified_hive",
+      "matched":"delta:matched"
+    }
+
+    _incomparable_properties = set([
+      "annos"
+    ])
+
+    def __init__(self, *args, **kwargs):
+        self._cells = []
+        self._annos = set()
+        self._diffs = set()
+
+        for prop in HiveObject._all_properties:
+            if prop in ["annos", "cells"]:
+                continue
+            setattr(self, prop, kwargs.get(prop))
+
+    def __iter__(self):
+        """Yields all CellObjects directly attached to this HiveObject."""
+        for c in self._cells:
+            yield c
+
+    def append(self, value):
+        _typecheck(value, CellObject)
+        self._cells.append(value)
+
+    def compare_to_original(self):
+        self._diffs = self.compare_to_other(self.original_hive, True)
+
+    def compare_to_other(self, other, ignore_original=False):
+        """Returns a set of all the properties found to differ."""
+        _typecheck(other, HiveObject)
+        diffs = set()
+        for prop in HiveObject._all_properties:
+            if prop in HiveObject._incomparable_properties:
+                continue
+            if ignore_original and prop == "original_hive":
+                continue
+
+            #Allow file system type to be case-insensitive
+            if getattr(self, prop) != getattr(other, prop):
+                diffs.add(prop)
+        return diffs
+
+    def print_regxml(self, output_fh=sys.stdout):
+        pe = self.to_partial_Element()
+        xml_wrapper = _ET_tostring(pe)
+        xml_foot = "</hive>"
+        #Check for an empty element
+        if xml_wrapper.strip()[-3:] == " />":
+            xml_head = xml_wrapper.strip()[:-3] + ">"
+        elif xml_wrapper.strip()[-2:] == "/>":
+            xml_head = xml_wrapper.strip()[:-2] + ">"
+        else:
+            xml_head = xml_wrapper.strip()[:-len(xml_foot)]
+
+        output_fh.write(xml_head)
+        output_fh.write("\n")
+
+        for cell in self._cells:
+            output_fh.write(cell.to_regxml())
+            output_fh.write("\n")
+
+        output_fh.write(xml_foot)
+        output_fh.write("\n")
+
+    def to_Element(self):
+        outel = self.to_partial_Element()
+        for cell in self._cells:
+            tmpel = cell.to_Element()
+            outel.append(tmpel)
+        return outel
+
+    def to_partial_Element(self):
+        outel = ET.Element("hive")
+
+        if self.filename:
+            tmpel = ET.Element("filename")
+            tmpel.text = self.filename
+            outel.append(tmpel)
+
+        if self.mtime:
+            tmpel = self.mtime.to_Element()
+            outel.append(tmpel)
+
+        if self.original_fileobject:
+            tmpel = self.original_fileobject.to_Element()
+            #NOTE: "delta" namespace intentionally omitted.
+            tmpel.tag = "original_fileobject"
+            outel.append(tmpel)
+
+        return outel
+
+    @property
+    def annos(self):
+        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
+        return self._annos
+
+    @annos.setter
+    def annos(self, val):
+        _typecheck(val, set)
+        self._annos = val
+
+    @property
+    def filename(self):
+        """Path of the hive file within the parent file system."""
+        return self._filename
+
+    @filename.setter
+    def filename(self, val):
+        self._filename = _strcast(val)
+
+    @property
+    def mtime(self):
+        return self._mtime
+
+    @mtime.setter
+    def mtime(self, val):
+        if val is None:
+            self._mtime = None
+        elif isinstance(val, TimestampObject):
+            self._mtime = val
+        else:
+            checked_val = TimestampObject(val, name="mtime")
+            self._mtime = checked_val
+
+    @property
+    def original_fileobject(self):
+        return self._original_fileobject
+
+    @original_fileobject.setter
+    def original_fileobject(self, val):
+        if not val is None:
+            _typecheck(val, FileObject)
+        self._original_fileobject = val
+
+    @property
+    def original_hive(self):
+        return self._original_hive
+
+    @original_hive.setter
+    def original_hive(self, val):
+        if not val is None:
+            _typecheck(val, HiveObject)
+        self._original_hive = val
+
+class ByteRun(object):
+
+    _all_properties = set([
+      "img_offset",
+      "fs_offset",
+      "file_offset",
+      "fill",
+      "len",
+      "type",
+      "uncompressed_len"
+    ])
+
+    def __init__(self, *args, **kwargs):
+        for prop in ByteRun._all_properties:
+            setattr(self, prop, kwargs.get(prop))
+
+    def __add__(self, other):
+        """
+        Joins two ByteRun objects into a single run if possible.  Returns a new object of the concatenation if successful, None if not.
+        """
+        _typecheck(other, ByteRun)
+        #Don't glom fills of different values
+        if self.fill != other.fill:
+            return None
+
+        #Don't glom typed byte runs (particularly since type has been observed to be 'resident')
+        if self.type != other.type:
+            return None
+
+        #Don't glom compressed runs
+        if not self.uncompressed_len is None or not other.uncompressed_len is None:
+            return None
+
+        if None in [self.len, other.len]:
+            return None
+
+        for prop in ["img_offset", "fs_offset", "file_offset"]:
+            if None in [getattr(self, prop), getattr(other, prop)]:
+                continue
+            if getattr(self, prop) + self.len == getattr(other, prop):
+                retval = copy.deepcopy(self)
+                retval.len += other.len
+                return retval
+        return None
+
+    def __eq__(self, other):
+        #Check type
+        if other is None:
+            return False
+        if not isinstance(other, ByteRun):
+            if not _warned_byterun_badtypecomp:
+                _logger.warning("A ByteRun comparison was called against a non-ByteRun object: " + repr(other) + ".")
+                _warned_byterun_badtypecomp = True
+            return False
+
+        #Check values
+        return \
+          self.img_offset == other.img_offset and \
+          self.fs_offset == other.fs_offset and \
+          self.file_offset == other.file_offset and \
+          self.fill == other.fill and \
+          self.len == other.len and \
+          self.type == other.type and \
+          self.uncompressed_len == other.uncompressed_len
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        parts = []
+        for prop in ByteRun._all_properties:
+            val = getattr(self, prop)
+            if not val is None:
+                parts.append("%s=%r" % (prop, val))
+        return "ByteRun(" + ", ".join(parts) + ")"
+
+    def populate_from_Element(self, e):
+        _typecheck(e, (ET.Element, ET.ElementTree))
+
+        #Split into namespace and tagname
+        (ns, tn) = _qsplit(e.tag)
+        assert tn == "byte_run"
+
+        copied_attrib = copy.deepcopy(e.attrib)
+
+        #Populate run properties from element attributes
+        for prop in ByteRun._all_properties:
+            if prop in copied_attrib:
+                val = copied_attrib.get(prop)
+                if not val is None:
+                    setattr(self, prop, val)
+                del copied_attrib[prop]
+        #Note remaining properties
+        for prop in copied_attrib:
+            if prop not in _warned_byterun_attribs:
+                _warned_byterun_attribs.add(prop)
+                _logger.warning("No instructions present for processing this attribute found on a byte run: %r." % prop)
+
+    def to_Element(self):
+        outel = ET.Element("byte_run")
+        for prop in ByteRun._all_properties:
+            val = getattr(self, prop)
+            #Skip null properties
+            if val is None:
+                continue
+
+            if isinstance(val, bytes):
+                outel.attrib[prop] = str(struct.unpack("b", val)[0])
+            else:
+                outel.attrib[prop] = str(val)
+
+        return outel
+
+    @property
+    def file_offset(self):
+        return self._file_offset
+
+    @file_offset.setter
+    def file_offset(self, val):
+        self._file_offset = _intcast(val)
+
+    @property
+    def fill(self):
+        """
+        At the moment, the fill value is assumed to be a single byte.  The value you receive from this property wll be None or a byte.  Setting fill to the string "0" will return the null byte when retrieved later.
+
+        For now, setting to any digital string (e.g. "41") will return a byte representing the integer casting string (e.g. the number 41), but this is subject to change pending some discussion.
+        """
+        return self._fill
+
+    @fill.setter
+    def fill(self, val):
+        if val is None:
+            self._fill = val
+        elif val == "0":
+            self._fill = b'\x00'
+        elif isinstance(val, bytes):
+            if len(val) != 1:
+                raise NotImplementedError("Received a %d-length fill byte string for a byte run.  Only 1-byte fill strings are accepted for now, pending further discussion.")
+            self._fill = val
+        elif isinstance(val, int):
+            #This is the easiest way between Python 2 and 3.  int.to_bytes would be better, but that is only in >=3.2.
+            self._fill = struct.pack("b", val)
+        elif isinstance(val, str) and val.isdigit():
+            #Recurse, changing type
+            self.fill = int(val)
+
+    @property
+    def fs_offset(self):
+        return self._fs_offset
+
+    @fs_offset.setter
+    def fs_offset(self, val):
+        self._fs_offset = _intcast(val)
+
+    @property
+    def img_offset(self):
+        return self._img_offset
+
+    @img_offset.setter
+    def img_offset(self, val):
+        self._img_offset = _intcast(val)
+
+    @property
+    def len(self):
+        return self._len
+
+    @len.setter
+    def len(self, val):
+        self._len = _intcast(val)
+
+    @property
+    def type(self):
+        return self._type
+
+    @type.setter
+    def type(self, val):
+        self._type = _strcast(val)
+
+    @property
+    def uncompressed_len(self):
+        return self._uncompressed_len
+
+    @uncompressed_len.setter
+    def uncompressed_len(self, val):
+        self._uncompressed_len = _intcast(val)
+
+class ByteRuns(object):
+    """
+    A list-like object for ByteRun objects.
+    """
+    #Must define these methods to adhere to the list protocol:
+    #__len__
+    #__getitem__
+    #__setitem__
+    #__delitem__
+    #__iter__
+    #append
+    #
+    #Refs:
+    #http://www.rafekettler.com/magicmethods.html
+    #http://stackoverflow.com/a/8841520
+
+    _facet_values = [None, "data", "inode", "name"]
+
+    def __init__(self, run_list=None, **kwargs):
+        self._facet = kwargs.get("facet")
+        self._listdata = []
+        if isinstance(run_list, list):
+            for run in run_list:
+                self.append(run)
+
+    def __delitem__(self, key):
+        del self._listdata[key]
+
+    def __eq__(self, other):
+        """Compares the byte run lists and the facet (allowing a null facet to match "data")."""
+        #Check type
+        if other is None:
+            return False
+        _typecheck(other, ByteRuns)
+
+        if self.facet != other.facet:
+            if set([self.facet, other.facet]) != set([None, "data"]):
+                return False
+        if len(self) != len(other):
+            #_logger.debug("len(self) = %d" % len(self))
+            #_logger.debug("len(other) = %d" % len(other))
+            return False
+        for (sbr_index, sbr) in enumerate(self):
+            obr = other[sbr_index]
+            #_logger.debug("sbr_index = %d" % sbr_index)
+            #_logger.debug("sbr = %r" % sbr)
+            #_logger.debug("obr = %r" % obr)
+            if sbr != obr:
+                return False
+        return True
+
+    def __getitem__(self, key):
+        return self._listdata.__getitem__(key)
+
+    def __iter__(self):
+        return iter(self._listdata)
+
+    def __len__(self):
+        return self._listdata.__len__()
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        parts = []
+        for run in self:
+            parts.append(repr(run))
+        maybe_facet = ""
+        if self.facet:
+            maybe_facet = "facet=%r, " % self.facet
+        return "ByteRuns(" + maybe_facet + "run_list=[" + ", ".join(parts) + "])"
+
+    def __setitem__(self, key, value):
+        _typecheck(value, ByteRun)
+        self._listdata[key] = value
+
+    def append(self, value):
+        """
+        Appends a ByteRun object to this container's list.
+        """
+        _typecheck(value, ByteRun)
+        self._listdata.append(value)
+
+    def glom(self, value):
+        """
+        Appends a ByteRun object to this container's list, after attempting to join the run with the last run already stored.
+        """
+        _typecheck(value, ByteRun)
+        if len(self._listdata) == 0:
+            self.append(value)
+        else:
+            last_run = self._listdata[-1]
+            maybe_new_run = last_run + value
+            if maybe_new_run is None:
+                self.append(value)
+            else:
+                self._listdata[-1] = maybe_new_run
+
+    def iter_contents(self, raw_image, buffer_size=1048576, sector_size=512, errlog=None, statlog=None):
+        """
+        Generator.  Yields contents, as byte strings one block at a time, given a backing raw image path.  Relies on The SleuthKit's img_cat, so contents can be extracted from any disk image type that TSK supports.
+        @param buffer_size The maximum size of the byte strings yielded.
+        @param sector_size The size of a disk sector in the raw image.  Required by img_cat.
+        """
+        if not isinstance(raw_image, str):
+            raise TypeError("iter_contents needs the string path to the image file.  Received: %r." % raw_image)
+
+        stderr_fh = None
+        if not errlog is None:
+            stderr_fh = open(errlog, "wb")
+
+        status_fh = None
+        if not statlog is None:
+            status_fh = open(errlog, "wb")
+
+        #The exit status of the last img_cat.
+        last_status = None
+
+        try:
+            for run in self:
+                if run.len is None:
+                    raise AttributeError("Byte runs can't be extracted if a run length is undefined.")
+
+                len_to_read = run.len
+
+                #If we have a fill character, just pump out that character
+                if not run.fill is None and len(run.fill) > 0:
+                    while len_to_read > 0:
+                        #This multiplication and slice should handle multi-byte fill characters, in case that ever comes up.
+                        yield (run.fill * buffer_size)[ : min(len_to_read, buffer_size)]
+                        len_to_read -= buffer_size
+                    #Next byte run
+                    continue
+
+                if run.img_offset is None:
+                    raise AttributeError("Byte runs can't be extracted if missing a fill character and image offset.")
+
+                cmd = ["img_cat"]
+                cmd.append("-b")
+                cmd.append(str(sector_size))
+                cmd.append("-s")
+                cmd.append(str(run.img_offset//sector_size))
+                cmd.append("-e")
+                cmd.append(str( (run.img_offset + run.len)//sector_size))
+                cmd.append(raw_image)
+                p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=stderr_fh)
+
+                #Do the buffered read
+                while len_to_read > 0:
+                    buffer_data = p.stdout.read(buffer_size)
+                    yield_data = buffer_data[ : min(len_to_read, buffer_size)]
+                    if len(yield_data) > 0:
+                        yield yield_data
+                    else:
+                        #Let the subprocess terminate so we can see the exit status
+                        p.wait()
+                        last_status = p.returncode
+                        if last_status != 0:
+                            raise subprocess.CalledProcessError(last_status, " ".join(cmd), "img_cat failed.")
+                    len_to_read -= buffer_size
+        except Exception as e:
+            #Cleanup in an exception
+            if not stderr_fh is None:
+                stderr_fh.close()
+
+            if not status_fh is None:
+                if isinstance(e, subprocess.CalledProcessError):
+                    status_fh.write(e.returncode)
+                else:
+                    status_fh.write("1")
+                status_fh.close()
+            raise e
+
+        #Cleanup when all's gone well.
+        if not status_fh is None:
+            if not last_status is None:
+                status_fh.write(last_status)
+            status_fh.close()
+        if not stderr_fh is None:
+            stderr_fh.close()
+
+    def populate_from_Element(self, e):
+        _typecheck(e, (ET.Element, ET.ElementTree))
+
+        #Split into namespace and tagname
+        (ns, tn) = _qsplit(e.tag)
+        assert tn == "byte_runs"
+
+        if "facet" in e.attrib:
+            self.facet = e.attrib["facet"]
+
+        #Look through direct-child elements to populate run array
+        for ce in e.findall("./*"):
+            (cns, ctn) = _qsplit(ce.tag)
+            if ctn == "byte_run":
+                nbr = ByteRun()
+                nbr.populate_from_Element(ce)
+                self.append(nbr)
+
+    def to_Element(self):
+        outel = ET.Element("byte_runs")
+        for run in self:
+            tmpel = run.to_Element()
+            outel.append(tmpel)
+        if self.facet:
+            outel.attrib["facet"] = self.facet
+        return outel
+
+    @property
+    def facet(self):
+        """Expected to be null, "data", "inode", or "name".  See FileObject.data_brs, FileObject.inode_brs, and FileObject.name_brs."""
+        return self._facet
+
+    @facet.setter
+    def facet(self, val):
+        if not val is None:
+            _typecheck(val, str)
+        if val not in ByteRuns._facet_values:
+            raise ValueError("A ByteRuns facet must be one of these: %r.  Received: %r." % (ByteRuns._facet_values, val))
+        self._facet = val
+
+re_precision = re.compile(r"(?P<num>\d+)(?P<unit>(|m|n)s|d)?")
+class TimestampObject(object):
+    """
+    Encodes the "dftime" type.  Wraps around dfxml.dftime, closely enough that this might just get folded into that class.
+
+    TimestampObjects implement a vs-null comparison workaround as in the SAS family of products:  Null, for ordering purposes, is considered to be a value less than negative infinity.
+    """
+
+    timestamp_name_list = ["mtime", "atime", "ctime", "crtime", "dtime", "bkup_time"]
+
+    def __init__(self, *args, **kwargs):
+        self.name = kwargs.get("name")
+        self.prec = kwargs.get("prec")
+        #_logger.debug("type(args) = %r" % type(args))
+        #_logger.debug("args = %r" % (args,))
+        if len(args) == 0:
+            self.time = None
+        elif len(args) == 1:
+            self.time = args[0]
+        else:
+            raise ValueError("Unexpected arguments.  Whole args tuple: %r." % (args,))
+
+        self._timestamp = None
+
+    def __eq__(self, other):
+        #Check type
+        if other is None:
+            return False
+        _typecheck(other, TimestampObject)
+
+        if self.name != other.name:
+            return False
+        if self.prec != other.prec:
+            return False
+        if self.time != other.time:
+            return False
+        return True
+
+    def __ge__(self, other):
+        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
+        if other is None:
+            return False
+        else:
+            self._comparison_sanity_check(other)
+        return self.time.__ge__(other.time)
+
+    def __gt__(self, other):
+        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
+        if other is None:
+            return False
+        else:
+            self._comparison_sanity_check(other)
+        return self.time.__gt__(other.time)
+
+    def __le__(self, other):
+        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
+        if other is None:
+            return True
+        else:
+            self._comparison_sanity_check(other)
+        return self.time.__le__(other.time)
+
+    def __lt__(self, other):
+        """Note: The semantics here and in other ordering functions are that "Null" is a value less than negative infinity."""
+        if other is None:
+            return True
+        else:
+            self._comparison_sanity_check(other)
+        return self.time.__lt__(other.time)
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        parts = []
+        if self.name:
+            parts.append("name=%r" % self.name)
+        if self.prec:
+            parts.append("prec=%r" % (self.prec,))
+        if self.time:
+            parts.append("%r" % self.time)
+        return "TimestampObject(" + ", ".join(parts) + ")"
+
+    def __str__(self):
+        if self.time:
+            return str(self.time)
+        else:
+            return self.__repr__()
+
+    def _comparison_sanity_check(self, other):
+        if None in (self.time, other.time):
+            raise ValueError("Can't compare TimestampObjects: %r, %r." % self, other)
+
+    def populate_from_Element(self, e):
+        _typecheck(e, (ET.Element, ET.ElementTree))
+        if "prec" in e.attrib:
+            self.prec = e.attrib["prec"]
+        self.time = e.text
+        (ns, tn) = _qsplit(e.tag)
+        self.name = tn
+
+    def to_Element(self):
+        _typecheck(self.name, str)
+        outel = ET.Element(self.name)
+        if self.prec:
+            outel.attrib["prec"] = "%d%s" % self.prec
+        if self.time:
+            outel.text = str(self.time)
+        return outel
+
+    @property
+    def name(self):
+        """The type of timestamp - modified (mtime), accessed (atime), etc."""
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        if not value is None:
+            if not value in TimestampObject.timestamp_name_list:
+                raise ValueError("The timestamp name must be in this list: %r.  Received: %r." % (TimestampObject.timestamp_name_list, value))
+        self._name = value
+
+    @property
+    def prec(self):
+        """
+        A pair, (resolution, unit); unit is a second (s), millisecond, nanosecond, or day (d).  The default unit is "s".  Can be passed as a string or a duple.
+        """
+        return self._prec
+
+    @prec.setter
+    def prec(self, value):
+        if value is None:
+            self._prec = None
+            return self._prec
+        elif isinstance(value, tuple) and \
+          len(value) == 2 and \
+          isinstance(value[0], int) and \
+          isinstance(value[1], str):
+            self._prec = value
+            return self._prec
+
+        m = re_precision.match(value)
+        md = m.groupdict()
+        tup = (int(md["num"]), md.get("unit") or "s")
+        #_logger.debug("tup = %r" % (tup,))
+        self._prec = tup
+
+    @property
+    def time(self):
+        """
+        The actual timestamp.  A dfxml.dftime object.  This class might be superfluous and end up collapsing into that...
+        """
+        return self._time
+
+    @time.setter
+    def time(self, value):
+        if value is None:
+            self._time = None
+        else:
+            checked_value = dfxml.dftime(value)
+            #_logger.debug("checked_value.timestamp() = %r" % checked_value.timestamp())
+            self._time = checked_value
+            #Propagate timestamp value to other formats
+            self._timestamp = self._time.timestamp()
+
+    @property
+    def timestamp(self):
+        """A Unix floating-point timestamp, as time.mktime returns.  Currently, there is no setter for this property."""
+        return self._timestamp
+
+
+class FileObject(object):
+    """
+    This class provides property accesses, an XML serializer (ElementTree-based), and a deserializer.
+    The properties interface is NOT function calls, but simple accesses.  That is, the old _fileobject_ style:
+
+        assert isinstance(fi, dfxml.fileobject)
+        fi.mtime()
+
+    is now replaced with:
+
+        assert isinstance(fi, Objects.FileObject)
+        fi.mtime
+    """
+
+    _all_properties = set([
+      "alloc",
+      "alloc_inode",
+      "alloc_name",
+      "annos",
+      "atime",
+      "bkup_time",
+      "byte_runs",
+      "compressed",
+      "crtime",
+      "ctime",
+      "data_brs",
+      "dtime",
+      "error",
+      "externals",
+      "filename",
+      "filesize",
+      "gid",
+      "id",
+      "inode",
+      "inode_brs",
+      "link_target",
+      "libmagic",
+      "md5",
+      "meta_type",
+      "mode",
+      "mtime",
+      "name_brs",
+      "name_type",
+      "nlink",
+      "original_fileobject",
+      "orphan",
+      "parent_object",
+      "partition",
+      "seq",
+      "sha1",
+      "sha256",
+      "sha512",
+      "uid",
+      "unalloc",
+      "unused",
+      "used"
+    ])
+
+    _br_facet_to_property = {
+      "data":"data_brs",
+      "inode":"inode_brs",
+      "name":"name_brs"
+    }
+
+    #TODO There may be need in the future to compare the annotations as well.  It complicates make_differential_dfxml too much for now.
+    _incomparable_properties = set([
+      "annos",
+      "byte_runs",
+      "id",
+      "unalloc",
+      "unused"
+    ])
+
+    _diff_attr_names = {
+      "new":"delta:new_file",
+      "deleted":"delta:deleted_file",
+      "renamed":"delta:renamed_file",
+      "changed":"delta:changed_file",
+      "modified":"delta:modified_file",
+      "matched":"delta:matched"
+    }
+
+    def __init__(self, *args, **kwargs):
+        #Prime all the properties
+        for prop in FileObject._all_properties:
+            if prop == "annos":
+                continue
+            elif prop == "externals":
+                setattr(self, prop, kwargs.get(prop, OtherNSElementList()))
+            else:
+                setattr(self, prop, kwargs.get(prop))
+        self._annos = set()
+        self._diffs = set()
+
+    def __eq__(self, other):
+        if other is None:
+            return False
+        _typecheck(other, FileObject)
+        for prop in FileObject._all_properties:
+            if prop in FileObject._incomparable_properties:
+                continue
+            if getattr(self, prop) != getattr(other, prop):
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        parts = []
+
+        for prop in sorted(FileObject._all_properties):
+            #Save data byte runs for the end, as theirs lists can get really long.
+            if prop not in ["byte_runs", "data_brs"]:
+                value = getattr(self, prop)
+                if not value is None:
+                    parts.append("%s=%r" % (prop, value))
+
+        if self.data_brs:
+            parts.append("data_brs=%r" % self.byte_runs)
+
+        return "FileObject(" + ", ".join(parts) + ")"
+
+    def compare_to_original(self, **kwargs):
+        file_ignores = kwargs.get("file_ignores", set())
+        self._diffs = self.compare_to_other(self.original_fileobject, True, file_ignores)
+
+    def compare_to_other(self, other, ignore_original=False, file_ignores=set()):
+        _typecheck(other, FileObject)
+
+        diffs = set()
+
+        for propname in FileObject._all_properties:
+            if propname in file_ignores:
+                continue
+            if propname in FileObject._incomparable_properties:
+                continue
+            if ignore_original and propname == "original_fileobject":
+                continue
+            oval = getattr(other, propname)
+            sval = getattr(self, propname)
+            if oval is None and sval is None:
+                continue
+            if oval != sval:
+                #_logger.debug("propname, oval, sval: %r, %r, %r" % (propname, oval, sval))
+                diffs.add(propname)
+
+        return diffs
+
+    def extract_facet(self, facet, image_path=None, buffer_size=1048576, partition_offset=None, sector_size=512, errlog=None, statlog=None, icat_threshold = 268435456):
+        """
+        Generator.  Extracts the facet with a SleuthKit tool, yielding chunks of the data.
+
+        @param buffer_size The facet data is yielded in chunks of at most this parameter's size. Default 1MiB.
+        @param partition_offset The offset of the file's containing partition, in bytes.  Needed for icat.  If not given, the FileObject's VolumeObject will be used.  If that's also absent, icat can't be used, and img_cat will instead be tried as a fallback (which means byte runs must be in the DFXML).
+        @param icat_threshold icat incurs extensive, non-sequential IO overhead to walk the filesystem to reach the facet's byte runs.  img_cat can be called on each byte run reported in the DFXML file, but on fragmented files this incurs overhead in process spawning.  Facets larger than this threshold are extracted with icat.  Default 256MiB.  Force icat by setting this to -1; force img_cat with infinity (float("inf")).
+        """
+
+        _image_path = image_path
+        if _image_path is None:
+            raise ValueError("The backing image path must be supplied.")
+
+        _partition_offset = partition_offset
+        if _partition_offset is None:
+            if self.volume_object:
+                _partition_offset = self.volume_object.partition_offset
+
+        #Try using icat; needs inode number and volume offset.  We're additionally requiring the filesize be known.
+        #TODO The icat needs a little more experimentation.
+        if False and facet == "content" and \
+          not self.filesize is None and \
+          self.filesize >= icat_threshold and \
+          not self.inode is None and \
+          not _partition_offset is None:
+            _logger.debug("Extracting with icat: %r." % self)
+
+            #Set up logging if desired
+            stderr_fh = sys.stderr
+            if not errlog is None:
+                stderr_fh = open(errlog, "wb")
+
+            status_fh = None
+            if not statlog is None:
+                status_fh = open(errlog, "w")
+
+            #Set up icat process
+            cmd = ["icat"]
+            cmd.append("-b")
+            cmd.append(str(sector_size))
+            cmd.append("-o")
+            cmd.append(str(self.volume_object.partition_offset//sector_size))
+            if not self.volume_object.ftype_str is None:
+                cmd.append("-f")
+                cmd.append(self.volume_object.ftype_str)
+            cmd.append(image_path)
+            cmd.append(str(self.inode))
+            p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=stderr_fh)
+
+            #Do a buffered read
+            len_to_read = self.filesize
+            while len_to_read > 0:
+                buffer_data = p.stdout.read(buffer_size)
+                yield_data = buffer_data[ : min(len_to_read, buffer_size)]
+                if len(yield_data) > 0:
+                    yield yield_data
+                else:
+                    #Let the subprocess terminate so we can see the exit status
+                    p.wait()
+                    last_status = p.returncode
+
+                    #Log the status if requested
+                    if not status_fh is None:
+                        status_fh.write(last_status)
+
+                    #Act on a bad status
+                    if last_status != 0:
+                        raise subprocess.CalledProcessError(last_status, " ".join(cmd), "icat failed.")
+                len_to_read -= buffer_size
+
+            #Clean up file handles
+            if status_fh: status_fh.close()
+            if stderr_fh: stderr_fh.close()
+
+        elif not self.byte_runs is None:
+            for chunk in self.byte_runs.iter_contents(_image_path, buffer_size, sector_size, errlog, statlog):
+                yield chunk
+
+    def is_allocated(self):
+        """Collapse potentially-partial allocation information into a yes, no, or unknown answer."""
+        if self.alloc_inode == True and self.alloc_name == True:
+            return True
+        if self.alloc_inode is None and self.alloc_name is None:
+            if self.alloc is None:
+                return None
+            else:
+                return self.alloc
+        #Partial allocation information at this point is assumed False.  In some file systems, like FAT, we only need one of alloc_inode and alloc_name for allocation status.  Guidelines on which should win out haven't been set yet, though, so wait on this.
+        return False
+
+    def populate_from_Element(self, e):
+        """Populates this FileObject's properties from an ElementTree Element.  The Element need not be retained."""
+        global _warned_elements
+        _typecheck(e, (ET.Element, ET.ElementTree))
+
+        #_logger.debug("FileObject.populate_from_Element(%r)" % e)
+
+        #Split into namespace and tagname
+        (ns, tn) = _qsplit(e.tag)
+        assert tn in ["fileobject", "original_fileobject", "parent_object"]
+
+        #Map "delta:" attributes of <fileobject>s into the self.annos set
+        #_logger.debug("self.annos, before: %r." % self.annos)
+        _read_differential_annotations(FileObject._diff_attr_names, e, self.annos)
+        #_logger.debug("self.annos, after: %r." % self.annos)
+
+        #Look through direct-child elements for other properties
+        for ce in e.findall("./*"):
+            (cns, ctn) = _qsplit(ce.tag)
+            #_logger.debug("Populating from child element: %r." % ce.tag)
+
+            #Inherit any marked changes
+            for attr in ce.attrib:
+                #_logger.debug("Inspecting attr for diff. annos: %r." % attr)
+                (ns, an) = _qsplit(attr)
+                if an == "changed_property" and ns == dfxml.XMLNS_DELTA:
+                    #_logger.debug("Identified changed property: %r." % ctn)
+                    #TODO There may be a more elegant way of handling the hashes and any other attribute-dependent element-to-property mapping.  Probably involving XPath.
+                    if ctn == "hashdigest":
+                        if "type" not in ce.attrib:
+                            raise AttributeError("Attribute 'type' not found.  Every hashdigest element should have a 'type' attribute to identify the hash type.")
+                        self.diffs.add(ce.attrib["type"].lower())
+                    elif ctn == "byte_runs":
+                        facet = ce.attrib.get("facet")
+                        prop = FileObject._br_facet_to_property.get(facet, "data_brs")
+                        self.diffs.add(prop)
+                    else:
+                        self.diffs.add(ctn)
+
+            if ctn == "byte_runs":
+                #byte_runs might be for file contents, the inode/MFT entry, or the directory entry naming the file.  Use the facet attribute to determine which.  If facet is absent, assume they're data byte runs.
+                if "facet" in ce.attrib:
+                    if ce.attrib["facet"] not in FileObject._br_facet_to_property:
+                        if not ce.attrib["facet"] in _warned_byterun_facets:
+                            _warned_byterun_facets.add(ce.attrib["facet"])
+                            _logger.warning("byte_runs facet %r was unexpected.  Will not interpret this element.")
+                    else:
+                        brs = ByteRuns()
+                        brs.populate_from_Element(ce)
+                        brs.facet = ce.attrib["facet"]
+                        setattr(self, FileObject._br_facet_to_property[brs.facet], brs)
+                else:
+                    self.byte_runs = ByteRuns()
+                    self.byte_runs.populate_from_Element(ce)
+            elif ctn == "hashdigest":
+                if ce.attrib["type"].lower() == "md5":
+                    self.md5 = ce.text
+                elif ce.attrib["type"].lower() == "sha1":
+                    self.sha1 = ce.text
+                elif ce.attrib["type"].lower() == "sha256":
+                    self.sha256 = ce.text
+                elif ce.attrib["type"].lower() == "sha512":
+                    self.sha512 = ce.text
+            elif ctn == "original_fileobject":
+                self.original_fileobject = FileObject()
+                self.original_fileobject.populate_from_Element(ce)
+            elif ctn == "parent_object":
+                self.parent_object = FileObject()
+                self.parent_object.populate_from_Element(ce)
+            elif ctn in ["atime", "bkup_time", "crtime", "ctime", "dtime", "mtime"]:
+                setattr(self, ctn, TimestampObject())
+                getattr(self, ctn).populate_from_Element(ce)
+            elif ctn in FileObject._all_properties:
+                setattr(self, ctn, ce.text)
+            elif cns not in [dfxml.XMLNS_DFXML, ""]:
+                #Put all non-DFXML-namespace elements into the externals list.
+                self.externals.append(ce)
+            else:
+                if (cns, ctn) not in _warned_elements:
+                    _warned_elements.add((cns, ctn))
+                    _logger.warning("Uncertain what to do with this element: %r" % ce)
+
+    def populate_from_stat(self, s):
+        """Populates FileObject fields from a stat() call."""
+        import os
+        _typecheck(s, os.stat_result)
+
+        self.mode = s.st_mode
+        self.nlink = s.st_nlink
+        self.uid = s.st_uid
+        self.gid = s.st_gid
+        self.filesize = s.st_size
+        #s.st_dev is ignored for now.
+        if platform.system() == "Windows":
+            # On Windows, Python 2 reports 0L.  Treat this as absent information.
+            # On Windows, Python 3 reports the "File ID" ( see "nFileIndexLow" remark at: https://msdn.microsoft.com/en-us/library/aa363788 ).  Record this as the inode number for now.  NOTE: in the future this may become a Windows-namespaced property "fileindex"; it may be prudent to later file a follow-on to Python Issue 32878 ( https://bugs.python.org/issue32878 ).
+            if sys.version_info[0] >= 3:
+                self.inode = s.st_ino
+        else:
+            self.inode = s.st_ino
+
+        if "st_mtime" in dir(s):
+            self.mtime = s.st_mtime
+
+        if "st_atime" in dir(s):
+            self.atime = s.st_atime
+
+        if "st_ctime" in dir(s):
+            self.ctime = s.st_ctime
+
+        if "st_birthtime" in dir(s):
+            self.crtime = s.st_birthtime
+
+    def to_Element(self):
+        """Creates an ElementTree Element with elements in DFXML schema order."""
+        outel = ET.Element("fileobject")
+
+        annos_whittle_set = copy.deepcopy(self.annos)
+        diffs_whittle_set = copy.deepcopy(self.diffs)
+
+        for annodiff in FileObject._diff_attr_names:
+            if annodiff in annos_whittle_set:
+                outel.attrib[FileObject._diff_attr_names[annodiff]] = "1"
+                annos_whittle_set.remove(annodiff)
+        if len(annos_whittle_set) > 0:
+            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
+
+        def _anno_change(el):
+            if el.tag in self.diffs:
+                el.attrib["delta:changed_property"] = "1"
+                diffs_whittle_set.remove(el.tag)
+
+        def _anno_hash(el):
+            if el.attrib["type"] in self.diffs:
+                el.attrib["delta:changed_property"] = "1"
+                diffs_whittle_set.remove(el.attrib["type"])
+
+        def _anno_byte_runs(el):
+            if "facet" in el.attrib:
+                prop = FileObject._br_facet_to_property[el.attrib["facet"]]
+            else:
+                prop = "data_brs"
+            if prop in self.diffs:
+                el.attrib["delta:changed_property"] = "1"
+                #_logger.debug("diffs_whittle_set = %r." % diffs_whittle_set)
+                diffs_whittle_set.remove(prop)
+
+        #Recall that Element text must be a string
+        def _append_str(name, value):
+            """Note that empty elements should be created if the element was removed."""
+            if not value is None or name in diffs_whittle_set:
+                tmpel = ET.Element(name)
+                if not value is None:
+                    tmpel.text = str(value)
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        def _append_time(name, value):
+            """Note that empty elements should be created if the element was removed."""
+            if not value is None or name in diffs_whittle_set:
+                if not value is None and value.time:
+                    tmpel = value.to_Element()
+                else:
+                    tmpel = ET.Element(name)
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        def _append_bool(name, value):
+            """Note that empty elements should be created if the element was removed."""
+            if not value is None or name in diffs_whittle_set:
+                tmpel = ET.Element(name)
+                if not value is None:
+                    tmpel.text = str(1 if value else 0)
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        _using_facets = False
+        def _append_byte_runs(name, value):
+            """The complicated part here is setting the "data" facet on the byte runs, because we assume that no facet definitions means that for this file, there's only the one byte_runs list for data."""
+            #_logger.debug("_append_byte_runs(%r, %r)" % (name, value))
+            if value or name in diffs_whittle_set:
+                if value:
+                    tmpel = value.to_Element()
+                    if "facet" in tmpel.attrib:
+                        _using_facets = True
+                else:
+                    tmpel = ET.Element("byte_runs")
+                    propname_to_facet = {
+                      "data_brs": "data",
+                      "inode_brs": "inode",
+                      "name_brs": "name"
+                    }
+                    if name in propname_to_facet:
+                        _using_facets = True
+                        tmpel.attrib["facet"] = propname_to_facet[name]
+                    elif _using_facets:
+                        tmpel.attrib["facet"] = propname_to_facet["data_brs"]
+                _anno_byte_runs(tmpel)
+                outel.append(tmpel)
+
+        def _append_externals():
+            for e in self.externals:
+                outel.append(e)
+
+        def _append_object(name, value, namespace_prefix=None):
+            """name must be the name of a property that has a to_Element() method.  namespace_prefix will be prepended as-is to the element tag."""
+            obj = value
+            if obj or name in diffs_whittle_set:
+                if obj:
+                    tmpel = obj.to_Element()
+                else:
+                    tmpel = ET.Element(name)
+                #Set the tag name here for properties like parent_object, a FileObject without being wholly a FileObject.
+                if namespace_prefix:
+                    tmpel.tag = namespace_prefix + name
+                else:
+                    tmpel.tag = name
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        def _append_hash(name, value):
+            if not value is None or name in diffs_whittle_set:
+                tmpel = ET.Element("hashdigest")
+                tmpel.attrib["type"] = name
+                if not value is None:
+                    tmpel.text = value
+                _anno_hash(tmpel)
+                outel.append(tmpel)
+
+        #The parent object is a one-off.  Duplicating the whole parent is wasteful, so create a shadow object that just outputs the important bits.
+        if not self.parent_object is None:
+            parent_object_shadow = FileObject()
+            parent_object_shadow.inode = self.parent_object.inode
+            _append_object("parent_object", parent_object_shadow)
+
+        _append_str("filename", self.filename)
+        _append_str("error", self.error)
+        _append_str("partition", self.partition)
+        _append_str("id", self.id)
+        _append_str("name_type", self.name_type)
+        _append_str("filesize", self.filesize)
+        #TODO Define a better flag for if we're going to output <alloc> elements.
+        if self.alloc_name is None and self.alloc_inode is None:
+            _append_bool("alloc", self.alloc)
+        else:
+            _append_bool("alloc_inode", self.alloc_inode)
+            _append_bool("alloc_name", self.alloc_name)
+        _append_bool("used", self.used)
+        _append_bool("orphan", self.orphan)
+        _append_bool("compressed", self.compressed)
+        _append_str("inode", self.inode)
+        _append_str("meta_type", self.meta_type)
+        _append_str("mode", self.mode)
+        _append_str("nlink", self.nlink)
+        _append_str("uid", self.uid)
+        _append_str("gid", self.gid)
+        _append_time("mtime", self.mtime)
+        _append_time("ctime", self.ctime)
+        _append_time("atime", self.atime)
+        _append_time("crtime", self.crtime)
+        _append_str("seq", self.seq)
+        _append_time("dtime", self.dtime)
+        _append_time("bkup_time", self.bkup_time)
+        _append_str("link_target", self.link_target)
+        _append_str("libmagic", self.libmagic)
+        _append_externals()
+        _append_byte_runs("inode_brs", self.inode_brs)
+        _append_byte_runs("name_brs", self.name_brs)
+        _append_byte_runs("data_brs", self.data_brs)
+        _append_hash("md5", self.md5)
+        _append_hash("sha1", self.sha1)
+        _append_hash("sha256", self.sha256)
+        _append_hash("sha512", self.sha512)
+        _append_object("original_fileobject", self.original_fileobject, "delta:")
+
+        if len(diffs_whittle_set) > 0:
+            _logger.warning("Did not annotate all of the differing properties of this file.  Remaining properties:  %r." % diffs_whittle_set)
+
+        return outel
+
+    def to_dfxml(self):
+        return _ET_tostring(self.to_Element())
+
+    @property
+    def alloc(self):
+        """Note that setting .alloc will affect the value of .unalloc, and vice versa.  The last one to set wins."""
+        global _nagged_alloc
+        if not _nagged_alloc:
+            #alloc isn't deprecated yet.
+            #_logger.warning("The FileObject.alloc property is deprecated.  Use .alloc_inode and/or .alloc_name instead.  .alloc is proxied as True if alloc_inode and alloc_name are both True.")
+            _nagged_alloc = True
+        if self.alloc_inode and self.alloc_name:
+            return True
+        else:
+            return self._alloc
+
+    @alloc.setter
+    def alloc(self, val):
+        self._alloc = _boolcast(val)
+        if not self._alloc is None:
+            self._unalloc = not self._alloc
+
+    @property
+    def alloc_inode(self):
+        return self._alloc_inode
+
+    @alloc_inode.setter
+    def alloc_inode(self, val):
+        self._alloc_inode = _boolcast(val)
+
+    @property
+    def alloc_name(self):
+        return self._alloc_name
+
+    @alloc_name.setter
+    def alloc_name(self, val):
+        self._alloc_name = _boolcast(val)
+
+    @property
+    def annos(self):
+        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
+        return self._annos
+
+    @annos.setter
+    def annos(self, val):
+        _typecheck(val, set)
+        self._annos = val
+
+    @property
+    def atime(self):
+        return self._atime
+
+    @atime.setter
+    def atime(self, val):
+        if val is None:
+            self._atime = None
+        elif isinstance(val, TimestampObject):
+            self._atime = val
+        else:
+            checked_val = TimestampObject(val, name="atime")
+            self._atime = checked_val
+
+    @property
+    def bkup_time(self):
+        return self._bkup_time
+
+    @bkup_time.setter
+    def bkup_time(self, val):
+        if val is None:
+            self._bkup_time = None
+        elif isinstance(val, TimestampObject):
+            self._bkup_time = val
+        else:
+            checked_val = TimestampObject(val, name="bkup_time")
+            self._bkup_time = checked_val
+
+    @property
+    def byte_runs(self):
+        """This property is now a synonym for the data byte runs (.data_brs)."""
+        return self.data_brs
+
+    @byte_runs.setter
+    def byte_runs(self, val):
+        self.data_brs = val
+
+    @property
+    def compressed(self):
+        return self._compressed
+
+    @compressed.setter
+    def compressed(self, val):
+        self._compressed = _boolcast(val)
+
+    @property
+    def ctime(self):
+        return self._ctime
+
+    @ctime.setter
+    def ctime(self, val):
+        if val is None:
+            self._ctime = None
+        elif isinstance(val, TimestampObject):
+            self._ctime = val
+        else:
+            checked_val = TimestampObject(val, name="ctime")
+            self._ctime = checked_val
+
+    @property
+    def crtime(self):
+        return self._crtime
+
+    @crtime.setter
+    def crtime(self, val):
+        if val is None:
+            self._crtime = None
+        elif isinstance(val, TimestampObject):
+            self._crtime = val
+        else:
+            checked_val = TimestampObject(val, name="crtime")
+            self._crtime = checked_val
+
+    @property
+    def data_brs(self):
+        """The byte runs that store the file's content."""
+        return self._data_brs
+
+    @data_brs.setter
+    def data_brs(self, val):
+        if not val is None:
+            _typecheck(val, ByteRuns)
+        self._data_brs = val
+
+    @property
+    def diffs(self):
+        """This property intentionally has no setter.  To populate, call compare_to_original() after assigning an original_fileobject."""
+        return self._diffs
+
+    @property
+    def dtime(self):
+        return self._dtime
+
+    @dtime.setter
+    def dtime(self, val):
+        if val is None:
+            self._dtime = None
+        elif isinstance(val, TimestampObject):
+            self._dtime = val
+        else:
+            checked_val = TimestampObject(val, name="dtime")
+            self._dtime = checked_val
+
+    @property
+    def error(self):
+        return self._error
+
+    @error.setter
+    def error(self, val):
+        self._error = _strcast(val)
+
+    @property
+    def filename(self):
+        return self._filename
+
+    @filename.setter
+    def filename(self, val):
+        self._filename = _strcast(val)
+    @property
+    def externals(self):
+        """
+        This property exposes XML elements of other namespaces.  Since these elements can be of arbitrary complexity, this list is solely comprised ofxml.etree.ElementTree.Element objects.  The tags must be a fully-qualified namespace (of the pattern {URI}localname).  If generating the Elements with a script instead of de-serializing from XML, you should issue an ElementTree register_namespace call with your namespace abbreviation prefix.
+        NOTE:  Diffs are currently NOT computed for external elements.
+        NOTE:  This property should be considered unstable, as the interface is in an early design phase.  Please notify the maintainers of this library (see the Git history for the Objects.py file) if you are using this interface and wish to be notified of updates."""
+        return self._externals
+
+    @externals.setter
+    def externals(self, val):
+        _typecheck(val, OtherNSElementList)
+        self._externals = val
+
+    @property
+    def filesize(self):
+        return self._filesize
+
+    @filesize.setter
+    def filesize(self, val):
+        self._filesize = _intcast(val)
+
+    @property
+    def gid(self):
+        return self._gid
+
+    @gid.setter
+    def gid(self, val):
+        self._gid = _strcast(val)
+
+    @property
+    def id(self):
+        return self._id
+
+    @id.setter
+    def id(self, val):
+        self._id = _intcast(val)
+
+    @property
+    def inode(self):
+        return self._inode
+
+    @inode.setter
+    def inode(self, val):
+        self._inode = _intcast(val)
+
+    @property
+    def libmagic(self):
+        return self._libmagic
+
+    @libmagic.setter
+    def libmagic(self, val):
+        self._libmagic = _strcast(val)
+
+    @property
+    def inode_brs(self):
+        """The byte run(s) that represents the file's metadata object (the inode or the MFT entry).  In file systems that do not distinguish between inode and directory entry, e.g. FAT, .inode_brs should be equivalent to .name_brs, if both fields are present."""
+        return self._inode_brs
+
+    @inode_brs.setter
+    def inode_brs(self, val):
+        if not val is None:
+            _typecheck(val, ByteRuns)
+        self._inode_brs = val
+
+    @property
+    def md5(self):
+        return self._md5
+
+    @md5.setter
+    def md5(self, val):
+        self._md5 = _strcast(val)
+
+    @property
+    def meta_type(self):
+        return self._meta_type
+
+    @meta_type.setter
+    def meta_type(self, val):
+        self._meta_type = _intcast(val)
+
+    @property
+    def mode(self):
+        """The security mode is represented in the FileObject as a base-10 integer.  It is also serialized as a decimal integer."""
+        return self._mode
+
+    @mode.setter
+    def mode(self, val):
+        self._mode = _intcast(val)
+
+    @property
+    def mtime(self):
+        return self._mtime
+
+    @mtime.setter
+    def mtime(self, val):
+        if val is None:
+            self._mtime = None
+        elif isinstance(val, TimestampObject):
+            self._mtime = val
+        else:
+            checked_val = TimestampObject(val, name="mtime")
+            self._mtime = checked_val
+
+    @property
+    def name_brs(self):
+        """The byte run(s) that represents the file's name object (the directory entry).  In file systems that do not distinguish between inode and directory entry, e.g. FAT, .inode_brs should be equivalent to .name_brs, if both fields are present."""
+        return self._name_brs
+
+    @name_brs.setter
+    def name_brs(self, val):
+        if not val is None:
+            _typecheck(val, ByteRuns)
+        self._name_brs = val
+
+    @property
+    def name_type(self):
+        return self._name_type
+
+    @name_type.setter
+    def name_type(self, val):
+        if val is None:
+            self._name_type = val
+        else:
+            cast_val = _strcast(val)
+            if cast_val not in ["-", "V", "b", "c", "d", "h", "l", "p", "r", "s", "v", "w"]:
+                raise ValueError("Unexpected name_type received: %r (casted to %r)." % (val, cast_val))
+            self._name_type = cast_val
+
+    @property
+    def nlink(self):
+        return self._nlink
+
+    @nlink.setter
+    def nlink(self, val):
+        self._nlink = _intcast(val)
+
+    @property
+    def orphan(self):
+        return self._orphan
+
+    @orphan.setter
+    def orphan(self, val):
+        self._orphan = _boolcast(val)
+
+    @property
+    def original_fileobject(self):
+        return self._original_fileobject
+
+    @original_fileobject.setter
+    def original_fileobject(self, val):
+        if not val is None:
+            _typecheck(val, FileObject)
+        self._original_fileobject = val
+
+    @property
+    def partition(self):
+        return self._partition
+
+    @partition.setter
+    def partition(self, val):
+        self._partition = _intcast(val)
+
+    @property
+    def parent_object(self):
+        """This object is an extremely sparse FileObject, containing just identifying information.  Alternately, it can be an entire object reference to the parent Object, though uniqueness should be checked."""
+        return self._parent_object
+
+    @parent_object.setter
+    def parent_object(self, val):
+        if not val is None:
+            _typecheck(val, FileObject)
+        self._parent_object = val
+
+    @property
+    def seq(self):
+        return self._seq
+
+    @seq.setter
+    def seq(self, val):
+        self._seq = _intcast(val)
+
+    @property
+    def sha1(self):
+        return self._sha1
+
+    @sha1.setter
+    def sha1(self, val):
+        self._sha1 = _strcast(val)
+
+    @property
+    def sha256(self):
+        return self._sha256
+
+    @sha256.setter
+    def sha256(self, val):
+        self._sha256 = _strcast(val)
+    
+    @property
+    def sha512(self):
+        return self._sha512
+        
+    @sha512.setter
+    def sha512(self, val):
+        self._sha512 = _strcast(val)
+
+    @property
+    def uid(self):
+        return self._uid
+
+    @uid.setter
+    def uid(self, val):
+        self._uid = _strcast(val)
+
+    @property
+    def unalloc(self):
+        """Note that setting .unalloc will affect the value of .alloc, and vice versa.  The last one to set wins."""
+        return self._unalloc
+
+    @unalloc.setter
+    def unalloc(self, val):
+        self._unalloc = _boolcast(val)
+        if not self._unalloc is None:
+            self._alloc = not self._unalloc
+
+    @property
+    def unused(self):
+        return self._used
+
+    @unused.setter
+    def unused(self, val):
+        self._unused = _intcast(val)
+        if not self._unused is None:
+            self._used = not self._unused
+
+    @property
+    def used(self):
+        return self._used
+
+    @used.setter
+    def used(self, val):
+        self._used = _intcast(val)
+        if not self._used is None:
+            self._unused = not self._used
+
+    @property
+    def volume_object(self):
+        """Reference to the containing volume object.  Not meant to be propagated with __repr__ or to_Element()."""
+        return self._volume_object
+
+    @volume_object.setter
+    def volume_object(self, val):
+        if not val is None:
+            _typecheck(val, VolumeObject)
+        self._volume_object = val
+
+class OtherNSElementList(list):
+    #Note that super() must be called with arguments to work in Python 2.
+
+    @classmethod
+    def _check_qname(cls, tagname):
+        (ns, ln) = _qsplit(tagname)
+        if ns == dfxml.XMLNS_DFXML:
+            raise ValueError("'External' elements must be a non-DFXML namespace.")
+        #Register qname for later output
+        #TODO Devise a module-level interface for namespace abreviations.
+
+    def __repr__(self):
+        #Unwrap the string representation of this class's type name (necessary because we don't necessarily know if it'll be Objects.Other... or just Other...).
+        _typestr = str(type(self))[ len("<class '") : -len("'>") ]
+        return _typestr + "(" + super(OtherNSElementList, self).__repr__() + ")"
+
+    def __setitem__(self, idx, value):
+        _typecheck(value, ET.Element)
+        OtherNSElementList._check_qname(value.tag)
+        super(OtherNSElementList, self).__setitem__(idx, value)
+
+    def append(self, value):
+        _typecheck(value, ET.Element)
+        OtherNSElementList._check_qname(value.tag)
+        super(OtherNSElementList, self).append(value)
+
+class CellObject(object):
+
+    _all_properties = set([
+      "alloc",
+      "annos",
+      "basename",
+      "byte_runs",
+      "cellpath",
+      "data",
+      "data_conversions",
+      "data_encoding",
+      "data_type",
+      "error",
+      "mtime",
+      "name_type",
+      "original_cellobject",
+      "parent_object",
+      "root"
+    ])
+
+    _diff_attr_names = {
+      "new":"delta:new_cell",
+      "deleted":"delta:deleted_cell",
+      "changed":"delta:changed_cell",
+      "modified":"delta:modified_cell",
+      "matched":"delta:matched"
+    }
+
+    #TODO There may be need in the future to compare the annotations as well.
+    _incomparable_properties = set([
+      "annos"
+    ])
+
+    def __init__(self, *args, **kwargs):
+        #These properties must be assigned first for sanity check dependencies
+        self.name_type = kwargs.get("name_type")
+
+        for prop in CellObject._all_properties:
+            if prop == "annos":
+                setattr(self, prop, kwargs.get(prop, set()))
+            else:
+                setattr(self, prop, kwargs.get(prop))
+
+        self._diffs = set()
+
+    def __eq__(self, other):
+        if other is None:
+            return False
+        _typecheck(other, CellObject)
+        for prop in CellObject._all_properties:
+            if prop in CellObject._incomparable_properties:
+                continue
+            if getattr(self, prop) != getattr(other, prop):
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        parts = []
+
+        for prop in sorted(list(CellObject._all_properties)):
+            if not getattr(self, prop) is None:
+                parts.append("%s=%r" % (prop, getattr(self, prop)))
+
+        return "CellObject(" + ", ".join(parts) + ")"
+
+    def compare_to_original(self):
+        self._diffs = self.compare_to_other(self.original_cellobject, True)
+
+    def compare_to_other(self, other, ignore_original=False):
+        _typecheck(other, CellObject)
+
+        diffs = set()
+
+        for propname in CellObject._all_properties:
+            if propname in CellObject._incomparable_properties:
+                continue
+            if ignore_original and propname == "original_cellobject":
+                continue
+            oval = getattr(other, propname)
+            sval = getattr(self, propname)
+            if oval is None and sval is None:
+                continue
+            if oval != sval:
+                #_logger.debug("propname, oval, sval: %r, %r, %r" % (propname, oval, sval))
+                diffs.add(propname)
+
+        return diffs
+
+    def populate_from_Element(self, e):
+        """Populates this CellObject's properties from an ElementTree Element.  The Element need not be retained."""
+        global _warned_elements
+        _typecheck(e, (ET.Element, ET.ElementTree))
+
+        _read_differential_annotations(CellObject._diff_attr_names, e, self.annos)
+
+        #Split into namespace and tagname
+        (ns, tn) = _qsplit(e.tag)
+        assert tn in ["cellobject", "original_cellobject", "parent_object"]
+
+        if e.attrib.get("root"):
+            self.root = e.attrib["root"]
+
+        #Look through direct-child elements for other properties
+        for ce in e.findall("./*"):
+            (cns, ctn) = _qsplit(ce.tag)
+            if ctn == "alloc":
+                self.alloc = ce.text
+            elif ctn == "basename":
+                self.basename = ce.text
+            elif ctn == "byte_runs":
+                self.byte_runs = ByteRuns()
+                self.byte_runs.populate_from_Element(ce)
+            elif ctn == "cellpath":
+                self.cellpath = ce.text
+            elif ctn == "data":
+                self.data = ce.text
+                if ce.attrib.get("encoding"):
+                    self.data_encoding = ce.attrib["encoding"]
+            elif ctn == "data_conversions":
+                self.data_conversions = dict()
+                for cce in ce:
+                    if cce.tag == "int":
+                        self.data_conversions["int"] = int()
+                    elif cce.tag == "string":
+                        self.data_conversions["string"] = cce.text
+                    elif cce.tag == "string_list":
+                        self.data_conversions["string_list"] = []
+                        for ccce in cce:
+                            self.data_conversions["string_list"].append(ccce.text)
+            elif ctn == "data_type":
+                self.data_type = ce.text
+            elif ctn == "error":
+                self.error = ce.text
+            elif ctn == "mtime":
+                self.mtime = TimestampObject()
+                self.mtime.populate_from_Element(ce)
+            elif ctn == "name_type":
+                self.name_type = ce.text
+            elif ctn == "original_cellobject":
+                self.original_cellobject = CellObject()
+                self.original_cellobject.populate_from_Element(ce)
+            elif ctn == "parent_object":
+                self.parent_object = CellObject()
+                self.parent_object.populate_from_Element(ce)
+            else:
+                if (cns, ctn) not in _warned_elements:
+                    _warned_elements.add((cns, ctn))
+                    _logger.warning("Uncertain what to do with this element: %r" % ce)
+
+        self.sanity_check()
+
+    def sanity_check(self):
+        if self.name_type and self.name_type != "k":
+            if self.mtime:
+                _logger.info("Error occurred sanity-checking this CellObject: %r." % self)
+                raise ValueError("A Registry Key (node) is the only kind of CellObject that can have a timestamp.")
+            if self.root:
+                _logger.info("Error occurred sanity-checking this CellObject: %r." % self)
+                raise ValueError("A Registry Key (node) is the only kind of CellObject that can have the 'root' attribute.")
+
+    def to_Element(self):
+        self.sanity_check()
+
+        outel = ET.Element("cellobject")
+
+        annos_whittle_set = copy.deepcopy(self.annos)
+        diffs_whittle_set = copy.deepcopy(self.diffs)
+
+        for annodiff in CellObject._diff_attr_names:
+            if annodiff in annos_whittle_set:
+                outel.attrib[CellObject._diff_attr_names[annodiff]] = "1"
+                annos_whittle_set.remove(annodiff)
+        if len(annos_whittle_set) > 0:
+            _logger.warning("Failed to export some differential annotations: %r." % annos_whittle_set)
+
+        def _anno_change(el):
+            if el.tag in self.diffs:
+                el.attrib["delta:changed_property"] = "1"
+                diffs_whittle_set.remove(el.tag)
+            #Do an additional check for data_encoding, which is serialized as an attribute.
+            if el.tag == "data" and "data_encoding" in self.diffs:
+                el.attrib["delta:changed_property"] = "1"
+                diffs_whittle_set.remove("data_encoding")
+
+        def _append_bool(name, value):
+            if not value is None or name in diffs_whittle_set:
+                tmpel = ET.Element(name)
+                if not value is None:
+                    tmpel.text = "1" if value else "0"
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        #Recall that Element text must be a string
+        def _append_str(name, value):
+            if not value is None or name in diffs_whittle_set:
+                tmpel = ET.Element(name)
+                if not value is None:
+                    tmpel.text = str(value)
+                _anno_change(tmpel)
+
+                if name == "data" and not self.data_encoding is None:
+                    tmpel.attrib["encoding"] = self.data_encoding
+
+                outel.append(tmpel)
+
+        def _append_object(name, value):
+            if not value is None or name in diffs_whittle_set:
+                if value is None:
+                    tmpel = ET.Element(name)
+                else:
+                    tmpel = value.to_Element()
+                _anno_change(tmpel)
+                outel.append(tmpel)
+
+        #TODO root should be an element too.  Revise schema.
+        if self.root:
+            outel.attrib["root"] = str(self.root)
+
+        _append_str("cellpath", self.cellpath)
+        _append_str("basename", self.basename)
+        _append_str("error", self.error)
+        _append_str("name_type", self.name_type)
+        _append_bool("alloc", self.alloc)
+        _append_object("mtime", self.mtime)
+        _append_str("data_type", self.data_type)
+        _append_str("data", self.data)
+
+        #The experimental conversions element needs its own code
+        if not self.data_conversions is None or "data_conversions" in diffs_whittle_set:
+            tmpel = ET.Element("data_conversions")
+            if not self.data_conversions is None:
+                if "int" in self.data_conversions:
+                    tmpcel = ET.Element("int")
+                    tmpcel.text = str(self.data_conversions["int"])
+                    tmpel.append(tmpcel)
+                if "string" in self.data_conversions:
+                    tmpcel = ET.Element("string")
+                    tmpcel.text = str(self.data_conversions["string"])
+                    tmpel.append(tmpcel)
+                if "string_list" in self.data_conversions:
+                    tmpcel = ET.Element("string_list")
+                    for s in self.data_conversions["string"]:
+                        tmpccel = ET.Element("string")
+                        tmpccel.text = s
+                        tmpcel.append(tmpccel)
+                    tmpel.append(tmpcel)
+
+            _anno_change(tmpel)
+            outel.append(tmpel)
+
+        _append_object("byte_runs", self.byte_runs)
+        _append_object("original_cellobject", self.original_cellobject)
+
+        if len(diffs_whittle_set) > 0:
+            _logger.warning("Did not annotate all of the differing properties of this file.  Remaining properties:  %r." % diffs_whittle_set)
+
+        return outel
+
+    def to_regxml(self):
+        return _ET_tostring(self.to_Element())
+
+    @property
+    def alloc(self):
+        return self._alloc
+
+    @alloc.setter
+    def alloc(self, val):
+        self._alloc = _boolcast(val)
+
+    @property
+    def annos(self):
+        """Set of differential annotations.  Expected members are the keys of this class's _diff_attr_names dictionary."""
+        return self._annos
+
+    @annos.setter
+    def annos(self, val):
+        _typecheck(val, set)
+        self._annos = val
+
+    @property
+    def basename(self):
+        return self._basename
+
+    @basename.setter
+    def basename(self, val):
+        if not val is None:
+            _typecheck(val, str)
+        self._basename = val
+
+    @property
+    def byte_runs(self):
+        return self._byte_runs
+
+    @byte_runs.setter
+    def byte_runs(self, val):
+        if not val is None:
+            _typecheck(val, ByteRuns)
+        self._byte_runs = val
+
+    @property
+    def cellpath(self):
+        return self._cellpath
+
+    @cellpath.setter
+    def cellpath(self, val):
+        if not val is None:
+            _typecheck(val, str)
+        self._cellpath = val
+
+    @property
+    def data(self):
+        """Expecting a base64-encoded string.  See conversions (according to the Hive parser's library) in data_conversions property."""
+        return self._data
+
+    @data.setter
+    def data(self, val):
+        if not val is None:
+            _typecheck(val, str)
+        self._data = val
+
+    @property
+    def data_conversions(self):
+        return self._data_conversions
+
+    @data_conversions.setter
+    def data_conversions(self, val):
+        if not val is None:
+            _typecheck(val, dict)
+        self._data_conversions = val
+
+    @property
+    def data_encoding(self):
+        """Expecting a string, typically 'base64'."""
+        return self._data_encoding
+
+    @data_encoding.setter
+    def data_encoding(self, val):
+        if not val is None:
+            _typecheck(val, str)
+        self._data_encoding = val
+
+    @property
+    def data_type(self):
+        """Expecting a string, e.g. "REG_MULTI_SZ", or an int, because value type is known to be overloaded as an integer storage field in some cells."""
+        return self._data_type
+
+    @data_type.setter
+    def data_type(self, val):
+        if not val in [
+          None,
+          "REG_NONE",
+          "REG_SZ",
+          "REG_EXPAND_SZ",
+          "REG_BINARY",
+          "REG_DWORD",
+          "REG_DWORD_BIG_ENDIAN",
+          "REG_LINK",
+          "REG_MULTI_SZ",
+          "REG_RESOURCE_LIST",
+          "REG_FULL_RESOURCE_DESCRIPTOR",
+          "REG_RESOURCE_REQUIREMENTS_LIST",
+          "REG_QWORD"
+        ]:
+            if not isinstance(val, int) or (isinstance(val, str) and val.isdigit()):
+                raise ValueError("Unexpected value data type received: %r, type %r." % (val, type(val)))
+        self._data_type = val
+
+    @property
+    def diffs(self):
+        return self._diffs
+
+    @diffs.setter
+    def diffs(self, value):
+        _typecheck(value, set)
+        self._diffs = value
+
+    @property
+    def error(self):
+        return self._error
+
+    @error.setter
+    def error(self, value):
+        if not value is None:
+            _typecheck(value, str)
+        self._error = value
+
+    @property
+    def hive_object(self):
+        """Reference to the containing hive object.  Not meant to be propagated with __repr__ or to_Element()."""
+        return self._hive_object
+
+    @hive_object.setter
+    def hive_object(self, val):
+        if not val is None:
+            _typecheck(val, HiveObject)
+        self._hive_object = val
+
+    @property
+    def mtime(self):
+        return self._mtime
+
+    @mtime.setter
+    def mtime(self, val):
+        if val is None:
+            self._mtime = None
+        elif isinstance(val, TimestampObject):
+            self._mtime = val
+        else:
+            self._mtime = TimestampObject(val, name="mtime")
+            self.sanity_check()
+
+    @property
+    def name_type(self):
+        return self._name_type
+
+    @name_type.setter
+    def name_type(self, val):
+        if not val is None:
+            assert val in ["k", "v"]
+        self._name_type = val
+
+    @property
+    def original_cellobject(self):
+        return self._original_cellobject
+
+    @original_cellobject.setter
+    def original_cellobject(self, val):
+        if not val is None:
+            _typecheck(val, CellObject)
+        self._original_cellobject = val
+
+    @property
+    def parent_object(self):
+        """This object is an extremely sparse CellObject, containing just identifying information.  Alternately, it can be an entire object reference to the parent Object, though uniqueness should be checked."""
+        return self._parent_object
+
+    @parent_object.setter
+    def parent_object(self, val):
+        if not val is None:
+            _typecheck(val, CellObject)
+        self._parent_object = val
+
+    @property
+    def root(self):
+        return self._root
+
+    @root.setter
+    def root(self, val):
+        self._root = _boolcast(val)
+
+
+def iterparse(filename, events=("start","end"), **kwargs):
+    """
+    Generator.  Yields a stream of populated DFXMLObjects, VolumeObjects and FileObjects, paired with an event type ("start" or "end").  The DFXMLObject and VolumeObjects do NOT have their child lists populated with this method - that is left to the calling program.
+
+    The event type interface is meant to match the interface of ElementTree's iterparse; this is simply for familiarity's sake.  DFXMLObjects and VolumeObjects are yielded with "start" when the stream of VolumeObject or FileObjects begins - that is, they are yielded after being fully constructed up to the potentially-lengthy child object stream.  FileObjects are yielded only with "end".
+
+    @param filename: A string
+    @param events: Events.  Optional.  A tuple of strings, containing "start" and/or "end".
+    @param dfxmlobject: A DFXMLObject document.  Optional.  A DFXMLObject is created and yielded in the object stream if this argument is not supplied.
+    @param fiwalk: Optional.  Path to a particular fiwalk build you want to run.
+    """
+
+    #The DFXML stream file handle.
+    fh = None
+    subp = None
+    fiwalk_path = kwargs.get("fiwalk", "fiwalk")
+    subp_command = [fiwalk_path, "-x", filename]
+    if filename.endswith("xml"):
+        fh = open(filename, "rb")
+    else:
+        subp = subprocess.Popen(subp_command, stdout=subprocess.PIPE)
+        fh = subp.stdout
+
+    _events = set()
+    for e in events:
+        if not e in ("start","end"):
+            raise ValueError("Unexpected event type: %r.  Expecting 'start', 'end'." % e)
+        _events.add(e)
+
+    dobj = kwargs.get("dfxmlobject", DFXMLObject())
+
+    #The only way to efficiently populate VolumeObjects is to populate the object when the stream has hit its first FileObject.
+    vobj = None
+
+    #It doesn't seem ElementTree allows fetching parents of Elements that are incomplete (just hit the "start" event).  So, build a volume Element when we've hit "<volume ... >", glomming all elements until the first fileobject is hit.
+    #Likewise with the Element for the DFXMLObject.
+    dfxml_proxy = None
+    volume_proxy = None
+
+    #State machine, used to track when the first fileobject of a volume is encountered.
+    READING_START = 0
+    READING_PRESTREAM = 1 #DFXML metadata, pre-Object stream
+    READING_VOLUMES = 2
+    READING_FILES = 3
+    READING_POSTSTREAM = 4 #DFXML metadata, post-Object stream (typically the <rusage> element)
+    _state = READING_START
+
+    for (ETevent, elem) in ET.iterparse(fh, events=("start-ns", "start", "end")):
+        #View the object event stream in debug mode
+        #_logger.debug("(event, elem) = (%r, %r)" % (ETevent, elem))
+        #if ETevent in ("start", "end"):
+        #    _logger.debug("_ET_tostring(elem) = %r" % _ET_tostring(elem))
+
+        #Track namespaces
+        if ETevent == "start-ns":
+            dobj.add_namespace(*elem)
+            ET.register_namespace(*elem)
+            continue
+
+        #Split tag name into namespace and local name
+        (ns, ln) = _qsplit(elem.tag)
+
+        if ETevent == "start":
+            if ln == "dfxml":
+                if _state != READING_START:
+                    raise ValueError("Encountered a <dfxml> element, but the parser isn't in its start state.  Recursive <dfxml> declarations aren't supported at this time.")
+                dfxml_proxy = ET.Element(elem.tag)
+                for k in elem.attrib:
+                    #Note that xmlns declarations don't appear in elem.attrib.
+                    dfxml_proxy.attrib[k] = elem.attrib[k]
+                _state = READING_PRESTREAM
+            elif ln == "volume":
+                if _state == READING_PRESTREAM:
+                    #Cut; yield DFXMLObject now.
+                    dobj.populate_from_Element(dfxml_proxy)
+                    if "start" in _events:
+                        yield ("start", dobj)
+                #Start populating a new Volume proxy.
+                volume_proxy = ET.Element(elem.tag)
+                for k in elem.attrib:
+                    volume_proxy.attrib[k] = elem.attrib[k]
+                _state = READING_VOLUMES
+            elif ln == "fileobject":
+                if _state == READING_PRESTREAM:
+                    #Cut; yield DFXMLObject now.
+                    dobj.populate_from_Element(dfxml_proxy)
+                    if "start" in _events:
+                        yield ("start", dobj)
+                elif _state == READING_VOLUMES:
+                    #_logger.debug("Encountered a fileobject while reading volume properties.  Yielding volume now.")
+                    #Cut; yield VolumeObject now.
+                    if volume_proxy is not None:
+                        vobj = VolumeObject()
+                        vobj.populate_from_Element(volume_proxy)
+                        if "start" in _events:
+                            yield ("start", vobj)
+                        #Reset
+                        volume_proxy.clear()
+                        volume_proxy = None
+                _state = READING_FILES
+        elif ETevent == "end":
+            if ln == "fileobject":
+                if _state in (READING_PRESTREAM, READING_POSTSTREAM):
+                    #This particular branch can be reached if there are trailing fileobject elements after the volume element.  This would happen if a tool needed to represent files (likely reassembled fragments) found outside all the partitions.
+                    #More frequently, we hit this point when there are no volume groupings.
+                    vobj = None
+                fi = FileObject()
+                fi.populate_from_Element(elem)
+                fi.volume_object = vobj
+                #_logger.debug("fi = %r" % fi)
+                if "end" in _events:
+                    yield ("end", fi)
+                #Reset
+                elem.clear()
+            elif ln == "dfxml":
+                if "end" in _events:
+                    #_logger.debug("end, dfxml, _state=%r" % _state)
+                    if _state == READING_PRESTREAM:
+                        #This DFXML document contains no volumes or files, but may contain other metadata.  Populate (which would normally be done before starting a child Object stream) and yield.
+                        dobj.populate_from_Element(dfxml_proxy)
+                        yield ("end", dobj)
+            elif ln == "volume":
+                if _state == READING_VOLUMES:
+                    #Create and yield VolumeObject now (because there were no file objects to trigger it in the "start" ElementTree events branch above)
+                    vobj = VolumeObject()
+                    vobj.populate_from_Element(volume_proxy)
+                    if "start" in _events:
+                        yield ("start", vobj)
+                if "end" in _events:
+                    yield ("end", vobj)
+                _state = READING_POSTSTREAM
+            elif _state == READING_VOLUMES:
+                #This is a volume property; glom onto the proxy.
+                if volume_proxy is not None:
+                    volume_proxy.append(elem)
+            elif _state == READING_PRESTREAM:
+                if ln in ["metadata", "creator", "source"] or ns != dfxml.XMLNS_DFXML:
+                    #This is a direct child of the DFXML document property; glom onto the proxy.
+                    if dfxml_proxy is not None:
+                        dfxml_proxy.append(elem)
+
+    #If we called Fiwalk, double-check that it exited successfully.
+    if not subp is None:
+        _logger.debug("Calling wait() to let the Fiwalk subprocess terminate...") #Just reading from subp.stdout doesn't let the process terminate; it only finishes working.
+        subp.wait()
+        if subp.returncode != 0:
+            e = subprocess.CalledProcessError("There was an error running Fiwalk.")
+            e.returncode = subp.returncode
+            e.cmd = subp_command
+            raise e
+        _logger.debug("...Done.")
+
+def parse(filename):
+    """Returns a DFXMLObject populated from the contents of the (string) filename argument."""
+    retval = None
+    appender = None
+    for (event, obj) in iterparse(filename):
+        if event == "start":
+            if isinstance(obj, DFXMLObject):
+                retval = obj
+                appender = obj
+            elif isinstance(obj, VolumeObject):
+                retval.append(obj)
+                appender = obj
+        elif event == "end":
+            if isinstance(obj, DFXMLObject):
+                if retval is None:
+                    retval = obj
+                appender = obj
+            if isinstance(obj, VolumeObject):
+                appender = retval
+            elif isinstance(obj, FileObject):
+                appender.append(obj)
+    return retval
+
+if __name__ == "__main__":
+    import argparse
+    parser = argparse.ArgumentParser()
+
+    logging.basicConfig(level=logging.DEBUG)
+    #Run unit tests
+
+    assert _intcast(-1) == -1
+    assert _intcast("-1") == -1
+    assert _qsplit("{http://www.w3.org/2001/XMLSchema}all") == ("http://www.w3.org/2001/XMLSchema","all")
+    assert _qsplit("http://www.w3.org/2001/XMLSchema}all") == (None, "http://www.w3.org/2001/XMLSchema}all")
+
+
+    fi = FileObject()
+
+    #Check property setting
+    fi.mtime = "1999-12-31T23:59:59Z"
+    _logger.debug("fi = %r" % fi)
+
+    #Check bad property setting
+    failed = None
+    try:
+        fi.mtime = "Not a timestamp"
+        failed = False
+    except:
+        failed = True
+    _logger.debug("fi = %r" % fi)
+    _logger.debug("failed = %r" % failed)
+    assert failed
+
+    t0 = TimestampObject(prec="100ns", name="mtime")
+    _logger.debug("t0 = %r" % t0)
+    assert t0.prec[0] == 100
+    assert t0.prec[1] == "ns"
+    t1 = TimestampObject("2009-01-23T01:23:45Z", prec="2", name="atime")
+    _logger.debug("t1 = %r" % t1)
+    assert t1.prec[0] == 2
+    assert t1.prec[1] == "s"
+
+    print("Unit tests passed.")
```

### Comparing `ifiscripts-2023.7.3.1/scripts/accession_register.py` & `ifiscripts-2023.7.3.2/scripts/accession_register.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/aipcreator.py` & `ifiscripts-2023.7.3.2/scripts/aipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/as11fixity.py` & `ifiscripts-2023.7.3.2/scripts/as11fixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/batchaipcreator.py` & `ifiscripts-2023.7.3.2/scripts/batchaipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/batchdiff_framemd5.py` & `ifiscripts-2023.7.3.2/scripts/batchdiff_framemd5.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/batchmakeshell.py` & `ifiscripts-2023.7.3.2/scripts/batchmakeshell.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/batchsipcreator.py` & `ifiscripts-2023.7.3.2/scripts/batchsipcreator.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-#!/usr/bin/env python3
-'''
-Allow sipcreator to batch process multiple folders in a directory
--dcp option is needed to process folders and grab html files
-'''
-import argparse
-import os
-import sys
-import ififuncs
-import sipcreator
-from masscopy import analyze_log
-
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Launches sipcreator.py on multiple objects.'
-        'Wraps objects into an Irish Film Institute SIP'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        '-i',
-        help='full path of input folder - this folder should contain subfolders which in turn contain video files', required=True
-    )
-    parser.add_argument(
-        '-o', '-output',
-        help='full path of output directory', required=True
-    )
-    parser.add_argument(
-        '-rename_uuid', action='store_true',
-        help='Use with caution! This will rename an object with a randonly generated UUID'
-    )
-    parser.add_argument(
-        '-user',
-        help='Declare who you are. If this is not set, you will be prompted.'
-    )
-    parser.add_argument(
-        '-l', action='store_true',
-        help='invokes the -lto argument in copyit.py - uses gcp instead of rsync.'
-    )
-    parser.add_argument(
-        '-d', '-dcp', action='store_true',
-        help='Adds DCP specific processing, like creating objects subfolder with text extracted from <ContentTitleText> in the CPL.'
-    )
-    parser.add_argument(
-        '-zip', action='store_true',
-        help='Uses makezip.py to store the objects in an uncompressed ZIP'
-    )
-    parser.add_argument(
-        '-oe',
-        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
-    )
-    parser.add_argument(
-        '-supplement_extension_pattern', nargs='+',
-        help='Enter the filename extensions, seperated by spaces, which determine which files to be added to the supplemental subfolder within the metadata directory. For example -supplement_extension_pattern xml pdf txt docx will take all filenames with these extensions within your input directory and store them in metadata/supplemental.  Use this for information that supplements your preservation objects but is not to be included in the objects folder.'
-    )
-    parser.add_argument(
-        '-object_extension_pattern', nargs='+',
-        help='Enter the filename extensions, seperated by spaces, which determine which files to be added to the objects directory. For example -object_extension_pattern mxf stl will take all filenames with these extensions within your input directory and store them in objects.'
-    )
-    parser.add_argument(
-        '-y',
-        action='store_true',
-        help='Answers YES to the question: Do you want to proceed? useful for unattended batches but not recommended without running -dryrun first'
-    )
-    parser.add_argument(
-        '-dryrun', action='store_true',
-        help='The script will reveal which identifiers will be assigned but will not actually perform any actions.'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-def main(args_):
-    ''''
-    Launch all the functions for creating an IFI SIP.
-    '''
-    args = parse_args(args_)
-    source_folder = args.i
-    print(args)
-    oe_dict = {}
-    user = ififuncs.determine_user(args)
-    if args.oe:
-        object_entry = args.oe
-    else:
-        object_entry = ififuncs.get_object_entry()
-    oe_digits = int(object_entry.replace('oe', ''))
-    for folder in sorted(os.listdir(source_folder)):
-        full_path = os.path.join(source_folder, folder)
-        if os.path.isdir(full_path):
-            try:
-                folder_contents = os.listdir(full_path)
-            except PermissionError:
-                continue
-            object_entry_complete = 'oe' + str(oe_digits)
-            inputs = []
-            supplements = []
-            for files in folder_contents:
-                if os.path.splitext(files)[1][1:].lower() in args.object_extension_pattern:
-                    inputs.append(os.path.join(full_path, files))
-                if os.path.splitext(files)[1][1:].lower() in args.supplement_extension_pattern:
-                    supplements.append(os.path.join(full_path, files))
-            if inputs:
-                print(' - Object Entry: %s\n - Inputs: %s\n - Supplements: %s\n' % (object_entry_complete, inputs, supplements))
-                oe_dict[object_entry_complete] = [inputs, supplements]
-                oe_digits += 1
-            else:
-                print('Skipping %s as there are no files in this folder that match the -object_extension_pattern' % full_path)
-    if args.dryrun:
-        print('Exiting as you selected -dryrun')
-        sys.exit()
-    logs = []
-    if args.y:
-        proceed = 'Y'
-    else:
-        proceed = ififuncs.ask_yes_no(
-            'Do you want to proceed?'
-        )
-    if proceed == 'Y':
-        for sips in sorted(oe_dict):
-            print(oe_dict[sips])
-            sipcreator_cmd = ['-i',]
-            for sipcreator_inputs in oe_dict[sips][0]:
-                sipcreator_cmd.append(sipcreator_inputs)
-            sipcreator_cmd += ['-supplement']
-            for sipcreator_supplements in oe_dict[sips][1]:
-                sipcreator_cmd.append(sipcreator_supplements)
-            sipcreator_cmd += ['-user', user, '-oe', sips, '-o', args.o]
-            if args.rename_uuid:
-                sipcreator_cmd.append('-rename_uuid')
-            if args.zip:
-                sipcreator_cmd.append('-zip')
-            if args.l:
-                sipcreator_cmd.append('-l')
-            print(sipcreator_cmd)
-            sipcreator_log, _ = sipcreator.main(sipcreator_cmd)
-            logs.append(sipcreator_log)
-            for i in logs:
-                if os.path.isfile(i):
-                    print(("%-*s   : copyit job was a %s" % (50, os.path.basename(i), analyze_log(i))))
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Allow sipcreator to batch process multiple folders in a directory
+-dcp option is needed to process folders and grab html files
+'''
+import argparse
+import os
+import sys
+import ififuncs
+import sipcreator
+from masscopy import analyze_log
+
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Launches sipcreator.py on multiple objects.'
+        'Wraps objects into an Irish Film Institute SIP'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        '-i',
+        help='full path of input folder - this folder should contain subfolders which in turn contain video files', required=True
+    )
+    parser.add_argument(
+        '-o', '-output',
+        help='full path of output directory', required=True
+    )
+    parser.add_argument(
+        '-rename_uuid', action='store_true',
+        help='Use with caution! This will rename an object with a randonly generated UUID'
+    )
+    parser.add_argument(
+        '-user',
+        help='Declare who you are. If this is not set, you will be prompted.'
+    )
+    parser.add_argument(
+        '-l', action='store_true',
+        help='invokes the -lto argument in copyit.py - uses gcp instead of rsync.'
+    )
+    parser.add_argument(
+        '-d', '-dcp', action='store_true',
+        help='Adds DCP specific processing, like creating objects subfolder with text extracted from <ContentTitleText> in the CPL.'
+    )
+    parser.add_argument(
+        '-zip', action='store_true',
+        help='Uses makezip.py to store the objects in an uncompressed ZIP'
+    )
+    parser.add_argument(
+        '-oe',
+        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
+    )
+    parser.add_argument(
+        '-supplement_extension_pattern', nargs='+',
+        help='Enter the filename extensions, seperated by spaces, which determine which files to be added to the supplemental subfolder within the metadata directory. For example -supplement_extension_pattern xml pdf txt docx will take all filenames with these extensions within your input directory and store them in metadata/supplemental.  Use this for information that supplements your preservation objects but is not to be included in the objects folder.'
+    )
+    parser.add_argument(
+        '-object_extension_pattern', nargs='+',
+        help='Enter the filename extensions, seperated by spaces, which determine which files to be added to the objects directory. For example -object_extension_pattern mxf stl will take all filenames with these extensions within your input directory and store them in objects.'
+    )
+    parser.add_argument(
+        '-y',
+        action='store_true',
+        help='Answers YES to the question: Do you want to proceed? useful for unattended batches but not recommended without running -dryrun first'
+    )
+    parser.add_argument(
+        '-dryrun', action='store_true',
+        help='The script will reveal which identifiers will be assigned but will not actually perform any actions.'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+def main(args_):
+    ''''
+    Launch all the functions for creating an IFI SIP.
+    '''
+    args = parse_args(args_)
+    source_folder = args.i
+    print(args)
+    oe_dict = {}
+    user = ififuncs.determine_user(args)
+    if args.oe:
+        object_entry = args.oe
+    else:
+        object_entry = ififuncs.get_object_entry()
+    oe_digits = int(object_entry.replace('oe', ''))
+    for folder in sorted(os.listdir(source_folder)):
+        full_path = os.path.join(source_folder, folder)
+        if os.path.isdir(full_path):
+            try:
+                folder_contents = os.listdir(full_path)
+            except PermissionError:
+                continue
+            object_entry_complete = 'oe' + str(oe_digits)
+            inputs = []
+            supplements = []
+            for files in folder_contents:
+                if os.path.splitext(files)[1][1:].lower() in args.object_extension_pattern:
+                    inputs.append(os.path.join(full_path, files))
+                if os.path.splitext(files)[1][1:].lower() in args.supplement_extension_pattern:
+                    supplements.append(os.path.join(full_path, files))
+            if inputs:
+                print(' - Object Entry: %s\n - Inputs: %s\n - Supplements: %s\n' % (object_entry_complete, inputs, supplements))
+                oe_dict[object_entry_complete] = [inputs, supplements]
+                oe_digits += 1
+            else:
+                print('Skipping %s as there are no files in this folder that match the -object_extension_pattern' % full_path)
+    if args.dryrun:
+        print('Exiting as you selected -dryrun')
+        sys.exit()
+    logs = []
+    if args.y:
+        proceed = 'Y'
+    else:
+        proceed = ififuncs.ask_yes_no(
+            'Do you want to proceed?'
+        )
+    if proceed == 'Y':
+        for sips in sorted(oe_dict):
+            print(oe_dict[sips])
+            sipcreator_cmd = ['-i',]
+            for sipcreator_inputs in oe_dict[sips][0]:
+                sipcreator_cmd.append(sipcreator_inputs)
+            sipcreator_cmd += ['-supplement']
+            for sipcreator_supplements in oe_dict[sips][1]:
+                sipcreator_cmd.append(sipcreator_supplements)
+            sipcreator_cmd += ['-user', user, '-oe', sips, '-o', args.o]
+            if args.rename_uuid:
+                sipcreator_cmd.append('-rename_uuid')
+            if args.zip:
+                sipcreator_cmd.append('-zip')
+            if args.l:
+                sipcreator_cmd.append('-l')
+            print(sipcreator_cmd)
+            sipcreator_log, _ = sipcreator.main(sipcreator_cmd)
+            logs.append(sipcreator_log)
+            for i in logs:
+                if os.path.isfile(i):
+                    print(("%-*s   : copyit job was a %s" % (50, os.path.basename(i), analyze_log(i))))
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/bitc.py` & `ifiscripts-2023.7.3.2/scripts/bitc.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-#!/usr/bin/env python3
-'''
-Accept options from command line and make access copy.
-Use bitc.py -h for help
-'''
-import argparse
-import subprocess
-import sys
-import os
-from ififuncs import hashlib_md5
-import ififuncs
-
-def getffprobe(variable, streamvalue, which_file):
-    '''
-    Returns a specific ffprobe technical metadata value.
-    This is a good candidate to be moved to ififuncs.
-    '''
-    variable = subprocess.check_output([
-        'ffprobe',
-        '-v', 'error',
-        '-select_streams', 'v:0',
-        '-show_entries',
-        streamvalue,
-        '-of', 'default=noprint_wrappers=1:nokey=1',
-        which_file
-    ])
-    return variable.decode(sys.stdout.encoding)
-
-
-def set_options(args_):
-    '''
-    Parse command line options.
-    '''
-    parser = argparse.ArgumentParser(
-        description='IFI Irish Film Institute H264 FFMPEG Encoder.'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        'input'
-    )
-    parser.add_argument(
-        '-clean',
-        action='store_true',
-        help='Disables watermark and timecode for a clean image'
-    )
-    parser.add_argument(
-        '-watermark',
-        action='store_true',
-        help='Disables timecode and only displays watermark'
-    )
-    parser.add_argument(
-        '-timecode',
-        action='store_true',
-        help='Disables watermark and only displays timecode'
-    )
-    parser.add_argument(
-        '-yadif',
-        action='store_true',
-        help='Yet Another DeInterlace Filter'
-    )
-    parser.add_argument(
-        '-middle',
-        action='store_true',
-        help='Put timecode in the middle'
-    )
-    parser.add_argument(
-        '-crf',
-        help='Set quality. Default is 23, lower number ='
-        ' large file/high quality, high number = small file/poor quality'
-    )
-    parser.add_argument(
-        '-o',
-        help='Set output directory.'
-        'The default directory is the same directory as input.'
-    )
-    parser.add_argument(
-        '-logo',
-        help='Full path to a transparent PNG that will be '
-        'overlaid in the top right corner.'
-    )
-    parser.add_argument(
-        '-scale',
-        help='Rescale video.'
-        ' Usage: -scale 1920x1080 or -scale 720x576 etc'
-    )
-    parser.add_argument(
-        '-md5',
-        action='store_true',
-        help='Get md5 sidecar for your output file'
-    )
-    parser.add_argument(
-        '-map',
-        action='store_true',
-        help='Force default mapping, eg. 1 audio/video stream'
-    )
-
-    parser.add_argument(
-        '-player',
-        action='store_true',
-        help='uses yadif, 4:3 DAR with 1:1 PAR, with no watermark or timecode.'
-    )
-    parser.add_argument(
-        '-wide',
-        action='store_true',help='Adds 16:9 metadata flag'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def build_filter(args, filename):
-    '''
-    Builds the ffmpeg -vf filtergraph, if needed.
-    '''
-    h264_options = []
-    filter_list = []
-    filtergraph = ''
-    if args.yadif:
-        h264_options.append('yadif')
-    if args.logo:
-        h264_options.append('overlay=main_w-overlay_w-5:5')
-    if args.scale:
-        h264_options.append('scale=%s' % args.scale)
-        # width_height = args.scale
-    if args.player:
-        args.clean = True
-        args.yadif = True
-    if not args.clean:
-        drawtext_option = setup_drawtext(args, filename)
-        h264_options.append(drawtext_option)
-    for option in h264_options:
-        filtergraph += option + ','
-    if len(filtergraph) > 0:
-        if filtergraph[-1] == ',':
-            filtergraph = filtergraph[:-1]
-        filter_list = ['-filter_complex', filtergraph]
-        print(filter_list)
-    return filter_list
-
-
-def get_filenames(args):
-    '''
-    Get information about filenames, paths etc.
-    '''
-    cli_input = args.input
-    # Input, either file or firectory, that we want to process.
-    # Store the directory containing the input file/directory.
-    wd = os.path.dirname(cli_input)
-    video_files = []
-    if wd == '':
-        cli_input = os.path.join(os.getcwd(), args.input)
-    # Check if input is a file.
-    # AFAIK, os.path.isfile only works if full path isn't present.
-    if os.path.isfile(cli_input):
-        video_files.append(cli_input)  # Add filename to list
-    # Check if input is a directory.
-    elif os.path.isdir(cli_input):
-        for files in os.listdir(cli_input):
-            if files.endswith(('.mov', '.mp4', '.mxf', '.mkv', '.avi')):
-                if files[0] != '.':
-                    video_files.append(os.path.join(cli_input, files))
-    # Prints some stuff if input isn't a file or directory.
-    else:
-        print("Your input isn't a file or a directory.")
-    return video_files
-
-
-def setup_drawtext(args, filename):
-    '''
-    Sets up the filtergraphs for either timecode, watermark or both.
-    '''
-    # HDV m2t streams report two height values, so the rsplit() just accepts the first.
-    video_height = float(getffprobe('video_height', 'stream=height', filename).rsplit()[0])
-    # Calculate appropriate font size
-    font_size = video_height / 12
-    watermark_size = video_height / 14
-    if sys.platform == "darwin":
-        font_path = "fontfile=/Library/Fonts/AppleGothic.ttf"
-    elif sys.platform.startswith("linux"):
-        font_path = "fontfile=/usr/share/fonts/truetype/freefont/FreeSerifBold.ttf"
-    elif sys.platform == "win32":
-        font_path = "'fontfile=C\:\\\Windows\\\Fonts\\\\'arial.ttf'"
-    # Get starting timecode
-    timecode_test_raw = getffprobe(
-        'timecode_test_raw',
-        'format_tags=timecode:stream_tags=timecode',
-        filename
-    )
-    framerate = getffprobe(
-        'get_frame_rate',
-        'stream=avg_frame_rate',
-        filename
-    ).rsplit()[0]
-    # This tests if there is actually a timecode present in the file.
-    if not timecode_test_raw:
-        # The timecode needs to be phrased in a way unique to each O.S.
-        # Note the backslashes.
-        # This section makes up a timecode if none is present in the file.
-        if sys.platform == "darwin" or sys.platform.startswith("linux"):
-            timecode_test = '01\\\:00\\\:00\\\:00'
-        elif sys.platform == "win32":
-            timecode_test = '01\:00\:00\:00'
-    else:
-        # If timecode is present, this will escape the colons
-        # so that it is compatible with each operating system.
-        if sys.platform == "darwin" or sys.platform.startswith("linux"):
-            timecode_test = timecode_test_raw.replace(':', '\\\:').rstrip()
-        elif sys.platform == "win32":
-            timecode_test = timecode_test_raw.replace(':', '\\:').rstrip()
-    # This removes the new line character from the framemrate.
-    if args.middle:
-        timecode_option = "drawtext=%s:fontcolor=white:fontsize=%s:timecode=%s:rate=%s:boxcolor=0x000000AA:box=1:x=(w-text_w)/2:y=(h-text_h)/2" % (font_path, font_size, timecode_test, framerate)
-        watermark_option = "drawtext=%s:fontcolor=white:text='IFI IRISH FILM ARCHIVE':x=(w-text_w)/2:y=h/1.2:fontsize=%s:alpha=0.4"  % (font_path, watermark_size)
-    else:
-        timecode_option = "drawtext=%s:fontcolor=white:fontsize=%s:timecode=%s:rate=%s:boxcolor=0x000000AA:box=1:x=(w-text_w)/2:y=h/1.2" % (font_path, font_size, timecode_test, framerate)
-        watermark_option = "drawtext=%s:fontcolor=white:text='IFI IRISH FILM ARCHIVE':x=(w-text_w)/2:y=(h-text_h)/2:fontsize=%s:alpha=0.4"  % (font_path, watermark_size)
-    bitc_watermark = timecode_option + ',' + watermark_option
-    if args.timecode:
-        return timecode_option
-    elif args.watermark:
-        return watermark_option
-    else:
-        return bitc_watermark
-
-
-def main(args_):
-    '''
-    Launch the various functions that will make a h264/mp4 access copy.
-    '''
-    ififuncs.check_existence(['ffprobe', 'ffmpeg'])
-    args = set_options(args_)
-    video_files = get_filenames(args)
-    for filename in video_files:
-        filter_list = build_filter(args, filename)
-        make_h264(filename, args, filter_list)
-
-
-def make_h264(filename, args, filter_list):
-    '''
-    Launches the actuall ffmpeg process using all the info gleaned so far.
-    '''
-    if args.crf:
-        crf_value = args.crf
-    else:
-        crf_value = '23'
-    if args.o:
-        output = args.o + '/' + os.path.basename(filename) + "_h264.mov"
-    else:
-        output = filename + "_h264.mov"
-    ffmpeg_args = [
-        'ffmpeg',
-        '-i', filename,
-    ]
-    if args.logo:
-        ffmpeg_args.extend(['-i', args.logo])
-    ffmpeg_args += [
-        '-c:a', 'aac',
-        '-c:v', 'libx264',
-        '-pix_fmt', 'yuv420p',
-        '-crf', crf_value
-    ]
-    if args.wide:
-        ffmpeg_args.append('-aspect')
-        ffmpeg_args.append('16:9')
-    if not args.map:
-        ffmpeg_args.append('-map')
-        ffmpeg_args.append('0:a?')
-        ffmpeg_args.append('-map')
-        ffmpeg_args.append('0:v')
-    if len(filter_list) > 0:
-        for _filter in filter_list:
-            ffmpeg_args.append(_filter)
-    ffmpeg_args.append(output)
-    print(ffmpeg_args)
-    subprocess.call(ffmpeg_args)
-    if args.md5:
-        manifest = '%s_manifest.md5' % filename
-        print('Generating md5 sidecar...')
-        h264_md5 = hashlib_md5(filename)
-        with open(manifest, 'wb') as fo:
-            fo.write('%s  %s' % (h264_md5, filename))
-
-if __name__ == "__main__":
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Accept options from command line and make access copy.
+Use bitc.py -h for help
+'''
+import argparse
+import subprocess
+import sys
+import os
+from ififuncs import hashlib_md5
+import ififuncs
+
+def getffprobe(variable, streamvalue, which_file):
+    '''
+    Returns a specific ffprobe technical metadata value.
+    This is a good candidate to be moved to ififuncs.
+    '''
+    variable = subprocess.check_output([
+        'ffprobe',
+        '-v', 'error',
+        '-select_streams', 'v:0',
+        '-show_entries',
+        streamvalue,
+        '-of', 'default=noprint_wrappers=1:nokey=1',
+        which_file
+    ])
+    return variable.decode(sys.stdout.encoding)
+
+
+def set_options(args_):
+    '''
+    Parse command line options.
+    '''
+    parser = argparse.ArgumentParser(
+        description='IFI Irish Film Institute H264 FFMPEG Encoder.'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        'input'
+    )
+    parser.add_argument(
+        '-clean',
+        action='store_true',
+        help='Disables watermark and timecode for a clean image'
+    )
+    parser.add_argument(
+        '-watermark',
+        action='store_true',
+        help='Disables timecode and only displays watermark'
+    )
+    parser.add_argument(
+        '-timecode',
+        action='store_true',
+        help='Disables watermark and only displays timecode'
+    )
+    parser.add_argument(
+        '-yadif',
+        action='store_true',
+        help='Yet Another DeInterlace Filter'
+    )
+    parser.add_argument(
+        '-middle',
+        action='store_true',
+        help='Put timecode in the middle'
+    )
+    parser.add_argument(
+        '-crf',
+        help='Set quality. Default is 23, lower number ='
+        ' large file/high quality, high number = small file/poor quality'
+    )
+    parser.add_argument(
+        '-o',
+        help='Set output directory.'
+        'The default directory is the same directory as input.'
+    )
+    parser.add_argument(
+        '-logo',
+        help='Full path to a transparent PNG that will be '
+        'overlaid in the top right corner.'
+    )
+    parser.add_argument(
+        '-scale',
+        help='Rescale video.'
+        ' Usage: -scale 1920x1080 or -scale 720x576 etc'
+    )
+    parser.add_argument(
+        '-md5',
+        action='store_true',
+        help='Get md5 sidecar for your output file'
+    )
+    parser.add_argument(
+        '-map',
+        action='store_true',
+        help='Force default mapping, eg. 1 audio/video stream'
+    )
+
+    parser.add_argument(
+        '-player',
+        action='store_true',
+        help='uses yadif, 4:3 DAR with 1:1 PAR, with no watermark or timecode.'
+    )
+    parser.add_argument(
+        '-wide',
+        action='store_true',help='Adds 16:9 metadata flag'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def build_filter(args, filename):
+    '''
+    Builds the ffmpeg -vf filtergraph, if needed.
+    '''
+    h264_options = []
+    filter_list = []
+    filtergraph = ''
+    if args.yadif:
+        h264_options.append('yadif')
+    if args.logo:
+        h264_options.append('overlay=main_w-overlay_w-5:5')
+    if args.scale:
+        h264_options.append('scale=%s' % args.scale)
+        # width_height = args.scale
+    if args.player:
+        args.clean = True
+        args.yadif = True
+    if not args.clean:
+        drawtext_option = setup_drawtext(args, filename)
+        h264_options.append(drawtext_option)
+    for option in h264_options:
+        filtergraph += option + ','
+    if len(filtergraph) > 0:
+        if filtergraph[-1] == ',':
+            filtergraph = filtergraph[:-1]
+        filter_list = ['-filter_complex', filtergraph]
+        print(filter_list)
+    return filter_list
+
+
+def get_filenames(args):
+    '''
+    Get information about filenames, paths etc.
+    '''
+    cli_input = args.input
+    # Input, either file or firectory, that we want to process.
+    # Store the directory containing the input file/directory.
+    wd = os.path.dirname(cli_input)
+    video_files = []
+    if wd == '':
+        cli_input = os.path.join(os.getcwd(), args.input)
+    # Check if input is a file.
+    # AFAIK, os.path.isfile only works if full path isn't present.
+    if os.path.isfile(cli_input):
+        video_files.append(cli_input)  # Add filename to list
+    # Check if input is a directory.
+    elif os.path.isdir(cli_input):
+        for files in os.listdir(cli_input):
+            if files.endswith(('.mov', '.mp4', '.mxf', '.mkv', '.avi')):
+                if files[0] != '.':
+                    video_files.append(os.path.join(cli_input, files))
+    # Prints some stuff if input isn't a file or directory.
+    else:
+        print("Your input isn't a file or a directory.")
+    return video_files
+
+
+def setup_drawtext(args, filename):
+    '''
+    Sets up the filtergraphs for either timecode, watermark or both.
+    '''
+    # HDV m2t streams report two height values, so the rsplit() just accepts the first.
+    video_height = float(getffprobe('video_height', 'stream=height', filename).rsplit()[0])
+    # Calculate appropriate font size
+    font_size = video_height / 12
+    watermark_size = video_height / 14
+    if sys.platform == "darwin":
+        font_path = "fontfile=/Library/Fonts/AppleGothic.ttf"
+    elif sys.platform.startswith("linux"):
+        font_path = "fontfile=/usr/share/fonts/truetype/freefont/FreeSerifBold.ttf"
+    elif sys.platform == "win32":
+        font_path = "'fontfile=C\:\\\Windows\\\Fonts\\\\'arial.ttf'"
+    # Get starting timecode
+    timecode_test_raw = getffprobe(
+        'timecode_test_raw',
+        'format_tags=timecode:stream_tags=timecode',
+        filename
+    )
+    framerate = getffprobe(
+        'get_frame_rate',
+        'stream=avg_frame_rate',
+        filename
+    ).rsplit()[0]
+    # This tests if there is actually a timecode present in the file.
+    if not timecode_test_raw:
+        # The timecode needs to be phrased in a way unique to each O.S.
+        # Note the backslashes.
+        # This section makes up a timecode if none is present in the file.
+        if sys.platform == "darwin" or sys.platform.startswith("linux"):
+            timecode_test = '01\\\:00\\\:00\\\:00'
+        elif sys.platform == "win32":
+            timecode_test = '01\:00\:00\:00'
+    else:
+        # If timecode is present, this will escape the colons
+        # so that it is compatible with each operating system.
+        if sys.platform == "darwin" or sys.platform.startswith("linux"):
+            timecode_test = timecode_test_raw.replace(':', '\\\:').rstrip()
+        elif sys.platform == "win32":
+            timecode_test = timecode_test_raw.replace(':', '\\:').rstrip()
+    # This removes the new line character from the framemrate.
+    if args.middle:
+        timecode_option = "drawtext=%s:fontcolor=white:fontsize=%s:timecode=%s:rate=%s:boxcolor=0x000000AA:box=1:x=(w-text_w)/2:y=(h-text_h)/2" % (font_path, font_size, timecode_test, framerate)
+        watermark_option = "drawtext=%s:fontcolor=white:text='IFI IRISH FILM ARCHIVE':x=(w-text_w)/2:y=h/1.2:fontsize=%s:alpha=0.4"  % (font_path, watermark_size)
+    else:
+        timecode_option = "drawtext=%s:fontcolor=white:fontsize=%s:timecode=%s:rate=%s:boxcolor=0x000000AA:box=1:x=(w-text_w)/2:y=h/1.2" % (font_path, font_size, timecode_test, framerate)
+        watermark_option = "drawtext=%s:fontcolor=white:text='IFI IRISH FILM ARCHIVE':x=(w-text_w)/2:y=(h-text_h)/2:fontsize=%s:alpha=0.4"  % (font_path, watermark_size)
+    bitc_watermark = timecode_option + ',' + watermark_option
+    if args.timecode:
+        return timecode_option
+    elif args.watermark:
+        return watermark_option
+    else:
+        return bitc_watermark
+
+
+def main(args_):
+    '''
+    Launch the various functions that will make a h264/mp4 access copy.
+    '''
+    ififuncs.check_existence(['ffprobe', 'ffmpeg'])
+    args = set_options(args_)
+    video_files = get_filenames(args)
+    for filename in video_files:
+        filter_list = build_filter(args, filename)
+        make_h264(filename, args, filter_list)
+
+
+def make_h264(filename, args, filter_list):
+    '''
+    Launches the actuall ffmpeg process using all the info gleaned so far.
+    '''
+    if args.crf:
+        crf_value = args.crf
+    else:
+        crf_value = '23'
+    if args.o:
+        output = args.o + '/' + os.path.basename(filename) + "_h264.mov"
+    else:
+        output = filename + "_h264.mov"
+    ffmpeg_args = [
+        'ffmpeg',
+        '-i', filename,
+    ]
+    if args.logo:
+        ffmpeg_args.extend(['-i', args.logo])
+    ffmpeg_args += [
+        '-c:a', 'aac',
+        '-c:v', 'libx264',
+        '-pix_fmt', 'yuv420p',
+        '-crf', crf_value
+    ]
+    if args.wide:
+        ffmpeg_args.append('-aspect')
+        ffmpeg_args.append('16:9')
+    if not args.map:
+        ffmpeg_args.append('-map')
+        ffmpeg_args.append('0:a?')
+        ffmpeg_args.append('-map')
+        ffmpeg_args.append('0:v')
+    if len(filter_list) > 0:
+        for _filter in filter_list:
+            ffmpeg_args.append(_filter)
+    ffmpeg_args.append(output)
+    print(ffmpeg_args)
+    subprocess.call(ffmpeg_args)
+    if args.md5:
+        manifest = '%s_manifest.md5' % filename
+        print('Generating md5 sidecar...')
+        h264_md5 = hashlib_md5(filename)
+        with open(manifest, 'wb') as fo:
+            fo.write('%s  %s' % (h264_md5, filename))
+
+if __name__ == "__main__":
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/concat.py` & `ifiscripts-2023.7.3.2/scripts/concat.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-#!/usr/bin/env python3
-'''
-Concatenates video files using FFmpeg stream copy for general use but
-particularly for XDCAM workflows in the IFI Irish Film Institute.
-Uses mkvpropedit to insert chapter markers for each source file.
-Optionally wraps the file into a package structure with checksum manifests.
-
-Written by Kieran O'Leary.
-'''
-import sys
-import subprocess
-import os
-import argparse
-import time
-import shutil
-import sipcreator
-import ififuncs
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Concatenate video files using ffmpeg stream copy'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        '-i', nargs='+',
-        help='full path of input directory', required=True
-    )
-    parser.add_argument(
-        '-o', '-output',
-        help='full path of output directory', required=True
-    )
-    parser.add_argument(
-        '-r', '-recursive',
-        help='recursively process all files in subdirectories. This could be potentially a disaster - so use with caution or with XDCAM', action='store_true'
-    )
-    parser.add_argument(
-        '--no-sip',
-        help='Do not run sipcreator.py on the resulting file.', action='store_true'
-    )
-    parser.add_argument(
-        '-user',
-        help='Declare who you are. If this is not set, you will be prompted.')
-    parser.add_argument(
-        '-oe',
-        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
-    )
-    parser.add_argument(
-        '-mov',
-        help='Uses MOV container instead of Matroska', action='store_true'
-    )
-    parser.add_argument(
-        '-nochapters',
-        help='Skips the mkvpropedit chapter creation function', action='store_true'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def ffmpeg_concat(concat_file, args, uuid, container):
-    '''
-    Launch the actual ffmpeg concatenation command.
-    '''
-    fmd5_logfile = os.path.join(args.o, '%s_concat.log' % uuid).replace('\\', '\\\\').replace(':', '\:')
-    fmd5_env_dict = ififuncs.set_environment(fmd5_logfile)
-    print( fmd5_logfile)
-    print( fmd5_env_dict)
-    cmd = [
-        'ffmpeg', '-report', '-f', 'concat', '-safe', '0',
-        '-i', concat_file,
-        '-c', 'copy', '-map', '0:v', '-map', '0:a?',
-        os.path.join(args.o, '%s.%s' % (uuid, container)),
-        '-f', 'md5', '-map', '0:v', '-map', '0:a?','-c', 'copy',  '-'
-    ]
-    print(cmd)
-    source_bitstream_md5 = subprocess.check_output(
-        cmd, env=fmd5_env_dict
-    )
-    return source_bitstream_md5.rstrip(), fmd5_logfile.replace('\\\\', '\\').replace('\:', ':')
-
-def recursive_file_list(video_files):
-    '''
-    Recursively searches through directories for AV files and adds to a list.
-    '''
-    # check if all inputs are actually directories
-    recursive_list = []
-    for directory in video_files:
-        if not os.path.isdir(directory):
-            print( 'You have selected the recursive option, but not all of your inputs are directories.')
-            sys.exit()
-        else:
-            for root, _, filenames in os.walk(directory):
-                for filename in filenames:
-                    if filename.endswith(('.MP4', '.mp4', '.mov', '.mkv', '.mxf', 'MXF')):
-                        recursive_list.append(os.path.join(root, filename))
-    print(recursive_list)
-    return recursive_list
-
-def make_chapters(video_files):
-    '''
-    Use mkvpropedit to insert chapter markers for each source video.
-    Each chapter's name will reflect the source filename of each clip.
-    '''
-    millis = ififuncs.get_milliseconds(video_files[0])
-    timestamp = ififuncs.convert_millis(int(millis))
-    chapter_list = [['00:00:00.000', os.path.basename(video_files[0])], [timestamp, os.path.basename(video_files[1])]]
-    count = 2
-    for video in video_files[1:]:
-        millis += ififuncs.get_milliseconds(video)
-        timestamp = ififuncs.convert_millis(int(millis))
-        if count == len(video_files):
-            continue
-        else:
-            chapter_list.append([timestamp, os.path.basename(video_files[count])])
-        count+=1
-    chapter_counter = 1
-    # uh use a real path/filename.
-    with open('chapters.txt', 'w') as fo:
-        for i in chapter_list:
-            fo.write('CHAPTER%s=%s\nCHAPTER%sNAME=%s\n' % (str(chapter_counter).zfill(2), i[0], str(chapter_counter).zfill(2), i[1]))
-            chapter_counter += 1
-
-
-def main(args_):
-    '''
-    Launches the functions that prepare and execute the concatenation.
-    '''
-    ififuncs.check_existence(['ffmpeg', 'mkvpropedit', 'mediainfo'])
-    uuid = ififuncs.create_uuid()
-    args = parse_args(args_)
-    print(args)
-    log_name_source = os.path.join(args.o, '%s_concat_log.log' % time.strftime("_%Y_%m_%dT%H_%M_%S"))
-    ififuncs.generate_log(log_name_source, 'concat.py started.')
-    if args.mov:
-        container = 'mov'
-    else:
-        container = 'mkv'
-    ififuncs.generate_log(
-        log_name_source,
-        'eventDetail=concat.py %s' % ififuncs.get_script_version('concat.py'))
-    ififuncs.generate_log(
-        log_name_source,
-        'Command line arguments: %s' % args
-    )
-    if args.user:
-        user = args.user
-    else:
-        user = ififuncs.get_user()
-    if args.oe:
-        if args.oe[:2] != 'oe':
-            print('First two characters must be \'oe\' and last four characters must be four digits')
-            object_entry = ififuncs.get_object_entry()
-        elif len(args.oe[2:]) not in range(4, 6):
-            print('First two characters must be \'oe\' and last four characters must be four digits')
-            object_entry = ififuncs.get_object_entry()
-        elif not args.oe[2:].isdigit():
-           object_entry = ififuncs.get_object_entry()
-           print('First two characters must be \'oe\' and last four characters must be four digits')
-        else:
-            object_entry = args.oe
-    else:
-        object_entry = ififuncs.get_object_entry()
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = agentName=%s' % user
-    )
-    source_uuid_check = ''
-    if os.path.isfile(args.i[0]):
-        source_uuid = ififuncs.get_source_uuid()
-    elif os.path.isdir(args.i[0]):
-        source_uuid_check = ififuncs.check_for_uuid(args)
-    if source_uuid_check == False:
-        source_uuid = ififuncs.get_source_uuid()
-    else: source_uuid = source_uuid_check
-    ififuncs.generate_log(
-        log_name_source,
-        'Relationship, derivation, has source=%s' % source_uuid
-    )
-    video_files = args.i
-    concat_file = ififuncs.get_temp_concat('concat_stuff')
-    ififuncs.generate_log(
-        log_name_source,
-        'concatenation file=%s' % concat_file)
-    if args.r:
-        video_files = recursive_file_list(video_files)
-    video_files = ififuncs.sanitise_filenames(video_files)
-    for source_files in video_files:
-        ififuncs.generate_log(
-            log_name_source,
-            'source_files = %s' % source_files)
-    make_chapters(video_files)
-    ififuncs.concat_textfile(video_files, concat_file)
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = Concatenation, status=started, eventType=Creation, agentName=ffmpeg, eventDetail=Source media concatenated into a single file output=%s' % os.path.join(args.o, '%s.%s' % (uuid, container)))
-    source_bitstream_md5, fmd5_logfile = ffmpeg_concat(concat_file, args, uuid, container)
-    output_file = os.path.join(args.o, '%s.%s' % (uuid, container))
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = Concatenation, status=finished, eventType=Creation, agentName=ffmpeg, eventDetail=Source media concatenated into a single file output=%s' % os.path.join(args.o, '%s.%s' % (uuid, container)))
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = losslessness verification, status=started, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation')
-    validation_logfile = os.path.join(args.o, '%s_validation.log' % uuid).replace('\\', '\\\\').replace(':', '\:')
-    validation_env_dict = ififuncs.set_environment(validation_logfile)
-    output_bitstream_md5 = subprocess.check_output([
-        'ffmpeg', '-report',
-        '-i', output_file,
-        '-f', 'md5', '-map', '0:v', '-map', '0:a?', '-c', 'copy', '-'
-    ], env=validation_env_dict).rstrip()
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = losslessness verification, status=finished, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation')
-    if source_bitstream_md5 == output_bitstream_md5:
-        print( 'process appears to be lossless')
-        print( source_bitstream_md5, output_bitstream_md5)
-        ififuncs.generate_log(
-        log_name_source,
-        'EVENT = losslessness verification, eventOutcome=pass')
-    else:
-        print( 'something went wrong - not lossless!')
-        print( source_bitstream_md5,output_bitstream_md5)
-        ififuncs.generate_log(
-        log_name_source,
-        'EVENT = losslessness verification, eventOutcome=fail')
-    if args.nochapters != True:
-        subprocess.call(['mkvpropedit', output_file, '-c', 'chapters.txt'])
-        ififuncs.generate_log(
-            log_name_source,
-            'EVENT = eventType=modification, agentName=mkvpropedit, eventDetail=Chapters added to file detailing start point of source clips.')
-        ififuncs.concat_textfile(video_files, concat_file)
-        with open(log_name_source, 'r') as concat_log:
-            concat_lines = concat_log.readlines()
-    if not args.no_sip:
-        sipcreator_log, sipcreator_manifest = sipcreator.main(['-i', output_file, '-u', uuid, '-oe', object_entry, '-user', user, '-o', args.o])
-        shutil.move(fmd5_logfile, os.path.dirname(sipcreator_log))
-        shutil.move(validation_logfile.replace('\\\\', '\\').replace('\:', ':'), os.path.dirname(sipcreator_log))
-        logs_dir = os.path.dirname(sipcreator_log)
-        ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(fmd5_logfile)))
-        ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir,(os.path.basename(validation_logfile.replace('\\\\', '\\').replace('\:', ':')))))
-        ififuncs.merge_logs(log_name_source, sipcreator_log, sipcreator_manifest)
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Concatenates video files using FFmpeg stream copy for general use but
+particularly for XDCAM workflows in the IFI Irish Film Institute.
+Uses mkvpropedit to insert chapter markers for each source file.
+Optionally wraps the file into a package structure with checksum manifests.
+
+Written by Kieran O'Leary.
+'''
+import sys
+import subprocess
+import os
+import argparse
+import time
+import shutil
+import sipcreator
+import ififuncs
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Concatenate video files using ffmpeg stream copy'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        '-i', nargs='+',
+        help='full path of input directory', required=True
+    )
+    parser.add_argument(
+        '-o', '-output',
+        help='full path of output directory', required=True
+    )
+    parser.add_argument(
+        '-r', '-recursive',
+        help='recursively process all files in subdirectories. This could be potentially a disaster - so use with caution or with XDCAM', action='store_true'
+    )
+    parser.add_argument(
+        '--no-sip',
+        help='Do not run sipcreator.py on the resulting file.', action='store_true'
+    )
+    parser.add_argument(
+        '-user',
+        help='Declare who you are. If this is not set, you will be prompted.')
+    parser.add_argument(
+        '-oe',
+        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
+    )
+    parser.add_argument(
+        '-mov',
+        help='Uses MOV container instead of Matroska', action='store_true'
+    )
+    parser.add_argument(
+        '-nochapters',
+        help='Skips the mkvpropedit chapter creation function', action='store_true'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def ffmpeg_concat(concat_file, args, uuid, container):
+    '''
+    Launch the actual ffmpeg concatenation command.
+    '''
+    fmd5_logfile = os.path.join(args.o, '%s_concat.log' % uuid).replace('\\', '\\\\').replace(':', '\:')
+    fmd5_env_dict = ififuncs.set_environment(fmd5_logfile)
+    print( fmd5_logfile)
+    print( fmd5_env_dict)
+    cmd = [
+        'ffmpeg', '-report', '-f', 'concat', '-safe', '0',
+        '-i', concat_file,
+        '-c', 'copy', '-map', '0:v', '-map', '0:a?',
+        os.path.join(args.o, '%s.%s' % (uuid, container)),
+        '-f', 'md5', '-map', '0:v', '-map', '0:a?','-c', 'copy',  '-'
+    ]
+    print(cmd)
+    source_bitstream_md5 = subprocess.check_output(
+        cmd, env=fmd5_env_dict
+    )
+    return source_bitstream_md5.rstrip(), fmd5_logfile.replace('\\\\', '\\').replace('\:', ':')
+
+def recursive_file_list(video_files):
+    '''
+    Recursively searches through directories for AV files and adds to a list.
+    '''
+    # check if all inputs are actually directories
+    recursive_list = []
+    for directory in video_files:
+        if not os.path.isdir(directory):
+            print( 'You have selected the recursive option, but not all of your inputs are directories.')
+            sys.exit()
+        else:
+            for root, _, filenames in os.walk(directory):
+                for filename in filenames:
+                    if filename.endswith(('.MP4', '.mp4', '.mov', '.mkv', '.mxf', 'MXF')):
+                        recursive_list.append(os.path.join(root, filename))
+    print(recursive_list)
+    return recursive_list
+
+def make_chapters(video_files):
+    '''
+    Use mkvpropedit to insert chapter markers for each source video.
+    Each chapter's name will reflect the source filename of each clip.
+    '''
+    millis = ififuncs.get_milliseconds(video_files[0])
+    timestamp = ififuncs.convert_millis(int(millis))
+    chapter_list = [['00:00:00.000', os.path.basename(video_files[0])], [timestamp, os.path.basename(video_files[1])]]
+    count = 2
+    for video in video_files[1:]:
+        millis += ififuncs.get_milliseconds(video)
+        timestamp = ififuncs.convert_millis(int(millis))
+        if count == len(video_files):
+            continue
+        else:
+            chapter_list.append([timestamp, os.path.basename(video_files[count])])
+        count+=1
+    chapter_counter = 1
+    # uh use a real path/filename.
+    with open('chapters.txt', 'w') as fo:
+        for i in chapter_list:
+            fo.write('CHAPTER%s=%s\nCHAPTER%sNAME=%s\n' % (str(chapter_counter).zfill(2), i[0], str(chapter_counter).zfill(2), i[1]))
+            chapter_counter += 1
+
+
+def main(args_):
+    '''
+    Launches the functions that prepare and execute the concatenation.
+    '''
+    ififuncs.check_existence(['ffmpeg', 'mkvpropedit', 'mediainfo'])
+    uuid = ififuncs.create_uuid()
+    args = parse_args(args_)
+    print(args)
+    log_name_source = os.path.join(args.o, '%s_concat_log.log' % time.strftime("_%Y_%m_%dT%H_%M_%S"))
+    ififuncs.generate_log(log_name_source, 'concat.py started.')
+    if args.mov:
+        container = 'mov'
+    else:
+        container = 'mkv'
+    ififuncs.generate_log(
+        log_name_source,
+        'eventDetail=concat.py %s' % ififuncs.get_script_version('concat.py'))
+    ififuncs.generate_log(
+        log_name_source,
+        'Command line arguments: %s' % args
+    )
+    if args.user:
+        user = args.user
+    else:
+        user = ififuncs.get_user()
+    if args.oe:
+        if args.oe[:2] != 'oe':
+            print('First two characters must be \'oe\' and last four characters must be four digits')
+            object_entry = ififuncs.get_object_entry()
+        elif len(args.oe[2:]) not in range(4, 6):
+            print('First two characters must be \'oe\' and last four characters must be four digits')
+            object_entry = ififuncs.get_object_entry()
+        elif not args.oe[2:].isdigit():
+           object_entry = ififuncs.get_object_entry()
+           print('First two characters must be \'oe\' and last four characters must be four digits')
+        else:
+            object_entry = args.oe
+    else:
+        object_entry = ififuncs.get_object_entry()
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = agentName=%s' % user
+    )
+    source_uuid_check = ''
+    if os.path.isfile(args.i[0]):
+        source_uuid = ififuncs.get_source_uuid()
+    elif os.path.isdir(args.i[0]):
+        source_uuid_check = ififuncs.check_for_uuid(args)
+    if source_uuid_check == False:
+        source_uuid = ififuncs.get_source_uuid()
+    else: source_uuid = source_uuid_check
+    ififuncs.generate_log(
+        log_name_source,
+        'Relationship, derivation, has source=%s' % source_uuid
+    )
+    video_files = args.i
+    concat_file = ififuncs.get_temp_concat('concat_stuff')
+    ififuncs.generate_log(
+        log_name_source,
+        'concatenation file=%s' % concat_file)
+    if args.r:
+        video_files = recursive_file_list(video_files)
+    video_files = ififuncs.sanitise_filenames(video_files)
+    for source_files in video_files:
+        ififuncs.generate_log(
+            log_name_source,
+            'source_files = %s' % source_files)
+    make_chapters(video_files)
+    ififuncs.concat_textfile(video_files, concat_file)
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = Concatenation, status=started, eventType=Creation, agentName=ffmpeg, eventDetail=Source media concatenated into a single file output=%s' % os.path.join(args.o, '%s.%s' % (uuid, container)))
+    source_bitstream_md5, fmd5_logfile = ffmpeg_concat(concat_file, args, uuid, container)
+    output_file = os.path.join(args.o, '%s.%s' % (uuid, container))
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = Concatenation, status=finished, eventType=Creation, agentName=ffmpeg, eventDetail=Source media concatenated into a single file output=%s' % os.path.join(args.o, '%s.%s' % (uuid, container)))
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = losslessness verification, status=started, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation')
+    validation_logfile = os.path.join(args.o, '%s_validation.log' % uuid).replace('\\', '\\\\').replace(':', '\:')
+    validation_env_dict = ififuncs.set_environment(validation_logfile)
+    output_bitstream_md5 = subprocess.check_output([
+        'ffmpeg', '-report',
+        '-i', output_file,
+        '-f', 'md5', '-map', '0:v', '-map', '0:a?', '-c', 'copy', '-'
+    ], env=validation_env_dict).rstrip()
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = losslessness verification, status=finished, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation')
+    if source_bitstream_md5 == output_bitstream_md5:
+        print( 'process appears to be lossless')
+        print( source_bitstream_md5, output_bitstream_md5)
+        ififuncs.generate_log(
+        log_name_source,
+        'EVENT = losslessness verification, eventOutcome=pass')
+    else:
+        print( 'something went wrong - not lossless!')
+        print( source_bitstream_md5,output_bitstream_md5)
+        ififuncs.generate_log(
+        log_name_source,
+        'EVENT = losslessness verification, eventOutcome=fail')
+    if args.nochapters != True:
+        subprocess.call(['mkvpropedit', output_file, '-c', 'chapters.txt'])
+        ififuncs.generate_log(
+            log_name_source,
+            'EVENT = eventType=modification, agentName=mkvpropedit, eventDetail=Chapters added to file detailing start point of source clips.')
+        ififuncs.concat_textfile(video_files, concat_file)
+        with open(log_name_source, 'r') as concat_log:
+            concat_lines = concat_log.readlines()
+    if not args.no_sip:
+        sipcreator_log, sipcreator_manifest = sipcreator.main(['-i', output_file, '-u', uuid, '-oe', object_entry, '-user', user, '-o', args.o])
+        shutil.move(fmd5_logfile, os.path.dirname(sipcreator_log))
+        shutil.move(validation_logfile.replace('\\\\', '\\').replace('\:', ':'), os.path.dirname(sipcreator_log))
+        logs_dir = os.path.dirname(sipcreator_log)
+        ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(fmd5_logfile)))
+        ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir,(os.path.basename(validation_logfile.replace('\\\\', '\\').replace('\:', ':')))))
+        ififuncs.merge_logs(log_name_source, sipcreator_log, sipcreator_manifest)
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/copyit.py` & `ifiscripts-2023.7.3.2/scripts/copyit.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,779 +1,779 @@
-#!/usr/bin/env python3
-
-'''
-Copy pastes drectories while comparing checksum manifests of src and dst.
-'''
-
-import sys
-import subprocess
-import os
-import filecmp
-import tempfile
-import time
-import argparse
-import hashlib
-import shutil
-import unicodedata
-from builtins import input
-import ififuncs
-from ififuncs import make_desktop_logs_dir, make_desktop_manifest_dir, generate_log
-
-
-def hashlib_md5(filename):
-    '''
-    Create an md5 checksum. This should use the ififuncs function instead.
-    '''
-    read_size = 0
-    last_percent_done = 0
-    md5_object = hashlib.md5()
-    total_size = os.path.getsize(filename)
-    with open(str(filename), 'rb') as file_object:
-        while True:
-            buf = file_object.read(2**20)
-            if not buf:
-                break
-            read_size += len(buf)
-            md5_object.update(buf)
-            percent_done = 100 * read_size / total_size
-            if percent_done > last_percent_done:
-                sys.stdout.write('[%d%%]\r' % percent_done)
-                sys.stdout.flush()
-                last_percent_done = percent_done
-    md5_output = md5_object.hexdigest()
-    return md5_output + '  ' + os.path.abspath(filename) +  '\n'
-
-
-def test_write_capabilities(directory, log_name_source):
-    '''
-    Checks if drives have write access.
-    Also checks if source is a file or directory (no file support right now)
-    '''
-    if os.path.isdir(directory):
-        temp = tempfile.mkstemp(dir=directory, suffix='.tmp')
-        os.close(temp[0]) # Needed for windows.
-        os.remove(temp[1])
-    elif os.path.isfile(directory):
-        print('\nFile transfer is not currently supported, only directories.\n')
-        generate_log(
-            log_name_source,
-            'Error: Attempted file transfer. Source and Destination must be a directory'
-        )
-        generate_log(log_name_source, 'move.py exit')
-        sys.exit()
-    else:
-        print((' %s is either not a directory or it does not exist' % directory))
-        generate_log(
-            log_name_source,
-            ' %s is either not a directory or it does not exist' % directory
-        )
-        generate_log(log_name_source, 'move.py exit')
-        sys.exit()
-
-
-def remove_bad_files(root_dir, log_name_source):
-    '''
-    Stolen and adapted from Ben Fino-Radin. Removes annoying files.
-    '''
-    rm_these = ['.DS_Store', 'Thumbs.db', 'desktop.ini', 'Desktop.ini']
-    for root, _, files in os.walk(root_dir):
-        for name in files:
-            path = os.path.join(root, name)
-            for i in rm_these:
-                if name == i:
-                    print(('***********************' + 'removing: ' + path))
-                    if not log_name_source == None:
-                        generate_log(
-                            log_name_source,
-                            'EVENT = Unwanted file removal - %s was removed' % path
-                        )
-                    try:
-                        os.remove(path)
-                    except OSError:
-                        print('can\'t delete as source is read-only')
-
-
-def make_manifest(
-        manifest_dir,
-        manifest_textfile, path_to_remove
-    ):
-    '''
-    Generates a checksum text manifest.
-    '''
-    checksum_list = []
-    manifest_generator = ''
-    source_counter = 0
-    print('Counting the amount of files to be processed.')
-    for root, directories, filenames in os.walk(manifest_dir):
-        directories[:] = [
-            d for d in directories if d[0] != '.'
-        ]
-        directories[:] = [
-            d for d in directories if d != 'System Volume Information'
-        ]
-        directories[:] = [
-                d for d in directories if d != '$RECYCLE.BIN'
-        ]
-        directories[:] = [
-                d for d in directories if d != 'Seagate'
-        ]
-        filenames = [
-            f for f in filenames if os.path.basename(root) != 'System Volume Information'
-        ]
-        filenames = [
-            f for f in filenames if f[0] != '.'
-        ]
-        for files in filenames:
-            source_counter += 1
-    counter2 = 1
-    if os.path.isdir(manifest_dir):
-        os.chdir(manifest_dir)
-        for root, directories, filenames in os.walk(manifest_dir):
-            directories[:] = [
-                d for d in directories if d[0] != '.'
-            ]
-            directories[:] = [
-                d for d in directories if d != 'System Volume Information'
-            ]
-            directories[:] = [
-                d for d in directories if d != '$RECYCLE.BIN'
-            ]
-            directories[:] = [
-                d for d in directories if d != 'Seagate'
-            ]
-            filenames = [
-                f for f in filenames if os.path.basename(root) != 'System Volume Information'
-            ]
-            filenames = [
-                f for f in filenames if f[0] != '.'
-            ]
-            for files in filenames:
-                checksum_list.append([root, files])
-    elif os.path.isfile(manifest_dir):
-        checksum_list = [[os.path.dirname(manifest_dir), os.path.basename(manifest_dir)]]
-    if len(checksum_list) == 1:
-        source_counter = 1
-    for files in checksum_list:
-        print(('Generating MD5 for %s - %d of %d' % (
-            os.path.join(files[0], files[1]), counter2, source_counter)
-            ))
-        md5 = hashlib_md5(os.path.join(files[0], files[1]))
-        root2 = files[0].replace(path_to_remove, '')
-        try:
-            if root2[0] == '/':
-                root2 = root2[1:]
-            if root2[0] == '\\':
-                root2 = root2[1:]
-        except: IndexError
-        manifest_generator += md5[:32] + '  ' + os.path.join(
-            root2, files[1]
-            ).replace("\\", "/") + '\n'
-        counter2 += 1
-    manifest_list = manifest_generator.splitlines()
-    files_in_manifest = len(manifest_list)
-    # http://stackoverflow.com/a/31306961/2188572
-    manifest_list = sorted(manifest_list, key=lambda x: (x[34:]))
-    with open(manifest_textfile, "w", encoding='utf-8') as text:
-        for i in manifest_list:
-            text.write(i + '\n')
-    return files_in_manifest
-
-
-def copy_dir(
-        source, destination_final_path,
-        log_name_source, rootpos, destination, dirname, args
-    ):
-    '''
-    Depending on which operating system is running the script, system tools
-    are launched that copy paste source files to destination.
-    '''
-    if sys.platform == "win32":
-        if os.path.isfile(source):
-            generate_log(
-                log_name_source,
-                'EVENT = File Transfer, status=started, agentName=Windows, module=shutil.copy2'
-            )
-            print('copying file with python/shutil')
-            shutil.copy2(source, destination_final_path)
-        else:
-            subprocess.call([
-                'robocopy', source,
-                destination_final_path,
-                '/E', '/XA:SH',
-                '/XD', '.*',
-                '/XD', '*System Volume Information*',
-                '/XD', 'Seagate',
-                '/XD', '$Recycle.bin', '/a-:SH', '/a+:R'
-            ])
-            generate_log(
-                log_name_source,
-                'EVENT = File Transfer, status=started, agentName=Windows O.S, agentName=Robocopy'
-            )
-    elif sys.platform == "darwin":
-        if args.l:
-            cmd = [
-                'gcp', '--preserve=mode,timestamps',
-                '-nRv', source, destination_final_path
-            ]
-            generate_log(
-                log_name_source, 'EVENT = File Transfer, status=started, agentName=OSX - agentName=gcp'
-            )
-            subprocess.call(cmd)
-        # https://github.com/amiaopensource/ltopers/blob/master/writelto#L51
-        else:
-            if rootpos == 'y':
-                if not os.path.isdir(destination + '/' + dirname):
-                    os.makedirs(destination + '/' + dirname)
-                cmd = [
-                    'rsync', '-rtv',
-                    '--exclude=.*', '--exclude=.*/',
-                    '--stats', '--progress',
-                    source, destination + '/' + dirname
-                ]
-            else:
-                cmd = [
-                    'rsync', '-rtv',
-                    '--exclude=.*', '--exclude=.*/',
-                    '--stats', '--progress', source, destination
-                ]
-            generate_log(
-                log_name_source, 'EVENT = File Transfer, status=started, agentName=OSX, agentName=rsync'
-            )
-            print(cmd)
-            subprocess.call(cmd)
-    elif 'linux' in sys.platform:
-        # https://github.com/amiaopensource/ltopers/blob/master/writelto#L51
-        cmd = [
-            'cp', '--preserve=mode,timestamps',
-            '-nRv', source, destination_final_path
-        ]
-        generate_log(
-            log_name_source, 'EVENT = File Transfer, status=started, agentName=Linux, agentName=cp'
-        )
-        subprocess.call(cmd)
-    generate_log(
-                log_name_source,
-                'EVENT = File Transfer, status=completed'
-            )
-
-def diff_report(file1, file2, log_name_source):
-    '''
-    Analyzes checksum manifests in order to find mismatches.
-    '''
-    print('Comparing manifests to verify file transfer')
-    try:
-        with open(file1, 'r') as file1_manifest:
-            sourcelist = file1_manifest.readlines()
-    except UnicodeDecodeError:
-        with open(file1, 'r', encoding='cp1252') as file1_manifest:
-            sourcelist = file1_manifest.readlines()
-    try:
-        with open(file2, 'r') as file2_manifest:
-            destlist = file2_manifest.readlines()
-    except UnicodeDecodeError:
-        with open(file2, 'r') as file2_manifest:
-            destlist = file2_manifest.readlines()
-    for i in sourcelist:
-        if i not in destlist:
-            print(('%s was expected, but a different value was found in destination manifest' % i.rstrip()))
-            generate_log(
-                log_name_source,
-                'ERROR = %s was expected, but a different value was found in destination manifest' % i.rstrip())
-    print(' - End of Diff report\n')
-
-
-def check_extra_files(file1, file2, log_name_source):
-    '''
-    Are there any extra files in the destination directory?
-    '''
-    try:
-        with open(file1, 'r') as file1_manifest:
-            sourcelist = file1_manifest.readlines()
-    except UnicodeDecodeError:
-        with open(file1, 'r', encoding='cp1251') as file1_manifest:
-            sourcelist = file1_manifest.readlines()
-    try:
-        with open(file2, 'r') as file2_manifest:
-            destlist = file2_manifest.readlines()
-    except UnicodeDecodeError:
-        with open(file2, 'r') as file2_manifest:
-            destlist = file2_manifest.readlines()
-    destlist_files = []
-    sourcelist_files = []
-    for dest_files in destlist:
-        destlist_files.append(dest_files[32:])
-    for source_files in sourcelist:
-        sourcelist_files.append(source_files[32:])
-    for i in destlist_files:
-        if i not in sourcelist_files:
-            print(('%s is in your destination manifest but is not in the source manifest' % i.rstrip()))
-            generate_log(
-                log_name_source,
-                'ERROR = %s is in your destination manifest but is not in the source manifest' % i.rstrip())
-    print(' - End of extra file report - if source and destination manifests appear visually identical, perhaps one manifest is utf-8 and the other is cp1252')
-
-
-def check_overwrite(file2check):
-    '''
-    Asks user if they want to overwrite pre-existing manifests.
-    '''
-    if os.path.isfile(file2check):
-        print('A manifest already exists at your destination. Overwrite? Y/N?')
-        overwrite_destination_manifest = ''
-        while overwrite_destination_manifest not in ('Y', 'y', 'N', 'n'):
-            overwrite_destination_manifest = input()
-            if overwrite_destination_manifest not in ('Y', 'y', 'N', 'n'):
-                print('Incorrect input. Please enter Y or N')
-        return overwrite_destination_manifest
-
-
-def manifest_file_count(manifest2check):
-    '''
-    Checks an ixisting manifest for file count and file list
-    '''
-    if os.path.isfile(manifest2check):
-        manifest_files = []
-        print('A manifest already exists - Checking if manifest is up to date')
-        try:
-            with open(manifest2check, "r", encoding='utf-8') as fo:
-                manifest_lines = [line.split(',') for line in fo.readlines()]
-        except UnicodeDecodeError:
-            with open(manifest2check, "r",  encoding='cp1252') as fo:
-                manifest_lines = [line.split(',') for line in fo.readlines()]
-        for line in manifest_lines:
-            manifest_files.append(line[0][34:].rstrip())
-        count_in_manifest = len(manifest_lines)
-        manifest_info = [count_in_manifest, manifest_files]
-    return manifest_info
-
-
-def check_overwrite_dir(dir2check):
-    '''
-    Asks user if they want to overwrite a pre-existing destination directory.
-    '''
-    if os.path.isdir(dir2check):
-        if len(os.listdir(dir2check)) > 1:
-            print('A directory already exists at your destination. Overwrite? Y/N?')
-            overwrite_destination_dir = ''
-            while overwrite_destination_dir not in ('Y', 'y', 'N', 'n'):
-                overwrite_destination_dir = input()
-                if overwrite_destination_dir not in ('Y', 'y', 'N', 'n'):
-                    print('Incorrect input. Please enter Y or N')
-            return overwrite_destination_dir
-        else:
-            print('A directory exists in your destination but it is empty so we shall proceed')
-
-def check_for_sip(args):
-    '''
-    This checks if the input folder contains the actual payload, eg:
-    the UUID folder(containing logs/metadata/objects) and the manifest sidecar.
-    '''
-    remove_bad_files(args, None)
-    for filenames in os.listdir(args):
-        # make sure that it's an IFI SIP.
-        if 'manifest.md5' in filenames:
-            if len(os.listdir(args)) <= 3: # to allow for  the sha512 manifest
-                dircheck = filenames.replace('_manifest.md5', '')
-                if os.path.isdir(os.path.join(args, dircheck)):
-                    return os.path.join(args, dircheck)
-
-
-def setup(args_):
-    '''
-    Sets a bunch of filename variables and parses command line.
-    some examples:
-    if manifest_sidecar = /home/kieranjol/fakeeeeee/fakeeeeee_manifest.md5
-    then manifes_root = /home/kieranjol/fakeeeeee_manifest.md5
-    '''
-    parser = argparse.ArgumentParser(
-        description='Copy directory with checksum comparison'
-                    'and manifest generation.Written by Kieran O\'Leary.')
-    parser.add_argument(
-        'source', help='Input directory'
-    )
-    parser.add_argument(
-        'destination',
-        help='Destination directory'
-    )
-    parser.add_argument(
-        '-l', '-lto',
-        action='store_true',
-        help='use gcp instead of rsync on osx for SPEED on LTO'
-    )
-    parser.add_argument(
-        '-move',
-        action='store_true',
-        help='Move files instead of copying - much faster!'
-    )
-    parser.add_argument(
-        '-justcopy',
-        action='store_true',
-        help='Do not generate destination manifest and verify integrity :('
-    )
-    parser.add_argument(
-        '-y',
-        action='store_true',
-        help='Answers YES to the question: Not enough free space, would you like to continue?'
-    )
-    rootpos = ''
-    dircheck = None
-    args = parser.parse_args(args_)
-    if os.path.isdir(args.source):
-        dircheck = check_for_sip(args.source)
-    if dircheck != None:
-        if os.path.isdir(dircheck):
-            source = check_for_sip(args.source)
-            destination = os.path.join(args.destination, os.path.basename(args.source))
-            os.makedirs(destination)
-    else:
-        source = os.path.abspath(args.source)
-        destination = args.destination
-    normpath = os.path.normpath(source)
-    #is there any benefit to this over os.path.basename
-    dirname = os.path.split(os.path.basename(source))[1]
-    if dirname == '':
-        rootpos = 'y'
-        '''
-        dirname = raw_input(
-            'What do you want your destination folder to be called?\n'
-        )
-        '''
-    relative_path = normpath.split(os.sep)[-1]
-    # or hardcode
-    destination_final_path = os.path.join(destination, dirname)
-    if rootpos == 'y':
-        manifest_destination = os.path.dirname(destination) + '/%s_manifest.md5' % os.path.basename(destination)
-    else:
-        manifest_destination = destination + '/%s_manifest.md5' % dirname
-    if os.path.isfile(manifest_destination):
-        print('Destination manifest already exists')
-    if rootpos == 'y':
-        manifest_filename = '%s_manifest.md5' % os.path.basename(destination)
-    else:
-        manifest_filename = '%s_manifest.md5' % dirname
-    desktop_manifest_dir = make_desktop_manifest_dir()
-    # manifest = desktop manifest, looks like this can get rewritten later.
-    manifest = os.path.join(
-        desktop_manifest_dir, manifest_filename
-    )
-    manifest_sidecar = os.path.join(
-        os.path.dirname(source), relative_path + '_manifest.md5'
-    )
-    manifest_root = source + '/%s_manifest.md5' % os.path.basename(source)
-    log_name_filename = dirname + time.strftime("_%Y_%m_%dT%H_%M_%S")
-    desktop_logs_dir = make_desktop_logs_dir()
-    log_name_source = "%s/%s.log" % (desktop_logs_dir, log_name_filename)
-    generate_log(log_name_source, 'copyit.py started.')
-    ififuncs.generate_log(
-        log_name_source,
-        'eventDetail=copyit.py %s' % ififuncs.get_script_version('copyit.py'))
-    generate_log(log_name_source, 'Source: %s' % source)
-    generate_log(log_name_source, 'Destination: %s'  % destination)
-    print('Checking total size of input folder')
-    total_input_size = ififuncs.get_folder_size(os.path.abspath(args.source))
-    print('Checking if enough space in destination folder')
-    free_space = ififuncs.get_free_space(args.destination)
-    if total_input_size > free_space:
-        print('You do not have enough free space!')
-        if args.y:
-            go_forth_blindly = 'Y'
-        else:
-            go_forth_blindly = ififuncs.ask_yes_no('Would you like to continue anyway? Press Y or N')
-        if go_forth_blindly == 'Y':
-            generate_log(log_name_source, 'You do not have enough free space!, but the user has decided to continue anyhow')
-        else:
-            generate_log(log_name_source, 'You do not have enough free space! - Exiting')
-            sys.exit()
-    return args, rootpos, manifest_sidecar, log_name_source, destination_final_path, manifest_root, manifest_destination, manifest, destination, dirname, desktop_manifest_dir
-
-def overwrite_check(
-        destination, log_name_source,
-        destination_final_path, manifest_destination
-    ):
-    '''
-    Possibly redundant - this launches other overwrite functions.
-    '''
-    try:
-        test_write_capabilities(destination, log_name_source)
-    except OSError:
-        print('You cannot write to your destination!')
-        generate_log(
-            log_name_source,
-            'EVENT = I/O Test - Failure - No write access to destination directory.'
-        )
-        sys.exit()
-    overwrite_destination_manifest = check_overwrite(manifest_destination)
-    overwrite_destination_dir = check_overwrite_dir(destination_final_path)
-    return overwrite_destination_manifest, overwrite_destination_dir
-
-
-def manifest_existence(
-        manifest_root, manifest_sidecar,
-        manifest, source_count, file_list, log_name_source
-    ):
-    '''
-    Checks for the three different kinds of source manifests:
-    Sidecar, desktop and root of drive
-    '''
-    count_in_manifest = 0
-    manifest_files = []
-    proceed = 'n'
-    if os.path.isfile(manifest_root):
-        proceed = 'y'
-        manifest_info = manifest_file_count(manifest_root)
-        count_in_manifest = manifest_info[0]
-        manifest_files = manifest_info[1]
-    elif os.path.isfile(manifest_sidecar):
-        manifest_info = manifest_file_count(manifest_sidecar)
-        proceed = 'y'
-        count_in_manifest = manifest_info[0]
-        manifest_files = manifest_info[1]
-    elif os.path.isfile(manifest):
-        manifest_info = manifest_file_count(manifest)
-        count_in_manifest = manifest_info[0]
-        manifest_files = manifest_info[1]
-        proceed = 'y'
-    if proceed == 'y':
-        if source_count != count_in_manifest:
-            print('checking which files are different')
-            for i in file_list:
-                if i not in manifest_files:
-                    print((i, 'is present in your source directory but not in the source manifest'))
-            for i in manifest_files:
-                if i not in file_list:
-                    print((i, 'is present in manifest but is missing in your source files'))
-            print('This manifest may be outdated as the number of files in your directory does not match the number of files in the manifest')
-            print(('There are', source_count, 'files in your source directory', count_in_manifest, 'in the manifest'))
-            generate_log(log_name_source, 'EVENT = Existing source manifest check - Failure - The number of files in the source directory is not equal to the number of files in the source manifest ')
-            sys.exit()
-    return proceed, count_in_manifest, manifest_files
-
-
-def make_destination_manifest(
-        overwrite_destination_manifest, log_name_source,
-        rootpos, destination_final_path,
-        manifest_destination, destination
-    ):
-    '''
-    Um, write destination manifest
-    '''
-    if overwrite_destination_manifest not in ('N', 'n'):
-        if overwrite_destination_manifest == None:
-            generate_log(
-                log_name_source, 'EVENT = Generating destination manifest: status=started, eventType=message digest calculation, module=hashlib'
-            )
-        else:
-            generate_log(
-                log_name_source,
-                'EVENT = Destination Manifest Overwrite - Destination manifest already exists - Overwriting.'
-            )
-        print('Generating destination manifest')
-        if rootpos == 'y':
-            files_in_manifest = make_manifest(
-                destination_final_path,
-                manifest_destination, os.path.dirname(destination)
-            )
-            generate_log(
-                log_name_source,
-                'EVENT = Generating destination manifest: status=completed'
-            )
-        else:
-            files_in_manifest = make_manifest(
-                destination_final_path,
-                manifest_destination, destination
-            )
-            generate_log(
-                log_name_source,
-                'EVENT = Generating destination manifest: status=completed')
-    else:
-        generate_log(
-            log_name_source,
-            'EVENT = File Transfer Overwrite - Destination directory already exists - Not Overwriting.'
-        )
-    remove_bad_files(destination_final_path, log_name_source)
-    return files_in_manifest
-
-
-def verify_copy(manifest, manifest_destination, log_name_source, overwrite_destination_manifest, files_in_manifest, destination_count, source_count):
-    unicode_mismatch = False
-    try:
-        with open(manifest, 'r', encoding='utf-8') as source_manifest_object:
-            source_manifest_lines = source_manifest_object.read()
-    except UnicodeDecodeError:
-        unicode_mismatch = True
-        with open(manifest, 'r',  encoding='cp1252') as source_manifest_object:
-            source_manifest_lines = source_manifest_object.read()
-    try:
-        with open(manifest_destination, 'r', encoding='utf-8') as destination_manifest_object:
-            destination_manifest_lines = destination_manifest_object.read()
-    except UnicodeDecodeError:
-        unicode_mismatch = True
-        with open(manifest_destination, 'r', encoding='cp1252') as destination_manifest_object:
-            destination_manifest_lines = destination_manifest_object.read()
-    if source_manifest_lines == destination_manifest_lines:
-        print("Your files have reached their destination and the checksums match")
-        generate_log(
-            log_name_source,
-            'EVENT = File Transfer Judgement - Success, eventOutcome=pass'
-        )
-    elif unicode_mismatch is True:
-        print(' - Checking if there is a text encoding mismatch that is triggering a false negative')
-        print(' - Using python to normalise the characters using unicodedata.normalize() purely for comparison')
-        source_manifest_casefolded = unicodedata.normalize('NFD', source_manifest_lines)
-        destination_manifest_casefolded = unicodedata.normalize('NFD', destination_manifest_lines)
-        generate_log(
-            log_name_source,
-            ' Using python to normalise the characters using unicodedata.normalize() purely for comparison'
-        )
-        if source_manifest_casefolded == destination_manifest_casefolded:
-            generate_log(
-                log_name_source,
-                'EVENT = File Transfer Judgement - Success, eventOutcome=pass, eventDetail=source and destination manifests appear to have different encodings and are only identical when compared by eye or when normalized'
-            )
-            print(' - Source and destination manifests appear to have different encodings and are only identical when compared by eye or when normalized')
-    else:
-        print("***********YOUR CHECKSUMS DO NOT MATCH*************")
-        if overwrite_destination_manifest not in ('N', 'n'):
-            generate_log(
-                log_name_source,
-                'EVENT = File Transfer Outcome - Failure, eventOutcome=fail'
-            )
-            print((' There are: \n %s files in your destination manifest \n' % files_in_manifest))
-            print((' %s files in your destination \n %s files at source' % (
-                destination_count, source_count)
-            ))
-            diff_report(manifest, manifest_destination, log_name_source)
-            check_extra_files(manifest, manifest_destination, log_name_source)
-            generate_log(log_name_source, 'EVENT = File Transfer Failure Explanation -  %s files in your destination,  %s files at source' % (destination_count, source_count))
-        else:
-            print((' %s files in your destination \n %s files at source' % (
-                destination_count, source_count)
-            ))
-def control_flow(manifest_sidecar, log_name_source, manifest, rootpos, args, source):
-    if os.path.isfile(manifest_sidecar):
-        print('Manifest Sidecar exists - Source manifest Generation will be skipped.')
-        generate_log(
-            log_name_source,
-            'EVENT = Manifest sidecar exists - source manifest generation will be skipped'
-        )
-        manifest = manifest_sidecar
-    elif not os.path.isfile(manifest):
-        try:
-            print('Generating source manifest')
-            generate_log(log_name_source, 'EVENT = Generating source manifest: status=started, eventType=message digest calculation, module=hashlib')
-            if rootpos == 'y':
-                make_manifest(
-                    os.path.abspath(args.source), manifest, os.path.abspath(args.source)
-                )
-            else:
-                make_manifest(
-                    source, manifest,
-                    os.path.dirname(source)
-                )
-            generate_log(log_name_source, 'EVENT = Generating source manifest: status=completed')
-        except OSError:
-            print('You do not have access to this directory. Perhaps it is read only, perhaps some files or folders have illegal characters, or the wrong file system\n')
-            sys.exit()
-    return manifest_sidecar, manifest, rootpos
-def main(args_):
-    '''
-    Launches the functions that will safely copy and paste your files.
-    '''
-    manifest_temp = '--' # add two characters so that I can slice for manifest_temp[1] later.
-    dircheck = None
-    args, rootpos, manifest_sidecar, log_name_source, destination_final_path, manifest_root, manifest_destination, manifest, destination, dirname, desktop_manifest_dir = setup(args_)
-    if os.path.isdir(args.source):
-        dircheck = check_for_sip(args.source)
-    if dircheck != None:
-        if os.path.isdir(dircheck):
-            source = check_for_sip(args.source)
-    else:
-        source = os.path.abspath(args.source)
-        destination = args.destination
-    overwrite_destination_manifest, overwrite_destination_dir = overwrite_check(
-        destination, log_name_source,
-        destination_final_path, manifest_destination
-    )
-    remove_bad_files(
-        source, log_name_source
-    )
-    source_count, file_list = ififuncs.count_stuff(
-        source
-    )
-    manifest_existence(
-        manifest_root, manifest_sidecar,
-        manifest, source_count,
-        file_list, log_name_source
-    )
-    manifest_sidecar, manifest, rootpos = control_flow(
-        manifest_sidecar, log_name_source, manifest, rootpos, args, source
-    )
-    if overwrite_destination_dir not in ('N', 'n'):
-        if overwrite_destination_dir != None:
-            generate_log(
-                log_name_source,
-                'EVENT = File Transfer Overwrite - Destination directory already exists - Overwriting.'
-            )
-        if not args.move:
-            copy_dir(
-                source, destination_final_path,
-                log_name_source, rootpos, destination, dirname, args
-            )
-        else:
-            shutil.move(source, destination_final_path)
-    else:
-        generate_log(
-            log_name_source,
-            'EVENT = File Transfer Overwrite - Destination directory already exists - Not Overwriting.'
-        )
-    if args.justcopy:
-        generate_log(
-            log_name_source,
-            'EVENT = Exiting without destination manifest or verification due to the use of -justcopy'
-        )
-        print('Exiting without destination manifest or verification due to the use of -justcopy')
-        sys.exit()
-    else:
-        files_in_manifest = make_destination_manifest(
-            overwrite_destination_manifest, log_name_source,
-            rootpos, destination_final_path,
-            manifest_destination,
-            destination
-        )
-        destination_count = 0
-        # dear god do this better, this is dreadful code!
-        for _, _, filenames in os.walk(destination_final_path):
-            for _ in filenames:
-                destination_count += 1 #works in windows at least
-        if rootpos == 'y':
-            manifest_temp = tempfile.mkstemp(
-                dir=desktop_manifest_dir, suffix='.md5'
-            )
-            os.close(manifest_temp[0]) # Needed for windows.
-            with open(manifest, 'r') as fo:
-                dest_manifest_list = fo.readlines()
-                with open(manifest_temp[1], 'w') as temp_object:
-                    for i in dest_manifest_list:
-                        temp_object.write(i[:33] + ' ' + os.path.basename(os.path.dirname(destination_final_path)) + '/' +  i[34:])
-                legacy_manifest = manifest
-                manifest = manifest_temp[1]
-        verify_copy(
-            manifest, manifest_destination, log_name_source, overwrite_destination_manifest, files_in_manifest, destination_count, source_count
-        )
-        manifest_rename = manifest[:-4] + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.md5'
-        if os.path.normpath(os.path.dirname(manifest)) == os.path.normpath(desktop_manifest_dir):
-            os.rename(manifest, manifest_rename)
-            shutil.move(manifest_rename, os.path.join(desktop_manifest_dir, 'old_manifests'))
-            if rootpos == 'y':
-                legacy_manifest_rename = legacy_manifest[:-4] + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.md5'
-                os.rename(legacy_manifest, legacy_manifest_rename)
-                shutil.move(legacy_manifest_rename, os.path.join(desktop_manifest_dir, 'old_manifests'))
-        # hack to also copy the sha512 manifest :(
-        # Stop the temp manifest from copying
-        if not os.path.basename(manifest_temp[1]) == os.path.basename(manifest):
-            sha512_manifest = manifest.replace('_manifest.md5', '_manifest-sha512.txt')
-            if os.path.isfile(sha512_manifest):
-                shutil.copy2(sha512_manifest, os.path.dirname(destination_final_path))
-                print(('%s has been copied to %s' % (sha512_manifest, os.path.dirname(destination_final_path))))
-        return log_name_source
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+
+'''
+Copy pastes drectories while comparing checksum manifests of src and dst.
+'''
+
+import sys
+import subprocess
+import os
+import filecmp
+import tempfile
+import time
+import argparse
+import hashlib
+import shutil
+import unicodedata
+from builtins import input
+import ififuncs
+from ififuncs import make_desktop_logs_dir, make_desktop_manifest_dir, generate_log
+
+
+def hashlib_md5(filename):
+    '''
+    Create an md5 checksum. This should use the ififuncs function instead.
+    '''
+    read_size = 0
+    last_percent_done = 0
+    md5_object = hashlib.md5()
+    total_size = os.path.getsize(filename)
+    with open(str(filename), 'rb') as file_object:
+        while True:
+            buf = file_object.read(2**20)
+            if not buf:
+                break
+            read_size += len(buf)
+            md5_object.update(buf)
+            percent_done = 100 * read_size / total_size
+            if percent_done > last_percent_done:
+                sys.stdout.write('[%d%%]\r' % percent_done)
+                sys.stdout.flush()
+                last_percent_done = percent_done
+    md5_output = md5_object.hexdigest()
+    return md5_output + '  ' + os.path.abspath(filename) +  '\n'
+
+
+def test_write_capabilities(directory, log_name_source):
+    '''
+    Checks if drives have write access.
+    Also checks if source is a file or directory (no file support right now)
+    '''
+    if os.path.isdir(directory):
+        temp = tempfile.mkstemp(dir=directory, suffix='.tmp')
+        os.close(temp[0]) # Needed for windows.
+        os.remove(temp[1])
+    elif os.path.isfile(directory):
+        print('\nFile transfer is not currently supported, only directories.\n')
+        generate_log(
+            log_name_source,
+            'Error: Attempted file transfer. Source and Destination must be a directory'
+        )
+        generate_log(log_name_source, 'move.py exit')
+        sys.exit()
+    else:
+        print((' %s is either not a directory or it does not exist' % directory))
+        generate_log(
+            log_name_source,
+            ' %s is either not a directory or it does not exist' % directory
+        )
+        generate_log(log_name_source, 'move.py exit')
+        sys.exit()
+
+
+def remove_bad_files(root_dir, log_name_source):
+    '''
+    Stolen and adapted from Ben Fino-Radin. Removes annoying files.
+    '''
+    rm_these = ['.DS_Store', 'Thumbs.db', 'desktop.ini', 'Desktop.ini']
+    for root, _, files in os.walk(root_dir):
+        for name in files:
+            path = os.path.join(root, name)
+            for i in rm_these:
+                if name == i:
+                    print(('***********************' + 'removing: ' + path))
+                    if not log_name_source == None:
+                        generate_log(
+                            log_name_source,
+                            'EVENT = Unwanted file removal - %s was removed' % path
+                        )
+                    try:
+                        os.remove(path)
+                    except OSError:
+                        print('can\'t delete as source is read-only')
+
+
+def make_manifest(
+        manifest_dir,
+        manifest_textfile, path_to_remove
+    ):
+    '''
+    Generates a checksum text manifest.
+    '''
+    checksum_list = []
+    manifest_generator = ''
+    source_counter = 0
+    print('Counting the amount of files to be processed.')
+    for root, directories, filenames in os.walk(manifest_dir):
+        directories[:] = [
+            d for d in directories if d[0] != '.'
+        ]
+        directories[:] = [
+            d for d in directories if d != 'System Volume Information'
+        ]
+        directories[:] = [
+                d for d in directories if d != '$RECYCLE.BIN'
+        ]
+        directories[:] = [
+                d for d in directories if d != 'Seagate'
+        ]
+        filenames = [
+            f for f in filenames if os.path.basename(root) != 'System Volume Information'
+        ]
+        filenames = [
+            f for f in filenames if f[0] != '.'
+        ]
+        for files in filenames:
+            source_counter += 1
+    counter2 = 1
+    if os.path.isdir(manifest_dir):
+        os.chdir(manifest_dir)
+        for root, directories, filenames in os.walk(manifest_dir):
+            directories[:] = [
+                d for d in directories if d[0] != '.'
+            ]
+            directories[:] = [
+                d for d in directories if d != 'System Volume Information'
+            ]
+            directories[:] = [
+                d for d in directories if d != '$RECYCLE.BIN'
+            ]
+            directories[:] = [
+                d for d in directories if d != 'Seagate'
+            ]
+            filenames = [
+                f for f in filenames if os.path.basename(root) != 'System Volume Information'
+            ]
+            filenames = [
+                f for f in filenames if f[0] != '.'
+            ]
+            for files in filenames:
+                checksum_list.append([root, files])
+    elif os.path.isfile(manifest_dir):
+        checksum_list = [[os.path.dirname(manifest_dir), os.path.basename(manifest_dir)]]
+    if len(checksum_list) == 1:
+        source_counter = 1
+    for files in checksum_list:
+        print(('Generating MD5 for %s - %d of %d' % (
+            os.path.join(files[0], files[1]), counter2, source_counter)
+            ))
+        md5 = hashlib_md5(os.path.join(files[0], files[1]))
+        root2 = files[0].replace(path_to_remove, '')
+        try:
+            if root2[0] == '/':
+                root2 = root2[1:]
+            if root2[0] == '\\':
+                root2 = root2[1:]
+        except: IndexError
+        manifest_generator += md5[:32] + '  ' + os.path.join(
+            root2, files[1]
+            ).replace("\\", "/") + '\n'
+        counter2 += 1
+    manifest_list = manifest_generator.splitlines()
+    files_in_manifest = len(manifest_list)
+    # http://stackoverflow.com/a/31306961/2188572
+    manifest_list = sorted(manifest_list, key=lambda x: (x[34:]))
+    with open(manifest_textfile, "w", encoding='utf-8') as text:
+        for i in manifest_list:
+            text.write(i + '\n')
+    return files_in_manifest
+
+
+def copy_dir(
+        source, destination_final_path,
+        log_name_source, rootpos, destination, dirname, args
+    ):
+    '''
+    Depending on which operating system is running the script, system tools
+    are launched that copy paste source files to destination.
+    '''
+    if sys.platform == "win32":
+        if os.path.isfile(source):
+            generate_log(
+                log_name_source,
+                'EVENT = File Transfer, status=started, agentName=Windows, module=shutil.copy2'
+            )
+            print('copying file with python/shutil')
+            shutil.copy2(source, destination_final_path)
+        else:
+            subprocess.call([
+                'robocopy', source,
+                destination_final_path,
+                '/E', '/XA:SH',
+                '/XD', '.*',
+                '/XD', '*System Volume Information*',
+                '/XD', 'Seagate',
+                '/XD', '$Recycle.bin', '/a-:SH', '/a+:R'
+            ])
+            generate_log(
+                log_name_source,
+                'EVENT = File Transfer, status=started, agentName=Windows O.S, agentName=Robocopy'
+            )
+    elif sys.platform == "darwin":
+        if args.l:
+            cmd = [
+                'gcp', '--preserve=mode,timestamps',
+                '-nRv', source, destination_final_path
+            ]
+            generate_log(
+                log_name_source, 'EVENT = File Transfer, status=started, agentName=OSX - agentName=gcp'
+            )
+            subprocess.call(cmd)
+        # https://github.com/amiaopensource/ltopers/blob/master/writelto#L51
+        else:
+            if rootpos == 'y':
+                if not os.path.isdir(destination + '/' + dirname):
+                    os.makedirs(destination + '/' + dirname)
+                cmd = [
+                    'rsync', '-rtv',
+                    '--exclude=.*', '--exclude=.*/',
+                    '--stats', '--progress',
+                    source, destination + '/' + dirname
+                ]
+            else:
+                cmd = [
+                    'rsync', '-rtv',
+                    '--exclude=.*', '--exclude=.*/',
+                    '--stats', '--progress', source, destination
+                ]
+            generate_log(
+                log_name_source, 'EVENT = File Transfer, status=started, agentName=OSX, agentName=rsync'
+            )
+            print(cmd)
+            subprocess.call(cmd)
+    elif 'linux' in sys.platform:
+        # https://github.com/amiaopensource/ltopers/blob/master/writelto#L51
+        cmd = [
+            'cp', '--preserve=mode,timestamps',
+            '-nRv', source, destination_final_path
+        ]
+        generate_log(
+            log_name_source, 'EVENT = File Transfer, status=started, agentName=Linux, agentName=cp'
+        )
+        subprocess.call(cmd)
+    generate_log(
+                log_name_source,
+                'EVENT = File Transfer, status=completed'
+            )
+
+def diff_report(file1, file2, log_name_source):
+    '''
+    Analyzes checksum manifests in order to find mismatches.
+    '''
+    print('Comparing manifests to verify file transfer')
+    try:
+        with open(file1, 'r') as file1_manifest:
+            sourcelist = file1_manifest.readlines()
+    except UnicodeDecodeError:
+        with open(file1, 'r', encoding='cp1252') as file1_manifest:
+            sourcelist = file1_manifest.readlines()
+    try:
+        with open(file2, 'r') as file2_manifest:
+            destlist = file2_manifest.readlines()
+    except UnicodeDecodeError:
+        with open(file2, 'r') as file2_manifest:
+            destlist = file2_manifest.readlines()
+    for i in sourcelist:
+        if i not in destlist:
+            print(('%s was expected, but a different value was found in destination manifest' % i.rstrip()))
+            generate_log(
+                log_name_source,
+                'ERROR = %s was expected, but a different value was found in destination manifest' % i.rstrip())
+    print(' - End of Diff report\n')
+
+
+def check_extra_files(file1, file2, log_name_source):
+    '''
+    Are there any extra files in the destination directory?
+    '''
+    try:
+        with open(file1, 'r') as file1_manifest:
+            sourcelist = file1_manifest.readlines()
+    except UnicodeDecodeError:
+        with open(file1, 'r', encoding='cp1251') as file1_manifest:
+            sourcelist = file1_manifest.readlines()
+    try:
+        with open(file2, 'r') as file2_manifest:
+            destlist = file2_manifest.readlines()
+    except UnicodeDecodeError:
+        with open(file2, 'r') as file2_manifest:
+            destlist = file2_manifest.readlines()
+    destlist_files = []
+    sourcelist_files = []
+    for dest_files in destlist:
+        destlist_files.append(dest_files[32:])
+    for source_files in sourcelist:
+        sourcelist_files.append(source_files[32:])
+    for i in destlist_files:
+        if i not in sourcelist_files:
+            print(('%s is in your destination manifest but is not in the source manifest' % i.rstrip()))
+            generate_log(
+                log_name_source,
+                'ERROR = %s is in your destination manifest but is not in the source manifest' % i.rstrip())
+    print(' - End of extra file report - if source and destination manifests appear visually identical, perhaps one manifest is utf-8 and the other is cp1252')
+
+
+def check_overwrite(file2check):
+    '''
+    Asks user if they want to overwrite pre-existing manifests.
+    '''
+    if os.path.isfile(file2check):
+        print('A manifest already exists at your destination. Overwrite? Y/N?')
+        overwrite_destination_manifest = ''
+        while overwrite_destination_manifest not in ('Y', 'y', 'N', 'n'):
+            overwrite_destination_manifest = input()
+            if overwrite_destination_manifest not in ('Y', 'y', 'N', 'n'):
+                print('Incorrect input. Please enter Y or N')
+        return overwrite_destination_manifest
+
+
+def manifest_file_count(manifest2check):
+    '''
+    Checks an ixisting manifest for file count and file list
+    '''
+    if os.path.isfile(manifest2check):
+        manifest_files = []
+        print('A manifest already exists - Checking if manifest is up to date')
+        try:
+            with open(manifest2check, "r", encoding='utf-8') as fo:
+                manifest_lines = [line.split(',') for line in fo.readlines()]
+        except UnicodeDecodeError:
+            with open(manifest2check, "r",  encoding='cp1252') as fo:
+                manifest_lines = [line.split(',') for line in fo.readlines()]
+        for line in manifest_lines:
+            manifest_files.append(line[0][34:].rstrip())
+        count_in_manifest = len(manifest_lines)
+        manifest_info = [count_in_manifest, manifest_files]
+    return manifest_info
+
+
+def check_overwrite_dir(dir2check):
+    '''
+    Asks user if they want to overwrite a pre-existing destination directory.
+    '''
+    if os.path.isdir(dir2check):
+        if len(os.listdir(dir2check)) > 1:
+            print('A directory already exists at your destination. Overwrite? Y/N?')
+            overwrite_destination_dir = ''
+            while overwrite_destination_dir not in ('Y', 'y', 'N', 'n'):
+                overwrite_destination_dir = input()
+                if overwrite_destination_dir not in ('Y', 'y', 'N', 'n'):
+                    print('Incorrect input. Please enter Y or N')
+            return overwrite_destination_dir
+        else:
+            print('A directory exists in your destination but it is empty so we shall proceed')
+
+def check_for_sip(args):
+    '''
+    This checks if the input folder contains the actual payload, eg:
+    the UUID folder(containing logs/metadata/objects) and the manifest sidecar.
+    '''
+    remove_bad_files(args, None)
+    for filenames in os.listdir(args):
+        # make sure that it's an IFI SIP.
+        if 'manifest.md5' in filenames:
+            if len(os.listdir(args)) <= 3: # to allow for  the sha512 manifest
+                dircheck = filenames.replace('_manifest.md5', '')
+                if os.path.isdir(os.path.join(args, dircheck)):
+                    return os.path.join(args, dircheck)
+
+
+def setup(args_):
+    '''
+    Sets a bunch of filename variables and parses command line.
+    some examples:
+    if manifest_sidecar = /home/kieranjol/fakeeeeee/fakeeeeee_manifest.md5
+    then manifes_root = /home/kieranjol/fakeeeeee_manifest.md5
+    '''
+    parser = argparse.ArgumentParser(
+        description='Copy directory with checksum comparison'
+                    'and manifest generation.Written by Kieran O\'Leary.')
+    parser.add_argument(
+        'source', help='Input directory'
+    )
+    parser.add_argument(
+        'destination',
+        help='Destination directory'
+    )
+    parser.add_argument(
+        '-l', '-lto',
+        action='store_true',
+        help='use gcp instead of rsync on osx for SPEED on LTO'
+    )
+    parser.add_argument(
+        '-move',
+        action='store_true',
+        help='Move files instead of copying - much faster!'
+    )
+    parser.add_argument(
+        '-justcopy',
+        action='store_true',
+        help='Do not generate destination manifest and verify integrity :('
+    )
+    parser.add_argument(
+        '-y',
+        action='store_true',
+        help='Answers YES to the question: Not enough free space, would you like to continue?'
+    )
+    rootpos = ''
+    dircheck = None
+    args = parser.parse_args(args_)
+    if os.path.isdir(args.source):
+        dircheck = check_for_sip(args.source)
+    if dircheck != None:
+        if os.path.isdir(dircheck):
+            source = check_for_sip(args.source)
+            destination = os.path.join(args.destination, os.path.basename(args.source))
+            os.makedirs(destination)
+    else:
+        source = os.path.abspath(args.source)
+        destination = args.destination
+    normpath = os.path.normpath(source)
+    #is there any benefit to this over os.path.basename
+    dirname = os.path.split(os.path.basename(source))[1]
+    if dirname == '':
+        rootpos = 'y'
+        '''
+        dirname = raw_input(
+            'What do you want your destination folder to be called?\n'
+        )
+        '''
+    relative_path = normpath.split(os.sep)[-1]
+    # or hardcode
+    destination_final_path = os.path.join(destination, dirname)
+    if rootpos == 'y':
+        manifest_destination = os.path.dirname(destination) + '/%s_manifest.md5' % os.path.basename(destination)
+    else:
+        manifest_destination = destination + '/%s_manifest.md5' % dirname
+    if os.path.isfile(manifest_destination):
+        print('Destination manifest already exists')
+    if rootpos == 'y':
+        manifest_filename = '%s_manifest.md5' % os.path.basename(destination)
+    else:
+        manifest_filename = '%s_manifest.md5' % dirname
+    desktop_manifest_dir = make_desktop_manifest_dir()
+    # manifest = desktop manifest, looks like this can get rewritten later.
+    manifest = os.path.join(
+        desktop_manifest_dir, manifest_filename
+    )
+    manifest_sidecar = os.path.join(
+        os.path.dirname(source), relative_path + '_manifest.md5'
+    )
+    manifest_root = source + '/%s_manifest.md5' % os.path.basename(source)
+    log_name_filename = dirname + time.strftime("_%Y_%m_%dT%H_%M_%S")
+    desktop_logs_dir = make_desktop_logs_dir()
+    log_name_source = "%s/%s.log" % (desktop_logs_dir, log_name_filename)
+    generate_log(log_name_source, 'copyit.py started.')
+    ififuncs.generate_log(
+        log_name_source,
+        'eventDetail=copyit.py %s' % ififuncs.get_script_version('copyit.py'))
+    generate_log(log_name_source, 'Source: %s' % source)
+    generate_log(log_name_source, 'Destination: %s'  % destination)
+    print('Checking total size of input folder')
+    total_input_size = ififuncs.get_folder_size(os.path.abspath(args.source))
+    print('Checking if enough space in destination folder')
+    free_space = ififuncs.get_free_space(args.destination)
+    if total_input_size > free_space:
+        print('You do not have enough free space!')
+        if args.y:
+            go_forth_blindly = 'Y'
+        else:
+            go_forth_blindly = ififuncs.ask_yes_no('Would you like to continue anyway? Press Y or N')
+        if go_forth_blindly == 'Y':
+            generate_log(log_name_source, 'You do not have enough free space!, but the user has decided to continue anyhow')
+        else:
+            generate_log(log_name_source, 'You do not have enough free space! - Exiting')
+            sys.exit()
+    return args, rootpos, manifest_sidecar, log_name_source, destination_final_path, manifest_root, manifest_destination, manifest, destination, dirname, desktop_manifest_dir
+
+def overwrite_check(
+        destination, log_name_source,
+        destination_final_path, manifest_destination
+    ):
+    '''
+    Possibly redundant - this launches other overwrite functions.
+    '''
+    try:
+        test_write_capabilities(destination, log_name_source)
+    except OSError:
+        print('You cannot write to your destination!')
+        generate_log(
+            log_name_source,
+            'EVENT = I/O Test - Failure - No write access to destination directory.'
+        )
+        sys.exit()
+    overwrite_destination_manifest = check_overwrite(manifest_destination)
+    overwrite_destination_dir = check_overwrite_dir(destination_final_path)
+    return overwrite_destination_manifest, overwrite_destination_dir
+
+
+def manifest_existence(
+        manifest_root, manifest_sidecar,
+        manifest, source_count, file_list, log_name_source
+    ):
+    '''
+    Checks for the three different kinds of source manifests:
+    Sidecar, desktop and root of drive
+    '''
+    count_in_manifest = 0
+    manifest_files = []
+    proceed = 'n'
+    if os.path.isfile(manifest_root):
+        proceed = 'y'
+        manifest_info = manifest_file_count(manifest_root)
+        count_in_manifest = manifest_info[0]
+        manifest_files = manifest_info[1]
+    elif os.path.isfile(manifest_sidecar):
+        manifest_info = manifest_file_count(manifest_sidecar)
+        proceed = 'y'
+        count_in_manifest = manifest_info[0]
+        manifest_files = manifest_info[1]
+    elif os.path.isfile(manifest):
+        manifest_info = manifest_file_count(manifest)
+        count_in_manifest = manifest_info[0]
+        manifest_files = manifest_info[1]
+        proceed = 'y'
+    if proceed == 'y':
+        if source_count != count_in_manifest:
+            print('checking which files are different')
+            for i in file_list:
+                if i not in manifest_files:
+                    print((i, 'is present in your source directory but not in the source manifest'))
+            for i in manifest_files:
+                if i not in file_list:
+                    print((i, 'is present in manifest but is missing in your source files'))
+            print('This manifest may be outdated as the number of files in your directory does not match the number of files in the manifest')
+            print(('There are', source_count, 'files in your source directory', count_in_manifest, 'in the manifest'))
+            generate_log(log_name_source, 'EVENT = Existing source manifest check - Failure - The number of files in the source directory is not equal to the number of files in the source manifest ')
+            sys.exit()
+    return proceed, count_in_manifest, manifest_files
+
+
+def make_destination_manifest(
+        overwrite_destination_manifest, log_name_source,
+        rootpos, destination_final_path,
+        manifest_destination, destination
+    ):
+    '''
+    Um, write destination manifest
+    '''
+    if overwrite_destination_manifest not in ('N', 'n'):
+        if overwrite_destination_manifest == None:
+            generate_log(
+                log_name_source, 'EVENT = Generating destination manifest: status=started, eventType=message digest calculation, module=hashlib'
+            )
+        else:
+            generate_log(
+                log_name_source,
+                'EVENT = Destination Manifest Overwrite - Destination manifest already exists - Overwriting.'
+            )
+        print('Generating destination manifest')
+        if rootpos == 'y':
+            files_in_manifest = make_manifest(
+                destination_final_path,
+                manifest_destination, os.path.dirname(destination)
+            )
+            generate_log(
+                log_name_source,
+                'EVENT = Generating destination manifest: status=completed'
+            )
+        else:
+            files_in_manifest = make_manifest(
+                destination_final_path,
+                manifest_destination, destination
+            )
+            generate_log(
+                log_name_source,
+                'EVENT = Generating destination manifest: status=completed')
+    else:
+        generate_log(
+            log_name_source,
+            'EVENT = File Transfer Overwrite - Destination directory already exists - Not Overwriting.'
+        )
+    remove_bad_files(destination_final_path, log_name_source)
+    return files_in_manifest
+
+
+def verify_copy(manifest, manifest_destination, log_name_source, overwrite_destination_manifest, files_in_manifest, destination_count, source_count):
+    unicode_mismatch = False
+    try:
+        with open(manifest, 'r', encoding='utf-8') as source_manifest_object:
+            source_manifest_lines = source_manifest_object.read()
+    except UnicodeDecodeError:
+        unicode_mismatch = True
+        with open(manifest, 'r',  encoding='cp1252') as source_manifest_object:
+            source_manifest_lines = source_manifest_object.read()
+    try:
+        with open(manifest_destination, 'r', encoding='utf-8') as destination_manifest_object:
+            destination_manifest_lines = destination_manifest_object.read()
+    except UnicodeDecodeError:
+        unicode_mismatch = True
+        with open(manifest_destination, 'r', encoding='cp1252') as destination_manifest_object:
+            destination_manifest_lines = destination_manifest_object.read()
+    if source_manifest_lines == destination_manifest_lines:
+        print("Your files have reached their destination and the checksums match")
+        generate_log(
+            log_name_source,
+            'EVENT = File Transfer Judgement - Success, eventOutcome=pass'
+        )
+    elif unicode_mismatch is True:
+        print(' - Checking if there is a text encoding mismatch that is triggering a false negative')
+        print(' - Using python to normalise the characters using unicodedata.normalize() purely for comparison')
+        source_manifest_casefolded = unicodedata.normalize('NFD', source_manifest_lines)
+        destination_manifest_casefolded = unicodedata.normalize('NFD', destination_manifest_lines)
+        generate_log(
+            log_name_source,
+            ' Using python to normalise the characters using unicodedata.normalize() purely for comparison'
+        )
+        if source_manifest_casefolded == destination_manifest_casefolded:
+            generate_log(
+                log_name_source,
+                'EVENT = File Transfer Judgement - Success, eventOutcome=pass, eventDetail=source and destination manifests appear to have different encodings and are only identical when compared by eye or when normalized'
+            )
+            print(' - Source and destination manifests appear to have different encodings and are only identical when compared by eye or when normalized')
+    else:
+        print("***********YOUR CHECKSUMS DO NOT MATCH*************")
+        if overwrite_destination_manifest not in ('N', 'n'):
+            generate_log(
+                log_name_source,
+                'EVENT = File Transfer Outcome - Failure, eventOutcome=fail'
+            )
+            print((' There are: \n %s files in your destination manifest \n' % files_in_manifest))
+            print((' %s files in your destination \n %s files at source' % (
+                destination_count, source_count)
+            ))
+            diff_report(manifest, manifest_destination, log_name_source)
+            check_extra_files(manifest, manifest_destination, log_name_source)
+            generate_log(log_name_source, 'EVENT = File Transfer Failure Explanation -  %s files in your destination,  %s files at source' % (destination_count, source_count))
+        else:
+            print((' %s files in your destination \n %s files at source' % (
+                destination_count, source_count)
+            ))
+def control_flow(manifest_sidecar, log_name_source, manifest, rootpos, args, source):
+    if os.path.isfile(manifest_sidecar):
+        print('Manifest Sidecar exists - Source manifest Generation will be skipped.')
+        generate_log(
+            log_name_source,
+            'EVENT = Manifest sidecar exists - source manifest generation will be skipped'
+        )
+        manifest = manifest_sidecar
+    elif not os.path.isfile(manifest):
+        try:
+            print('Generating source manifest')
+            generate_log(log_name_source, 'EVENT = Generating source manifest: status=started, eventType=message digest calculation, module=hashlib')
+            if rootpos == 'y':
+                make_manifest(
+                    os.path.abspath(args.source), manifest, os.path.abspath(args.source)
+                )
+            else:
+                make_manifest(
+                    source, manifest,
+                    os.path.dirname(source)
+                )
+            generate_log(log_name_source, 'EVENT = Generating source manifest: status=completed')
+        except OSError:
+            print('You do not have access to this directory. Perhaps it is read only, perhaps some files or folders have illegal characters, or the wrong file system\n')
+            sys.exit()
+    return manifest_sidecar, manifest, rootpos
+def main(args_):
+    '''
+    Launches the functions that will safely copy and paste your files.
+    '''
+    manifest_temp = '--' # add two characters so that I can slice for manifest_temp[1] later.
+    dircheck = None
+    args, rootpos, manifest_sidecar, log_name_source, destination_final_path, manifest_root, manifest_destination, manifest, destination, dirname, desktop_manifest_dir = setup(args_)
+    if os.path.isdir(args.source):
+        dircheck = check_for_sip(args.source)
+    if dircheck != None:
+        if os.path.isdir(dircheck):
+            source = check_for_sip(args.source)
+    else:
+        source = os.path.abspath(args.source)
+        destination = args.destination
+    overwrite_destination_manifest, overwrite_destination_dir = overwrite_check(
+        destination, log_name_source,
+        destination_final_path, manifest_destination
+    )
+    remove_bad_files(
+        source, log_name_source
+    )
+    source_count, file_list = ififuncs.count_stuff(
+        source
+    )
+    manifest_existence(
+        manifest_root, manifest_sidecar,
+        manifest, source_count,
+        file_list, log_name_source
+    )
+    manifest_sidecar, manifest, rootpos = control_flow(
+        manifest_sidecar, log_name_source, manifest, rootpos, args, source
+    )
+    if overwrite_destination_dir not in ('N', 'n'):
+        if overwrite_destination_dir != None:
+            generate_log(
+                log_name_source,
+                'EVENT = File Transfer Overwrite - Destination directory already exists - Overwriting.'
+            )
+        if not args.move:
+            copy_dir(
+                source, destination_final_path,
+                log_name_source, rootpos, destination, dirname, args
+            )
+        else:
+            shutil.move(source, destination_final_path)
+    else:
+        generate_log(
+            log_name_source,
+            'EVENT = File Transfer Overwrite - Destination directory already exists - Not Overwriting.'
+        )
+    if args.justcopy:
+        generate_log(
+            log_name_source,
+            'EVENT = Exiting without destination manifest or verification due to the use of -justcopy'
+        )
+        print('Exiting without destination manifest or verification due to the use of -justcopy')
+        sys.exit()
+    else:
+        files_in_manifest = make_destination_manifest(
+            overwrite_destination_manifest, log_name_source,
+            rootpos, destination_final_path,
+            manifest_destination,
+            destination
+        )
+        destination_count = 0
+        # dear god do this better, this is dreadful code!
+        for _, _, filenames in os.walk(destination_final_path):
+            for _ in filenames:
+                destination_count += 1 #works in windows at least
+        if rootpos == 'y':
+            manifest_temp = tempfile.mkstemp(
+                dir=desktop_manifest_dir, suffix='.md5'
+            )
+            os.close(manifest_temp[0]) # Needed for windows.
+            with open(manifest, 'r') as fo:
+                dest_manifest_list = fo.readlines()
+                with open(manifest_temp[1], 'w') as temp_object:
+                    for i in dest_manifest_list:
+                        temp_object.write(i[:33] + ' ' + os.path.basename(os.path.dirname(destination_final_path)) + '/' +  i[34:])
+                legacy_manifest = manifest
+                manifest = manifest_temp[1]
+        verify_copy(
+            manifest, manifest_destination, log_name_source, overwrite_destination_manifest, files_in_manifest, destination_count, source_count
+        )
+        manifest_rename = manifest[:-4] + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.md5'
+        if os.path.normpath(os.path.dirname(manifest)) == os.path.normpath(desktop_manifest_dir):
+            os.rename(manifest, manifest_rename)
+            shutil.move(manifest_rename, os.path.join(desktop_manifest_dir, 'old_manifests'))
+            if rootpos == 'y':
+                legacy_manifest_rename = legacy_manifest[:-4] + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.md5'
+                os.rename(legacy_manifest, legacy_manifest_rename)
+                shutil.move(legacy_manifest_rename, os.path.join(desktop_manifest_dir, 'old_manifests'))
+        # hack to also copy the sha512 manifest :(
+        # Stop the temp manifest from copying
+        if not os.path.basename(manifest_temp[1]) == os.path.basename(manifest):
+            sha512_manifest = manifest.replace('_manifest.md5', '_manifest-sha512.txt')
+            if os.path.isfile(sha512_manifest):
+                shutil.copy2(sha512_manifest, os.path.dirname(destination_final_path))
+                print(('%s has been copied to %s' % (sha512_manifest, os.path.dirname(destination_final_path))))
+        return log_name_source
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/dcpaccess.py` & `ifiscripts-2023.7.3.2/scripts/dcpaccess.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,519 +1,519 @@
-#!/usr/bin/env python
-
-import sys
-try:
-    from lxml import etree
-except ImportError:
-    print ('*** ERROR - LXML IS MISSING ***\nThis external module is required for xml parsing.\nInstall with  `pip install lxml`.\nYou may need to restart your terminal or your computer, but it should work immediately.\nYou may need to run `sudo pip install lxml` on some osx/linux machines.\n If having issues installing lxml on windows, download the relevant .whl file from here http://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml and run `pip install /path/to/lxml_filename.whl')
-    sys.exit()
-import pdb
-from glob import glob
-import csv
-import os
-from os import listdir
-from os.path import isfile, join
-import subprocess
-import base64
-import time
-import re
-import smtplib
-import argparse
-import mimetypes
-from email.mime.multipart import MIMEMultipart
-from email import encoders
-from email.message import Message
-from email.mime.audio import MIMEAudio
-from email.mime.base import MIMEBase
-from email.mime.image import MIMEImage
-from email.mime.text import MIMEText
-import tempfile
-from decimal import *
-from sys import platform as _platform
-getcontext().prec = 4
-
-# Use argparse for command line options.
-parser = argparse.ArgumentParser(description='Unencrypted DCP to H264 transcoder.'
-                                 ' Written by Kieran O\'Leary.')
-parser.add_argument('input')
-'''
-parser.add_argument(
-                    '-bag', 
-                    action='store_true',help='bag the dcp_dir if it passes the hash check')
-'''
-parser.add_argument(
-                    '-m', 
-                    action='store_true',help='send email report')
-parser.add_argument(
-                    '-s', 
-                    action='store_true',help='Burn in subtitles. This will take a long time. It makes more sense to make a clean copy first, then make subtitled surrogates from that new copy. Jpeg2000 decoding is slow, ProRes or h264 is significantly faster.')
-parser.add_argument(
-                    '-p', 
-                    action='store_true',help='Use Apple ProRes 4:2:2 HQ instead of H264')
-parser.add_argument(
-                    '-hd',
-                    action='store_true',help='Scale to 1920:1080 while preserving the aspect ratio')
-parser.add_argument(
-                    '-lowres',
-                    help='[0,1,2]Use the jpeg2000 lowres option for rescaling and speed increases. Accepts a value of 0 (original size), 1 (50 PERCENT size), 2 (25 PERCENT size)')
-args = parser.parse_args()
-'''
-if args.bag:
-    bagging = 'enabled'
-else:
-    bagging = 'disabled'
-'''
-ififuncs.check_existence(['ffprobe', 'ffmpeg'])
-if args.m:
-    email = 'enabled'
-else:
-    email = 'disabled'
-if args.s:
-    print( '***********************************************')
-    print ('You have chosen to burn in subtitles. This will take a long time. A better approach may be to make a clean transcode to a high quality format such as PRORES and make further clean or subtitled surrogates from that new copy. ')
-    print ('***********************************************')
-    time.sleep(1)
-lut_path = os.path.join(os.path.abspath(os.path.dirname(sys.argv[0])), '26_XYZ-22_Rec709.cube')
-# Set a bunch of variables for filenaming.    
-dcp_dir               = args.input
-# This temp directory should work on all operating systems. 
-temp_dir              = tempfile.gettempdir()
-video_concat_filename = os.path.basename(dcp_dir) + '_video_concat' + time.strftime("_%Y_%m_%dT%H_%M_%S")
-audio_concat_filename = os.path.basename(dcp_dir) + '_audio_concat' + time.strftime("_%Y_%m_%dT%H_%M_%S")
-# Slashes are significant for ffmpeg concat files.
-if _platform == "win32":
-    video_concat_textfile = os.path.expanduser("~\Desktop\%s.txt") % video_concat_filename
-    audio_concat_textfile = os.path.expanduser("~\Desktop\%s.txt") % audio_concat_filename
-else:
-    video_concat_textfile = temp_dir + "/%s.txt" % video_concat_filename
-    audio_concat_textfile = temp_dir + "/%s.txt" % audio_concat_filename
-    
-
-def find_assetmap():   
-    if 'ASSETMAP' in dcp_files:
-        assetmap = 'ASSETMAP'
-    elif 'ASSETMAP.xml' in dcp_files:
-        assetmap = 'ASSETMAP.xml'
-    return assetmap
-        
-        
-# Begin recursive search through sub-directories for DCPs.  
-def choose_cpl(): 
-    global cpl_list
-    # Some DCPs have multiple CPLs!       
-    cpl_number = 1
-    print ('Multiple CPL files found')
-    for i in cpl_list:
-        print (cpl_number,  i)
-        cpl_number += 1   
-    print( 'Please select which CPL you would like to process')
-    chosen_cpl = raw_input()
-    cpl_parse = etree.parse(cpl_list[int(chosen_cpl) - 1]) # The -1 is due to python zero-indexing.
-    if args.s:
-        cpl_namespace      = cpl_parse.xpath('namespace-uri(.)') 
-        subtitle_language  =  cpl_parse.findall('//ns:MainSubtitle/ns:Language',namespaces={'ns': cpl_namespace})
-        print( 'This CPL contains ', subtitle_language[0].text, ' subtitles. Proceed?')         
-    return cpl_parse 
-    
-    
-def find_cpl():
-    # Generate an empty list as there may be multiple CPLs.    
-    # Get a list of all XML files in the main DCP directory.
-    xmlfiles = glob('*.xml')
-    # Loop through xmlfiles in order to find any CPLL files.
-    for i in xmlfiles:
-        try:  
-            xmlname = etree.parse(i)
-        except SyntaxError:
-            print( 'not a valid CPL!')
-            continue
-        except KeyError:
-            print( 'Missing CPL!')
-            continue
-        xml_namespace = xmlname.xpath('namespace-uri(.)')
-        # Create list of CPLs.
-        if 'CPL' in xml_namespace:
-            cpl_list.append(i) 
-        if len(cpl_list) == 0:  
-            continue
-        elif len(cpl_list) == 1:
-            cpl_parse = etree.parse(cpl_list[0])
-    if len(cpl_list) > 1:
-        cpl_parse = choose_cpl() 
-        # As there can be multiple subtitles, This options gives some info/choice.
-        subs_confirmation  = raw_input('Y/N')       
-        while subs_confirmation not in ['Y','y']:
-            cpl_parse = choose_cpl()
-            subs_confirmation  = raw_input('Y/N')    
-            return cpl_parse
-        return cpl_parse    
-    else:
-        return cpl_parse  
-
-        
-def delay_check(media_type,cpl_parse, cpl_namespace ):
-    # Check if there is an intended audio delay.
-    count   = cpl_parse.xpath('count(//ns:%s/ns:EntryPoint)' % media_type,namespaces={'ns': cpl_namespace} )
-    xmluuid_list               = cpl_parse.xpath('//ns:%s/ns:Id' % media_type,namespaces={'ns': cpl_namespace})
-    EntryPoint_list            = cpl_parse.xpath('//ns:%s/ns:EntryPoint' % media_type,namespaces={'ns': cpl_namespace})
-    dur_list                   = cpl_parse.xpath('//ns:%s/ns:Duration' % media_type,namespaces={'ns': cpl_namespace})
-    dur_intrinsic_list         = cpl_parse.xpath('//ns:%s/ns:IntrinsicDuration' % media_type,namespaces={'ns': cpl_namespace})
-    counter = 0
-    delays  = 0
-    audio_delay = {}
-    while counter < count:
-        audio_delay_values = []
-        xmluuid = xmluuid_list[counter]
-        EntryPoint = EntryPoint_list[counter]
-        entrypoint_audio      = float(EntryPoint.text)
-        if EntryPoint.text != '0':
-            delays += 1
-            # EntryPoint is in frames. The following converts to seconds.
-            entrypoint_audio  = float(EntryPoint.text) 
-            entrypoint_audio  = float(entrypoint_audio) / float(fps) # Change to EditRate variable.
-            entrypoint_audio  = round(entrypoint_audio, 3)
-        audio_delay_values.append(entrypoint_audio) 
-        dur                   = dur_list[counter]
-        dur_intrinsic         = dur_intrinsic_list[counter]
-        tail_test             = int(dur_intrinsic.text) - int(dur.text)
-        if tail_test > 0:
-            delays +=1
-        tail_delay = int(dur.text)
-        tail_delay = float(tail_delay) / float(fps)
-        tail_delay = round(tail_delay, 3)
-        audio_delay_values.append(tail_delay)
-        audio_delay_values.append(file_paths[xmluuid.text][0])
-        # audio_delay stores [entrypoint, tail_delay, file_path]
-        audio_delay[xmluuid.text] = audio_delay_values
-        counter += 1
-    test_list = []
-    test_list.append(audio_delay)
-    test_list.append(delays)
-    return test_list
-            
-            
-def burn_subs():
-    counter = 0
-    subs_counter = 0
-    count = len(subs)
-    sub_delay = 1
-    if not len(subs) == len(pic_mxfs):
-        print('The amount of picture files does not equal the amount of subtitles. This feature is not supported yet. Sorry!')
-        sub_delay = 0
-        # This assumes that if there are less subtitles than video files, it's because there's an extra AV reel at the head.A more robust option will be added later. Right now this fixes the one use case I've seen.
-    if delays != 0:
-        for i in audio_delay:
-            # Wrapping PCM in matroska as WAV has 4 gig limit.
-            subprocess.call(['ffmpeg','-ss',str(audio_delay[i][0]),
-            '-i',audio_delay[i][2],'-t',str(audio_delay[i][1]),
-            '-c:a','copy', temp_dir + '/'+ audio_delay[i][2] + '.mkv'])    
-    while counter < count:
-        srt_file = temp_dir + '/' + os.path.basename(subs[subs_counter]) +'.srt'
-        output_filename = os.path.basename(dcp_dir) + '_subs_reel' + str(counter + 1) + time.strftime("_%Y_%m_%dT%H_%M_%S")
-        output_subs_mkv = os.path.expanduser("~/Desktop/%s.mkv") % output_filename
-        try:  
-            xmlo = etree.parse(subs[subs_counter])
-        except SyntaxError:
-            if 'mxf' in srt_file:
-                print('Subtitle file is most likely an SMPTE MXF which is not currently supported.')
-            else:
-                print ('not a valid CPL!')
-            counter +=1
-            continue
-        except KeyError:
-            print ('Missing CPL!')
-            counter +=1
-            continue
-        sub_count = int(xmlo.xpath('count(//Subtitle)'))
-        current_sub_counter = 0
-        with open(srt_file, "w") as myfile:
-               print ('Transforming ', sub_count, 'subtitles')
-        while current_sub_counter < sub_count:
-            counter2 = current_sub_counter +1
-            in_point = xmlo.xpath('//Subtitle')[current_sub_counter].attrib['TimeIn']
-            out      = xmlo.xpath('//Subtitle')[current_sub_counter].attrib['TimeOut']
-            in_point = in_point[:8] + '.' + in_point[9:]
-            out      = out[:8] + '.' + out[9:]
-            with open(srt_file, "a") as myfile:
-                myfile.write(str(current_sub_counter + 1) + '\n')
-                myfile.write(in_point + ' --> ' + out + '\n')
-                bla =  [bla.text for bla in xmlo.iterfind('.//Subtitle[%s]//Text' % int(counter2) ) ]
-                for i in bla:
-                        myfile.write(i.encode("utf-8") + '\n')
-                myfile.write('\n')
-                print( 'Transforming ' + str(current_sub_counter) + ' of' + str(count) + ' subtitles\r') ,
-            current_sub_counter +=1 
-        current_sub_counter= 0
-        os.chdir(os.path.dirname(lut_path))
-        if args.lowres:
-            resolution = args.lowres
-        else:
-            resolution = '0'
-        if delays == 0:
-            print( 'There were no audio delays.')
-            command = ['ffmpeg', '-lowres', resolution, '-c:v ','libopenjpeg','-i',pic_mxfs[counter],'-i',aud_mxfs[counter],
-            '-c:a','copy', '-c:v', 'libx264', '-vf', 'lut3d=26_XYZ-22_Rec709.cube']
-        else:
-            command = ['ffmpeg', '-lowres', resolution, '-c:v ','libopenjpeg','-i',pic_mxfs[counter],'-i',temp_dir + '/' + aud_mxfs[counter] + '.mkv',
-            '-c:a','copy', '-c:v', 'libx264','-vf', 'lut3d=26_XYZ-22_Rec709.cube']
-        pix_fmt = ['-pix_fmt','yuv420p']   
-        subs_command =  ['-vf', 'format=yuv420p,subtitles=%s' % srt_file]
-        if sub_delay > 0:
-            command += subs_command
-            sub_delay += 1
-            subs_counter +=1
-        elif sub_delay == 0:
-            command += pix_fmt
-            subs_counter = 0
-            sub_delay += 1
-        command += [output_subs_mkv ]
-        print (command)
-        subprocess.call(command)
-        counter += 1 
-    sys.exit()
-    
-    
-def concat():
-            # Create concat file. There is definitely a better way of doing this. Patch welcome ;)
-            if _platform == "win32":
-                dir_append    = dir + '\\'
-                concat_string = 'file \'' 
-                concat_append = '\''
-            else:
-                dir_append    = dir + '/'
-                concat_string = 'file \'' 
-                concat_append = '\''
-            if num_video_delays == 0:
-                picture_files_fix1 = [dir_append + x for x in pic_mxfs]
-            else:
-                picture_files_fix1 = [temp_dir + '/' + x + '.mkv' for x in pic_mxfs]
-            # http://stackoverflow.com/a/2050721/2188572
-            picture_files_fix2 = [concat_string + x for x in picture_files_fix1]
-            finalpic           = [x + concat_append for x in picture_files_fix2]
-            if num_audio_delays == 0:
-                audio_files_fix1 = [dir_append + x  for x in aud_mxfs]
-            else:
-                audio_files_fix1 = [temp_dir + '/' + x + '.mkv' for x in aud_mxfs]
-            audio_files_fix2     = [concat_string + x for x in audio_files_fix1]
-            finalaudio           = [x + concat_append for x in audio_files_fix2]
-            concat_list = []
-            concat_list.append(finalaudio)
-            concat_list.append(finalpic)   
-            return concat_list 
-            
-            
-def send_gmail():
-    emailfrom = ""
-    emailto = ['', '']
-    #emailto = ", ".join(emailto)
-    fileToSend = ''
-    username = ""
-    password = ""
-
-    msg = MIMEMultipart()
-    msg["From"] = emailfrom
-    msg["To"] = ", ".join(emailto)
-    msg["Subject"] = "Hash check complete"
-    msg.preamble = "testtesttest"
-    body = MIMEText("example email body")
-    msg.attach(body)
-
-    ctype, encoding = mimetypes.guess_type(fileToSend)
-    if ctype is None or encoding is not None:
-        ctype = "application/octet-stream"
-
-    maintype, subtype = ctype.split("/", 1)
-
-    if maintype == "text":
-        fp = open(fileToSend)
-        # Note: we should handle calculating the charset
-        attachment = MIMEText(fp.read(), _subtype=subtype)
-        fp.close()
-    elif maintype == "image":
-        fp = open(fileToSend, "rb")
-        attachment = MIMEImage(fp.read(), _subtype=subtype)
-        fp.close()
-    elif maintype == "audio":
-        fp = open(fileToSend, "rb")
-        attachment = MIMEAudio(fp.read(), _subtype=subtype)
-        fp.close()
-    else:
-        fp = open(fileToSend, "rb")
-        attachment = MIMEBase(maintype, subtype)
-        attachment.set_payload(fp.read())
-        fp.close()
-        encoders.encode_base64(attachment)
-    attachment.add_header("Content-Disposition", "attachment", filename=fileToSend)
-    msg.attach(attachment)
-
-
-    server_ssl = smtplib.SMTP_SSL("smtp.gmail.com", 465)
-    server_ssl.ehlo() # optional, called by login()
-    server_ssl.login(username, password)  
-    # ssl server doesn't support or need tls, so don't call server_ssl.starttls() 
-    server_ssl.sendmail(emailfrom, emailto, msg.as_string())
-    print(msg.as_string())
-    #server_ssl.quit()
-    server_ssl.close()
-    print ('successfully sent the mail')  
-    
-# Write the list of filenames containing picture to a textfile. 
-# http://www.pythonforbeginners.com/files/reading-and-writing-files-in-python
-def write_textfile(textfile, list_type):
-    file = open(textfile, "w")
-    for item in list_type:
-      file.write("%s\n" % item)
-    file.close()  # ffmpeg can't access the textfile until it's closed.   
-          
-for root,dirnames,filenames in os.walk(dcp_dir):
-    if ("ASSETMAP.xml"  in filenames) or ("ASSETMAP"  in filenames) :
-        dir = root
-        output_filename       = os.path.basename(dir) + '_muxed' + time.strftime("_%Y_%m_%dT%H_%M_%S")
-        output                = os.path.expanduser("~/Desktop/%s.mkv") % output_filename
-        if args.p:
-           codec = ['prores','-profile:v','3', '-c:a', 'copy']
-           output      = os.path.expanduser("~/Desktop/%s.mov") % output_filename
-        else:   
-           codec = ['libx264','-pix_fmt','yuv420p', '-crf', '19' ,'-preset','veryfast', '-c:a', 'aac']
-        # Change directory to directory with video files.
-        # Changing directory makes globbing easier (from my experience anyhow).
-        os.chdir(dir)
-
-        # Scan the main DCP directory for an assetmap. 
-        dcp_files = [f for f in listdir(dir) if isfile(join(dir, f))]
-        assetmap  = find_assetmap()
-
-        # Parse the assetmap in order to find the namespace.  
-        try:  
-            assetmap_xml = etree.parse(assetmap)
-        except SyntaxError:
-
-            print('Not a valid ASSETMAP!')
-            continue
-           
-        assetmap_namespace = assetmap_xml.xpath('namespace-uri(.)')     
-
-        cpl_list = []
-
-        cpl_parse = find_cpl() 
-    
-        cpl_namespace = cpl_parse.xpath('namespace-uri(.)') 
-        subtitle_language    =  cpl_parse.findall('//ns:MainSubtitle/ns:Language',namespaces={'ns': cpl_namespace})  
-        xmluuid              =  cpl_parse.findall('//ns:MainPicture/ns:Id',namespaces={'ns': cpl_namespace})
-        xmluuid_audio        =  cpl_parse.findall('//ns:MainSound/ns:Id',namespaces={'ns': cpl_namespace})
-        xmluuid_subs         =  cpl_parse.findall('//ns:MainSubtitle/ns:Id',namespaces={'ns': cpl_namespace})
-        duration_image       =  cpl_parse.findall('//ns:MainPicture/ns:Duration',namespaces={'ns': cpl_namespace})
-        duration_audio       =  cpl_parse.findall('//ns:MainSound/ns:Duration',namespaces={'ns': cpl_namespace})
-        intrinsic_image      =  cpl_parse.findall('//ns:MainPicture/ns:IntrinsicDuration',namespaces={'ns': cpl_namespace})
-        intrinsic_audio      =  cpl_parse.findall('//ns:MainSound/ns:IntrinsicDuration',namespaces={'ns': cpl_namespace})
-        entry_image          =  cpl_parse.findall('//ns:MainPicture/ns:EntryPoint',namespaces={'ns': cpl_namespace})
-        entry_audio          =  cpl_parse.findall('//ns:MainSound/ns:EntryPoint',namespaces={'ns': cpl_namespace})
-        
-        video_fps            =  cpl_parse.xpath('//ns:MainPicture/ns:EditRate',namespaces={'ns': cpl_namespace})
-        for i in video_fps:
-            fps = i.text[:-1]
-        # http://stackoverflow.com/questions/37038148/extract-value-from-element-when-second-namespace-is-used-in-lxml/37038309
-        # Some DCPS use a specific namespace for closed captions.
-        if len(xmluuid_subs) == 0:
-            xmluuid_subs = cpl_parse.xpath('//proto2007:MainClosedCaption/proto2004:Id', namespaces={
-                'proto2004': 'http://www.digicine.com/PROTO-ASDCP-CPL-20040511#',
-                'proto2007': 'http://www.digicine.com/PROTO-ASDCP-CC-CPL-20070926#',
-            })
-        
-        audio_delay = {}
-        file_paths  = {} 
-        # Begin analysis of assetmap xml.
-
-        assetmap_paths =  assetmap_xml.findall('//ns:Path',namespaces={'ns': assetmap_namespace})
-        assetmap_uuids =  assetmap_xml.findall('//ns:Asset/ns:Id',namespaces={'ns': assetmap_namespace})
-            
-        counter = 0 
-        while counter <= len(assetmap_paths) -1 :
-
-            if 'file:///' in assetmap_paths[counter].text:
-                remove_this = 'file:///'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
-            elif 'file://' in assetmap_paths[counter].text:
-                remove_this = 'file://'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")            
-
-            elif 'file:/' in assetmap_paths[counter].text:
-                remove_this = 'file:/'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")           
-
-            file_paths[assetmap_uuids[counter].text] = [assetmap_paths[counter].text] # {assetmapuuid:assetmapfilename}
-            counter += 1
-            
-        pic_mxfs = [] 
-          
-        for pic_uuid_object in xmluuid:
-            for pic_uuid in file_paths[pic_uuid_object.text]:            
-                pic_mxfs.append(pic_uuid)
-                 
-        aud_mxfs = []   
-        for aud_uuid_object in xmluuid_audio:
-            for aud_uuid in file_paths[aud_uuid_object.text]:            
-                aud_mxfs.append(aud_uuid)
-
-
-        subs = []   
-        for sub_uuid_object in xmluuid_subs:
-            for sub_uuid in file_paths[sub_uuid_object.text]:            
-                subs.append(sub_uuid)
-    
-        audio_delay_info = delay_check('MainSound',cpl_parse, cpl_namespace)
-        video_delay_info = delay_check('MainPicture',cpl_parse, cpl_namespace)
-
-        audio_delay      = audio_delay_info[0]
-        num_audio_delays  = audio_delay_info[1]
-        video_delay      = video_delay_info[0]
-        num_video_delays  = video_delay_info[1]
-
-        if args.s:
-            burn_subs()
-        concat_list = concat()
-        finalaudio  = concat_list[0]
-        finalpic    = concat_list[1]
-        if num_audio_delays == 0:
-            print( 'There were no audio delays.')
-        else:
-            for i in audio_delay:
-                print( 'rewrapping')
-                # Wrapping PCM in matroska as WAV has 4 gig limit.
-                rewrap = ['ffmpeg','-ss',str(audio_delay[i][0]),'-c:v ','libopenjpeg',
-                '-i',audio_delay[i][2],'-t',str(audio_delay[i][1]),
-                '-c:a','copy', temp_dir + '/'+ audio_delay[i][2] + '.mkv']
-                print rewrap
-                subprocess.call(rewrap)
-        if num_video_delays == 0:
-            print( 'There were no video delays.')
-        else:
-            for i in video_delay:
-                print( 'rewrapping')
-                # Wrapping PCM in matroska as WAV has 4 gig limit.
-                rewrap = ['ffmpeg','-ss',str(video_delay[i][0]),'-c:v ','libopenjpeg',
-                '-i',video_delay[i][2],'-t',str(video_delay[i][1]),
-                '-c:a','copy', temp_dir + '/'+ video_delay[i][2] + '.mkv']
-                print(rewrap)
-                subprocess.call(rewrap)        
-        write_textfile(video_concat_textfile, finalpic)
-        write_textfile(audio_concat_textfile, finalaudio)
-        os.chdir(os.path.dirname(lut_path))
-        if args.lowres:
-            resolution = args.lowres
-        else:
-            resolution = '0'
-        command = ['ffmpeg','-lowres', resolution,'-f','concat','-safe', '0','-c:v ','libopenjpeg',
-                   '-i',video_concat_textfile,'-f','concat','-safe', '0',
-                   '-i',audio_concat_textfile, '-vf', 'lut3d=./26_XYZ-22_Rec709.cube','-c:v']
-
-        command += codec
-        if args.hd:
-            command += ['-vf', "scale=1920:-1,setsar=1/1,pad=1920:1080:0:(oh-ih)/2,lut3d=26_XYZ-22_Rec709.cube"]
-        command += [output]
-        print (command)
-        subprocess.call(command)        
-        # Removes PKLs from list of files to hash, as these files are not in manifest.
-
-if email == 'enabled': 
-    send_gmail()
-
+#!/usr/bin/env python
+
+import sys
+try:
+    from lxml import etree
+except ImportError:
+    print ('*** ERROR - LXML IS MISSING ***\nThis external module is required for xml parsing.\nInstall with  `pip install lxml`.\nYou may need to restart your terminal or your computer, but it should work immediately.\nYou may need to run `sudo pip install lxml` on some osx/linux machines.\n If having issues installing lxml on windows, download the relevant .whl file from here http://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml and run `pip install /path/to/lxml_filename.whl')
+    sys.exit()
+import pdb
+from glob import glob
+import csv
+import os
+from os import listdir
+from os.path import isfile, join
+import subprocess
+import base64
+import time
+import re
+import smtplib
+import argparse
+import mimetypes
+from email.mime.multipart import MIMEMultipart
+from email import encoders
+from email.message import Message
+from email.mime.audio import MIMEAudio
+from email.mime.base import MIMEBase
+from email.mime.image import MIMEImage
+from email.mime.text import MIMEText
+import tempfile
+from decimal import *
+from sys import platform as _platform
+getcontext().prec = 4
+
+# Use argparse for command line options.
+parser = argparse.ArgumentParser(description='Unencrypted DCP to H264 transcoder.'
+                                 ' Written by Kieran O\'Leary.')
+parser.add_argument('input')
+'''
+parser.add_argument(
+                    '-bag', 
+                    action='store_true',help='bag the dcp_dir if it passes the hash check')
+'''
+parser.add_argument(
+                    '-m', 
+                    action='store_true',help='send email report')
+parser.add_argument(
+                    '-s', 
+                    action='store_true',help='Burn in subtitles. This will take a long time. It makes more sense to make a clean copy first, then make subtitled surrogates from that new copy. Jpeg2000 decoding is slow, ProRes or h264 is significantly faster.')
+parser.add_argument(
+                    '-p', 
+                    action='store_true',help='Use Apple ProRes 4:2:2 HQ instead of H264')
+parser.add_argument(
+                    '-hd',
+                    action='store_true',help='Scale to 1920:1080 while preserving the aspect ratio')
+parser.add_argument(
+                    '-lowres',
+                    help='[0,1,2]Use the jpeg2000 lowres option for rescaling and speed increases. Accepts a value of 0 (original size), 1 (50 PERCENT size), 2 (25 PERCENT size)')
+args = parser.parse_args()
+'''
+if args.bag:
+    bagging = 'enabled'
+else:
+    bagging = 'disabled'
+'''
+ififuncs.check_existence(['ffprobe', 'ffmpeg'])
+if args.m:
+    email = 'enabled'
+else:
+    email = 'disabled'
+if args.s:
+    print( '***********************************************')
+    print ('You have chosen to burn in subtitles. This will take a long time. A better approach may be to make a clean transcode to a high quality format such as PRORES and make further clean or subtitled surrogates from that new copy. ')
+    print ('***********************************************')
+    time.sleep(1)
+lut_path = os.path.join(os.path.abspath(os.path.dirname(sys.argv[0])), '26_XYZ-22_Rec709.cube')
+# Set a bunch of variables for filenaming.    
+dcp_dir               = args.input
+# This temp directory should work on all operating systems. 
+temp_dir              = tempfile.gettempdir()
+video_concat_filename = os.path.basename(dcp_dir) + '_video_concat' + time.strftime("_%Y_%m_%dT%H_%M_%S")
+audio_concat_filename = os.path.basename(dcp_dir) + '_audio_concat' + time.strftime("_%Y_%m_%dT%H_%M_%S")
+# Slashes are significant for ffmpeg concat files.
+if _platform == "win32":
+    video_concat_textfile = os.path.expanduser("~\Desktop\%s.txt") % video_concat_filename
+    audio_concat_textfile = os.path.expanduser("~\Desktop\%s.txt") % audio_concat_filename
+else:
+    video_concat_textfile = temp_dir + "/%s.txt" % video_concat_filename
+    audio_concat_textfile = temp_dir + "/%s.txt" % audio_concat_filename
+    
+
+def find_assetmap():   
+    if 'ASSETMAP' in dcp_files:
+        assetmap = 'ASSETMAP'
+    elif 'ASSETMAP.xml' in dcp_files:
+        assetmap = 'ASSETMAP.xml'
+    return assetmap
+        
+        
+# Begin recursive search through sub-directories for DCPs.  
+def choose_cpl(): 
+    global cpl_list
+    # Some DCPs have multiple CPLs!       
+    cpl_number = 1
+    print ('Multiple CPL files found')
+    for i in cpl_list:
+        print (cpl_number,  i)
+        cpl_number += 1   
+    print( 'Please select which CPL you would like to process')
+    chosen_cpl = raw_input()
+    cpl_parse = etree.parse(cpl_list[int(chosen_cpl) - 1]) # The -1 is due to python zero-indexing.
+    if args.s:
+        cpl_namespace      = cpl_parse.xpath('namespace-uri(.)') 
+        subtitle_language  =  cpl_parse.findall('//ns:MainSubtitle/ns:Language',namespaces={'ns': cpl_namespace})
+        print( 'This CPL contains ', subtitle_language[0].text, ' subtitles. Proceed?')         
+    return cpl_parse 
+    
+    
+def find_cpl():
+    # Generate an empty list as there may be multiple CPLs.    
+    # Get a list of all XML files in the main DCP directory.
+    xmlfiles = glob('*.xml')
+    # Loop through xmlfiles in order to find any CPLL files.
+    for i in xmlfiles:
+        try:  
+            xmlname = etree.parse(i)
+        except SyntaxError:
+            print( 'not a valid CPL!')
+            continue
+        except KeyError:
+            print( 'Missing CPL!')
+            continue
+        xml_namespace = xmlname.xpath('namespace-uri(.)')
+        # Create list of CPLs.
+        if 'CPL' in xml_namespace:
+            cpl_list.append(i) 
+        if len(cpl_list) == 0:  
+            continue
+        elif len(cpl_list) == 1:
+            cpl_parse = etree.parse(cpl_list[0])
+    if len(cpl_list) > 1:
+        cpl_parse = choose_cpl() 
+        # As there can be multiple subtitles, This options gives some info/choice.
+        subs_confirmation  = raw_input('Y/N')       
+        while subs_confirmation not in ['Y','y']:
+            cpl_parse = choose_cpl()
+            subs_confirmation  = raw_input('Y/N')    
+            return cpl_parse
+        return cpl_parse    
+    else:
+        return cpl_parse  
+
+        
+def delay_check(media_type,cpl_parse, cpl_namespace ):
+    # Check if there is an intended audio delay.
+    count   = cpl_parse.xpath('count(//ns:%s/ns:EntryPoint)' % media_type,namespaces={'ns': cpl_namespace} )
+    xmluuid_list               = cpl_parse.xpath('//ns:%s/ns:Id' % media_type,namespaces={'ns': cpl_namespace})
+    EntryPoint_list            = cpl_parse.xpath('//ns:%s/ns:EntryPoint' % media_type,namespaces={'ns': cpl_namespace})
+    dur_list                   = cpl_parse.xpath('//ns:%s/ns:Duration' % media_type,namespaces={'ns': cpl_namespace})
+    dur_intrinsic_list         = cpl_parse.xpath('//ns:%s/ns:IntrinsicDuration' % media_type,namespaces={'ns': cpl_namespace})
+    counter = 0
+    delays  = 0
+    audio_delay = {}
+    while counter < count:
+        audio_delay_values = []
+        xmluuid = xmluuid_list[counter]
+        EntryPoint = EntryPoint_list[counter]
+        entrypoint_audio      = float(EntryPoint.text)
+        if EntryPoint.text != '0':
+            delays += 1
+            # EntryPoint is in frames. The following converts to seconds.
+            entrypoint_audio  = float(EntryPoint.text) 
+            entrypoint_audio  = float(entrypoint_audio) / float(fps) # Change to EditRate variable.
+            entrypoint_audio  = round(entrypoint_audio, 3)
+        audio_delay_values.append(entrypoint_audio) 
+        dur                   = dur_list[counter]
+        dur_intrinsic         = dur_intrinsic_list[counter]
+        tail_test             = int(dur_intrinsic.text) - int(dur.text)
+        if tail_test > 0:
+            delays +=1
+        tail_delay = int(dur.text)
+        tail_delay = float(tail_delay) / float(fps)
+        tail_delay = round(tail_delay, 3)
+        audio_delay_values.append(tail_delay)
+        audio_delay_values.append(file_paths[xmluuid.text][0])
+        # audio_delay stores [entrypoint, tail_delay, file_path]
+        audio_delay[xmluuid.text] = audio_delay_values
+        counter += 1
+    test_list = []
+    test_list.append(audio_delay)
+    test_list.append(delays)
+    return test_list
+            
+            
+def burn_subs():
+    counter = 0
+    subs_counter = 0
+    count = len(subs)
+    sub_delay = 1
+    if not len(subs) == len(pic_mxfs):
+        print('The amount of picture files does not equal the amount of subtitles. This feature is not supported yet. Sorry!')
+        sub_delay = 0
+        # This assumes that if there are less subtitles than video files, it's because there's an extra AV reel at the head.A more robust option will be added later. Right now this fixes the one use case I've seen.
+    if delays != 0:
+        for i in audio_delay:
+            # Wrapping PCM in matroska as WAV has 4 gig limit.
+            subprocess.call(['ffmpeg','-ss',str(audio_delay[i][0]),
+            '-i',audio_delay[i][2],'-t',str(audio_delay[i][1]),
+            '-c:a','copy', temp_dir + '/'+ audio_delay[i][2] + '.mkv'])    
+    while counter < count:
+        srt_file = temp_dir + '/' + os.path.basename(subs[subs_counter]) +'.srt'
+        output_filename = os.path.basename(dcp_dir) + '_subs_reel' + str(counter + 1) + time.strftime("_%Y_%m_%dT%H_%M_%S")
+        output_subs_mkv = os.path.expanduser("~/Desktop/%s.mkv") % output_filename
+        try:  
+            xmlo = etree.parse(subs[subs_counter])
+        except SyntaxError:
+            if 'mxf' in srt_file:
+                print('Subtitle file is most likely an SMPTE MXF which is not currently supported.')
+            else:
+                print ('not a valid CPL!')
+            counter +=1
+            continue
+        except KeyError:
+            print ('Missing CPL!')
+            counter +=1
+            continue
+        sub_count = int(xmlo.xpath('count(//Subtitle)'))
+        current_sub_counter = 0
+        with open(srt_file, "w") as myfile:
+               print ('Transforming ', sub_count, 'subtitles')
+        while current_sub_counter < sub_count:
+            counter2 = current_sub_counter +1
+            in_point = xmlo.xpath('//Subtitle')[current_sub_counter].attrib['TimeIn']
+            out      = xmlo.xpath('//Subtitle')[current_sub_counter].attrib['TimeOut']
+            in_point = in_point[:8] + '.' + in_point[9:]
+            out      = out[:8] + '.' + out[9:]
+            with open(srt_file, "a") as myfile:
+                myfile.write(str(current_sub_counter + 1) + '\n')
+                myfile.write(in_point + ' --> ' + out + '\n')
+                bla =  [bla.text for bla in xmlo.iterfind('.//Subtitle[%s]//Text' % int(counter2) ) ]
+                for i in bla:
+                        myfile.write(i.encode("utf-8") + '\n')
+                myfile.write('\n')
+                print( 'Transforming ' + str(current_sub_counter) + ' of' + str(count) + ' subtitles\r') ,
+            current_sub_counter +=1 
+        current_sub_counter= 0
+        os.chdir(os.path.dirname(lut_path))
+        if args.lowres:
+            resolution = args.lowres
+        else:
+            resolution = '0'
+        if delays == 0:
+            print( 'There were no audio delays.')
+            command = ['ffmpeg', '-lowres', resolution, '-c:v ','libopenjpeg','-i',pic_mxfs[counter],'-i',aud_mxfs[counter],
+            '-c:a','copy', '-c:v', 'libx264', '-vf', 'lut3d=26_XYZ-22_Rec709.cube']
+        else:
+            command = ['ffmpeg', '-lowres', resolution, '-c:v ','libopenjpeg','-i',pic_mxfs[counter],'-i',temp_dir + '/' + aud_mxfs[counter] + '.mkv',
+            '-c:a','copy', '-c:v', 'libx264','-vf', 'lut3d=26_XYZ-22_Rec709.cube']
+        pix_fmt = ['-pix_fmt','yuv420p']   
+        subs_command =  ['-vf', 'format=yuv420p,subtitles=%s' % srt_file]
+        if sub_delay > 0:
+            command += subs_command
+            sub_delay += 1
+            subs_counter +=1
+        elif sub_delay == 0:
+            command += pix_fmt
+            subs_counter = 0
+            sub_delay += 1
+        command += [output_subs_mkv ]
+        print (command)
+        subprocess.call(command)
+        counter += 1 
+    sys.exit()
+    
+    
+def concat():
+            # Create concat file. There is definitely a better way of doing this. Patch welcome ;)
+            if _platform == "win32":
+                dir_append    = dir + '\\'
+                concat_string = 'file \'' 
+                concat_append = '\''
+            else:
+                dir_append    = dir + '/'
+                concat_string = 'file \'' 
+                concat_append = '\''
+            if num_video_delays == 0:
+                picture_files_fix1 = [dir_append + x for x in pic_mxfs]
+            else:
+                picture_files_fix1 = [temp_dir + '/' + x + '.mkv' for x in pic_mxfs]
+            # http://stackoverflow.com/a/2050721/2188572
+            picture_files_fix2 = [concat_string + x for x in picture_files_fix1]
+            finalpic           = [x + concat_append for x in picture_files_fix2]
+            if num_audio_delays == 0:
+                audio_files_fix1 = [dir_append + x  for x in aud_mxfs]
+            else:
+                audio_files_fix1 = [temp_dir + '/' + x + '.mkv' for x in aud_mxfs]
+            audio_files_fix2     = [concat_string + x for x in audio_files_fix1]
+            finalaudio           = [x + concat_append for x in audio_files_fix2]
+            concat_list = []
+            concat_list.append(finalaudio)
+            concat_list.append(finalpic)   
+            return concat_list 
+            
+            
+def send_gmail():
+    emailfrom = ""
+    emailto = ['', '']
+    #emailto = ", ".join(emailto)
+    fileToSend = ''
+    username = ""
+    password = ""
+
+    msg = MIMEMultipart()
+    msg["From"] = emailfrom
+    msg["To"] = ", ".join(emailto)
+    msg["Subject"] = "Hash check complete"
+    msg.preamble = "testtesttest"
+    body = MIMEText("example email body")
+    msg.attach(body)
+
+    ctype, encoding = mimetypes.guess_type(fileToSend)
+    if ctype is None or encoding is not None:
+        ctype = "application/octet-stream"
+
+    maintype, subtype = ctype.split("/", 1)
+
+    if maintype == "text":
+        fp = open(fileToSend)
+        # Note: we should handle calculating the charset
+        attachment = MIMEText(fp.read(), _subtype=subtype)
+        fp.close()
+    elif maintype == "image":
+        fp = open(fileToSend, "rb")
+        attachment = MIMEImage(fp.read(), _subtype=subtype)
+        fp.close()
+    elif maintype == "audio":
+        fp = open(fileToSend, "rb")
+        attachment = MIMEAudio(fp.read(), _subtype=subtype)
+        fp.close()
+    else:
+        fp = open(fileToSend, "rb")
+        attachment = MIMEBase(maintype, subtype)
+        attachment.set_payload(fp.read())
+        fp.close()
+        encoders.encode_base64(attachment)
+    attachment.add_header("Content-Disposition", "attachment", filename=fileToSend)
+    msg.attach(attachment)
+
+
+    server_ssl = smtplib.SMTP_SSL("smtp.gmail.com", 465)
+    server_ssl.ehlo() # optional, called by login()
+    server_ssl.login(username, password)  
+    # ssl server doesn't support or need tls, so don't call server_ssl.starttls() 
+    server_ssl.sendmail(emailfrom, emailto, msg.as_string())
+    print(msg.as_string())
+    #server_ssl.quit()
+    server_ssl.close()
+    print ('successfully sent the mail')  
+    
+# Write the list of filenames containing picture to a textfile. 
+# http://www.pythonforbeginners.com/files/reading-and-writing-files-in-python
+def write_textfile(textfile, list_type):
+    file = open(textfile, "w")
+    for item in list_type:
+      file.write("%s\n" % item)
+    file.close()  # ffmpeg can't access the textfile until it's closed.   
+          
+for root,dirnames,filenames in os.walk(dcp_dir):
+    if ("ASSETMAP.xml"  in filenames) or ("ASSETMAP"  in filenames) :
+        dir = root
+        output_filename       = os.path.basename(dir) + '_muxed' + time.strftime("_%Y_%m_%dT%H_%M_%S")
+        output                = os.path.expanduser("~/Desktop/%s.mkv") % output_filename
+        if args.p:
+           codec = ['prores','-profile:v','3', '-c:a', 'copy']
+           output      = os.path.expanduser("~/Desktop/%s.mov") % output_filename
+        else:   
+           codec = ['libx264','-pix_fmt','yuv420p', '-crf', '19' ,'-preset','veryfast', '-c:a', 'aac']
+        # Change directory to directory with video files.
+        # Changing directory makes globbing easier (from my experience anyhow).
+        os.chdir(dir)
+
+        # Scan the main DCP directory for an assetmap. 
+        dcp_files = [f for f in listdir(dir) if isfile(join(dir, f))]
+        assetmap  = find_assetmap()
+
+        # Parse the assetmap in order to find the namespace.  
+        try:  
+            assetmap_xml = etree.parse(assetmap)
+        except SyntaxError:
+
+            print('Not a valid ASSETMAP!')
+            continue
+           
+        assetmap_namespace = assetmap_xml.xpath('namespace-uri(.)')     
+
+        cpl_list = []
+
+        cpl_parse = find_cpl() 
+    
+        cpl_namespace = cpl_parse.xpath('namespace-uri(.)') 
+        subtitle_language    =  cpl_parse.findall('//ns:MainSubtitle/ns:Language',namespaces={'ns': cpl_namespace})  
+        xmluuid              =  cpl_parse.findall('//ns:MainPicture/ns:Id',namespaces={'ns': cpl_namespace})
+        xmluuid_audio        =  cpl_parse.findall('//ns:MainSound/ns:Id',namespaces={'ns': cpl_namespace})
+        xmluuid_subs         =  cpl_parse.findall('//ns:MainSubtitle/ns:Id',namespaces={'ns': cpl_namespace})
+        duration_image       =  cpl_parse.findall('//ns:MainPicture/ns:Duration',namespaces={'ns': cpl_namespace})
+        duration_audio       =  cpl_parse.findall('//ns:MainSound/ns:Duration',namespaces={'ns': cpl_namespace})
+        intrinsic_image      =  cpl_parse.findall('//ns:MainPicture/ns:IntrinsicDuration',namespaces={'ns': cpl_namespace})
+        intrinsic_audio      =  cpl_parse.findall('//ns:MainSound/ns:IntrinsicDuration',namespaces={'ns': cpl_namespace})
+        entry_image          =  cpl_parse.findall('//ns:MainPicture/ns:EntryPoint',namespaces={'ns': cpl_namespace})
+        entry_audio          =  cpl_parse.findall('//ns:MainSound/ns:EntryPoint',namespaces={'ns': cpl_namespace})
+        
+        video_fps            =  cpl_parse.xpath('//ns:MainPicture/ns:EditRate',namespaces={'ns': cpl_namespace})
+        for i in video_fps:
+            fps = i.text[:-1]
+        # http://stackoverflow.com/questions/37038148/extract-value-from-element-when-second-namespace-is-used-in-lxml/37038309
+        # Some DCPS use a specific namespace for closed captions.
+        if len(xmluuid_subs) == 0:
+            xmluuid_subs = cpl_parse.xpath('//proto2007:MainClosedCaption/proto2004:Id', namespaces={
+                'proto2004': 'http://www.digicine.com/PROTO-ASDCP-CPL-20040511#',
+                'proto2007': 'http://www.digicine.com/PROTO-ASDCP-CC-CPL-20070926#',
+            })
+        
+        audio_delay = {}
+        file_paths  = {} 
+        # Begin analysis of assetmap xml.
+
+        assetmap_paths =  assetmap_xml.findall('//ns:Path',namespaces={'ns': assetmap_namespace})
+        assetmap_uuids =  assetmap_xml.findall('//ns:Asset/ns:Id',namespaces={'ns': assetmap_namespace})
+            
+        counter = 0 
+        while counter <= len(assetmap_paths) -1 :
+
+            if 'file:///' in assetmap_paths[counter].text:
+                remove_this = 'file:///'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
+            elif 'file://' in assetmap_paths[counter].text:
+                remove_this = 'file://'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")            
+
+            elif 'file:/' in assetmap_paths[counter].text:
+                remove_this = 'file:/'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")           
+
+            file_paths[assetmap_uuids[counter].text] = [assetmap_paths[counter].text] # {assetmapuuid:assetmapfilename}
+            counter += 1
+            
+        pic_mxfs = [] 
+          
+        for pic_uuid_object in xmluuid:
+            for pic_uuid in file_paths[pic_uuid_object.text]:            
+                pic_mxfs.append(pic_uuid)
+                 
+        aud_mxfs = []   
+        for aud_uuid_object in xmluuid_audio:
+            for aud_uuid in file_paths[aud_uuid_object.text]:            
+                aud_mxfs.append(aud_uuid)
+
+
+        subs = []   
+        for sub_uuid_object in xmluuid_subs:
+            for sub_uuid in file_paths[sub_uuid_object.text]:            
+                subs.append(sub_uuid)
+    
+        audio_delay_info = delay_check('MainSound',cpl_parse, cpl_namespace)
+        video_delay_info = delay_check('MainPicture',cpl_parse, cpl_namespace)
+
+        audio_delay      = audio_delay_info[0]
+        num_audio_delays  = audio_delay_info[1]
+        video_delay      = video_delay_info[0]
+        num_video_delays  = video_delay_info[1]
+
+        if args.s:
+            burn_subs()
+        concat_list = concat()
+        finalaudio  = concat_list[0]
+        finalpic    = concat_list[1]
+        if num_audio_delays == 0:
+            print( 'There were no audio delays.')
+        else:
+            for i in audio_delay:
+                print( 'rewrapping')
+                # Wrapping PCM in matroska as WAV has 4 gig limit.
+                rewrap = ['ffmpeg','-ss',str(audio_delay[i][0]),'-c:v ','libopenjpeg',
+                '-i',audio_delay[i][2],'-t',str(audio_delay[i][1]),
+                '-c:a','copy', temp_dir + '/'+ audio_delay[i][2] + '.mkv']
+                print rewrap
+                subprocess.call(rewrap)
+        if num_video_delays == 0:
+            print( 'There were no video delays.')
+        else:
+            for i in video_delay:
+                print( 'rewrapping')
+                # Wrapping PCM in matroska as WAV has 4 gig limit.
+                rewrap = ['ffmpeg','-ss',str(video_delay[i][0]),'-c:v ','libopenjpeg',
+                '-i',video_delay[i][2],'-t',str(video_delay[i][1]),
+                '-c:a','copy', temp_dir + '/'+ video_delay[i][2] + '.mkv']
+                print(rewrap)
+                subprocess.call(rewrap)        
+        write_textfile(video_concat_textfile, finalpic)
+        write_textfile(audio_concat_textfile, finalaudio)
+        os.chdir(os.path.dirname(lut_path))
+        if args.lowres:
+            resolution = args.lowres
+        else:
+            resolution = '0'
+        command = ['ffmpeg','-lowres', resolution,'-f','concat','-safe', '0','-c:v ','libopenjpeg',
+                   '-i',video_concat_textfile,'-f','concat','-safe', '0',
+                   '-i',audio_concat_textfile, '-vf', 'lut3d=./26_XYZ-22_Rec709.cube','-c:v']
+
+        command += codec
+        if args.hd:
+            command += ['-vf', "scale=1920:-1,setsar=1/1,pad=1920:1080:0:(oh-ih)/2,lut3d=26_XYZ-22_Rec709.cube"]
+        command += [output]
+        print (command)
+        subprocess.call(command)        
+        # Removes PKLs from list of files to hash, as these files are not in manifest.
+
+if email == 'enabled': 
+    send_gmail()
+
```

### Comparing `ifiscripts-2023.7.3.1/scripts/dcpfixity.py` & `ifiscripts-2023.7.3.2/scripts/dcpfixity.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-#!/usr/bin/env python
-
-from lxml import etree
-import sys
-import pdb
-from glob import glob
-import csv
-import os
-from os import listdir
-from os.path import isfile, join
-import subprocess
-import base64
-import time
-import re
-import smtplib
-import argparse
-import mimetypes
-from email.mime.multipart import MIMEMultipart
-from email import encoders
-from email.message import Message
-from email.mime.audio import MIMEAudio
-from email.mime.base import MIMEBase
-from email.mime.image import MIMEImage
-from email.mime.text import MIMEText
-try:
-    import bagit
-except ImportError:
-    print 'skipping error'
-ififuncs.check_existence(['ffprobe', 'ffmpeg'])
-parser = argparse.ArgumentParser(description='DCP FIXITY checker/bagging tool.'
-                                 ' Written by Kieran O\'Leary.')
-parser.add_argument('input')
-parser.add_argument(
-                    '-bag', 
-                    action='store_true',help='bag the dcp_dir if it passes the hash check')
-parser.add_argument(
-                    '-csv', 
-                    action='store_true',help='File level csv is stored as sidecar to dcp directory')
-parser.add_argument(
-                    '-m', 
-                    action='store_true',help='send email report')
-args = parser.parse_args()
-
-if args.bag:
-    bagging = 'enabled'
-else:
-    bagging = 'disabled'
-
-if args.m:
-    email = 'enabled'
-else:
-    email = 'disabled'
-#bagrm =  os.path.abspath('bag-rm.py') 
-#bagit =  os.path.abspath('bagit.py') 
-#print bagrm
-dcp_dir = args.input
-# Two csv functions. One to create a csv, the other to add info to.
-def create_csv(csv_file, *args):
-    f = open(csv_file, 'wb')
-    try:
-        writer = csv.writer(f)
-        writer.writerow(*args)
-    finally:
-        f.close()
-        
-def append_csv(csv_file, *args):
-    f = open(csv_file, 'ab')
-    try:
-        writer = csv.writer(f)
-        writer.writerow(*args)
-    finally:
-        f.close()
-
-# Create a new .csv file with headings.  
-# CSV filename will be DCp directory name + time/date.
-
-# CSV will be saved to your Desktop.
-
-
-csv_report_filename = os.path.basename(dcp_dir) + '_dcp_level' + time.strftime("_%Y_%m_%dT%H_%M_%S")
-# CSV will be saved to your Desktop.
-
-csv_report = os.path.expanduser("~/Desktop/%s.csv") % csv_report_filename        
-create_csv(csv_report, ('DCP NAME', 'DIRECTORY NAME', 'JUDGEMENT'))
-
-if args.csv:
-    csv_setting = 'enabled'
-
-    
-    
-else:
-    csv_setting = 'disabled'
-    csv_filename = os.path.basename(dcp_dir) + '_file_level' + time.strftime("_%Y_%m_%dT%H_%M_%S")
-    csvfile = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
-    #csv_file = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
-    create_csv(csvfile, ('MXF HASH', 'STORED HASH', 'FILENAME', 'JUDGEMENT'))
-for root,dirnames,filenames in os.walk(dcp_dir):
-    if ("ASSETMAP.xml"  in filenames) or ("ASSETMAP"  in filenames) :
-        dir = root
-        #print os.path.basename(os.path.dirname(root)) 
-        filenoext = os.path.splitext(os.path.dirname(root))[0]
-        #print filenoext + 'dfsdfjkljoewuiljkdfs'
-        # Change directory to directory with video files
-
-        if csv_setting == 'enabled': 
-            #print filenoext
-            # Generate new directory names in AIP
-            fixity_dir   = "%s/fixity" % filenoext
-            os.makedirs(fixity_dir)
-            csvfile = fixity_dir + '/' + os.path.basename(os.path.dirname(root)) + '_item_level' + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.csv'
-            #csv_file = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
-            create_csv(csvfile, ('MXF HASH', 'STORED HASH', 'FILENAME', 'JUDGEMENT'))
-        
-        
-        # Changing directory makes globbing easier (from my experience anyhow).
-        os.chdir(dir)
-
-        # Scan the main DCP directory for an assetmap.
-        dcp_files = [f for f in listdir(dir) if isfile(join(dir, f))]
-        if 'ASSETMAP' in dcp_files:
-            assetmap = 'ASSETMAP'
-        elif 'ASSETMAP.xml' in dcp_files:
-            assetmap = 'ASSETMAP.xml'
-
-        # Parse the assetmap in order to find the namespace.  
-        try:  
-            assetmap_xml = etree.parse(assetmap)
-        except SyntaxError:
-            append_csv(csvfile,('NOT A VALID ASSETMAP', 'NOT A VALID ASSETMAP', dir,'NOT A VALID ASSETMAP'))
-            append_csv(csv_report,(os.path.basename(dir), dir, 'NOT A VALID ASSETMAP'))
-            print 'not an assetmap!!!!'
-            continue
-           
-        assetmap_namespace = assetmap_xml.xpath('namespace-uri(.)')
-
-        
-
-        # Get a list of all XML files in the main DCP directory.
-        xmlfiles = glob('*.xml')
-
-        # Generate an empty list as there may be multiple PKLs.
-        pkl_list = []
-
-        # Loop through xmlfiles in order to find any PKL files.
-        for i in xmlfiles:
-            try:  
-                xmlname = etree.parse(i)
-            except SyntaxError:
-                append_csv(csvfile,('NOT A VALID PKL', 'NOT A VALID PKL', dir,'NOT A VALID PKL'))
-                append_csv(csv_report,(os.path.basename(dir), dir, 'NOT A VALID PKL'))
-                print 'not a valid PKL!!!!'
-                continue
-            except KeyError:
-                append_csv(csvfile,('PKL APPEARS TO BE MISSING', 'PKL APPEARS TO BE MISSING', dir,'PKL APPEARS TO BE MISSING'))
-                append_csv(csv_report,(os.path.basename(dir), dir, 'PKL APPEARS TO BE MISSING'))
-                print 'Missing PKL!!!!'
-                continue
-            
-            is_pkl = xmlname.xpath('namespace-uri(.)')
-            if 'PKL' in is_pkl:
-                pkl_list.append(i)
-            
-        if len(pkl_list) == 0:
-            
-            append_csv(csvfile,('PKL APPEARS TO BE MISSING', 'PKL APPEARS TO BE MISSING', dir,'PKL APPEARS TO BE MISSING'))
-            append_csv(csv_report,(os.path.basename(dir), dir, 'PKL APPEARS TO BE MISSING'))
-            continue
-        
-              
-        # Generate an empty dictionary that will link the PKL hashes to each UUID.        
-        pkl_hashes = {}
-
-        # Loop through the PKLs and link each hash to a UUID.
-        for i in pkl_list: 
-            pkl_parse = etree.parse(i)
-            pkl_namespace = pkl_parse.xpath('namespace-uri(.)') 
-            hashes =  pkl_parse.findall('//ns:Hash',namespaces={'ns': pkl_namespace})
-            xmluuid =  pkl_parse.findall('//ns:Asset/ns:Id',namespaces={'ns': pkl_namespace})
-
-            counter = 0
-            
-            while counter <= len(hashes) -1 : # The -1 is there because of lxml's zero indexing.
-                pkl_hashes[xmluuid[counter].text] = hashes[counter].text # {pkl_uuid:pkl_hash}
-                counter +=1
-                
-        # Begin analysis of assetmap xml.
-        counter = 0
-        assetmap_paths =  assetmap_xml.findall('//ns:Path',namespaces={'ns': assetmap_namespace})
-        assetmap_uuids =  assetmap_xml.findall('//ns:Asset/ns:Id',namespaces={'ns': assetmap_namespace})
-        #while counter <= len(assetmap_paths) -1 :
-            
-        counter = 0
-
-        file_paths = {}
-        
-        while counter <= len(assetmap_paths) -1 :
-            if 'file:///' in assetmap_paths[counter].text:
-                remove_this = 'file:///'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
-            elif 'file://' in assetmap_paths[counter].text:
-                remove_this = 'file://'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")            
-
-            elif 'file:/' in assetmap_paths[counter].text:
-                remove_this = 'file:/'
-                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
-            
-
-            file_paths[assetmap_uuids[counter].text] = [assetmap_paths[counter].text] # {assetmapuuid:assetmapfilename}
-            counter +=1
-
-        # Removes PKLs from list of files to hash, as these files are not in manifest.
-        keys_to_remove = [] 
-
-        for i in file_paths:
-            if file_paths[i][0] in pkl_list:
-                keys_to_remove.append(i)
-        # PKL files are deleted from the file_paths dictionary. 
-        for i in keys_to_remove:
-            del file_paths[i]       
-
-        # Check if there are any files missing from the DCP.
-
-        missing_files = []
-        for i in file_paths:
-            if not os.path.isfile(file_paths[i][0]): # This checks if the file exists.
-                print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - **********' + file_paths[i][0] + ' is missing **********'
-                missing_files.append(i)
-                # Add missing file info to the csv.
-                append_csv(csvfile,('MISSING FILE', pkl_hashes[i], os.path.abspath(file_paths[i][0]),'MISSING FILE'))
-
-        # This removes the missing files from the hashable list. 
-        for i in missing_files:
-            del file_paths[i]
-            del pkl_hashes[i]
-
-        # Generate fresh hashes on the actual files in the DCP.           
-        for i in file_paths:  
-            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - Generating fresh hash for ' + file_paths[i][0]
-            # Create SHA-1 binary hashes with OPENSSL.
-            
-            openssl_hash = subprocess.check_output(['openssl',
-                                                    'sha1',
-                                                    '-binary',
-                                                     file_paths[i][0]])
-            # Encode the hashes as base64.
-            b64hash =  base64.b64encode(openssl_hash)
-            # Append hashes to the list within the file_paths dictionary. 
-            file_paths[i].append(b64hash)
-
-        # Compare the hashes in the PKL manifest to the fresh hashes. 
-        hash_mismatches = []       
-        for i in file_paths:
-            if file_paths[i][1] == pkl_hashes[i]:
-                print file_paths[i][0] + ' is ok'
-                append_csv(csvfile,(file_paths[i][1], pkl_hashes[i], os.path.abspath(file_paths[i][0]),'HASH MATCH'))
-            else:
-                print file_paths[i][0] + ' mismatch'
-                hash_mismatches.append(file_paths[i][0])
-                append_csv(csvfile,(file_paths[i][1], pkl_hashes[i], os.path.abspath(file_paths[i][0]),'HASH MISMATCH'))
-            
-                
-        if len(hash_mismatches) > 0:
-            report = ' but THERE ARE HASH MISMATCHES. SCROLL UP FOR MORE INFO OR CHECK THE CSV'
-            baggable = 'n'
-            print 'This DCP will not be bagged as it could not pass a fixity check'
-        else:
-            report = ' and all hashes match.'
-            baggable = 'y'
-
-        if len(missing_files) > 0:
-            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - WARNING - THERE ARE FILES MISSING FROM THIS DCP. SCROLL UP FOR MORE INFO OR CHECK THE CSV'
-            append_csv(csv_report,(os.path.dirname(root), dir, 'FILES MISSING - CHECK REPORT'))
-            print 'This DCP will not be bagged as it could not pass a fixity check'
-        else: 
-            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - All files are present in your DCP' + report
-            append_csv(csv_report,(os.path.dirname(root), dir,'All files present ' + report))
-            
-        if bagging == 'enabled':
-            if baggable == 'y':
-                #pdb.set_trace()
-                if os.path.dirname(root) != args.input:
-                   
-
-                    dir = os.path.dirname(root)
-                    
-                    if args.input == os.path.dirname(dir):
-                        os.chdir(dir)
-
-                        bag = bagit.make_bag(dir)
-                        
-                    else:
-                        print 'bagging not supported for this folder structure right now'
-                else:
-                     
-                     print 'bagging not supported for this folder structure right now'
-if email == 'enabled': 
-    emailfrom = ""
-    emailto = ['', '']
-    #emailto = ", ".join(emailto)
-    fileToSend = csv_report
-    username = ""
-    password = ""
-
-    msg = MIMEMultipart()
-    msg["From"] = emailfrom
-    msg["To"] = ", ".join(emailto)
-    msg["Subject"] = "Hash check complete"
-    msg.preamble = "testtesttest"
-    body = MIMEText("example email body")
-    msg.attach(body)
-
-    ctype, encoding = mimetypes.guess_type(fileToSend)
-    if ctype is None or encoding is not None:
-        ctype = "application/octet-stream"
-
-    maintype, subtype = ctype.split("/", 1)
-
-    if maintype == "text":
-        fp = open(fileToSend)
-        # Note: we should handle calculating the charset
-        attachment = MIMEText(fp.read(), _subtype=subtype)
-        fp.close()
-    elif maintype == "image":
-        fp = open(fileToSend, "rb")
-        attachment = MIMEImage(fp.read(), _subtype=subtype)
-        fp.close()
-    elif maintype == "audio":
-        fp = open(fileToSend, "rb")
-        attachment = MIMEAudio(fp.read(), _subtype=subtype)
-        fp.close()
-    else:
-        fp = open(fileToSend, "rb")
-        attachment = MIMEBase(maintype, subtype)
-        attachment.set_payload(fp.read())
-        fp.close()
-        encoders.encode_base64(attachment)
-    attachment.add_header("Content-Disposition", "attachment", filename=fileToSend)
-    msg.attach(attachment)
-
-
-    server_ssl = smtplib.SMTP_SSL("smtp.gmail.com", 465)
-    server_ssl.ehlo() # optional, called by login()
-    server_ssl.login(username, password)  
-    # ssl server doesn't support or need tls, so don't call server_ssl.starttls() 
-    server_ssl.sendmail(emailfrom, emailto, msg.as_string())
-    print msg.as_string()
-    #server_ssl.quit()
-    server_ssl.close()
-    print 'successfully sent the mail'    
+#!/usr/bin/env python
+
+from lxml import etree
+import sys
+import pdb
+from glob import glob
+import csv
+import os
+from os import listdir
+from os.path import isfile, join
+import subprocess
+import base64
+import time
+import re
+import smtplib
+import argparse
+import mimetypes
+from email.mime.multipart import MIMEMultipart
+from email import encoders
+from email.message import Message
+from email.mime.audio import MIMEAudio
+from email.mime.base import MIMEBase
+from email.mime.image import MIMEImage
+from email.mime.text import MIMEText
+try:
+    import bagit
+except ImportError:
+    print 'skipping error'
+ififuncs.check_existence(['ffprobe', 'ffmpeg'])
+parser = argparse.ArgumentParser(description='DCP FIXITY checker/bagging tool.'
+                                 ' Written by Kieran O\'Leary.')
+parser.add_argument('input')
+parser.add_argument(
+                    '-bag', 
+                    action='store_true',help='bag the dcp_dir if it passes the hash check')
+parser.add_argument(
+                    '-csv', 
+                    action='store_true',help='File level csv is stored as sidecar to dcp directory')
+parser.add_argument(
+                    '-m', 
+                    action='store_true',help='send email report')
+args = parser.parse_args()
+
+if args.bag:
+    bagging = 'enabled'
+else:
+    bagging = 'disabled'
+
+if args.m:
+    email = 'enabled'
+else:
+    email = 'disabled'
+#bagrm =  os.path.abspath('bag-rm.py') 
+#bagit =  os.path.abspath('bagit.py') 
+#print bagrm
+dcp_dir = args.input
+# Two csv functions. One to create a csv, the other to add info to.
+def create_csv(csv_file, *args):
+    f = open(csv_file, 'wb')
+    try:
+        writer = csv.writer(f)
+        writer.writerow(*args)
+    finally:
+        f.close()
+        
+def append_csv(csv_file, *args):
+    f = open(csv_file, 'ab')
+    try:
+        writer = csv.writer(f)
+        writer.writerow(*args)
+    finally:
+        f.close()
+
+# Create a new .csv file with headings.  
+# CSV filename will be DCp directory name + time/date.
+
+# CSV will be saved to your Desktop.
+
+
+csv_report_filename = os.path.basename(dcp_dir) + '_dcp_level' + time.strftime("_%Y_%m_%dT%H_%M_%S")
+# CSV will be saved to your Desktop.
+
+csv_report = os.path.expanduser("~/Desktop/%s.csv") % csv_report_filename        
+create_csv(csv_report, ('DCP NAME', 'DIRECTORY NAME', 'JUDGEMENT'))
+
+if args.csv:
+    csv_setting = 'enabled'
+
+    
+    
+else:
+    csv_setting = 'disabled'
+    csv_filename = os.path.basename(dcp_dir) + '_file_level' + time.strftime("_%Y_%m_%dT%H_%M_%S")
+    csvfile = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
+    #csv_file = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
+    create_csv(csvfile, ('MXF HASH', 'STORED HASH', 'FILENAME', 'JUDGEMENT'))
+for root,dirnames,filenames in os.walk(dcp_dir):
+    if ("ASSETMAP.xml"  in filenames) or ("ASSETMAP"  in filenames) :
+        dir = root
+        #print os.path.basename(os.path.dirname(root)) 
+        filenoext = os.path.splitext(os.path.dirname(root))[0]
+        #print filenoext + 'dfsdfjkljoewuiljkdfs'
+        # Change directory to directory with video files
+
+        if csv_setting == 'enabled': 
+            #print filenoext
+            # Generate new directory names in AIP
+            fixity_dir   = "%s/fixity" % filenoext
+            os.makedirs(fixity_dir)
+            csvfile = fixity_dir + '/' + os.path.basename(os.path.dirname(root)) + '_item_level' + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.csv'
+            #csv_file = os.path.expanduser("~/Desktop/%s.csv") % csv_filename
+            create_csv(csvfile, ('MXF HASH', 'STORED HASH', 'FILENAME', 'JUDGEMENT'))
+        
+        
+        # Changing directory makes globbing easier (from my experience anyhow).
+        os.chdir(dir)
+
+        # Scan the main DCP directory for an assetmap.
+        dcp_files = [f for f in listdir(dir) if isfile(join(dir, f))]
+        if 'ASSETMAP' in dcp_files:
+            assetmap = 'ASSETMAP'
+        elif 'ASSETMAP.xml' in dcp_files:
+            assetmap = 'ASSETMAP.xml'
+
+        # Parse the assetmap in order to find the namespace.  
+        try:  
+            assetmap_xml = etree.parse(assetmap)
+        except SyntaxError:
+            append_csv(csvfile,('NOT A VALID ASSETMAP', 'NOT A VALID ASSETMAP', dir,'NOT A VALID ASSETMAP'))
+            append_csv(csv_report,(os.path.basename(dir), dir, 'NOT A VALID ASSETMAP'))
+            print 'not an assetmap!!!!'
+            continue
+           
+        assetmap_namespace = assetmap_xml.xpath('namespace-uri(.)')
+
+        
+
+        # Get a list of all XML files in the main DCP directory.
+        xmlfiles = glob('*.xml')
+
+        # Generate an empty list as there may be multiple PKLs.
+        pkl_list = []
+
+        # Loop through xmlfiles in order to find any PKL files.
+        for i in xmlfiles:
+            try:  
+                xmlname = etree.parse(i)
+            except SyntaxError:
+                append_csv(csvfile,('NOT A VALID PKL', 'NOT A VALID PKL', dir,'NOT A VALID PKL'))
+                append_csv(csv_report,(os.path.basename(dir), dir, 'NOT A VALID PKL'))
+                print 'not a valid PKL!!!!'
+                continue
+            except KeyError:
+                append_csv(csvfile,('PKL APPEARS TO BE MISSING', 'PKL APPEARS TO BE MISSING', dir,'PKL APPEARS TO BE MISSING'))
+                append_csv(csv_report,(os.path.basename(dir), dir, 'PKL APPEARS TO BE MISSING'))
+                print 'Missing PKL!!!!'
+                continue
+            
+            is_pkl = xmlname.xpath('namespace-uri(.)')
+            if 'PKL' in is_pkl:
+                pkl_list.append(i)
+            
+        if len(pkl_list) == 0:
+            
+            append_csv(csvfile,('PKL APPEARS TO BE MISSING', 'PKL APPEARS TO BE MISSING', dir,'PKL APPEARS TO BE MISSING'))
+            append_csv(csv_report,(os.path.basename(dir), dir, 'PKL APPEARS TO BE MISSING'))
+            continue
+        
+              
+        # Generate an empty dictionary that will link the PKL hashes to each UUID.        
+        pkl_hashes = {}
+
+        # Loop through the PKLs and link each hash to a UUID.
+        for i in pkl_list: 
+            pkl_parse = etree.parse(i)
+            pkl_namespace = pkl_parse.xpath('namespace-uri(.)') 
+            hashes =  pkl_parse.findall('//ns:Hash',namespaces={'ns': pkl_namespace})
+            xmluuid =  pkl_parse.findall('//ns:Asset/ns:Id',namespaces={'ns': pkl_namespace})
+
+            counter = 0
+            
+            while counter <= len(hashes) -1 : # The -1 is there because of lxml's zero indexing.
+                pkl_hashes[xmluuid[counter].text] = hashes[counter].text # {pkl_uuid:pkl_hash}
+                counter +=1
+                
+        # Begin analysis of assetmap xml.
+        counter = 0
+        assetmap_paths =  assetmap_xml.findall('//ns:Path',namespaces={'ns': assetmap_namespace})
+        assetmap_uuids =  assetmap_xml.findall('//ns:Asset/ns:Id',namespaces={'ns': assetmap_namespace})
+        #while counter <= len(assetmap_paths) -1 :
+            
+        counter = 0
+
+        file_paths = {}
+        
+        while counter <= len(assetmap_paths) -1 :
+            if 'file:///' in assetmap_paths[counter].text:
+                remove_this = 'file:///'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
+            elif 'file://' in assetmap_paths[counter].text:
+                remove_this = 'file://'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")            
+
+            elif 'file:/' in assetmap_paths[counter].text:
+                remove_this = 'file:/'
+                assetmap_paths[counter].text =  assetmap_paths[counter].text.replace(remove_this,"")
+            
+
+            file_paths[assetmap_uuids[counter].text] = [assetmap_paths[counter].text] # {assetmapuuid:assetmapfilename}
+            counter +=1
+
+        # Removes PKLs from list of files to hash, as these files are not in manifest.
+        keys_to_remove = [] 
+
+        for i in file_paths:
+            if file_paths[i][0] in pkl_list:
+                keys_to_remove.append(i)
+        # PKL files are deleted from the file_paths dictionary. 
+        for i in keys_to_remove:
+            del file_paths[i]       
+
+        # Check if there are any files missing from the DCP.
+
+        missing_files = []
+        for i in file_paths:
+            if not os.path.isfile(file_paths[i][0]): # This checks if the file exists.
+                print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - **********' + file_paths[i][0] + ' is missing **********'
+                missing_files.append(i)
+                # Add missing file info to the csv.
+                append_csv(csvfile,('MISSING FILE', pkl_hashes[i], os.path.abspath(file_paths[i][0]),'MISSING FILE'))
+
+        # This removes the missing files from the hashable list. 
+        for i in missing_files:
+            del file_paths[i]
+            del pkl_hashes[i]
+
+        # Generate fresh hashes on the actual files in the DCP.           
+        for i in file_paths:  
+            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - Generating fresh hash for ' + file_paths[i][0]
+            # Create SHA-1 binary hashes with OPENSSL.
+            
+            openssl_hash = subprocess.check_output(['openssl',
+                                                    'sha1',
+                                                    '-binary',
+                                                     file_paths[i][0]])
+            # Encode the hashes as base64.
+            b64hash =  base64.b64encode(openssl_hash)
+            # Append hashes to the list within the file_paths dictionary. 
+            file_paths[i].append(b64hash)
+
+        # Compare the hashes in the PKL manifest to the fresh hashes. 
+        hash_mismatches = []       
+        for i in file_paths:
+            if file_paths[i][1] == pkl_hashes[i]:
+                print file_paths[i][0] + ' is ok'
+                append_csv(csvfile,(file_paths[i][1], pkl_hashes[i], os.path.abspath(file_paths[i][0]),'HASH MATCH'))
+            else:
+                print file_paths[i][0] + ' mismatch'
+                hash_mismatches.append(file_paths[i][0])
+                append_csv(csvfile,(file_paths[i][1], pkl_hashes[i], os.path.abspath(file_paths[i][0]),'HASH MISMATCH'))
+            
+                
+        if len(hash_mismatches) > 0:
+            report = ' but THERE ARE HASH MISMATCHES. SCROLL UP FOR MORE INFO OR CHECK THE CSV'
+            baggable = 'n'
+            print 'This DCP will not be bagged as it could not pass a fixity check'
+        else:
+            report = ' and all hashes match.'
+            baggable = 'y'
+
+        if len(missing_files) > 0:
+            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - WARNING - THERE ARE FILES MISSING FROM THIS DCP. SCROLL UP FOR MORE INFO OR CHECK THE CSV'
+            append_csv(csv_report,(os.path.dirname(root), dir, 'FILES MISSING - CHECK REPORT'))
+            print 'This DCP will not be bagged as it could not pass a fixity check'
+        else: 
+            print time.strftime("%Y-%m-%dT%H:%M:%S") + ' - All files are present in your DCP' + report
+            append_csv(csv_report,(os.path.dirname(root), dir,'All files present ' + report))
+            
+        if bagging == 'enabled':
+            if baggable == 'y':
+                #pdb.set_trace()
+                if os.path.dirname(root) != args.input:
+                   
+
+                    dir = os.path.dirname(root)
+                    
+                    if args.input == os.path.dirname(dir):
+                        os.chdir(dir)
+
+                        bag = bagit.make_bag(dir)
+                        
+                    else:
+                        print 'bagging not supported for this folder structure right now'
+                else:
+                     
+                     print 'bagging not supported for this folder structure right now'
+if email == 'enabled': 
+    emailfrom = ""
+    emailto = ['', '']
+    #emailto = ", ".join(emailto)
+    fileToSend = csv_report
+    username = ""
+    password = ""
+
+    msg = MIMEMultipart()
+    msg["From"] = emailfrom
+    msg["To"] = ", ".join(emailto)
+    msg["Subject"] = "Hash check complete"
+    msg.preamble = "testtesttest"
+    body = MIMEText("example email body")
+    msg.attach(body)
+
+    ctype, encoding = mimetypes.guess_type(fileToSend)
+    if ctype is None or encoding is not None:
+        ctype = "application/octet-stream"
+
+    maintype, subtype = ctype.split("/", 1)
+
+    if maintype == "text":
+        fp = open(fileToSend)
+        # Note: we should handle calculating the charset
+        attachment = MIMEText(fp.read(), _subtype=subtype)
+        fp.close()
+    elif maintype == "image":
+        fp = open(fileToSend, "rb")
+        attachment = MIMEImage(fp.read(), _subtype=subtype)
+        fp.close()
+    elif maintype == "audio":
+        fp = open(fileToSend, "rb")
+        attachment = MIMEAudio(fp.read(), _subtype=subtype)
+        fp.close()
+    else:
+        fp = open(fileToSend, "rb")
+        attachment = MIMEBase(maintype, subtype)
+        attachment.set_payload(fp.read())
+        fp.close()
+        encoders.encode_base64(attachment)
+    attachment.add_header("Content-Disposition", "attachment", filename=fileToSend)
+    msg.attach(attachment)
+
+
+    server_ssl = smtplib.SMTP_SSL("smtp.gmail.com", 465)
+    server_ssl.ehlo() # optional, called by login()
+    server_ssl.login(username, password)  
+    # ssl server doesn't support or need tls, so don't call server_ssl.starttls() 
+    server_ssl.sendmail(emailfrom, emailto, msg.as_string())
+    print msg.as_string()
+    #server_ssl.quit()
+    server_ssl.close()
+    print 'successfully sent the mail'
```

### Comparing `ifiscripts-2023.7.3.1/scripts/deletefiles.py` & `ifiscripts-2023.7.3.2/scripts/deletefiles.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/dfxml.py` & `ifiscripts-2023.7.3.2/scripts/dfxml.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,1720 +1,1720 @@
-#!/usr/bin/env python
-#
-# dfxml.py
-# Digital Forensics XML classes
-
-"""Digital Forensics XML classes.
-This module contains a number of classes for dealing with dfxml files,  both using
-the XML DOM model and using the EXPAT model.
-
-The following moduel functions are defined:
- isone(x)   - returns true if something is equal to 1 (useful for <ALLOC>1</ALLOC>
- safeInt(x) - converts something to an int but never raises an exception
-
-The following classes are defined in this module:
- byte_run   - the class for representing a run on the disk
- dftime     - represents time. Can be in either Unix timestamp or ISO8601.
-              Interconverts as necessary.
- fileobject - represents a DFXML fileobject.
-
-
-byte_runs() is function that returns an array of byterun objects.
-Each object has the attributes:
-  file_offset - offset from the beginning of the file
-  img_offset  - offset from the beginning of the image
-  len         - the number of bytes
-  fs_offset   - offset from the beginning of the file system
-
-where encoding, if present, is 0 for raw, 1 for NTFS compressed.
-
-"""
-
-__version__ = "1.0.2"
-
-import sys
-import re
-from sys import stderr
-from subprocess import Popen,PIPE
-import base64
-import hashlib
-import os
-
-import datetime
-
-import logging
-_logger = logging.getLogger(os.path.basename(__file__))
-
-tsk_virtual_filenames = set(['$FAT1','$FAT2'])
-
-XMLNS_DC = "http://purl.org/dc/elements/1.1/"
-XMLNS_DFXML = "http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML"
-XMLNS_DELTA = "http://www.forensicswiki.org/wiki/Forensic_Disk_Differencing"
-
-def isone(x):
-    """Return true if something is one (number or string)"""
-    try:
-        return int(x)==1;
-    except TypeError:
-        return False
-
-def safeInt(x):
-    """Return an integer or False.  False is returned, rather than None, because you can
-    divide False by 3 but you can't divide None by 3.
-
-    NOTE: This function could be written as:
-
-    def safeInt(x):
-        return int(x) if x else False
-
-    but that doesn't work on older version of Python."""
-    if x: return int(x)
-    return False
-
-def timestamp2iso8601(ts):
-    import time
-    return time.strftime("%FT%TZ",time.gmtime(ts))
-
-from datetime import tzinfo,timedelta
-class GMTMIN(tzinfo):
-    def __init__(self,minoffset):         # DST starts last Sunday in March
-        self.minoffset = minoffset
-    def utcoffset(self, dt):
-        return timedelta(minutes=self.minoffset)
-    def dst(self, dt):
-        return timedelta(0)
-    def tzname(self,dt):
-         return "GMT+%02d%02d" % (self.minoffset/60,self.minoffset%60)
-
-def parse_iso8601(ts):
-    Z = ts.find('Z')
-    if Z>0:
-        return datetime.datetime.strptime(ts[:Z],"%Y-%m-%dT%H:%M:%S")
-    raise RuntimeError("parse_iso8601: ISO8601 format {} not recognized".format(ts))
-
-
-rx_iso8601 = re.compile("(\d\d\d\d)-(\d\d)-(\d\d)[T ](\d\d):(\d\d):(\d\d)(\.\d+)?(Z|[-+]\d\d:?\d\d)?")
-def iso8601Tdatetime(s):
-    """SLG's conversion of ISO8601 to datetime"""
-    m = rx_iso8601.search(s)
-    if not m:
-        raise ValueError("Cannot parse: "+s)
-    # Get the microseconds
-    try:
-        microseconds = int(float(m.group(7)) * 1000000)
-    except TypeError:
-        microseconds = 0
-    # Figure tz offset
-    offset = None
-    minoffset = None
-    if m.group(8):
-        if m.group(8)=="Z":
-            minoffset = 0
-        elif m.group(8)[0:1] in "-+":
-            minoffset = int(m.group(8)[0:3]) * 60 + int(m.group(8)[-2:])
-    z = s.find("Z")
-    if z>=0:
-        offset = 0
-    # Build the response
-    if minoffset:
-        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
-                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
-                                 microseconds,GMTMIN(minoffset))
-    elif offset:
-        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
-                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
-                                 microseconds,GMTMIN(offset))
-    else:
-        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
-                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
-                                 microseconds)
-
-#This format is as specified in RFC 822, section 5.1, and matches the adjustments in RFC 1123, section 5.2.14.  It appears in email and HTTP headers.
-rx_rfc822datetime = re.compile("(?P<day>\d{1,2}) (?P<month>Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) (?P<year>\d{4}) (?P<hours>\d\d):(?P<minutes>\d\d):(?P<seconds>\d\d) (?P<timezone>Z|[-+]\d\d:?\d\d)")
-three_letter_month_dict = {
-  "Jan": 1,
-  "Feb": 2,
-  "Mar": 3,
-  "Apr": 4,
-  "May": 5,
-  "Jun": 6,
-  "Jul": 7,
-  "Aug": 8,
-  "Sep": 9,
-  "Oct": 10,
-  "Nov": 11,
-  "Dec": 12
-}
-def rfc822Tdatetime(s):
-    """
-    AJN's conversion of times occurring in RFC 822 data to datetime.
-    Follows SLG's pattern.
-    """
-    m = rx_rfc822datetime.search(s)
-    if not m:
-        raise ValueError("Cannot parse as an RFC 822 timestamp: %r." % s)
-    mgd = m.groupdict()
-    # Figure tz offset
-    offset = None
-    minoffset = None
-    match_timezone = mgd.get("timezone")
-    if match_timezone:
-        if match_timezone == "Z":
-            minoffset = 0
-        elif match_timezone[0] in "-+":
-            minoffset = int(match_timezone[0:-2]) * 60 + int(match_timezone[-2:])
-    #TODO Find a reason to use the 'offset' variable? (Hour offset, vs. minute offset?)
-    if minoffset:
-        return datetime.datetime(
-          int(mgd["year"]),
-          three_letter_month_dict[mgd["month"]],
-          int(mgd["day"]),
-          int(mgd["hours"]),
-          int(mgd["minutes"]),
-          int(mgd["seconds"]),
-          0,
-          GMTMIN(minoffset)
-        )
-    else:
-        return datetime.datetime(
-          int(mgd["year"]),
-          three_letter_month_dict[mgd["month"]],
-          int(mgd["day"]),
-          int(mgd["hours"]),
-          int(mgd["minutes"]),
-          int(mgd["seconds"]),
-          0
-        )
-
-################################################################
-###
-###  byte_run class
-###
-
-class byte_run:
-    """The internal representation for a byte run. 
-
-    byte_runs have the following attributes:
-    .img_offset  = offset of the byte run from the image start, in bytes
-    .len         = the length of the run, in bytes (prevoiusly called 'bytes')
-    .sector_size = sector size of the underlying media
-
-    Originally this was an array,
-    which is faster than an attributed object. But this approach is more expandable,
-    and it's only 70% the speed of an array under Python3.0.
-        
-    Note that Python 3 removed the __cmp__ class method:
-        <http://docs.python.org/release/3.0.1/whatsnew/3.0.html#ordering-comparisons>
-    """
-    # declaring slots prevents other attributes from appearing,
-    # but that prevents the code from working with new XML that has new fields.
-    # __slots__ = ["file_offset","img_offset","len","fill","sector_size"]
-    def __init__(self,img_offset=None,len=None,file_offset=None):
-        self.img_offset = img_offset
-        self.file_offset = file_offset
-        self.len = len
-        self.sector_size = 512          # default
-        self.hashdigest  = dict()       # 
-
-    def __lt__(self,other):
-        if self.img_offset is not None and other.img_offset is not None:
-            return self.img_offset < other.img_offset
-        elif self.file_offset is not None and other.file_offset is not None:
-            return self.file_offset < other.file_offset
-        else:
-            raise ValueError("Byte run objects are incomparable")
-    
-    def __eq__(self,other):
-        if self.img_offset is not None and other.img_offset is not None:
-            return self.img_offset == other.img_offset
-        elif self.file_offset is not None and other.file_offset is not None:
-            return self.file_offset == other.file_offset
-        else:
-            raise ValueError("Byte run objects are incomparable")
-
-    def __str__(self):
-        try:
-            return "byte_run[img_offset={0}; file_offset={1} len={2}] ".format(
-                self.img_offset,self.file_offset,self.len)
-        except (AttributeError, TypeError):
-            #Catch attributes that are missing or mis-typed (e.g. NoneType)
-            pass
-        try:
-            return "byte_run[file_offset={0}; fill={1}; len={2}]".format(
-                self.file_offset,self.fill,self.len)
-        except AttributeError:
-            pass
-        try:
-            return "byte_run[file_offset={0}; uncompressed_len={1}]".format(
-                self.file_offset,self.uncompressed_len)
-        except AttributeError:
-            return "byte_run"+str(dir(self))
-    
-    def start_sector(self):
-        return self.img_offset // self.sector_size
-
-    def sector_count(self):
-        return self.len // self.sector_size
-
-    def has_sector(self,s):
-        if self.sector_size==0:
-            raise ValueError("%s: sector_size cannot be 0" % (self))
-        if self.img_offset is None or self.len is None:
-            # Sparse files don't have data allocated on disk
-            return False
-        try:
-            return self.img_offset <= s * self.sector_size < self.img_offset+self.len
-        except AttributeError:
-            # Doesn't have necessary attributes to answer true.
-            # Usually this happens with runs of a constant value
-            return False       
-
-    def extra_len(self):
-        return self.len % self.sector_size
-
-    def decode_xml_attributes(self,attr):
-        for (key,value) in attr.items():
-            try:
-                setattr(self,key,int(value))
-            except ValueError:
-                setattr(self,key,value)
-
-        
-    def decode_sax_attributes(self,attr):
-        for (key,value) in attr.items():
-            if key=='bytes': key=='len' # tag changed name; provide backwards compatiability 
-            try:
-                setattr(self,key,int(value))
-            except ValueError:
-                setattr(self,key,value)
-        
-class ComparableMixin(object):
-    """
-    Comparator "Abstract" class.  Classes inheriting this must define a _cmpkey() method.
-    
-    Credit to Lennart Regebro for the total implementation of this class, found equivalently from:
-    http://regebro.wordpress.com/2010/12/13/python-implementing-rich-comparison-the-correct-way/
-    http://stackoverflow.com/questions/6907323/comparable-classes-in-python-3/6913420#6913420
-    """
-    def _compare(self, other, method):
-        try:
-            return method(self._cmpkey(), other._cmpkey())
-        except (AttributeError, TypeError):
-            # _cmpkey not implemented, or return different type,
-            # so I can't compare with "other".
-            return NotImplemented
-
-    def __lt__(self, other):
-        return self._compare(other, lambda s, o: s < o)
-
-    def __le__(self, other):
-        return self._compare(other, lambda s, o: s <= o)
-
-    def __eq__(self, other):
-        return self._compare(other, lambda s, o: s == o)
-
-    def __ge__(self, other):
-        return self._compare(other, lambda s, o: s >= o)
-
-    def __gt__(self, other):
-        return self._compare(other, lambda s, o: s > o)
-
-    def __ne__(self, other):
-        return self._compare(other, lambda s, o: s != o)
-
-class dftime(ComparableMixin):
-    """Represents a DFXML time. Automatically converts between representations and caches the
-    results as necessary.."""
-    UTC = GMTMIN(0)
-
-    def ts2datetime(self,ts):
-        import datetime
-        return datetime.datetime.utcfromtimestamp(ts).replace(tzinfo=dftime.UTC)
-
-    def __init__(self,val):
-        #'unicode' is not a type in Python 3; 'basestring' is not a type in Python 2.
-        if sys.version_info >= (3,0):
-            _basestring = str
-        else:
-            _basestring = basestring
-        if isinstance(val, str) or isinstance(val,_basestring):
-            #
-            #Test for ISO 8601 format - "YYYY-MM-DD" should have hyphen at val[4]
-            if len(val)>5 and val[4]=="-":
-                self.iso8601_ = val
-            elif len(val) > 15 and ":" in val[13:15]:
-                #Maybe the data are instead the timestamp format found in email headers?
-                #(The check for 13:15 gets the 14th and 15th characters, since the day can be single- or double-digit.)
-                self.datetime_ = rfc822Tdatetime(val)
-            else:
-                #Maybe the data are a string-wrapped int or float?
-                #If this fails, the string format is completely unexpected, so just raise an error.
-                self.timestamp_ = float(val)
-        elif type(val)==int or type(val)==float:
-            self.timestamp_ = val
-        elif isinstance(val, datetime.datetime):
-            self.datetime_ = val
-            #TODO Unit-test this with a timezone-less datetime
-        elif val==None:
-            self.timestamp_ = None
-            self.iso8601_   = None
-        elif isinstance(val, dftime):
-            #If we instead use .timestamp_, we risk having a timezone conversion error
-            self.iso8601_ = val.iso8601()
-        else:
-            raise ValueError("Unknown type '%s' for DFXML time value" % (str(type(val))))
-    def __str__(self):
-        return self.iso8601() or ""
-    def __repr__(self):
-        return repr(self.iso8601()) or "None"
-    def __le__(self,b):
-        if b is None: return None
-        return self.iso8601().__le__(b.iso8601())
-    def __gt__(self,b):
-        if b is None: return None
-        return self.iso8601().__gt__(b.iso8601())
-    def _cmpkey(self):
-        """Provide a key to use for comparisons; for use with ComparableMixin parent class."""
-        return self.timestamp()
-    
-    def __eq__(self,b):
-        if b == None:
-            #This will always be False - if self were None, we wouldn't be in this __eq__ method.
-            return False
-        return self.timestamp()==b.timestamp()
-
-    def iso8601(self):
-        # Do we have a cached representation?
-        import time
-        try:
-            return self.iso8601_
-        except AttributeError:
-            pass
-        
-        # Do we have a datetime representation?
-        try:
-            self.iso8601_ = self.datetime_.isoformat()
-            return self.iso8601_
-        except AttributeError:
-            # We better have a Unix timestamp representation?
-            self.iso8601_ = time.strftime("%Y-%m-%dT%H:%M:%SZ",time.gmtime(self.timestamp_))
-            return self.iso8601_
-    
-    def timestamp(self):
-        import time
-        # Do we have a cached representation?
-        try:
-            return self.timestamp_
-        except AttributeError:
-            pass
-
-        # Do we have a datetime_ object?
-        try:
-            self.timestamp_ = time.mktime(self.datetime_.timetuple())
-            return self.timestamp_
-        except AttributeError:
-            self.datetime_ = iso8601Tdatetime(self.iso8601_)
-            self.timestamp_ = time.mktime(self.datetime_.timetuple())
-            return self.timestamp_
-        
-    def datetime(self):
-        import datetime
-        # return the datetime from parsing either iso8601 or from parsing timestamp
-        try:
-            self.datetime_ = self.ts2datetime(self.timestamp_)
-            # This needs to be in UTC offset. How annoying.
-            return self.datetime_
-        except AttributeError:
-            self.datetime_ = iso8601Tdatetime(self.iso8601_)
-            return self.datetime_
-
-class registry_object:
-    def __init__(self):
-        self.object_index = {}
-        self._mtime = None
-        
-        """Keep handy a handle on the registry object"""
-        self.registry_handle = self
-
-    def mtime(self):
-        return self._mtime
-
-class registry_cell_object:
-    def __init__(self):
-        self._byte_runs  = []
-
-        """This is a pointer to a registry_key_object.  The root node has no parent key."""
-        self.parent_key = None
-
-        self._name        = None
-
-        self._full_path   = None
-
-        """Keys have two types:  "root" (0x2c,0xac) and not-root.  Values have several more types."""
-        self._type        = None
-
-        """Keep handy a handle on the registry object"""
-        self.registry_handle = None
-        
-        """Name the cell type, for str() and repr()."""
-        self._cell_type = "(undefined cell object type)"
-
-        """Only applicable to values."""
-        self._sha1 = None
-
-    def name(self):
-        """This is the name of the present key or value."""
-        return self._name
-
-    def full_path(self):
-        """
-        This is the full path from the root of the hive, with keys acting like directories and the value name acting like the basename.
-
-        Unlike DFXML, registry paths are delimited with a backslash due to the forward slash being a legal and commonly observed character in cell names.
-        """
-        return self._full_path
-
-    def type(self):
-        """
-        This is the data type of the cell.  Keys can be root or not-root; values have several types, like UTF-8, binary, etc.
-        Presently, this exports as a string representation of the type, not the numeric type code.
-        """
-        return self._type
-
-    def _myname(self):
-        """This function is called by repr and str, due to (vague memories of) the possibility of an infinite loop if __repr__ calls __self__."""
-        if len(self._byte_runs) > 0:
-            addr = str(self._byte_runs[0].file_offset)
-        else:
-            addr = "(unknown)"
-        return "".join(["<", self._cell_type, " for hive file offset ", addr, ">"])
-
-    def __repr__(self):
-        return self._myname()
-    def __str__(self):
-        return self._myname()
-
-    def mtime(self):
-        raise NotImplementedError("registry_cell_object.mtime() not over-ridden!")
-
-    def byte_runs(self):
-        """Returns a sorted array of byte_run objects."""
-        #If this idiom is confusing, see:  http://henry.precheur.org/python/copy_list
-        ret = list(self._byte_runs)
-        return ret
-
-    def sha1(self):
-        """
-        Return None. Meant to be overwritten.
-        """
-        return None
-
-    def md5(self):
-        """
-        Return None. Meant to be overwritten.
-        """
-        return None
-    def sha512(self):
-        """
-        Return None. Meant to be overwritten.
-        """
-        return None
-
-class registry_key_object(registry_cell_object):
-    def __init__(self):
-        registry_cell_object.__init__(self)
-        self._mtime = None
-        self.values = {}
-        self.used = True  #TODO Add toggling logic for when hivexml (eventually) processes recovered keys
-        self._cell_type = "registry_key_object"
-    def mtime(self):
-        return self._mtime
-    def root(self):
-        if self.type() is None:
-            return None
-        return self.type() == "root"
-
-class registry_value_object(registry_cell_object):
-    def __init__(self):
-        registry_cell_object.__init__(self)
-        self.value_data  = None
-
-        self._cell_type = "registry_value_object"
-        
-        #TODO Replace to be in line with fileobjects: fileobject.hashdigest is a dictionary
-        self._hashcache = dict()
-
-        """List for the string-list type of value."""
-        self.strings = None
-
-    def mtime(self):
-        """Return nothing.  Alternatively, we might return mtime of parent key in the future."""
-        return None
-    #    if self.parent_key:
-    #        return self.parent_key.mtime()
-    #    else:
-    #        return None
-
-    def _hash(self, hashfunc):
-        """
-        Return cached hash, populating cache if necessary.
-        hashfunc expected values: The functions hashlib.sha1, hashlib.sha256, hashlib.md5.
-        If self.value_data is None, or there are no strings in a "string-list" type, this should return None.
-        Interpretation: Registry values of type "string-list" are hashed by feeding each element of the list into the hash .update() function. All other Registry values are fed in the same way, as a 1-element list.
-        For example, a string type value cell with data "a" fed into this function returns md5("a") (if hashlib.md5 were requested).  A string-list type value cell with data ["a","b"] returns md5("ab").
-        This is a simplification to deal with Registry string encodings, and may change in the future.
-        """
-        if self._hashcache.get(repr(hashfunc)) is None:
-            feed_list = []
-            if self.type() == "string-list":
-                feed_list = self.strings
-            elif not self.value_data is None:
-                feed_list.append(self.value_data)
-            #Normalize to hash .update() required type
-            for (elemindex, elem) in enumerate(feed_list):
-                if type(elem) == type(""):
-                    #String data take a little extra care:
-                    #"The bytes in your ... file are being automatically decoded to Unicode by Python 3 as you read from the file"
-                    #http://stackoverflow.com/a/7778340/1207160
-                    feed_list[elemindex] = elem.encode("utf-8")
-            #Hash if there's data to hash
-            if len(feed_list) > 0:
-                h = hashfunc()
-                for elem in feed_list:
-                    h.update(elem)
-                self._hashcache[repr(hashfunc)] = h.hexdigest()
-        return self._hashcache.get(repr(hashfunc))
-
-    def sha1(self):
-        return self._hash(hashlib.sha1)
-
-    def sha256(self):
-        return self._hash(hashlib.sha256)
-
-    def md5(self):
-        return self._hash(hashlib.md5)
-    def sha512(self):
-        return self._hash(hashlib.sha512)
-
-class fileobject:
-    """The base class for file objects created either through XML DOM or EXPAT"""
-    TIMETAGLIST=['atime','mtime','ctime','dtime','crtime']
-
-    def __init__(self,imagefile=None):
-        self.imagefile  = imagefile
-        self.hashdigest = dict()
-        
-    def __str__(self):
-        try:
-            fn = self.filename()
-        except KeyError:
-            fn = "???"
-        return "fileobject %s byte_runs: %s" % (fn, " ".join([str(x) for x in self.byte_runs()]))
-
-    def partition(self):
-        """Partion number of the file"""
-        return self.tag("partition")
-
-    def filename(self):
-        """Complement name of the file (sometimes called pathname)"""
-        return self.tag("filename")
-
-    def ext(self):
-        """Extension, as a lowercase string without the leading '.'"""
-        import string
-        (base,ext) = os.path.splitext(self.filename())
-        if ext == '':
-            return None
-        else:
-            return ext[1:]
-
-    def filesize(self):
-        """Size of the file, in bytes"""
-        return safeInt(self.tag("filesize"))
-
-    def uid(self):
-        """UID of the file"""
-        return safeInt(self.tag("uid"))
-
-    def gid(self):
-        """GID of the file"""
-        return safeInt(self.tag("gid"))
-
-    def meta_type(self):
-        """Meta-type of the file"""
-        return safeInt(self.tag("meta_type"))
-
-    def mode(self):
-        """Mode of the file"""
-        return safeInt(self.tag("mode"))
-
-    def ctime(self):
-        """Metadata Change Time (sometimes Creation Time), as number of seconds
-        since January 1, 1970 (Unix time)"""
-        t = self.tag("ctime")
-        if t: return dftime(t)
-        return None
-        
-    def atime(self):
-        """Access time, as number of seconds since January 1, 1970 (Unix time)"""
-        t = self.tag("atime")
-        if t: return dftime(t)
-        return None
-        
-    def crtime(self):
-        """CR time, as number of seconds since January 1, 1970 (Unix time)"""
-        t = self.tag("crtime")
-        if t: return dftime(t)
-        return None
-        
-    def mtime(self):
-        """Modify time, as number of seconds since January 1, 1970 (Unix time)"""
-        t = self.tag("mtime")
-        if t: return dftime(t)
-        return None
-        
-    def dtime(self):
-        """ext2 dtime"""
-        t = self.tag("dtime")
-        if t: return dftime(t)
-        return None
-
-    def times(self):
-        """Return a dictionary of all times that the system has"""
-        ret = {}
-        for tag in self.TIMETAGLIST:
-            if self.has_tag(tag):
-                try:
-                    ret[tag] = dftime(self.tag(tag))
-                except TypeError:
-                    pass
-        return ret
-
-    def sha1(self):
-        """Returns the SHA1 in hex"""
-        return self.tag("sha1")
-
-    def sha256(self):
-        """Returns the SHA256 in hex"""
-        return self.tag("sha256")
-
-    def md5(self):
-        """Returns the MD5 in hex"""
-        return self.tag("md5")
-    def sha512(self):
-        """Returns the SHA512 in hex"""
-        return self.tag("sha512")
-
-    def fragments(self):
-        """Returns number of file fragments"""
-        return len(self.byte_runs())
-
-    def name_type(self):
-        """Return the contents of the name_type tag"""
-        return self.tag("name_type")
-
-    def is_virtual(self):
-        """Returns true if the fi entry is a TSK virtual entry"""
-        return self.filename() in tsk_virtual_filenames
-
-    def is_dir(self):
-        """Returns true if file is a directory"""
-        return self.name_type()=='d'
-
-    def is_file(self):
-        """Returns true if file is a file"""
-        return self.name_type()=='r' or self.name_type()==None
-
-    def inode(self):
-        """Inode; may be a number or SleuthKit x-y-z format"""
-        return self.tag("inode")
-
-    def allocated_inode(self):
-        """Returns True if the file's inode data structure is allocated, False otherwise.  (Does not return None.)"""
-        return isone(self.tag("alloc_inode"))
-
-    def allocated_name(self):
-        """Returns True if the file's name data structure is allocated, False otherwise.  (Does not return None.)"""
-        return isone(self.tag("alloc_name"))
-
-    def allocated(self):
-        """Returns True if the file is allocated, False if it was not
-        (that is, if it was deleted or is an orphan).
-        Note that we need to be tolerant of mixed case, as it was changed.
-        We also need to tolerate the case of the unalloc tag being used.
-        """
-        if self.filename()=="$OrphanFiles": return False
-        if self.allocated_inode() and self.allocated_name():
-            return True
-        else:
-            return isone(self.tag("alloc")) or isone(self.tag("ALLOC")) or not isone(self.tag("unalloc"))
-
-    def compressed(self):
-        if not self.has_tag("compressed") and not self.has_tag("compressed") : return False
-        return isone(self.tag("compressed")) or isone(self.tag("COMPRESSED"))
-
-    def encrypted(self):
-        if not self.has_tag("encrypted") and not self.has_tag("encrypted") : return False
-        return isone(self.tag("encrypted")) or isone(self.tag("ENCRYPTED"))
-
-    def file_present(self,imagefile=None):
-        """Returns true if the file is present in the disk image"""
-        if self.filesize()==0:
-            return False               # empty files are never present
-        if imagefile==None:
-            imagefile=self.imagefile # use this one
-        for hashname in ['md5','sha1','sha256', 'sha512']:
-            oldhash = self.tag(hashname)
-            if oldhash:
-                newhash = hashlib.new(hashname,self.contents(imagefile=imagefile)).hexdigest()
-                return oldhash==newhash
-        raise ValueError("Cannot process file "+self.filename()+": no hash in "+str(self))
-
-    def has_contents(self):
-        """True if the file has one or more bytes"""
-        return len(self.byte_runs())>0
-
-    def has_sector(self,s):
-        """True if sector s is contained in one of the byte_runs."""
-        for run in self.byte_runs():
-            if run.has_sector(s): return True
-        return False
-
-    def libmagic(self):
-        """Returns libmagic string if the string is specified
-           in the xml, or None otherwise"""
-        return self.tag("libmagic")
-
-    def content_for_run(self,run=None,imagefile=None):
-        """ Returns the content for a specific run. This is a convenience feature
-        which does not touch the file object if an imagefile is provided."""
-        if imagefile is None: imagefile=self.imagefile
-        if run is None: raise ValueError("content_for_run called without a 'run' argument.")
-
-        if run.len == -1:
-            return chr(0) * run.len
-        elif hasattr(run,'fill'):
-            return chr(run.fill) * run.len
-        else:
-            imagefile.seek(run.img_offset)
-            return imagefile.read(run.len)
-
-    def contents(self,imagefile=None,icat_fallback=True):
-        """ Returns the contents of all the runs concatenated together. For allocated files
-        this should be the original file contents. """
-        if imagefile is None     : imagefile=self.imagefile
-        if imagefile is None     : raise ValueError("imagefile is unknown")
-        if self.encrypted()      : raise ValueError("Cannot generate content for encrypted files")
-        if self.compressed() or imagefile.name.endswith(".aff") or imagefile.name.endswith(".E01"):
-            if icat_fallback:
-                # 
-                # For now, compressed files rely on icat rather than python interface
-                #
-                offset     = safeInt(self.volume.offset)
-                block_size = safeInt(self.volume.block_size)
-                if block_size==0: block_size = 512
-                inode = self.inode()
-                if inode :
-                    block_size = 512
-                    fstype_flag = ""
-                    fstype = self.volume.ftype_str()
-                    if fstype != None:
-                        fstype_flag = '-f' + fstype
-                        cmd = ['icat',fstype_flag,'-b',str(block_size),'-o',str(offset//block_size),imagefile.name,str(inode)]
-                    else:
-                        cmd = ['icat','-b',str(block_size),'-o',str(offset//block_size),imagefile.name,str(inode)]
-                    (data,err) = Popen(cmd, stdout=PIPE,stderr=PIPE).communicate()
-                    # Check for an error
-                    if len(err) > 0 :
-                        #sys.stderr.write("Debug: type(err) = %r.\n" % type(err))
-                        raise ValueError("icat error (" + str(err).strip() + "): "+" ".join(cmd))
-                    return data
-                else :
-                    raise ValueError("Inode missing from file in compressed format.")
-            raise ValueError("Cannot read raw bytes in compressed disk image")
-        res = []
-        for run in self.byte_runs():
-            res.append(self.content_for_run(run=run,imagefile=imagefile))
-        return "".join(res)
-
-    def tempfile(self,calcMD5=False,calcSHA1=False,calcSHA256=False):
-        """Return the contents of imagefile in a named temporary file. If
-        calcMD5, calcSHA1, or calcSHA256 are set TRUE, then the object
-        returned has a hashlib object as self.md5 or self.sha1 with the
-        requested hash."""
-        import tempfile
-        tf = tempfile.NamedTemporaryFile()
-        if calcMD5: tf.md5 = hashlib.md5()
-        if calcSHA1: tf.sha1 = hashlib.sha1()
-        if calcSHA256: tf.sha256 = hashlib.sha256()
-        for run in self.byte_runs():
-            self.imagefile.seek(run.img_offset)
-            count = run.len
-            while count>0:
-                xfer_len = min(count,1024*1024)        # transfer up to a megabyte at a time
-                buf = self.imagefile.read(xfer_len)
-                if len(buf)==0: break
-                tf.write(buf)
-                if calcMD5: tf.md5.update(buf)
-                if calcSHA1: tf.sha1.update(buf)
-                if calcSHA256: tf.sha256.update(buf)
-                count -= xfer_len
-        tf.flush()
-        return tf
-        
-    def savefile(self,filename=None):
-        """Saves the file."""
-        with open(filename,"wb") as f:
-            for run in self.byte_runs():
-                self.imagefile.seek(run.img_offset)
-                count = run.len
-                while count>0:
-                    xfer_len = min(count,1024*1024)        # transfer up to a megabyte at a time 
-                    buf = self.imagefile.read(xfer_len)
-                    if len(buf)==0: break
-                    f.write(buf)
-                    count -= xfer_len
-
-
-    def frag_start_sector(self,fragment):
-        return self.byte_runs()[fragment].img_offset / 512
-
-    def name_type(self):
-        return self.tag("name_type")
-
-class fileobject_dom(fileobject):
-    """file objects created through the DOM. Each object has the XML document
-    stored in the .doc attribute."""    
-    def __init__(self,xmldoc,imagefile=None):
-        fileobject.__init__(self,imagefile=imagefile)
-        self.doc = xmldoc
-
-    def tag(self,name):
-        """Returns the wholeText for any given NAME. Raises KeyError
-        if the NAME does not exist."""
-        try:
-            return self.doc.getElementsByTagName(name)[0].firstChild.wholeText
-        except IndexError:
-            # Check for a hash tag with legacy API
-            if name in ['md5','sha1','sha256']:
-                for e in self.doc.getElementsByTagName('hashdigest'):
-                    if e.getAttribute('type').lower()==name:
-                        return e.firstChild.wholeText
-            raise KeyError(name+" not in XML")
-
-    def has_tag(self,name) :
-        try:
-            temp=self.doc.getElementsByTagName(name)[0].firstChild.wholeText
-            return True
-        except IndexError:
-            # Check for a hash tag with legacy API
-            if name in ['md5','sha1','sha256', 'sha512']:
-                for e in self.doc.getElementsByTagName('hashdigest'):
-                    if e.getAttribute('type').lower()==name:
-                        return True
-            return False
-
-    def byte_runs(self):
-        """Returns a sorted array of byte_run objects.
-        """
-        ret = []
-        try:
-            for run in self.doc.getElementsByTagName("byte_runs")[0].childNodes:
-                b = byte_run()
-                if run.nodeType==run.ELEMENT_NODE:
-                    b.decode_xml_attributes(run.attributes)
-                    ret.append(b)
-        except IndexError:
-            pass
-        ret.sort(key=lambda r:r.file_offset)
-        return ret
-
-class saxobject:
-    # saxobject is a mix-in that makes it easy to turn XML tags into functions.
-    # If the sax tag is registered, then a function with the tag's name is created.
-    # Calling the function returns the value for the tag that is stored in the _tags{}
-    # dictionary. The _tags{} dictionary is filled by the _end_element() method that is defined.
-    # For fileobjects all tags are remembered.
-    def __init__(self):
-        self._tags     = {}
-    def tag(self,name):
-        """Returns the XML text for a given NAME."""
-        return self._tags.get(name,None)
-    def has_tag(self,name) : return name in self._tags
-
-def register_sax_tag(tagclass,name):
-    setattr(tagclass,name,lambda self:self.tag(name))
-
-
-class fileobject_sax(fileobject,saxobject):
-    """file objects created through expat. This class is created with a tags array and a set of byte runs."""
-    def __init__(self,imagefile=None,xml=None):
-        fileobject.__init__(self,imagefile=imagefile)
-        saxobject.__init__(self)
-        self._byte_runs = []
-    def byte_runs(self):
-        """Returns an array of byte_run objects."""
-        return self._byte_runs
-
-
-class volumeobject_sax(saxobject):
-    """A class that represents the volume."""
-    def __init__(self):
-        if hasattr(saxobject, "__init__"):
-            saxobject.__init__(self)
-        self.offset = 0
-        self.block_size = 0
-
-    def __str__(self):
-        return "volume "+(str(self._tags))
-
-    def partition_offset(self):
-        try:
-            return self.tag('partition_offset')
-        except KeyError:
-            return self.tag('Partition_Offset')
-
-register_sax_tag(volumeobject_sax,'ftype')
-register_sax_tag(volumeobject_sax,'ftype_str')
-register_sax_tag(volumeobject_sax,'block_count')
-register_sax_tag(volumeobject_sax,'first_block')
-register_sax_tag(volumeobject_sax,'last_block')
-    
-class imageobject_sax(saxobject):
-    """A class that represents the disk image"""
-register_sax_tag(imageobject_sax,'imagesize')
-register_sax_tag(imageobject_sax,'image_filename')
-
-
-class creatorobject_sax(saxobject):
-    """A class that represents the <creator> section of a DFXML file"""
-for tag in ['creator','program','version']:
-    register_sax_tag(creatorobject_sax,tag)
-
-################################################################
-
-################################################################
-
-def safe_b64decode(b64data):
-    """
-    This function takes care of the logistics of base64 decoding XML data in Python 2 and 3.
-    Recall that Python3 requires b64decode operate on bytes, not a string.
-        Ref: <http://bugs.python.org/issue4769#msg115690>
-    A forum post that noted several encoding differences between Python 2 and 3:
-        <http://stackoverflow.com/questions/9327993/python3-unicode-escape-doesnt-work-with-non-ascii-bytes>
-    """
-    if sys.version_info.major == 2:
-        return base64.b64decode(b64data).decode("unicode_escape")
-    elif sys.version_info.major == 3:
-        dtype = str(type(b64data))
-        to_decode = None
-        if dtype == "<class 'str'>":
-            to_decode = b64data.encode("ascii")
-        elif dtype == "<class 'bytes'>":
-            to_decode = b64data
-        return base64.b64decode(to_decode).decode("unicode_escape")
-    else:
-        raise Exception("Not sure how to parse base64 data outside Python versions 2 or 3.")
-
-class xml_reader:
-    def __init__(self):
-        self.cdata = None
-        self.tagstack = ['xml']
-    
-    def _char_data(self, data):
-        """Handles XML data"""
-        if self.cdata != None:
-            self.cdata += data
-
-    def process_xml_stream(self,xml_stream,callback,preserve_fis=False):
-        "Run the reader on a given XML input stream"
-        self.callback = callback
-        self.preserve_fis = preserve_fis
-        self.fi_history = []
-        import xml.parsers.expat
-        p = xml.parsers.expat.ParserCreate()
-        p.StartElementHandler  = self._start_element
-        p.EndElementHandler    = self._end_element
-        p.CharacterDataHandler = self._char_data
-        p.ParseFile(xml_stream)    
-
-class regxml_reader(xml_reader):
-    def __init__(self,flags=None):
-        self.flags = flags
-        xml_reader.__init__(self)  #TODO wait, shouldn't flags go in here?
-        self.objectstack = []
-        self.registry_object = None
-        self.nonce = 0
-
-    def _start_element(self, name, attrs):
-        """
-        The objectstack conditionally grows, depending on type of element processed
-        * msregistry (hive):  Create a new msregistry object, append to objectstack
-        * key (node):  Create a new key object, append to objectstack
-        * mtime:  The text is going to become a property of the parent element; do not append to objectstack.
-        * value:  Create a new value object, append to objectstack.
-        """
-        new_object = None
-        if name in ["msregistry","hive"]:
-            new_object = registry_object()
-            self.objectstack.append(new_object)
-            self.registry_object = new_object
-        elif name in ["key","node"]:
-            new_object = registry_key_object()
-            
-            #Note these two tests for root and parent _are_ supposed to be independent tests.
-            if attrs.get("root",None) == "1":
-                new_object._type = "root"
-            else:
-                new_object._type = ""
-
-            if len(self.objectstack) > 1:
-                new_object.parent_key = self.objectstack[-1]
-
-            #Sanity check:  root key implies no parent
-            if new_object.type() == "root":
-                assert new_object.parent_key == None
-            #Sanity check:  no parent implies root key --OR-- recovered key
-            if new_object.parent_key == None:
-                assert new_object.used == False or new_object.type() == "root"
-
-            #Define new_object.name
-            #Force a name for keys. If the key has no recorded name, apply artificial name prefix to nonce.
-            name_data = attrs.get("name")
-            if name_data == None:
-                new_object._name = "__DFXML_NONCE_" + str(self.nonce)
-                self.nonce += 1
-            else:
-                enc = attrs.get("name_encoding")
-                if enc == "base64":
-                    new_object._name = safe_b64decode(name_data)
-                else:
-                    new_object._name = name_data
-
-            if new_object.parent_key == None:
-                new_object._full_path = "\\" + new_object.name()
-                # TODO need a name scheme for orphan references, when we start processing orphans
-            else:
-                new_object._full_path = new_object.parent_key.full_path() + "\\" + new_object.name()
-            self.objectstack.append(new_object)
-        elif name in ["value"]:
-            new_object = registry_value_object()
-            new_object.parent_key = self.objectstack[-1]
-            new_object._type = attrs.get("type",None)
-
-            if new_object.type() == "string-list":
-                new_object.strings = []
-            
-            #Store decoded name
-            if attrs.get("default",None) == "1":
-                new_object._name = "Default"
-                if attrs.get("name",attrs.get("key",None)) is not None:
-                    #TODO Notify: concurrently set name attribute and default-name flag
-                    pass
-            else:
-                enc = attrs.get("name_encoding",attrs.get("key_encoding"))
-                name_data = attrs.get("name",attrs.get("key",None))
-                if enc == "base64":
-                    try:
-                        new_object._name = base64.b64decode(name_data.encode("ascii")).decode("unicode_escape")
-                    except:
-                        sys.stderr.write("name_data={}  type={}\n".format(name_data,type(name_data)))
-                        raise
-                else:
-                    new_object._name = name_data
-            new_object._full_path = new_object.parent_key.full_path() + "\\" + new_object.name()
-
-            #Store decoded value
-            new_object.value_data = self.decoded_value(attrs)
-            self.objectstack.append(new_object)
-        elif name in ["mtime"]:
-            self.cdata = ""
-        elif name in ["string"]:
-            self.cdata = ""
-        elif name in ["byte_runs"]:
-            pass
-        elif name in ["byte_run"]:
-            parent = self.objectstack[-1]
-            parent._byte_runs.append(byte_run(file_offset=attrs.get("file_offset"), len=attrs.get("len")))
-        else:
-            raise ValueError("regxml_reader._start_element: Don't know how to start element %s.\n" % name)
-        #Give all cell objects a handle on the registry
-        if new_object != None:
-            new_object.registry_handle = self.registry_object
-
-    def decoded_value(self, attrs):
-        value_data = attrs.get("value",None)
-        if value_data:
-            # TODO adjust hivexml to not use a plain "encoding" attribute
-            value_encoding = attrs.get("encoding", attrs.get("value_encoding")) 
-            if value_encoding == "base64":
-                if sys.version_info.major>2:
-                    value_data = bytes(value_data,encoding='ascii')
-                return base64.b64decode(value_data)
-            else:
-                return value_data
-        else:
-            return None
-
-    def _end_element(self, name):
-        """
-        The callback is invoked for each stack-popping operation, except the root.
-        """
-        # TODO sanity-check the objectstack
-        if name in ["msregistry","hive"]:
-            pass
-        elif name in ["key","node"]:
-            finished_object = self.objectstack.pop()
-            #Add finished object to object index
-            if finished_object.full_path() in self.registry_object.object_index:
-                raise ValueError("regxml_reader._end_element:  Same key path found more than once: " +
-                                 finished_object.full_path())
-            self.registry_object.object_index[finished_object.full_path()] = finished_object
-            self.callback(finished_object)
-        elif name in ["mtime"]:
-            self.objectstack[-1]._mtime = dftime(self.cdata)
-            self.cdata = None
-        elif name in ["value"]:
-            finished_object = self.objectstack.pop()
-            #TODO Simplify once hivexml is patched to have value/@value instead of value/[cdata]
-            if finished_object.value_data == None:
-                finished_object.value_data = self.cdata
-            self.callback(finished_object)
-        elif name in ["string"]:
-            value_object = self.objectstack[-1]
-            if value_object.strings == None:
-                raise ValueError("regxml_reader._end_element:  parsing error, string element found, but parent's type can't support a string list.")
-            value_object.strings.append(self.cdata)
-            self.cdata = None
-        elif name in ["byte_runs","byte_run"]:
-            pass
-        else:
-            raise ValueError("regxml_reader._end_element: Don't know how to end element %s.\n" % name)
-
-class fileobject_reader(xml_reader):
-    """Class which uses the SAX expat-based XML reader.
-    Reads an FIWALK XML input file and automatically creates
-    volumeobject_sax and fileobject_sax objects, but just returns the filoeobject
-    objects.."""
-    def __init__(self,imagefile=None,flags=None):
-        self.creator      = None
-        self.volumeobject = None
-        self.fileobject   = None
-        self.imageobject  = imageobject_sax()
-        self.imagefile    = imagefile
-        self.flags        = flags
-        self._sax_fi_pointer = None
-        xml_reader.__init__(self)
-
-    @property
-    def _sax_fi_pointer(self):
-        """
-        This internal field of a fileobject_reader is a simple state machine.  A DFXML stream can contain fileobjects which contain original_fileobjects, which require the same parsing mechanisms.  This pointer saves on duplicating code with the SAX parser.
-
-        Type: None, or dfxml.fileobject.  Type enforced by the setter method.
-        """
-        return self._sax_fi_pointer_ 
-    @_sax_fi_pointer.setter
-    def _sax_fi_pointer(self, val):
-        if val is None:
-            self._sax_fi_pointer_ = None
-        else:
-            assert isinstance(val, fileobject)
-            self._sax_fi_pointer_ = val
-        
-    def _start_element(self, name, attrs):
-        """ Handles the start of an element for the XPAT scanner"""
-        _logger.debug("fileobject_reader._start_element: name = %r" % name)
-        self.tagstack.append(name)
-        self.cdata = ""          # new element, so reset the data
-        if name=="volume":
-            self.volumeobject            = volumeobject_sax()
-            self.volumeobject.block_size = 512 # reasonable default
-            self.volumeobject.image      = self.imageobject
-            if "offset" in attrs:
-                self.volumeobject.offset = int(attrs["offset"]) 
-            return
-        if name=="block_size":
-            pass
-        if name=="fileobject":
-            self.fileobject = fileobject_sax(imagefile=self.imagefile)
-            self.fileobject.volume = self.volumeobject
-            self._sax_fi_pointer = self.fileobject
-            return
-        if name=="original_fileobject":
-            self.fileobject.original_fileobject = fileobject_sax(imagefile=self.imagefile)
-            #self.original_fileobject.volume = self.volumeobject #TODO
-            self._sax_fi_pointer = self.fileobject.original_fileobject
-            return
-        if name=='hashdigest':
-            self.hashdigest_type = attrs['type'] 
-        if self.fileobject and (name=="run" or name=="byte_run"):
-            b = byte_run()
-            b.decode_sax_attributes(attrs)
-            self.fileobject._byte_runs.append(b)
-            return
-
-
-    def _end_element(self, name):
-        """Handles the end of an element for the XPAT scanner"""
-        assert(self.tagstack.pop()==name) # make sure that the stack matches
-        if name=="volume":
-            self.volumeobject = None
-            return
-        if name=="block_size" and len(self.tagstack) > 1 : 
-            if self.tagstack[-1] == "volume" : 
-                self.volumeobject.block_size = int(self.cdata)
-                self.cdata=None
-            return
-        if name=="fileobject":
-            self.callback(self.fileobject)
-            if self.preserve_fis:
-                self.fi_history.append(self.fileobject)
-            self.fileobject = None
-            return
-        if name=="original_fileobject":
-            self._sax_fi_pointer = self.fileobject
-            return
-        if name=='hashdigest' and len(self.tagstack)>0:
-            top = self.tagstack[-1]            # what the hash was for
-            alg = self.hashdigest_type.lower() # name of the hash algorithm used
-            if top=='byte_run':
-                self._sax_fi_pointer._byte_runs[-1].hashdigest[alg] = self.cdata
-            if top in ["fileobject", "original_fileobject"]:
-                self._sax_fi_pointer._tags[alg] = self.cdata # legacy
-                self._sax_fi_pointer.hashdigest[alg] = self.cdata
-            self.cdata = None
-            return
-
-        if self._sax_fi_pointer:             # in file objects, all tags are remembered
-            self._sax_fi_pointer._tags[name] = self.cdata
-            self.cdata = None
-            return
-        # Special case: <source><image_filename>fn</image_filename></source>
-        # gets put in <image_filename>fn</image_filename>
-        if name in ['image_filename','imagefile'] and self.tagstack[-1]=='source':
-            self.imageobject._tags['image_filename'] = self.cdata
-
-class volumeobject_reader(xml_reader):
-    """Reads just the <volume> section of a DFXML file"""
-    def __init__(self):
-        self.volumeobject = False
-        xml_reader.__init__(self)
-        self.imageobject  = imageobject_sax()
-
-    def _start_element(self, name, attrs):
-        """ Handles the start of an element for the XPAT scanner"""
-        self.tagstack.append(name)
-        if name=="volume":
-            self.volumeobject = volumeobject_sax()
-            self.volumeobject.image = self.imageobject
-            return
-        if name=="fileobject":
-            self.cdata = None            # don't record this
-            return
-        self.cdata = ""                  # new element; otherwise data is ignored
-
-    def _end_element(self, name):
-        """Handles the end of an eleement for the XPAT scanner"""
-        assert(self.tagstack.pop()==name)
-        if name=="volume":
-            self.callback(self.volumeobject)
-            self.volumeobject = None
-            return
-        if self.tagstack[-1]=='volume' and self.volumeobject:             # in the volume
-            self.volumeobject._tags[name] = self.cdata
-            self.cdata = None
-            return
-        if self.tagstack[-1] in ['fiwalk','dfxml']:
-            self.imageobject._tags[name] = self.cdata
-            return
-
-        # Special case: <source><image_filename>fn</image_filename></source> gets put in <image_filename>fn</image_filename>
-        if name in ['image_filename','imagefile'] and self.tagstack[-1]=='source':
-            self.imageobject._tags['image_filename'] = self.cdata
-        return
-
-
-class FinishedReadingCreator(Exception):
-    """Class to indicate that creator object has been read"""
-
-class creatorobject_reader(xml_reader):
-    """Reads the <creator> section of a DFXML file"""
-    def __init__(self):
-        self.creatorobject = False
-        xml_reader.__init__(self)
-
-    def _start_element(self, name, attrs):
-        """ Handles the start of an element for the XPAT scanner"""
-        self.tagstack.append(name)
-        if name=="creator":
-            self.creatorobject = creatorobject_sax()
-            return
-        if self.creatorobject:
-            self.cdata = ""     # capture cdata for creatorobject
-
-    def _end_element(self, name):
-        """Handles the end of an eleement for the XPAT scanner"""
-        assert(self.tagstack.pop()==name)
-        if name=="creator":
-            self.callback(self.creatorobject)
-            self.creatorobject = None
-            raise FinishedReadingCreator("Done")
-        if self.tagstack[-1]=='creator' and self.creatorobject: # in the creator
-            self.creatorobject._tags[name] = self.cdata
-            self.cdata = None
-            return
-
-
-def combine_runs(runs):
-    """Given an array of bytrun elements, combine the runs and return a new array."""
-    if runs==[]: return []
-    ret = [runs[0]]
-    for run in runs[1:]:
-        # if the last one ends where this run begins, just extend
-        # otherwise append
-        last = ret[-1]
-        if last.img_offset+last.len == run.img_offset:
-            ret[-1] = byte_run(img_offset = last.img_offset,
-                              len = last.len + run.len)
-            continue
-        else:
-            ret.append(run)
-    return ret
-
-class extentdb:
-    """A class to a database of extents and report if they collide.
-    Currently this is not an efficient implementation, but it could become
-    more efficient in the future. When it does, every program that uses
-    this implementation will get faster too!  Each extent is represented
-    as a byte_run object"""
-    def __init__(self,sectorsize=512):
-        self.db = []                    # the database of runs
-        self.sectorsize = 512
-        pass
-    
-    def report(self,f):
-        """Print information about the database"""
-        f.write("sectorsize: %d\n" % self.sectorsize)
-        for run in sorted(self.db):
-            f.write("   [@%8d ; %8d]\n" % (run.img_offset,run.len))
-        f.write("total entries in database: %d\n\n" % len(r))
-    
-    def sectors_for_bytes(self,count):
-        """Returns the number of sectors necessary to hold COUNT bytes"""
-        return (count+self.sectorsize-1)//self.sectorsize
-    
-    def sectors_for_run(self,run):
-        """Returns an array of the sectors for a given run"""
-        start_sector = run.img_offset/self.sectorsize
-        sector_count = self.sectors_for_bytes(run.len)
-        return range(start_sector,start_sector+sector_count)
-
-    def run_for_sector(self,sector_number,count=1):
-        """Returns the run for a specified sector, and optionally a count of sectors"""
-        return byte_run(len=count*self.sectorsize,img_offset=sector_number * self.sectorsize)
-
-    def intersects(self,extent):
-        """Returns the intersecting extent, or None if there is none"""
-        if extent.len==0: return True    # 0 length intersects with everything
-        if extent.len<0: raise ValueError("Length cannot be negative:"+str(extent))
-        start = extent.img_offset
-        stop  = extent.img_offset+extent.len
-        for d in self.db:
-            if d.img_offset <= start < d.img_offset+d.len: return d
-            if d.img_offset < stop  < d.img_offset+d.len: return d
-            if start<d.img_offset and d.img_offset+d.len <= stop: return d
-        return None
-
-    def intersects_runs(self,runs):
-        """Returns the intersecting extent for a set of runs, or None
-        if there is none."""
-        for r in runs:
-            v = self.intersects(r)
-            if v: return v
-        return None
-
-    def intersects_sector(self,sector):
-        """Returns the intersecting extent for a specified sector, None otherwise.
-        Sector numbers start at 0."""
-        return self.intersects(self.run_for_sector(sector))
-
-    def add(self,extent):
-        """Adds an EXTENT (start,length) to the database.
-        Raises ValueError if there is an intersection."""
-        v = self.intersects(extent)
-        if v:
-            raise ValueError("Cannot add "+str(extent)+": it intersects "+str(v))
-        self.db.append(extent)
-
-    def add_runs(self,runs):
-        """Adds all of the runs to the extent database"""
-        for r in runs:
-            self.add(r)
-
-    def runs_for_sectors(self,sectors):
-        """Given a list of SECTORS, return a list of RUNS.
-        Automatically combines adjacent runs."""
-
-        runs = [byte_run(len=self.sectorsize,img_offset=x*self.sectorsize) for x in sectors]
-        return combine_runs(runs)
-
-    def add_sectors(self,sectors):
-        """Adds the sectors in the list to the database."""
-        self.add_runs(self.runs_for_sectors(sectors))
-
-    def sectors_not_in_db(self,run):
-        """For a given run, return a list of sectors not in the extent db"""
-        return filter(lambda x:not self.intersects_sector(x),self.sectors_for_run(run))
-
-
-def read_dfxml(xmlfile=None,imagefile=None,flags=0,callback=None,preserve_fis=False):
-    """Processes an image using expat, calling a callback for every file object encountered.
-    If xmlfile is provided, use that as the xmlfile, otherwise runs fiwalk."""
-    if not callback:
-        raise ValueError("callback must be specified")
-    r = fileobject_reader(imagefile=imagefile,flags=flags)
-    if xmlfile and hasattr(xmlfile, "name") and xmlfile.name.endswith(".gz"):
-        buf = xmlfile.read(3)
-        if buf== b'\x1f\x8b\x08':
-            import gzip
-            xmlfile = gzip.open(xmlfile.name,'rb')
-        else:
-            xmlfile.seek(0,0)   # go back to beginning
-    r.process_xml_stream(xmlfile,callback,preserve_fis)
-    return r
-
-def iter_dfxml(xmlfile, preserve_elements=False, imagefile=None):
-    """Returns an interator that yields fileobjects from a DFXML file.
-    
-    @param preserve_elements
-    Yielded fileobjects can also retain the xml.etree.ElementTree.Element,
-    the fileobject's source XML as a manipulable object.
-    Pass preserve_elements=True to get fi.xml_element.
-    NOTE: Retaining Elements is quite memory-intensive.  Creating a MAC
-    timeline from DFXML of the "CFREDS Hacking" image (a 34MB XML file)
-    using demo_mac_timeline_iter.py maxed at 65MB of RAM without
-    preserve_elements, and about 650MB with.  
-    
-    This function might be extended in the future to call Fiwalk (and
-    thus become what fileobjects_iter was supposed to be).
-
-    Note that to serialize the fileobjects to strings, you may wish to
-    use the ET_tostring wrapper function in this module.  The
-    ET.tostring function will print XML namespaces if the input XML has
-    an affiliated namespace.  This is presently necessary from the
-    repeated use of the DFXML sax code, but might not be necessary in
-    the future.
-    ElementTree-and-namespace references:
-      Reading with XML namespaces:
-        http://effbot.org/zone/element-namespaces.htm
-        http://stackoverflow.com/a/13475333/1207160
-        http://stackoverflow.com/a/1319417/1207160
-        http://stackoverflow.com/a/14853417/1207160
-      Writing with XML namespaces:
-        http://stackoverflow.com/a/3895958/1207160
-"""
-    import io
-    import xml.etree.ElementTree as ET
-
-    ET.register_namespace("", XMLNS_DFXML)
-
-    if not xmlfile:
-        raise ValueError("xmlfile must be specified")
-    qtagname = "{%s}fileobject" % XMLNS_DFXML
-    for event, elem in ET.iterparse(xmlfile, ("start","end")):
-        if event == "end":
-            #Note that ElementTree qualifies tag names if possible.  Thus, the paired check.
-            if elem.tag in ["fileobject", qtagname]:
-                xmlstring = ET.tostring(elem)
-                pseudof = io.BytesIO()
-                pseudof.write(xmlstring)
-                pseudof.seek(0)
-                def temp_callback(fi):
-                    #TODO The volumeobject isn't populated this way; need to catch with iterparse.
-                    if preserve_elements:
-                        fi.xml_element = elem
-                reader = read_dfxml(xmlfile=pseudof, imagefile=imagefile, callback=temp_callback, preserve_fis=True)
-                yield reader.fi_history[0]
-                if not preserve_elements:
-                    elem.clear()
-
-
-#This regular expression removes xmlns declarations from elements.
-#Note it will fail if the namespace includes a quote character.
-rx_xmlns = r"""\sxmlns(:\S+)?=['"][^'"]+['"]"""
-
-def ET_tostring(*pargs, **kwargs):
-    """
-    The ElementTree XML interface produces redundant namespace
-    declarations if you print an element at a time.  This method simply
-    removes all xmlns delcarations from the string.
-    """
-    global rx_xmlns
-    import xml.etree.ElementTree as ET
-    tempstring = ET.tostring(*pargs, **kwargs)
-    retval = re.sub(rx_xmlns, "", tempstring)
-    return retval
-
-
-def read_regxml(xmlfile=None,flags=0,callback=None):
-    """Processes an image using expat, calling a callback for node encountered."""
-    import xml.parsers.expat
-    if not callback:
-        raise ValueError("callback must be specified")
-    if not xmlfile:
-        raise ValueError("regxml file must be specified")
-    r = regxml_reader(flags=flags)
-    try:
-        r.process_xml_stream(xmlfile,callback)
-    except xml.parsers.expat.ExpatError as e:
-        stderr.write("XML parsing error for file \"" + xmlfile.name + "\".  Object stack:\n")
-        for x in r.objectstack:
-            stderr.write(str(x) + "\n")
-        stderr.write("(Done.)\n")
-        raise e
-    return r
-
-def fileobjects_sax(xmlfile=None,imagefile=None,flags=0):
-    """Returns a LIST of fileobjects extracted from the given
-    imagefile. If XMLFILE is provided, read the objects are read
-    directly from the XML, otherwise this method runs fiwalk with the
-    specified FLAGS."""
-    ret = []
-    read_dfxml(xmlfile=xmlfile,imagefile=imagefile,flags=flags,
-                     callback=lambda fi:ret.append(fi))
-    return ret
-
-def fileobjects_iter(xmlfile=None,imagefile=None,flags=0):
-    """Returns an iterator that returns fileobjects extracted from the given
-    imagefile. If XMLFILE is provided, read the objects are read
-    directly from the XML, otherwise this method runs fiwalk with the
-    specified FLAGS."""
-    print("For reasons we do not understand, fileobjects_iter currently does not work.")
-    def local_iter(fi):
-        yield fi
-    read_dfxml(xmlfile=xmlfile,imagefile=imagefile,flags=flags,callback=local_iter)
-
-def fileobjects_dom(xmlfile=None,imagefile=None,flags=0):
-    """Returns a tuple consisting of (XML,LIST) where XML is the
-    document of the imagefile's fiwalk and LIST is a list of file
-    objects extracted from that document."""
-
-    import xml.dom.minidom
-    doc =  xml.dom.minidom.parseString(xmlfile.read())
-    ret = []
-    for xmlfi in doc.getElementsByTagName("fileobject"):
-        fi = fileobject_dom(xmlfi,imagefile=imagefile)
-        ret.append(fi)
-    return (doc,ret)
-
-def volumeobjects_sax(xmlfile=None,imagefile=None,flags=0):
-    ret = []
-    r = volumeobject_reader()
-    r.process_xml_stream(xmlfile,imagefile=None,callback=lambda vo:ret.append(vo))
-    return ret
-    
-def creatorobjects_sax(xmlfile=None,flags=0):
-    r = creatorobject_reader()
-    ret = []
-    try:
-        r.process_xml_stream(xmlfile,callback=lambda vo:ret.append(vo))
-    except FinishedReadingCreator as e:
-        pass
-    return ret
-        
-################################################################
-if __name__=="__main__":
-    from optparse import OptionParser
-    parser = OptionParser()
-    parser.add_option("-r","--regress",action="store_true")
-    (options,args) = parser.parse_args()
-
-    def check_equal(a,b,want=None):
-        da = dftime(a)
-        db = dftime(b)
-        result = da==db
-        warn = ""
-        if result != want:
-            warn = " (!)"
-        print("a=%s b=%s want=%s equal=%s%s" % (da,db,want,result,warn))
-    
-    def check_greater(a,b,want=None):
-        da = dftime(a)
-        db = dftime(b)
-        result = da>db
-        warn = ""
-        if result != want:
-            warn = " (!)"
-        print("a=%s b=%s want=%s greater=%s%s" % (da,db,want,result,warn))
-
-    if options.regress:
-        print("Testing unicode value parsing.")
-        #Test base64 encoding of the "Registered" symbol, encountered in a key name in the M57-Patents corpus.
-        test_unicode_string = "\xae"
-        if sys.version_info.major == 2:
-            #The test string doesn't quite get defined right that way in Python 2
-            test_unicode_string = unicode(test_unicode_string, encoding="latin-1")
-            test_unicode_string_escaped = test_unicode_string.encode("unicode_escape")
-            test_base64_bytes = base64.b64encode(test_unicode_string_escaped)
-        elif sys.version_info.major == 3:
-            test_unicode_string_escaped = test_unicode_string.encode("unicode_escape")
-            test_base64_bytes = base64.b64encode(test_unicode_string_escaped)
-        else:
-            #Just hard-code value, no examples yet for this language version.
-            test_base64_bytes = b'XHhhZQ=='
-        test_base64_string = test_base64_bytes.decode("ascii")
-        #test_base64_string is the kind of string data you'd expect to encounter in base64-encoded values processing RegXML.
-        assert test_unicode_string == safe_b64decode(test_base64_bytes)
-        assert test_unicode_string == safe_b64decode(test_base64_string)
-        print("Unicode value parsing good!")
-        print("Testing time string parsing")
-        test_rfc822tdatetime = rfc822Tdatetime("26 Jun 2012 22:34:58 -0700")
-        assert test_rfc822tdatetime.tzinfo is not None
-        print("Time string parsing good!")
-        print("Testing dftime values")
-        #check_equal("1900-01-02T02:03:04Z",-2208895016,True) #AJN time.mktime doesn't seem to support old times any more
-        a_pacific_dftime = dftime("26 Jun 2012 22:34:58 -0700")
-        assert 0.0 == dftime(a_pacific_dftime.iso8601()).timestamp() - a_pacific_dftime.timestamp()
-        check_equal("2000-01-02T02:03:04Z","2000-01-02T03:03:04-0100",False)
-        check_equal("2000-01-02T02:03:04-0100","2000-01-02T02:03:04-0100",True)
-        check_equal("2000-01-02T02:03:04-0100","2000-01-02T02:03:04-0200",False)
-        check_equal("2000-01-02T02:03:04-0100","2000-01-02T01:03:04-0200",True)
-        check_greater("2000-01-02T04:04:05-0100","2000-01-02T03:04:05-0100",True)
-        check_greater("2000-01-02T03:04:05-0200","2000-01-02T03:04:05-0100",True)
-        check_greater("2009-11-17T00:33:30.9375Z","2009-11-17T00:33:30Z",True)
-        check_equal("2009-11-17T00:33:30.9375Z","2009-11-17T00:33:30Z",False)
-        check_equal("2009-11-17T00:33:30.0000Z","2009-11-17T00:33:30Z",True)
-        check_equal("27 Jun 2012 06:02:00 -0000","27 Jun 2012 05:02:00 -0100",True)
-        check_equal("27 Jun 2012 06:02:00 -0000","2012-06-27T06:02:00Z",True)
-        check_equal("26 Jun 2012 22:34:58 -0700","2012-06-27T05:34:58Z", True)
-        print("dftime values passed.")
-        print("Testing byte_run overlap engine:")
-        db = extentdb()
-        a = byte_run(img_offset=0,len=5)
-        db.add(a)
-        b = byte_run(5,5)
-        db.add(b)
-        try:
-            assert db.intersects(byte_run(0,5))==byte_run(0,5)
-        except:
-            print(type(cmp))
-            print(db.intersects(byte_run(0,5)))
-            print(byte_run(0,5))
-            raise
-        assert db.intersects(byte_run(0,1))
-        assert db.intersects(byte_run(2,3))
-        assert db.intersects(byte_run(4,1))
-        assert db.intersects(byte_run(5,1))
-        assert db.intersects(byte_run(6,1))
-        assert db.intersects(byte_run(9,1))
-        assert db.intersects(byte_run(-1,5))
-        assert db.intersects(byte_run(-1,10))
-        assert db.intersects(byte_run(-1,11))
-        assert db.intersects(byte_run(-1,1))==None
-        assert db.intersects(byte_run(10,1))==None
-        print("Overlap engine good!")
-        assert re.sub(rx_xmlns, "", """<fileobject xmlns="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML">""") == "<fileobject>"
-        assert re.sub(rx_xmlns, "", """<fileobject xmlns:dfxml="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML">""") == "<fileobject>"
-        assert re.sub(rx_xmlns, "", """<fileobject delta:new_file="1">""") == """<fileobject delta:new_file="1">"""
-        assert re.sub(rx_xmlns, "", """<fileobject xmlns="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML" attr="1">""") == """<fileobject attr="1">"""
-        print("XML namespace regex good!")
+#!/usr/bin/env python
+#
+# dfxml.py
+# Digital Forensics XML classes
+
+"""Digital Forensics XML classes.
+This module contains a number of classes for dealing with dfxml files,  both using
+the XML DOM model and using the EXPAT model.
+
+The following moduel functions are defined:
+ isone(x)   - returns true if something is equal to 1 (useful for <ALLOC>1</ALLOC>
+ safeInt(x) - converts something to an int but never raises an exception
+
+The following classes are defined in this module:
+ byte_run   - the class for representing a run on the disk
+ dftime     - represents time. Can be in either Unix timestamp or ISO8601.
+              Interconverts as necessary.
+ fileobject - represents a DFXML fileobject.
+
+
+byte_runs() is function that returns an array of byterun objects.
+Each object has the attributes:
+  file_offset - offset from the beginning of the file
+  img_offset  - offset from the beginning of the image
+  len         - the number of bytes
+  fs_offset   - offset from the beginning of the file system
+
+where encoding, if present, is 0 for raw, 1 for NTFS compressed.
+
+"""
+
+__version__ = "1.0.2"
+
+import sys
+import re
+from sys import stderr
+from subprocess import Popen,PIPE
+import base64
+import hashlib
+import os
+
+import datetime
+
+import logging
+_logger = logging.getLogger(os.path.basename(__file__))
+
+tsk_virtual_filenames = set(['$FAT1','$FAT2'])
+
+XMLNS_DC = "http://purl.org/dc/elements/1.1/"
+XMLNS_DFXML = "http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML"
+XMLNS_DELTA = "http://www.forensicswiki.org/wiki/Forensic_Disk_Differencing"
+
+def isone(x):
+    """Return true if something is one (number or string)"""
+    try:
+        return int(x)==1;
+    except TypeError:
+        return False
+
+def safeInt(x):
+    """Return an integer or False.  False is returned, rather than None, because you can
+    divide False by 3 but you can't divide None by 3.
+
+    NOTE: This function could be written as:
+
+    def safeInt(x):
+        return int(x) if x else False
+
+    but that doesn't work on older version of Python."""
+    if x: return int(x)
+    return False
+
+def timestamp2iso8601(ts):
+    import time
+    return time.strftime("%FT%TZ",time.gmtime(ts))
+
+from datetime import tzinfo,timedelta
+class GMTMIN(tzinfo):
+    def __init__(self,minoffset):         # DST starts last Sunday in March
+        self.minoffset = minoffset
+    def utcoffset(self, dt):
+        return timedelta(minutes=self.minoffset)
+    def dst(self, dt):
+        return timedelta(0)
+    def tzname(self,dt):
+         return "GMT+%02d%02d" % (self.minoffset/60,self.minoffset%60)
+
+def parse_iso8601(ts):
+    Z = ts.find('Z')
+    if Z>0:
+        return datetime.datetime.strptime(ts[:Z],"%Y-%m-%dT%H:%M:%S")
+    raise RuntimeError("parse_iso8601: ISO8601 format {} not recognized".format(ts))
+
+
+rx_iso8601 = re.compile("(\d\d\d\d)-(\d\d)-(\d\d)[T ](\d\d):(\d\d):(\d\d)(\.\d+)?(Z|[-+]\d\d:?\d\d)?")
+def iso8601Tdatetime(s):
+    """SLG's conversion of ISO8601 to datetime"""
+    m = rx_iso8601.search(s)
+    if not m:
+        raise ValueError("Cannot parse: "+s)
+    # Get the microseconds
+    try:
+        microseconds = int(float(m.group(7)) * 1000000)
+    except TypeError:
+        microseconds = 0
+    # Figure tz offset
+    offset = None
+    minoffset = None
+    if m.group(8):
+        if m.group(8)=="Z":
+            minoffset = 0
+        elif m.group(8)[0:1] in "-+":
+            minoffset = int(m.group(8)[0:3]) * 60 + int(m.group(8)[-2:])
+    z = s.find("Z")
+    if z>=0:
+        offset = 0
+    # Build the response
+    if minoffset:
+        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
+                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
+                                 microseconds,GMTMIN(minoffset))
+    elif offset:
+        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
+                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
+                                 microseconds,GMTMIN(offset))
+    else:
+        return datetime.datetime(int(m.group(1)),int(m.group(2)),int(m.group(3)),
+                                 int(m.group(4)),int(m.group(5)),int(m.group(6)),
+                                 microseconds)
+
+#This format is as specified in RFC 822, section 5.1, and matches the adjustments in RFC 1123, section 5.2.14.  It appears in email and HTTP headers.
+rx_rfc822datetime = re.compile("(?P<day>\d{1,2}) (?P<month>Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) (?P<year>\d{4}) (?P<hours>\d\d):(?P<minutes>\d\d):(?P<seconds>\d\d) (?P<timezone>Z|[-+]\d\d:?\d\d)")
+three_letter_month_dict = {
+  "Jan": 1,
+  "Feb": 2,
+  "Mar": 3,
+  "Apr": 4,
+  "May": 5,
+  "Jun": 6,
+  "Jul": 7,
+  "Aug": 8,
+  "Sep": 9,
+  "Oct": 10,
+  "Nov": 11,
+  "Dec": 12
+}
+def rfc822Tdatetime(s):
+    """
+    AJN's conversion of times occurring in RFC 822 data to datetime.
+    Follows SLG's pattern.
+    """
+    m = rx_rfc822datetime.search(s)
+    if not m:
+        raise ValueError("Cannot parse as an RFC 822 timestamp: %r." % s)
+    mgd = m.groupdict()
+    # Figure tz offset
+    offset = None
+    minoffset = None
+    match_timezone = mgd.get("timezone")
+    if match_timezone:
+        if match_timezone == "Z":
+            minoffset = 0
+        elif match_timezone[0] in "-+":
+            minoffset = int(match_timezone[0:-2]) * 60 + int(match_timezone[-2:])
+    #TODO Find a reason to use the 'offset' variable? (Hour offset, vs. minute offset?)
+    if minoffset:
+        return datetime.datetime(
+          int(mgd["year"]),
+          three_letter_month_dict[mgd["month"]],
+          int(mgd["day"]),
+          int(mgd["hours"]),
+          int(mgd["minutes"]),
+          int(mgd["seconds"]),
+          0,
+          GMTMIN(minoffset)
+        )
+    else:
+        return datetime.datetime(
+          int(mgd["year"]),
+          three_letter_month_dict[mgd["month"]],
+          int(mgd["day"]),
+          int(mgd["hours"]),
+          int(mgd["minutes"]),
+          int(mgd["seconds"]),
+          0
+        )
+
+################################################################
+###
+###  byte_run class
+###
+
+class byte_run:
+    """The internal representation for a byte run. 
+
+    byte_runs have the following attributes:
+    .img_offset  = offset of the byte run from the image start, in bytes
+    .len         = the length of the run, in bytes (prevoiusly called 'bytes')
+    .sector_size = sector size of the underlying media
+
+    Originally this was an array,
+    which is faster than an attributed object. But this approach is more expandable,
+    and it's only 70% the speed of an array under Python3.0.
+        
+    Note that Python 3 removed the __cmp__ class method:
+        <http://docs.python.org/release/3.0.1/whatsnew/3.0.html#ordering-comparisons>
+    """
+    # declaring slots prevents other attributes from appearing,
+    # but that prevents the code from working with new XML that has new fields.
+    # __slots__ = ["file_offset","img_offset","len","fill","sector_size"]
+    def __init__(self,img_offset=None,len=None,file_offset=None):
+        self.img_offset = img_offset
+        self.file_offset = file_offset
+        self.len = len
+        self.sector_size = 512          # default
+        self.hashdigest  = dict()       # 
+
+    def __lt__(self,other):
+        if self.img_offset is not None and other.img_offset is not None:
+            return self.img_offset < other.img_offset
+        elif self.file_offset is not None and other.file_offset is not None:
+            return self.file_offset < other.file_offset
+        else:
+            raise ValueError("Byte run objects are incomparable")
+    
+    def __eq__(self,other):
+        if self.img_offset is not None and other.img_offset is not None:
+            return self.img_offset == other.img_offset
+        elif self.file_offset is not None and other.file_offset is not None:
+            return self.file_offset == other.file_offset
+        else:
+            raise ValueError("Byte run objects are incomparable")
+
+    def __str__(self):
+        try:
+            return "byte_run[img_offset={0}; file_offset={1} len={2}] ".format(
+                self.img_offset,self.file_offset,self.len)
+        except (AttributeError, TypeError):
+            #Catch attributes that are missing or mis-typed (e.g. NoneType)
+            pass
+        try:
+            return "byte_run[file_offset={0}; fill={1}; len={2}]".format(
+                self.file_offset,self.fill,self.len)
+        except AttributeError:
+            pass
+        try:
+            return "byte_run[file_offset={0}; uncompressed_len={1}]".format(
+                self.file_offset,self.uncompressed_len)
+        except AttributeError:
+            return "byte_run"+str(dir(self))
+    
+    def start_sector(self):
+        return self.img_offset // self.sector_size
+
+    def sector_count(self):
+        return self.len // self.sector_size
+
+    def has_sector(self,s):
+        if self.sector_size==0:
+            raise ValueError("%s: sector_size cannot be 0" % (self))
+        if self.img_offset is None or self.len is None:
+            # Sparse files don't have data allocated on disk
+            return False
+        try:
+            return self.img_offset <= s * self.sector_size < self.img_offset+self.len
+        except AttributeError:
+            # Doesn't have necessary attributes to answer true.
+            # Usually this happens with runs of a constant value
+            return False       
+
+    def extra_len(self):
+        return self.len % self.sector_size
+
+    def decode_xml_attributes(self,attr):
+        for (key,value) in attr.items():
+            try:
+                setattr(self,key,int(value))
+            except ValueError:
+                setattr(self,key,value)
+
+        
+    def decode_sax_attributes(self,attr):
+        for (key,value) in attr.items():
+            if key=='bytes': key=='len' # tag changed name; provide backwards compatiability 
+            try:
+                setattr(self,key,int(value))
+            except ValueError:
+                setattr(self,key,value)
+        
+class ComparableMixin(object):
+    """
+    Comparator "Abstract" class.  Classes inheriting this must define a _cmpkey() method.
+    
+    Credit to Lennart Regebro for the total implementation of this class, found equivalently from:
+    http://regebro.wordpress.com/2010/12/13/python-implementing-rich-comparison-the-correct-way/
+    http://stackoverflow.com/questions/6907323/comparable-classes-in-python-3/6913420#6913420
+    """
+    def _compare(self, other, method):
+        try:
+            return method(self._cmpkey(), other._cmpkey())
+        except (AttributeError, TypeError):
+            # _cmpkey not implemented, or return different type,
+            # so I can't compare with "other".
+            return NotImplemented
+
+    def __lt__(self, other):
+        return self._compare(other, lambda s, o: s < o)
+
+    def __le__(self, other):
+        return self._compare(other, lambda s, o: s <= o)
+
+    def __eq__(self, other):
+        return self._compare(other, lambda s, o: s == o)
+
+    def __ge__(self, other):
+        return self._compare(other, lambda s, o: s >= o)
+
+    def __gt__(self, other):
+        return self._compare(other, lambda s, o: s > o)
+
+    def __ne__(self, other):
+        return self._compare(other, lambda s, o: s != o)
+
+class dftime(ComparableMixin):
+    """Represents a DFXML time. Automatically converts between representations and caches the
+    results as necessary.."""
+    UTC = GMTMIN(0)
+
+    def ts2datetime(self,ts):
+        import datetime
+        return datetime.datetime.utcfromtimestamp(ts).replace(tzinfo=dftime.UTC)
+
+    def __init__(self,val):
+        #'unicode' is not a type in Python 3; 'basestring' is not a type in Python 2.
+        if sys.version_info >= (3,0):
+            _basestring = str
+        else:
+            _basestring = basestring
+        if isinstance(val, str) or isinstance(val,_basestring):
+            #
+            #Test for ISO 8601 format - "YYYY-MM-DD" should have hyphen at val[4]
+            if len(val)>5 and val[4]=="-":
+                self.iso8601_ = val
+            elif len(val) > 15 and ":" in val[13:15]:
+                #Maybe the data are instead the timestamp format found in email headers?
+                #(The check for 13:15 gets the 14th and 15th characters, since the day can be single- or double-digit.)
+                self.datetime_ = rfc822Tdatetime(val)
+            else:
+                #Maybe the data are a string-wrapped int or float?
+                #If this fails, the string format is completely unexpected, so just raise an error.
+                self.timestamp_ = float(val)
+        elif type(val)==int or type(val)==float:
+            self.timestamp_ = val
+        elif isinstance(val, datetime.datetime):
+            self.datetime_ = val
+            #TODO Unit-test this with a timezone-less datetime
+        elif val==None:
+            self.timestamp_ = None
+            self.iso8601_   = None
+        elif isinstance(val, dftime):
+            #If we instead use .timestamp_, we risk having a timezone conversion error
+            self.iso8601_ = val.iso8601()
+        else:
+            raise ValueError("Unknown type '%s' for DFXML time value" % (str(type(val))))
+    def __str__(self):
+        return self.iso8601() or ""
+    def __repr__(self):
+        return repr(self.iso8601()) or "None"
+    def __le__(self,b):
+        if b is None: return None
+        return self.iso8601().__le__(b.iso8601())
+    def __gt__(self,b):
+        if b is None: return None
+        return self.iso8601().__gt__(b.iso8601())
+    def _cmpkey(self):
+        """Provide a key to use for comparisons; for use with ComparableMixin parent class."""
+        return self.timestamp()
+    
+    def __eq__(self,b):
+        if b == None:
+            #This will always be False - if self were None, we wouldn't be in this __eq__ method.
+            return False
+        return self.timestamp()==b.timestamp()
+
+    def iso8601(self):
+        # Do we have a cached representation?
+        import time
+        try:
+            return self.iso8601_
+        except AttributeError:
+            pass
+        
+        # Do we have a datetime representation?
+        try:
+            self.iso8601_ = self.datetime_.isoformat()
+            return self.iso8601_
+        except AttributeError:
+            # We better have a Unix timestamp representation?
+            self.iso8601_ = time.strftime("%Y-%m-%dT%H:%M:%SZ",time.gmtime(self.timestamp_))
+            return self.iso8601_
+    
+    def timestamp(self):
+        import time
+        # Do we have a cached representation?
+        try:
+            return self.timestamp_
+        except AttributeError:
+            pass
+
+        # Do we have a datetime_ object?
+        try:
+            self.timestamp_ = time.mktime(self.datetime_.timetuple())
+            return self.timestamp_
+        except AttributeError:
+            self.datetime_ = iso8601Tdatetime(self.iso8601_)
+            self.timestamp_ = time.mktime(self.datetime_.timetuple())
+            return self.timestamp_
+        
+    def datetime(self):
+        import datetime
+        # return the datetime from parsing either iso8601 or from parsing timestamp
+        try:
+            self.datetime_ = self.ts2datetime(self.timestamp_)
+            # This needs to be in UTC offset. How annoying.
+            return self.datetime_
+        except AttributeError:
+            self.datetime_ = iso8601Tdatetime(self.iso8601_)
+            return self.datetime_
+
+class registry_object:
+    def __init__(self):
+        self.object_index = {}
+        self._mtime = None
+        
+        """Keep handy a handle on the registry object"""
+        self.registry_handle = self
+
+    def mtime(self):
+        return self._mtime
+
+class registry_cell_object:
+    def __init__(self):
+        self._byte_runs  = []
+
+        """This is a pointer to a registry_key_object.  The root node has no parent key."""
+        self.parent_key = None
+
+        self._name        = None
+
+        self._full_path   = None
+
+        """Keys have two types:  "root" (0x2c,0xac) and not-root.  Values have several more types."""
+        self._type        = None
+
+        """Keep handy a handle on the registry object"""
+        self.registry_handle = None
+        
+        """Name the cell type, for str() and repr()."""
+        self._cell_type = "(undefined cell object type)"
+
+        """Only applicable to values."""
+        self._sha1 = None
+
+    def name(self):
+        """This is the name of the present key or value."""
+        return self._name
+
+    def full_path(self):
+        """
+        This is the full path from the root of the hive, with keys acting like directories and the value name acting like the basename.
+
+        Unlike DFXML, registry paths are delimited with a backslash due to the forward slash being a legal and commonly observed character in cell names.
+        """
+        return self._full_path
+
+    def type(self):
+        """
+        This is the data type of the cell.  Keys can be root or not-root; values have several types, like UTF-8, binary, etc.
+        Presently, this exports as a string representation of the type, not the numeric type code.
+        """
+        return self._type
+
+    def _myname(self):
+        """This function is called by repr and str, due to (vague memories of) the possibility of an infinite loop if __repr__ calls __self__."""
+        if len(self._byte_runs) > 0:
+            addr = str(self._byte_runs[0].file_offset)
+        else:
+            addr = "(unknown)"
+        return "".join(["<", self._cell_type, " for hive file offset ", addr, ">"])
+
+    def __repr__(self):
+        return self._myname()
+    def __str__(self):
+        return self._myname()
+
+    def mtime(self):
+        raise NotImplementedError("registry_cell_object.mtime() not over-ridden!")
+
+    def byte_runs(self):
+        """Returns a sorted array of byte_run objects."""
+        #If this idiom is confusing, see:  http://henry.precheur.org/python/copy_list
+        ret = list(self._byte_runs)
+        return ret
+
+    def sha1(self):
+        """
+        Return None. Meant to be overwritten.
+        """
+        return None
+
+    def md5(self):
+        """
+        Return None. Meant to be overwritten.
+        """
+        return None
+    def sha512(self):
+        """
+        Return None. Meant to be overwritten.
+        """
+        return None
+
+class registry_key_object(registry_cell_object):
+    def __init__(self):
+        registry_cell_object.__init__(self)
+        self._mtime = None
+        self.values = {}
+        self.used = True  #TODO Add toggling logic for when hivexml (eventually) processes recovered keys
+        self._cell_type = "registry_key_object"
+    def mtime(self):
+        return self._mtime
+    def root(self):
+        if self.type() is None:
+            return None
+        return self.type() == "root"
+
+class registry_value_object(registry_cell_object):
+    def __init__(self):
+        registry_cell_object.__init__(self)
+        self.value_data  = None
+
+        self._cell_type = "registry_value_object"
+        
+        #TODO Replace to be in line with fileobjects: fileobject.hashdigest is a dictionary
+        self._hashcache = dict()
+
+        """List for the string-list type of value."""
+        self.strings = None
+
+    def mtime(self):
+        """Return nothing.  Alternatively, we might return mtime of parent key in the future."""
+        return None
+    #    if self.parent_key:
+    #        return self.parent_key.mtime()
+    #    else:
+    #        return None
+
+    def _hash(self, hashfunc):
+        """
+        Return cached hash, populating cache if necessary.
+        hashfunc expected values: The functions hashlib.sha1, hashlib.sha256, hashlib.md5.
+        If self.value_data is None, or there are no strings in a "string-list" type, this should return None.
+        Interpretation: Registry values of type "string-list" are hashed by feeding each element of the list into the hash .update() function. All other Registry values are fed in the same way, as a 1-element list.
+        For example, a string type value cell with data "a" fed into this function returns md5("a") (if hashlib.md5 were requested).  A string-list type value cell with data ["a","b"] returns md5("ab").
+        This is a simplification to deal with Registry string encodings, and may change in the future.
+        """
+        if self._hashcache.get(repr(hashfunc)) is None:
+            feed_list = []
+            if self.type() == "string-list":
+                feed_list = self.strings
+            elif not self.value_data is None:
+                feed_list.append(self.value_data)
+            #Normalize to hash .update() required type
+            for (elemindex, elem) in enumerate(feed_list):
+                if type(elem) == type(""):
+                    #String data take a little extra care:
+                    #"The bytes in your ... file are being automatically decoded to Unicode by Python 3 as you read from the file"
+                    #http://stackoverflow.com/a/7778340/1207160
+                    feed_list[elemindex] = elem.encode("utf-8")
+            #Hash if there's data to hash
+            if len(feed_list) > 0:
+                h = hashfunc()
+                for elem in feed_list:
+                    h.update(elem)
+                self._hashcache[repr(hashfunc)] = h.hexdigest()
+        return self._hashcache.get(repr(hashfunc))
+
+    def sha1(self):
+        return self._hash(hashlib.sha1)
+
+    def sha256(self):
+        return self._hash(hashlib.sha256)
+
+    def md5(self):
+        return self._hash(hashlib.md5)
+    def sha512(self):
+        return self._hash(hashlib.sha512)
+
+class fileobject:
+    """The base class for file objects created either through XML DOM or EXPAT"""
+    TIMETAGLIST=['atime','mtime','ctime','dtime','crtime']
+
+    def __init__(self,imagefile=None):
+        self.imagefile  = imagefile
+        self.hashdigest = dict()
+        
+    def __str__(self):
+        try:
+            fn = self.filename()
+        except KeyError:
+            fn = "???"
+        return "fileobject %s byte_runs: %s" % (fn, " ".join([str(x) for x in self.byte_runs()]))
+
+    def partition(self):
+        """Partion number of the file"""
+        return self.tag("partition")
+
+    def filename(self):
+        """Complement name of the file (sometimes called pathname)"""
+        return self.tag("filename")
+
+    def ext(self):
+        """Extension, as a lowercase string without the leading '.'"""
+        import string
+        (base,ext) = os.path.splitext(self.filename())
+        if ext == '':
+            return None
+        else:
+            return ext[1:]
+
+    def filesize(self):
+        """Size of the file, in bytes"""
+        return safeInt(self.tag("filesize"))
+
+    def uid(self):
+        """UID of the file"""
+        return safeInt(self.tag("uid"))
+
+    def gid(self):
+        """GID of the file"""
+        return safeInt(self.tag("gid"))
+
+    def meta_type(self):
+        """Meta-type of the file"""
+        return safeInt(self.tag("meta_type"))
+
+    def mode(self):
+        """Mode of the file"""
+        return safeInt(self.tag("mode"))
+
+    def ctime(self):
+        """Metadata Change Time (sometimes Creation Time), as number of seconds
+        since January 1, 1970 (Unix time)"""
+        t = self.tag("ctime")
+        if t: return dftime(t)
+        return None
+        
+    def atime(self):
+        """Access time, as number of seconds since January 1, 1970 (Unix time)"""
+        t = self.tag("atime")
+        if t: return dftime(t)
+        return None
+        
+    def crtime(self):
+        """CR time, as number of seconds since January 1, 1970 (Unix time)"""
+        t = self.tag("crtime")
+        if t: return dftime(t)
+        return None
+        
+    def mtime(self):
+        """Modify time, as number of seconds since January 1, 1970 (Unix time)"""
+        t = self.tag("mtime")
+        if t: return dftime(t)
+        return None
+        
+    def dtime(self):
+        """ext2 dtime"""
+        t = self.tag("dtime")
+        if t: return dftime(t)
+        return None
+
+    def times(self):
+        """Return a dictionary of all times that the system has"""
+        ret = {}
+        for tag in self.TIMETAGLIST:
+            if self.has_tag(tag):
+                try:
+                    ret[tag] = dftime(self.tag(tag))
+                except TypeError:
+                    pass
+        return ret
+
+    def sha1(self):
+        """Returns the SHA1 in hex"""
+        return self.tag("sha1")
+
+    def sha256(self):
+        """Returns the SHA256 in hex"""
+        return self.tag("sha256")
+
+    def md5(self):
+        """Returns the MD5 in hex"""
+        return self.tag("md5")
+    def sha512(self):
+        """Returns the SHA512 in hex"""
+        return self.tag("sha512")
+
+    def fragments(self):
+        """Returns number of file fragments"""
+        return len(self.byte_runs())
+
+    def name_type(self):
+        """Return the contents of the name_type tag"""
+        return self.tag("name_type")
+
+    def is_virtual(self):
+        """Returns true if the fi entry is a TSK virtual entry"""
+        return self.filename() in tsk_virtual_filenames
+
+    def is_dir(self):
+        """Returns true if file is a directory"""
+        return self.name_type()=='d'
+
+    def is_file(self):
+        """Returns true if file is a file"""
+        return self.name_type()=='r' or self.name_type()==None
+
+    def inode(self):
+        """Inode; may be a number or SleuthKit x-y-z format"""
+        return self.tag("inode")
+
+    def allocated_inode(self):
+        """Returns True if the file's inode data structure is allocated, False otherwise.  (Does not return None.)"""
+        return isone(self.tag("alloc_inode"))
+
+    def allocated_name(self):
+        """Returns True if the file's name data structure is allocated, False otherwise.  (Does not return None.)"""
+        return isone(self.tag("alloc_name"))
+
+    def allocated(self):
+        """Returns True if the file is allocated, False if it was not
+        (that is, if it was deleted or is an orphan).
+        Note that we need to be tolerant of mixed case, as it was changed.
+        We also need to tolerate the case of the unalloc tag being used.
+        """
+        if self.filename()=="$OrphanFiles": return False
+        if self.allocated_inode() and self.allocated_name():
+            return True
+        else:
+            return isone(self.tag("alloc")) or isone(self.tag("ALLOC")) or not isone(self.tag("unalloc"))
+
+    def compressed(self):
+        if not self.has_tag("compressed") and not self.has_tag("compressed") : return False
+        return isone(self.tag("compressed")) or isone(self.tag("COMPRESSED"))
+
+    def encrypted(self):
+        if not self.has_tag("encrypted") and not self.has_tag("encrypted") : return False
+        return isone(self.tag("encrypted")) or isone(self.tag("ENCRYPTED"))
+
+    def file_present(self,imagefile=None):
+        """Returns true if the file is present in the disk image"""
+        if self.filesize()==0:
+            return False               # empty files are never present
+        if imagefile==None:
+            imagefile=self.imagefile # use this one
+        for hashname in ['md5','sha1','sha256', 'sha512']:
+            oldhash = self.tag(hashname)
+            if oldhash:
+                newhash = hashlib.new(hashname,self.contents(imagefile=imagefile)).hexdigest()
+                return oldhash==newhash
+        raise ValueError("Cannot process file "+self.filename()+": no hash in "+str(self))
+
+    def has_contents(self):
+        """True if the file has one or more bytes"""
+        return len(self.byte_runs())>0
+
+    def has_sector(self,s):
+        """True if sector s is contained in one of the byte_runs."""
+        for run in self.byte_runs():
+            if run.has_sector(s): return True
+        return False
+
+    def libmagic(self):
+        """Returns libmagic string if the string is specified
+           in the xml, or None otherwise"""
+        return self.tag("libmagic")
+
+    def content_for_run(self,run=None,imagefile=None):
+        """ Returns the content for a specific run. This is a convenience feature
+        which does not touch the file object if an imagefile is provided."""
+        if imagefile is None: imagefile=self.imagefile
+        if run is None: raise ValueError("content_for_run called without a 'run' argument.")
+
+        if run.len == -1:
+            return chr(0) * run.len
+        elif hasattr(run,'fill'):
+            return chr(run.fill) * run.len
+        else:
+            imagefile.seek(run.img_offset)
+            return imagefile.read(run.len)
+
+    def contents(self,imagefile=None,icat_fallback=True):
+        """ Returns the contents of all the runs concatenated together. For allocated files
+        this should be the original file contents. """
+        if imagefile is None     : imagefile=self.imagefile
+        if imagefile is None     : raise ValueError("imagefile is unknown")
+        if self.encrypted()      : raise ValueError("Cannot generate content for encrypted files")
+        if self.compressed() or imagefile.name.endswith(".aff") or imagefile.name.endswith(".E01"):
+            if icat_fallback:
+                # 
+                # For now, compressed files rely on icat rather than python interface
+                #
+                offset     = safeInt(self.volume.offset)
+                block_size = safeInt(self.volume.block_size)
+                if block_size==0: block_size = 512
+                inode = self.inode()
+                if inode :
+                    block_size = 512
+                    fstype_flag = ""
+                    fstype = self.volume.ftype_str()
+                    if fstype != None:
+                        fstype_flag = '-f' + fstype
+                        cmd = ['icat',fstype_flag,'-b',str(block_size),'-o',str(offset//block_size),imagefile.name,str(inode)]
+                    else:
+                        cmd = ['icat','-b',str(block_size),'-o',str(offset//block_size),imagefile.name,str(inode)]
+                    (data,err) = Popen(cmd, stdout=PIPE,stderr=PIPE).communicate()
+                    # Check for an error
+                    if len(err) > 0 :
+                        #sys.stderr.write("Debug: type(err) = %r.\n" % type(err))
+                        raise ValueError("icat error (" + str(err).strip() + "): "+" ".join(cmd))
+                    return data
+                else :
+                    raise ValueError("Inode missing from file in compressed format.")
+            raise ValueError("Cannot read raw bytes in compressed disk image")
+        res = []
+        for run in self.byte_runs():
+            res.append(self.content_for_run(run=run,imagefile=imagefile))
+        return "".join(res)
+
+    def tempfile(self,calcMD5=False,calcSHA1=False,calcSHA256=False):
+        """Return the contents of imagefile in a named temporary file. If
+        calcMD5, calcSHA1, or calcSHA256 are set TRUE, then the object
+        returned has a hashlib object as self.md5 or self.sha1 with the
+        requested hash."""
+        import tempfile
+        tf = tempfile.NamedTemporaryFile()
+        if calcMD5: tf.md5 = hashlib.md5()
+        if calcSHA1: tf.sha1 = hashlib.sha1()
+        if calcSHA256: tf.sha256 = hashlib.sha256()
+        for run in self.byte_runs():
+            self.imagefile.seek(run.img_offset)
+            count = run.len
+            while count>0:
+                xfer_len = min(count,1024*1024)        # transfer up to a megabyte at a time
+                buf = self.imagefile.read(xfer_len)
+                if len(buf)==0: break
+                tf.write(buf)
+                if calcMD5: tf.md5.update(buf)
+                if calcSHA1: tf.sha1.update(buf)
+                if calcSHA256: tf.sha256.update(buf)
+                count -= xfer_len
+        tf.flush()
+        return tf
+        
+    def savefile(self,filename=None):
+        """Saves the file."""
+        with open(filename,"wb") as f:
+            for run in self.byte_runs():
+                self.imagefile.seek(run.img_offset)
+                count = run.len
+                while count>0:
+                    xfer_len = min(count,1024*1024)        # transfer up to a megabyte at a time 
+                    buf = self.imagefile.read(xfer_len)
+                    if len(buf)==0: break
+                    f.write(buf)
+                    count -= xfer_len
+
+
+    def frag_start_sector(self,fragment):
+        return self.byte_runs()[fragment].img_offset / 512
+
+    def name_type(self):
+        return self.tag("name_type")
+
+class fileobject_dom(fileobject):
+    """file objects created through the DOM. Each object has the XML document
+    stored in the .doc attribute."""    
+    def __init__(self,xmldoc,imagefile=None):
+        fileobject.__init__(self,imagefile=imagefile)
+        self.doc = xmldoc
+
+    def tag(self,name):
+        """Returns the wholeText for any given NAME. Raises KeyError
+        if the NAME does not exist."""
+        try:
+            return self.doc.getElementsByTagName(name)[0].firstChild.wholeText
+        except IndexError:
+            # Check for a hash tag with legacy API
+            if name in ['md5','sha1','sha256']:
+                for e in self.doc.getElementsByTagName('hashdigest'):
+                    if e.getAttribute('type').lower()==name:
+                        return e.firstChild.wholeText
+            raise KeyError(name+" not in XML")
+
+    def has_tag(self,name) :
+        try:
+            temp=self.doc.getElementsByTagName(name)[0].firstChild.wholeText
+            return True
+        except IndexError:
+            # Check for a hash tag with legacy API
+            if name in ['md5','sha1','sha256', 'sha512']:
+                for e in self.doc.getElementsByTagName('hashdigest'):
+                    if e.getAttribute('type').lower()==name:
+                        return True
+            return False
+
+    def byte_runs(self):
+        """Returns a sorted array of byte_run objects.
+        """
+        ret = []
+        try:
+            for run in self.doc.getElementsByTagName("byte_runs")[0].childNodes:
+                b = byte_run()
+                if run.nodeType==run.ELEMENT_NODE:
+                    b.decode_xml_attributes(run.attributes)
+                    ret.append(b)
+        except IndexError:
+            pass
+        ret.sort(key=lambda r:r.file_offset)
+        return ret
+
+class saxobject:
+    # saxobject is a mix-in that makes it easy to turn XML tags into functions.
+    # If the sax tag is registered, then a function with the tag's name is created.
+    # Calling the function returns the value for the tag that is stored in the _tags{}
+    # dictionary. The _tags{} dictionary is filled by the _end_element() method that is defined.
+    # For fileobjects all tags are remembered.
+    def __init__(self):
+        self._tags     = {}
+    def tag(self,name):
+        """Returns the XML text for a given NAME."""
+        return self._tags.get(name,None)
+    def has_tag(self,name) : return name in self._tags
+
+def register_sax_tag(tagclass,name):
+    setattr(tagclass,name,lambda self:self.tag(name))
+
+
+class fileobject_sax(fileobject,saxobject):
+    """file objects created through expat. This class is created with a tags array and a set of byte runs."""
+    def __init__(self,imagefile=None,xml=None):
+        fileobject.__init__(self,imagefile=imagefile)
+        saxobject.__init__(self)
+        self._byte_runs = []
+    def byte_runs(self):
+        """Returns an array of byte_run objects."""
+        return self._byte_runs
+
+
+class volumeobject_sax(saxobject):
+    """A class that represents the volume."""
+    def __init__(self):
+        if hasattr(saxobject, "__init__"):
+            saxobject.__init__(self)
+        self.offset = 0
+        self.block_size = 0
+
+    def __str__(self):
+        return "volume "+(str(self._tags))
+
+    def partition_offset(self):
+        try:
+            return self.tag('partition_offset')
+        except KeyError:
+            return self.tag('Partition_Offset')
+
+register_sax_tag(volumeobject_sax,'ftype')
+register_sax_tag(volumeobject_sax,'ftype_str')
+register_sax_tag(volumeobject_sax,'block_count')
+register_sax_tag(volumeobject_sax,'first_block')
+register_sax_tag(volumeobject_sax,'last_block')
+    
+class imageobject_sax(saxobject):
+    """A class that represents the disk image"""
+register_sax_tag(imageobject_sax,'imagesize')
+register_sax_tag(imageobject_sax,'image_filename')
+
+
+class creatorobject_sax(saxobject):
+    """A class that represents the <creator> section of a DFXML file"""
+for tag in ['creator','program','version']:
+    register_sax_tag(creatorobject_sax,tag)
+
+################################################################
+
+################################################################
+
+def safe_b64decode(b64data):
+    """
+    This function takes care of the logistics of base64 decoding XML data in Python 2 and 3.
+    Recall that Python3 requires b64decode operate on bytes, not a string.
+        Ref: <http://bugs.python.org/issue4769#msg115690>
+    A forum post that noted several encoding differences between Python 2 and 3:
+        <http://stackoverflow.com/questions/9327993/python3-unicode-escape-doesnt-work-with-non-ascii-bytes>
+    """
+    if sys.version_info.major == 2:
+        return base64.b64decode(b64data).decode("unicode_escape")
+    elif sys.version_info.major == 3:
+        dtype = str(type(b64data))
+        to_decode = None
+        if dtype == "<class 'str'>":
+            to_decode = b64data.encode("ascii")
+        elif dtype == "<class 'bytes'>":
+            to_decode = b64data
+        return base64.b64decode(to_decode).decode("unicode_escape")
+    else:
+        raise Exception("Not sure how to parse base64 data outside Python versions 2 or 3.")
+
+class xml_reader:
+    def __init__(self):
+        self.cdata = None
+        self.tagstack = ['xml']
+    
+    def _char_data(self, data):
+        """Handles XML data"""
+        if self.cdata != None:
+            self.cdata += data
+
+    def process_xml_stream(self,xml_stream,callback,preserve_fis=False):
+        "Run the reader on a given XML input stream"
+        self.callback = callback
+        self.preserve_fis = preserve_fis
+        self.fi_history = []
+        import xml.parsers.expat
+        p = xml.parsers.expat.ParserCreate()
+        p.StartElementHandler  = self._start_element
+        p.EndElementHandler    = self._end_element
+        p.CharacterDataHandler = self._char_data
+        p.ParseFile(xml_stream)    
+
+class regxml_reader(xml_reader):
+    def __init__(self,flags=None):
+        self.flags = flags
+        xml_reader.__init__(self)  #TODO wait, shouldn't flags go in here?
+        self.objectstack = []
+        self.registry_object = None
+        self.nonce = 0
+
+    def _start_element(self, name, attrs):
+        """
+        The objectstack conditionally grows, depending on type of element processed
+        * msregistry (hive):  Create a new msregistry object, append to objectstack
+        * key (node):  Create a new key object, append to objectstack
+        * mtime:  The text is going to become a property of the parent element; do not append to objectstack.
+        * value:  Create a new value object, append to objectstack.
+        """
+        new_object = None
+        if name in ["msregistry","hive"]:
+            new_object = registry_object()
+            self.objectstack.append(new_object)
+            self.registry_object = new_object
+        elif name in ["key","node"]:
+            new_object = registry_key_object()
+            
+            #Note these two tests for root and parent _are_ supposed to be independent tests.
+            if attrs.get("root",None) == "1":
+                new_object._type = "root"
+            else:
+                new_object._type = ""
+
+            if len(self.objectstack) > 1:
+                new_object.parent_key = self.objectstack[-1]
+
+            #Sanity check:  root key implies no parent
+            if new_object.type() == "root":
+                assert new_object.parent_key == None
+            #Sanity check:  no parent implies root key --OR-- recovered key
+            if new_object.parent_key == None:
+                assert new_object.used == False or new_object.type() == "root"
+
+            #Define new_object.name
+            #Force a name for keys. If the key has no recorded name, apply artificial name prefix to nonce.
+            name_data = attrs.get("name")
+            if name_data == None:
+                new_object._name = "__DFXML_NONCE_" + str(self.nonce)
+                self.nonce += 1
+            else:
+                enc = attrs.get("name_encoding")
+                if enc == "base64":
+                    new_object._name = safe_b64decode(name_data)
+                else:
+                    new_object._name = name_data
+
+            if new_object.parent_key == None:
+                new_object._full_path = "\\" + new_object.name()
+                # TODO need a name scheme for orphan references, when we start processing orphans
+            else:
+                new_object._full_path = new_object.parent_key.full_path() + "\\" + new_object.name()
+            self.objectstack.append(new_object)
+        elif name in ["value"]:
+            new_object = registry_value_object()
+            new_object.parent_key = self.objectstack[-1]
+            new_object._type = attrs.get("type",None)
+
+            if new_object.type() == "string-list":
+                new_object.strings = []
+            
+            #Store decoded name
+            if attrs.get("default",None) == "1":
+                new_object._name = "Default"
+                if attrs.get("name",attrs.get("key",None)) is not None:
+                    #TODO Notify: concurrently set name attribute and default-name flag
+                    pass
+            else:
+                enc = attrs.get("name_encoding",attrs.get("key_encoding"))
+                name_data = attrs.get("name",attrs.get("key",None))
+                if enc == "base64":
+                    try:
+                        new_object._name = base64.b64decode(name_data.encode("ascii")).decode("unicode_escape")
+                    except:
+                        sys.stderr.write("name_data={}  type={}\n".format(name_data,type(name_data)))
+                        raise
+                else:
+                    new_object._name = name_data
+            new_object._full_path = new_object.parent_key.full_path() + "\\" + new_object.name()
+
+            #Store decoded value
+            new_object.value_data = self.decoded_value(attrs)
+            self.objectstack.append(new_object)
+        elif name in ["mtime"]:
+            self.cdata = ""
+        elif name in ["string"]:
+            self.cdata = ""
+        elif name in ["byte_runs"]:
+            pass
+        elif name in ["byte_run"]:
+            parent = self.objectstack[-1]
+            parent._byte_runs.append(byte_run(file_offset=attrs.get("file_offset"), len=attrs.get("len")))
+        else:
+            raise ValueError("regxml_reader._start_element: Don't know how to start element %s.\n" % name)
+        #Give all cell objects a handle on the registry
+        if new_object != None:
+            new_object.registry_handle = self.registry_object
+
+    def decoded_value(self, attrs):
+        value_data = attrs.get("value",None)
+        if value_data:
+            # TODO adjust hivexml to not use a plain "encoding" attribute
+            value_encoding = attrs.get("encoding", attrs.get("value_encoding")) 
+            if value_encoding == "base64":
+                if sys.version_info.major>2:
+                    value_data = bytes(value_data,encoding='ascii')
+                return base64.b64decode(value_data)
+            else:
+                return value_data
+        else:
+            return None
+
+    def _end_element(self, name):
+        """
+        The callback is invoked for each stack-popping operation, except the root.
+        """
+        # TODO sanity-check the objectstack
+        if name in ["msregistry","hive"]:
+            pass
+        elif name in ["key","node"]:
+            finished_object = self.objectstack.pop()
+            #Add finished object to object index
+            if finished_object.full_path() in self.registry_object.object_index:
+                raise ValueError("regxml_reader._end_element:  Same key path found more than once: " +
+                                 finished_object.full_path())
+            self.registry_object.object_index[finished_object.full_path()] = finished_object
+            self.callback(finished_object)
+        elif name in ["mtime"]:
+            self.objectstack[-1]._mtime = dftime(self.cdata)
+            self.cdata = None
+        elif name in ["value"]:
+            finished_object = self.objectstack.pop()
+            #TODO Simplify once hivexml is patched to have value/@value instead of value/[cdata]
+            if finished_object.value_data == None:
+                finished_object.value_data = self.cdata
+            self.callback(finished_object)
+        elif name in ["string"]:
+            value_object = self.objectstack[-1]
+            if value_object.strings == None:
+                raise ValueError("regxml_reader._end_element:  parsing error, string element found, but parent's type can't support a string list.")
+            value_object.strings.append(self.cdata)
+            self.cdata = None
+        elif name in ["byte_runs","byte_run"]:
+            pass
+        else:
+            raise ValueError("regxml_reader._end_element: Don't know how to end element %s.\n" % name)
+
+class fileobject_reader(xml_reader):
+    """Class which uses the SAX expat-based XML reader.
+    Reads an FIWALK XML input file and automatically creates
+    volumeobject_sax and fileobject_sax objects, but just returns the filoeobject
+    objects.."""
+    def __init__(self,imagefile=None,flags=None):
+        self.creator      = None
+        self.volumeobject = None
+        self.fileobject   = None
+        self.imageobject  = imageobject_sax()
+        self.imagefile    = imagefile
+        self.flags        = flags
+        self._sax_fi_pointer = None
+        xml_reader.__init__(self)
+
+    @property
+    def _sax_fi_pointer(self):
+        """
+        This internal field of a fileobject_reader is a simple state machine.  A DFXML stream can contain fileobjects which contain original_fileobjects, which require the same parsing mechanisms.  This pointer saves on duplicating code with the SAX parser.
+
+        Type: None, or dfxml.fileobject.  Type enforced by the setter method.
+        """
+        return self._sax_fi_pointer_ 
+    @_sax_fi_pointer.setter
+    def _sax_fi_pointer(self, val):
+        if val is None:
+            self._sax_fi_pointer_ = None
+        else:
+            assert isinstance(val, fileobject)
+            self._sax_fi_pointer_ = val
+        
+    def _start_element(self, name, attrs):
+        """ Handles the start of an element for the XPAT scanner"""
+        _logger.debug("fileobject_reader._start_element: name = %r" % name)
+        self.tagstack.append(name)
+        self.cdata = ""          # new element, so reset the data
+        if name=="volume":
+            self.volumeobject            = volumeobject_sax()
+            self.volumeobject.block_size = 512 # reasonable default
+            self.volumeobject.image      = self.imageobject
+            if "offset" in attrs:
+                self.volumeobject.offset = int(attrs["offset"]) 
+            return
+        if name=="block_size":
+            pass
+        if name=="fileobject":
+            self.fileobject = fileobject_sax(imagefile=self.imagefile)
+            self.fileobject.volume = self.volumeobject
+            self._sax_fi_pointer = self.fileobject
+            return
+        if name=="original_fileobject":
+            self.fileobject.original_fileobject = fileobject_sax(imagefile=self.imagefile)
+            #self.original_fileobject.volume = self.volumeobject #TODO
+            self._sax_fi_pointer = self.fileobject.original_fileobject
+            return
+        if name=='hashdigest':
+            self.hashdigest_type = attrs['type'] 
+        if self.fileobject and (name=="run" or name=="byte_run"):
+            b = byte_run()
+            b.decode_sax_attributes(attrs)
+            self.fileobject._byte_runs.append(b)
+            return
+
+
+    def _end_element(self, name):
+        """Handles the end of an element for the XPAT scanner"""
+        assert(self.tagstack.pop()==name) # make sure that the stack matches
+        if name=="volume":
+            self.volumeobject = None
+            return
+        if name=="block_size" and len(self.tagstack) > 1 : 
+            if self.tagstack[-1] == "volume" : 
+                self.volumeobject.block_size = int(self.cdata)
+                self.cdata=None
+            return
+        if name=="fileobject":
+            self.callback(self.fileobject)
+            if self.preserve_fis:
+                self.fi_history.append(self.fileobject)
+            self.fileobject = None
+            return
+        if name=="original_fileobject":
+            self._sax_fi_pointer = self.fileobject
+            return
+        if name=='hashdigest' and len(self.tagstack)>0:
+            top = self.tagstack[-1]            # what the hash was for
+            alg = self.hashdigest_type.lower() # name of the hash algorithm used
+            if top=='byte_run':
+                self._sax_fi_pointer._byte_runs[-1].hashdigest[alg] = self.cdata
+            if top in ["fileobject", "original_fileobject"]:
+                self._sax_fi_pointer._tags[alg] = self.cdata # legacy
+                self._sax_fi_pointer.hashdigest[alg] = self.cdata
+            self.cdata = None
+            return
+
+        if self._sax_fi_pointer:             # in file objects, all tags are remembered
+            self._sax_fi_pointer._tags[name] = self.cdata
+            self.cdata = None
+            return
+        # Special case: <source><image_filename>fn</image_filename></source>
+        # gets put in <image_filename>fn</image_filename>
+        if name in ['image_filename','imagefile'] and self.tagstack[-1]=='source':
+            self.imageobject._tags['image_filename'] = self.cdata
+
+class volumeobject_reader(xml_reader):
+    """Reads just the <volume> section of a DFXML file"""
+    def __init__(self):
+        self.volumeobject = False
+        xml_reader.__init__(self)
+        self.imageobject  = imageobject_sax()
+
+    def _start_element(self, name, attrs):
+        """ Handles the start of an element for the XPAT scanner"""
+        self.tagstack.append(name)
+        if name=="volume":
+            self.volumeobject = volumeobject_sax()
+            self.volumeobject.image = self.imageobject
+            return
+        if name=="fileobject":
+            self.cdata = None            # don't record this
+            return
+        self.cdata = ""                  # new element; otherwise data is ignored
+
+    def _end_element(self, name):
+        """Handles the end of an eleement for the XPAT scanner"""
+        assert(self.tagstack.pop()==name)
+        if name=="volume":
+            self.callback(self.volumeobject)
+            self.volumeobject = None
+            return
+        if self.tagstack[-1]=='volume' and self.volumeobject:             # in the volume
+            self.volumeobject._tags[name] = self.cdata
+            self.cdata = None
+            return
+        if self.tagstack[-1] in ['fiwalk','dfxml']:
+            self.imageobject._tags[name] = self.cdata
+            return
+
+        # Special case: <source><image_filename>fn</image_filename></source> gets put in <image_filename>fn</image_filename>
+        if name in ['image_filename','imagefile'] and self.tagstack[-1]=='source':
+            self.imageobject._tags['image_filename'] = self.cdata
+        return
+
+
+class FinishedReadingCreator(Exception):
+    """Class to indicate that creator object has been read"""
+
+class creatorobject_reader(xml_reader):
+    """Reads the <creator> section of a DFXML file"""
+    def __init__(self):
+        self.creatorobject = False
+        xml_reader.__init__(self)
+
+    def _start_element(self, name, attrs):
+        """ Handles the start of an element for the XPAT scanner"""
+        self.tagstack.append(name)
+        if name=="creator":
+            self.creatorobject = creatorobject_sax()
+            return
+        if self.creatorobject:
+            self.cdata = ""     # capture cdata for creatorobject
+
+    def _end_element(self, name):
+        """Handles the end of an eleement for the XPAT scanner"""
+        assert(self.tagstack.pop()==name)
+        if name=="creator":
+            self.callback(self.creatorobject)
+            self.creatorobject = None
+            raise FinishedReadingCreator("Done")
+        if self.tagstack[-1]=='creator' and self.creatorobject: # in the creator
+            self.creatorobject._tags[name] = self.cdata
+            self.cdata = None
+            return
+
+
+def combine_runs(runs):
+    """Given an array of bytrun elements, combine the runs and return a new array."""
+    if runs==[]: return []
+    ret = [runs[0]]
+    for run in runs[1:]:
+        # if the last one ends where this run begins, just extend
+        # otherwise append
+        last = ret[-1]
+        if last.img_offset+last.len == run.img_offset:
+            ret[-1] = byte_run(img_offset = last.img_offset,
+                              len = last.len + run.len)
+            continue
+        else:
+            ret.append(run)
+    return ret
+
+class extentdb:
+    """A class to a database of extents and report if they collide.
+    Currently this is not an efficient implementation, but it could become
+    more efficient in the future. When it does, every program that uses
+    this implementation will get faster too!  Each extent is represented
+    as a byte_run object"""
+    def __init__(self,sectorsize=512):
+        self.db = []                    # the database of runs
+        self.sectorsize = 512
+        pass
+    
+    def report(self,f):
+        """Print information about the database"""
+        f.write("sectorsize: %d\n" % self.sectorsize)
+        for run in sorted(self.db):
+            f.write("   [@%8d ; %8d]\n" % (run.img_offset,run.len))
+        f.write("total entries in database: %d\n\n" % len(r))
+    
+    def sectors_for_bytes(self,count):
+        """Returns the number of sectors necessary to hold COUNT bytes"""
+        return (count+self.sectorsize-1)//self.sectorsize
+    
+    def sectors_for_run(self,run):
+        """Returns an array of the sectors for a given run"""
+        start_sector = run.img_offset/self.sectorsize
+        sector_count = self.sectors_for_bytes(run.len)
+        return range(start_sector,start_sector+sector_count)
+
+    def run_for_sector(self,sector_number,count=1):
+        """Returns the run for a specified sector, and optionally a count of sectors"""
+        return byte_run(len=count*self.sectorsize,img_offset=sector_number * self.sectorsize)
+
+    def intersects(self,extent):
+        """Returns the intersecting extent, or None if there is none"""
+        if extent.len==0: return True    # 0 length intersects with everything
+        if extent.len<0: raise ValueError("Length cannot be negative:"+str(extent))
+        start = extent.img_offset
+        stop  = extent.img_offset+extent.len
+        for d in self.db:
+            if d.img_offset <= start < d.img_offset+d.len: return d
+            if d.img_offset < stop  < d.img_offset+d.len: return d
+            if start<d.img_offset and d.img_offset+d.len <= stop: return d
+        return None
+
+    def intersects_runs(self,runs):
+        """Returns the intersecting extent for a set of runs, or None
+        if there is none."""
+        for r in runs:
+            v = self.intersects(r)
+            if v: return v
+        return None
+
+    def intersects_sector(self,sector):
+        """Returns the intersecting extent for a specified sector, None otherwise.
+        Sector numbers start at 0."""
+        return self.intersects(self.run_for_sector(sector))
+
+    def add(self,extent):
+        """Adds an EXTENT (start,length) to the database.
+        Raises ValueError if there is an intersection."""
+        v = self.intersects(extent)
+        if v:
+            raise ValueError("Cannot add "+str(extent)+": it intersects "+str(v))
+        self.db.append(extent)
+
+    def add_runs(self,runs):
+        """Adds all of the runs to the extent database"""
+        for r in runs:
+            self.add(r)
+
+    def runs_for_sectors(self,sectors):
+        """Given a list of SECTORS, return a list of RUNS.
+        Automatically combines adjacent runs."""
+
+        runs = [byte_run(len=self.sectorsize,img_offset=x*self.sectorsize) for x in sectors]
+        return combine_runs(runs)
+
+    def add_sectors(self,sectors):
+        """Adds the sectors in the list to the database."""
+        self.add_runs(self.runs_for_sectors(sectors))
+
+    def sectors_not_in_db(self,run):
+        """For a given run, return a list of sectors not in the extent db"""
+        return filter(lambda x:not self.intersects_sector(x),self.sectors_for_run(run))
+
+
+def read_dfxml(xmlfile=None,imagefile=None,flags=0,callback=None,preserve_fis=False):
+    """Processes an image using expat, calling a callback for every file object encountered.
+    If xmlfile is provided, use that as the xmlfile, otherwise runs fiwalk."""
+    if not callback:
+        raise ValueError("callback must be specified")
+    r = fileobject_reader(imagefile=imagefile,flags=flags)
+    if xmlfile and hasattr(xmlfile, "name") and xmlfile.name.endswith(".gz"):
+        buf = xmlfile.read(3)
+        if buf== b'\x1f\x8b\x08':
+            import gzip
+            xmlfile = gzip.open(xmlfile.name,'rb')
+        else:
+            xmlfile.seek(0,0)   # go back to beginning
+    r.process_xml_stream(xmlfile,callback,preserve_fis)
+    return r
+
+def iter_dfxml(xmlfile, preserve_elements=False, imagefile=None):
+    """Returns an interator that yields fileobjects from a DFXML file.
+    
+    @param preserve_elements
+    Yielded fileobjects can also retain the xml.etree.ElementTree.Element,
+    the fileobject's source XML as a manipulable object.
+    Pass preserve_elements=True to get fi.xml_element.
+    NOTE: Retaining Elements is quite memory-intensive.  Creating a MAC
+    timeline from DFXML of the "CFREDS Hacking" image (a 34MB XML file)
+    using demo_mac_timeline_iter.py maxed at 65MB of RAM without
+    preserve_elements, and about 650MB with.  
+    
+    This function might be extended in the future to call Fiwalk (and
+    thus become what fileobjects_iter was supposed to be).
+
+    Note that to serialize the fileobjects to strings, you may wish to
+    use the ET_tostring wrapper function in this module.  The
+    ET.tostring function will print XML namespaces if the input XML has
+    an affiliated namespace.  This is presently necessary from the
+    repeated use of the DFXML sax code, but might not be necessary in
+    the future.
+    ElementTree-and-namespace references:
+      Reading with XML namespaces:
+        http://effbot.org/zone/element-namespaces.htm
+        http://stackoverflow.com/a/13475333/1207160
+        http://stackoverflow.com/a/1319417/1207160
+        http://stackoverflow.com/a/14853417/1207160
+      Writing with XML namespaces:
+        http://stackoverflow.com/a/3895958/1207160
+"""
+    import io
+    import xml.etree.ElementTree as ET
+
+    ET.register_namespace("", XMLNS_DFXML)
+
+    if not xmlfile:
+        raise ValueError("xmlfile must be specified")
+    qtagname = "{%s}fileobject" % XMLNS_DFXML
+    for event, elem in ET.iterparse(xmlfile, ("start","end")):
+        if event == "end":
+            #Note that ElementTree qualifies tag names if possible.  Thus, the paired check.
+            if elem.tag in ["fileobject", qtagname]:
+                xmlstring = ET.tostring(elem)
+                pseudof = io.BytesIO()
+                pseudof.write(xmlstring)
+                pseudof.seek(0)
+                def temp_callback(fi):
+                    #TODO The volumeobject isn't populated this way; need to catch with iterparse.
+                    if preserve_elements:
+                        fi.xml_element = elem
+                reader = read_dfxml(xmlfile=pseudof, imagefile=imagefile, callback=temp_callback, preserve_fis=True)
+                yield reader.fi_history[0]
+                if not preserve_elements:
+                    elem.clear()
+
+
+#This regular expression removes xmlns declarations from elements.
+#Note it will fail if the namespace includes a quote character.
+rx_xmlns = r"""\sxmlns(:\S+)?=['"][^'"]+['"]"""
+
+def ET_tostring(*pargs, **kwargs):
+    """
+    The ElementTree XML interface produces redundant namespace
+    declarations if you print an element at a time.  This method simply
+    removes all xmlns delcarations from the string.
+    """
+    global rx_xmlns
+    import xml.etree.ElementTree as ET
+    tempstring = ET.tostring(*pargs, **kwargs)
+    retval = re.sub(rx_xmlns, "", tempstring)
+    return retval
+
+
+def read_regxml(xmlfile=None,flags=0,callback=None):
+    """Processes an image using expat, calling a callback for node encountered."""
+    import xml.parsers.expat
+    if not callback:
+        raise ValueError("callback must be specified")
+    if not xmlfile:
+        raise ValueError("regxml file must be specified")
+    r = regxml_reader(flags=flags)
+    try:
+        r.process_xml_stream(xmlfile,callback)
+    except xml.parsers.expat.ExpatError as e:
+        stderr.write("XML parsing error for file \"" + xmlfile.name + "\".  Object stack:\n")
+        for x in r.objectstack:
+            stderr.write(str(x) + "\n")
+        stderr.write("(Done.)\n")
+        raise e
+    return r
+
+def fileobjects_sax(xmlfile=None,imagefile=None,flags=0):
+    """Returns a LIST of fileobjects extracted from the given
+    imagefile. If XMLFILE is provided, read the objects are read
+    directly from the XML, otherwise this method runs fiwalk with the
+    specified FLAGS."""
+    ret = []
+    read_dfxml(xmlfile=xmlfile,imagefile=imagefile,flags=flags,
+                     callback=lambda fi:ret.append(fi))
+    return ret
+
+def fileobjects_iter(xmlfile=None,imagefile=None,flags=0):
+    """Returns an iterator that returns fileobjects extracted from the given
+    imagefile. If XMLFILE is provided, read the objects are read
+    directly from the XML, otherwise this method runs fiwalk with the
+    specified FLAGS."""
+    print("For reasons we do not understand, fileobjects_iter currently does not work.")
+    def local_iter(fi):
+        yield fi
+    read_dfxml(xmlfile=xmlfile,imagefile=imagefile,flags=flags,callback=local_iter)
+
+def fileobjects_dom(xmlfile=None,imagefile=None,flags=0):
+    """Returns a tuple consisting of (XML,LIST) where XML is the
+    document of the imagefile's fiwalk and LIST is a list of file
+    objects extracted from that document."""
+
+    import xml.dom.minidom
+    doc =  xml.dom.minidom.parseString(xmlfile.read())
+    ret = []
+    for xmlfi in doc.getElementsByTagName("fileobject"):
+        fi = fileobject_dom(xmlfi,imagefile=imagefile)
+        ret.append(fi)
+    return (doc,ret)
+
+def volumeobjects_sax(xmlfile=None,imagefile=None,flags=0):
+    ret = []
+    r = volumeobject_reader()
+    r.process_xml_stream(xmlfile,imagefile=None,callback=lambda vo:ret.append(vo))
+    return ret
+    
+def creatorobjects_sax(xmlfile=None,flags=0):
+    r = creatorobject_reader()
+    ret = []
+    try:
+        r.process_xml_stream(xmlfile,callback=lambda vo:ret.append(vo))
+    except FinishedReadingCreator as e:
+        pass
+    return ret
+        
+################################################################
+if __name__=="__main__":
+    from optparse import OptionParser
+    parser = OptionParser()
+    parser.add_option("-r","--regress",action="store_true")
+    (options,args) = parser.parse_args()
+
+    def check_equal(a,b,want=None):
+        da = dftime(a)
+        db = dftime(b)
+        result = da==db
+        warn = ""
+        if result != want:
+            warn = " (!)"
+        print("a=%s b=%s want=%s equal=%s%s" % (da,db,want,result,warn))
+    
+    def check_greater(a,b,want=None):
+        da = dftime(a)
+        db = dftime(b)
+        result = da>db
+        warn = ""
+        if result != want:
+            warn = " (!)"
+        print("a=%s b=%s want=%s greater=%s%s" % (da,db,want,result,warn))
+
+    if options.regress:
+        print("Testing unicode value parsing.")
+        #Test base64 encoding of the "Registered" symbol, encountered in a key name in the M57-Patents corpus.
+        test_unicode_string = "\xae"
+        if sys.version_info.major == 2:
+            #The test string doesn't quite get defined right that way in Python 2
+            test_unicode_string = unicode(test_unicode_string, encoding="latin-1")
+            test_unicode_string_escaped = test_unicode_string.encode("unicode_escape")
+            test_base64_bytes = base64.b64encode(test_unicode_string_escaped)
+        elif sys.version_info.major == 3:
+            test_unicode_string_escaped = test_unicode_string.encode("unicode_escape")
+            test_base64_bytes = base64.b64encode(test_unicode_string_escaped)
+        else:
+            #Just hard-code value, no examples yet for this language version.
+            test_base64_bytes = b'XHhhZQ=='
+        test_base64_string = test_base64_bytes.decode("ascii")
+        #test_base64_string is the kind of string data you'd expect to encounter in base64-encoded values processing RegXML.
+        assert test_unicode_string == safe_b64decode(test_base64_bytes)
+        assert test_unicode_string == safe_b64decode(test_base64_string)
+        print("Unicode value parsing good!")
+        print("Testing time string parsing")
+        test_rfc822tdatetime = rfc822Tdatetime("26 Jun 2012 22:34:58 -0700")
+        assert test_rfc822tdatetime.tzinfo is not None
+        print("Time string parsing good!")
+        print("Testing dftime values")
+        #check_equal("1900-01-02T02:03:04Z",-2208895016,True) #AJN time.mktime doesn't seem to support old times any more
+        a_pacific_dftime = dftime("26 Jun 2012 22:34:58 -0700")
+        assert 0.0 == dftime(a_pacific_dftime.iso8601()).timestamp() - a_pacific_dftime.timestamp()
+        check_equal("2000-01-02T02:03:04Z","2000-01-02T03:03:04-0100",False)
+        check_equal("2000-01-02T02:03:04-0100","2000-01-02T02:03:04-0100",True)
+        check_equal("2000-01-02T02:03:04-0100","2000-01-02T02:03:04-0200",False)
+        check_equal("2000-01-02T02:03:04-0100","2000-01-02T01:03:04-0200",True)
+        check_greater("2000-01-02T04:04:05-0100","2000-01-02T03:04:05-0100",True)
+        check_greater("2000-01-02T03:04:05-0200","2000-01-02T03:04:05-0100",True)
+        check_greater("2009-11-17T00:33:30.9375Z","2009-11-17T00:33:30Z",True)
+        check_equal("2009-11-17T00:33:30.9375Z","2009-11-17T00:33:30Z",False)
+        check_equal("2009-11-17T00:33:30.0000Z","2009-11-17T00:33:30Z",True)
+        check_equal("27 Jun 2012 06:02:00 -0000","27 Jun 2012 05:02:00 -0100",True)
+        check_equal("27 Jun 2012 06:02:00 -0000","2012-06-27T06:02:00Z",True)
+        check_equal("26 Jun 2012 22:34:58 -0700","2012-06-27T05:34:58Z", True)
+        print("dftime values passed.")
+        print("Testing byte_run overlap engine:")
+        db = extentdb()
+        a = byte_run(img_offset=0,len=5)
+        db.add(a)
+        b = byte_run(5,5)
+        db.add(b)
+        try:
+            assert db.intersects(byte_run(0,5))==byte_run(0,5)
+        except:
+            print(type(cmp))
+            print(db.intersects(byte_run(0,5)))
+            print(byte_run(0,5))
+            raise
+        assert db.intersects(byte_run(0,1))
+        assert db.intersects(byte_run(2,3))
+        assert db.intersects(byte_run(4,1))
+        assert db.intersects(byte_run(5,1))
+        assert db.intersects(byte_run(6,1))
+        assert db.intersects(byte_run(9,1))
+        assert db.intersects(byte_run(-1,5))
+        assert db.intersects(byte_run(-1,10))
+        assert db.intersects(byte_run(-1,11))
+        assert db.intersects(byte_run(-1,1))==None
+        assert db.intersects(byte_run(10,1))==None
+        print("Overlap engine good!")
+        assert re.sub(rx_xmlns, "", """<fileobject xmlns="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML">""") == "<fileobject>"
+        assert re.sub(rx_xmlns, "", """<fileobject xmlns:dfxml="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML">""") == "<fileobject>"
+        assert re.sub(rx_xmlns, "", """<fileobject delta:new_file="1">""") == """<fileobject delta:new_file="1">"""
+        assert re.sub(rx_xmlns, "", """<fileobject xmlns="http://www.forensicswiki.org/wiki/Category:Digital_Forensics_XML" attr="1">""") == """<fileobject attr="1">"""
+        print("XML namespace regex good!")
```

### Comparing `ifiscripts-2023.7.3.1/scripts/ffv1mkvvalidate.py` & `ifiscripts-2023.7.3.2/scripts/ffv1mkvvalidate.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,197 @@
-#!/usr/bin/env python3
-'''
-Runs mediaconch on FFV1/MKV files.
-The process will validate the files against the FFV1/MKV/PCM standards.
-'''
-import os
-import subprocess
-import sys
-import time
-import argparse
-from lxml import etree
-import ififuncs
-
-
-def logname_check(basename, logs_dir):
-    '''
-    Currently we have a few different logname patterns in our packages.
-    This attempts to return the appropriate one.
-    '''
-    makeffv1_logfile = os.path.join(
-        logs_dir, basename +'.mov_log.log')
-    generic_logfile = os.path.join(
-        logs_dir, basename +'_log.log')
-    mxf_logfile = os.path.join(
-        logs_dir, basename +'.mxf_log.log')
-    sipcreator_logfile = os.path.join(
-        logs_dir, basename + '_sip_log.log')
-    mkv_log = os.path.join(
-        logs_dir, basename +'.mkv_log.log')
-    if os.path.isfile(makeffv1_logfile):
-        return makeffv1_logfile
-    if os.path.isfile(generic_logfile):
-        return generic_logfile
-    if os.path.isfile(mxf_logfile):
-        return mxf_logfile
-    if os.path.isfile(sipcreator_logfile):
-        return sipcreator_logfile
-    if os.path.isfile(mkv_log):
-        return mkv_log
-
-
-def log_results(manifest, log, parent_dir):
-    '''
-    Updates the existing log file. This is copy pasted from validate.py.
-    Eventally, both functions should be merged and moved into ififuncs.
-    '''
-    updated_manifest = []
-    basename = os.path.basename(manifest).replace('_manifest.md5', '')
-    sip_dir = parent_dir
-    logs_dir = os.path.join(sip_dir, 'logs')
-    logname = logname_check(basename, logs_dir)
-    logfile = os.path.join(logs_dir, logname)
-    ififuncs.generate_log(
-        log,
-        'EVENT = Logs consolidation - Log from %s merged into %s' % (log, logfile)
-    )
-    if os.path.isfile(logfile):
-        with open(log, 'r') as fo:
-            validate_log = fo.readlines()
-        with open(logfile, 'ab') as ba:
-            for lines in validate_log:
-                ba.write(lines)
-    with open(manifest, 'r') as manifesto:
-        manifest_lines = manifesto.readlines()
-        for lines in manifest_lines:
-            if os.path.basename(logname) in lines:
-                lines = lines[:31].replace(lines[:31], ififuncs.hashlib_md5(logfile)) + lines[32:]
-            updated_manifest.append(lines)
-    with open(manifest, 'wb') as fo:
-        for lines in updated_manifest:
-            fo.write(lines)
-def setup(full_path, user):
-    '''
-    Sets up filepaths for the rest of the script.
-    This also checks if a mediaconch xml already exists.
-    '''
-    desktop_logs_dir = ififuncs.make_desktop_logs_dir()
-    log_name_source_ = os.path.basename(full_path) + time.strftime("_%Y_%m_%dT%H_%M_%S")
-    log_name_source = "%s/%s_mediaconch_validation.log" % (desktop_logs_dir, log_name_source_)
-    filename = os.path.basename(full_path)
-    object_dir = os.path.dirname(full_path)
-    parent_dir = os.path.dirname(object_dir)
-    sip_root = os.path.dirname(parent_dir)
-    metadata_dir = os.path.join(parent_dir, 'metadata')
-    manifest = os.path.join(
-        sip_root, os.path.basename(parent_dir) + '_manifest.md5'
-    )
-    if not os.path.isfile(manifest):
-        print('manifest does not exist %s' % manifest)
-        return 'skipping'
-    if os.path.isdir(metadata_dir):
-        mediaconch_xmlfile_basename = '%s_mediaconch_validation.xml' % filename
-        mediaconch_xmlfile = os.path.join(
-            metadata_dir, mediaconch_xmlfile_basename
-        )
-        if os.path.isfile(mediaconch_xmlfile):
-            print('mediaconch xml already exists')
-            return 'skipping'
-    else:
-        print('no metadata directory found. Exiting.')
-    return log_name_source, user, mediaconch_xmlfile, manifest, full_path, parent_dir
-
-
-def launch_mediaconch(log_name_source, user, mediaconch_xmlfile, manifest, full_path):
-    '''
-    Run mediaconch on files.
-    '''
-    ififuncs.generate_log(
-        log_name_source,
-        'EVENT = ffv1mkvvalidate.py started'
-    )
-    ififuncs.generate_log(
-        log_name_source,
-        'agentName=%s' % user
-    )
-    ififuncs.generate_log(
-        log_name_source,
-        'eventDetail=ffv1mkvvalidate.py %s' % ififuncs.get_script_version('ffv1mkvvalidate.py')
-    )
-    mediaconch_version = subprocess.check_output(['mediaconch', '-v']).rstrip()
-    ififuncs.generate_log(
-        log_name_source,
-        'agentName=mediaconch, agentversion=%s' % mediaconch_version
-    )
-    if not os.path.isfile(mediaconch_xmlfile):
-        ififuncs.make_mediaconch(full_path, mediaconch_xmlfile)
-        ififuncs.manifest_update(manifest, mediaconch_xmlfile)
-
-
-def parse_mediaconch(mediaconch_xml):
-    '''
-    Parses the mediaconch implementation check report.
-    Returns a dictionary containing the overview of the PASS/FAILs.
-    '''
-    mediaconch_xml_object = etree.parse(mediaconch_xml)
-    mediaconch_namespace = mediaconch_xml_object.xpath('namespace-uri(.)')
-    validation_outcome = mediaconch_xml_object.xpath(
-        '/ns:MediaConch/ns:media/ns:implementationChecks',
-        namespaces={'ns':mediaconch_namespace}
-    )
-    return validation_outcome[0].attrib
-
-def parse_args():
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Recursively validates all MKV files using mediaconch'
-        'Report is written in XML format to the metadata folder and'
-        'manifests and logs are updated'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        'input',
-        help='full path of input directory. All mkv files will be processed.'
-    )
-    parsed_args = parser.parse_args()
-    return parsed_args
-def main():
-    '''
-    Launches the functions that will validate your FFV1/MKV files.
-    '''
-    ififuncs.check_existence(['mediaconch'])
-    args = parse_args()
-    source = args.input
-    user = ififuncs.get_user()
-    for root, _, filenames in os.walk(source):
-        for filename in filenames:
-            if filename[0] != '.' and filename.endswith('.mkv'):
-                if setup(os.path.join(root, filename), user) == 'skipping':
-                    continue
-                else:
-                    log_name_source, user, mediaconch_xmlfile, manifest, full_path, parent_dir = setup(
-                        os.path.join(root, filename), user
-                    )
-                    launch_mediaconch(
-                        log_name_source, user, mediaconch_xmlfile, manifest, full_path,
-                    )
-                    validation_outcome = parse_mediaconch(mediaconch_xmlfile)
-                    print(str(validation_outcome))
-                    if int(validation_outcome['fail_count']) > 0:
-                        print('Validation failed!')
-                        event_outcome = 'fail'
-                    elif int(validation_outcome['fail_count']) == 0:
-                        print('validation successful')
-                        event_outcome = 'pass'
-                    ififuncs.generate_log(
-                        log_name_source,
-                        'EVENT = eventType=validation, eventOutcome=%s, eventDetail=%s' % (
-                            event_outcome, str(validation_outcome)
-                        )
-                    )
-                    log_results(manifest, log_name_source, parent_dir)
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+'''
+Runs mediaconch on FFV1/MKV files.
+The process will validate the files against the FFV1/MKV/PCM standards.
+'''
+import os
+import subprocess
+import sys
+import time
+import argparse
+from lxml import etree
+import ififuncs
+
+
+def logname_check(basename, logs_dir):
+    '''
+    Currently we have a few different logname patterns in our packages.
+    This attempts to return the appropriate one.
+    '''
+    makeffv1_logfile = os.path.join(
+        logs_dir, basename +'.mov_log.log')
+    generic_logfile = os.path.join(
+        logs_dir, basename +'_log.log')
+    mxf_logfile = os.path.join(
+        logs_dir, basename +'.mxf_log.log')
+    sipcreator_logfile = os.path.join(
+        logs_dir, basename + '_sip_log.log')
+    mkv_log = os.path.join(
+        logs_dir, basename +'.mkv_log.log')
+    if os.path.isfile(makeffv1_logfile):
+        return makeffv1_logfile
+    if os.path.isfile(generic_logfile):
+        return generic_logfile
+    if os.path.isfile(mxf_logfile):
+        return mxf_logfile
+    if os.path.isfile(sipcreator_logfile):
+        return sipcreator_logfile
+    if os.path.isfile(mkv_log):
+        return mkv_log
+
+
+def log_results(manifest, log, parent_dir):
+    '''
+    Updates the existing log file. This is copy pasted from validate.py.
+    Eventally, both functions should be merged and moved into ififuncs.
+    '''
+    updated_manifest = []
+    basename = os.path.basename(manifest).replace('_manifest.md5', '')
+    sip_dir = parent_dir
+    logs_dir = os.path.join(sip_dir, 'logs')
+    logname = logname_check(basename, logs_dir)
+    logfile = os.path.join(logs_dir, logname)
+    ififuncs.generate_log(
+        log,
+        'EVENT = Logs consolidation - Log from %s merged into %s' % (log, logfile)
+    )
+    if os.path.isfile(logfile):
+        with open(log, 'r') as fo:
+            validate_log = fo.readlines()
+        with open(logfile, 'ab') as ba:
+            for lines in validate_log:
+                ba.write(lines)
+    with open(manifest, 'r') as manifesto:
+        manifest_lines = manifesto.readlines()
+        for lines in manifest_lines:
+            if os.path.basename(logname) in lines:
+                lines = lines[:31].replace(lines[:31], ififuncs.hashlib_md5(logfile)) + lines[32:]
+            updated_manifest.append(lines)
+    with open(manifest, 'wb') as fo:
+        for lines in updated_manifest:
+            fo.write(lines)
+def setup(full_path, user):
+    '''
+    Sets up filepaths for the rest of the script.
+    This also checks if a mediaconch xml already exists.
+    '''
+    desktop_logs_dir = ififuncs.make_desktop_logs_dir()
+    log_name_source_ = os.path.basename(full_path) + time.strftime("_%Y_%m_%dT%H_%M_%S")
+    log_name_source = "%s/%s_mediaconch_validation.log" % (desktop_logs_dir, log_name_source_)
+    filename = os.path.basename(full_path)
+    object_dir = os.path.dirname(full_path)
+    parent_dir = os.path.dirname(object_dir)
+    sip_root = os.path.dirname(parent_dir)
+    metadata_dir = os.path.join(parent_dir, 'metadata')
+    manifest = os.path.join(
+        sip_root, os.path.basename(parent_dir) + '_manifest.md5'
+    )
+    if not os.path.isfile(manifest):
+        print('manifest does not exist %s' % manifest)
+        return 'skipping'
+    if os.path.isdir(metadata_dir):
+        mediaconch_xmlfile_basename = '%s_mediaconch_validation.xml' % filename
+        mediaconch_xmlfile = os.path.join(
+            metadata_dir, mediaconch_xmlfile_basename
+        )
+        if os.path.isfile(mediaconch_xmlfile):
+            print('mediaconch xml already exists')
+            return 'skipping'
+    else:
+        print('no metadata directory found. Exiting.')
+    return log_name_source, user, mediaconch_xmlfile, manifest, full_path, parent_dir
+
+
+def launch_mediaconch(log_name_source, user, mediaconch_xmlfile, manifest, full_path):
+    '''
+    Run mediaconch on files.
+    '''
+    ififuncs.generate_log(
+        log_name_source,
+        'EVENT = ffv1mkvvalidate.py started'
+    )
+    ififuncs.generate_log(
+        log_name_source,
+        'agentName=%s' % user
+    )
+    ififuncs.generate_log(
+        log_name_source,
+        'eventDetail=ffv1mkvvalidate.py %s' % ififuncs.get_script_version('ffv1mkvvalidate.py')
+    )
+    mediaconch_version = subprocess.check_output(['mediaconch', '-v']).rstrip()
+    ififuncs.generate_log(
+        log_name_source,
+        'agentName=mediaconch, agentversion=%s' % mediaconch_version
+    )
+    if not os.path.isfile(mediaconch_xmlfile):
+        ififuncs.make_mediaconch(full_path, mediaconch_xmlfile)
+        ififuncs.manifest_update(manifest, mediaconch_xmlfile)
+
+
+def parse_mediaconch(mediaconch_xml):
+    '''
+    Parses the mediaconch implementation check report.
+    Returns a dictionary containing the overview of the PASS/FAILs.
+    '''
+    mediaconch_xml_object = etree.parse(mediaconch_xml)
+    mediaconch_namespace = mediaconch_xml_object.xpath('namespace-uri(.)')
+    validation_outcome = mediaconch_xml_object.xpath(
+        '/ns:MediaConch/ns:media/ns:implementationChecks',
+        namespaces={'ns':mediaconch_namespace}
+    )
+    return validation_outcome[0].attrib
+
+def parse_args():
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Recursively validates all MKV files using mediaconch'
+        'Report is written in XML format to the metadata folder and'
+        'manifests and logs are updated'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        'input',
+        help='full path of input directory. All mkv files will be processed.'
+    )
+    parsed_args = parser.parse_args()
+    return parsed_args
+def main():
+    '''
+    Launches the functions that will validate your FFV1/MKV files.
+    '''
+    ififuncs.check_existence(['mediaconch'])
+    args = parse_args()
+    source = args.input
+    user = ififuncs.get_user()
+    for root, _, filenames in os.walk(source):
+        for filename in filenames:
+            if filename[0] != '.' and filename.endswith('.mkv'):
+                if setup(os.path.join(root, filename), user) == 'skipping':
+                    continue
+                else:
+                    log_name_source, user, mediaconch_xmlfile, manifest, full_path, parent_dir = setup(
+                        os.path.join(root, filename), user
+                    )
+                    launch_mediaconch(
+                        log_name_source, user, mediaconch_xmlfile, manifest, full_path,
+                    )
+                    validation_outcome = parse_mediaconch(mediaconch_xmlfile)
+                    print(str(validation_outcome))
+                    if int(validation_outcome['fail_count']) > 0:
+                        print('Validation failed!')
+                        event_outcome = 'fail'
+                    elif int(validation_outcome['fail_count']) == 0:
+                        print('validation successful')
+                        event_outcome = 'pass'
+                    ififuncs.generate_log(
+                        log_name_source,
+                        'EVENT = eventType=validation, eventOutcome=%s, eventDetail=%s' % (
+                            event_outcome, str(validation_outcome)
+                        )
+                    )
+                    log_results(manifest, log_name_source, parent_dir)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/framemd5.py` & `ifiscripts-2023.7.3.2/scripts/framemd5.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/ififuncs.py` & `ifiscripts-2023.7.3.2/scripts/ififuncs.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/loopline_repackage.py` & `ifiscripts-2023.7.3.2/scripts/loopline_repackage.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/make_mediaconch.py` & `ifiscripts-2023.7.3.2/scripts/make_mediaconch.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-#!/usr/bin/env python3
-'''
-Generates Mediaconch xml reports
-Accepts a file extension pattern and a policy input
-Reports of fails are generated to the screen
-Sidecars in XML format generated
-'''
-import argparse
-import os
-import subprocess
-import logging
-
-logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
-def parse_args():
-    '''
-    Accept command line arguments
-    '''
-    parser = argparse.ArgumentParser(description='Generates Mediaconch xml reports'
-    'Accepts a file extension pattern and a policy input'
-    'Reports of fails are generated to the screen'
-    'Sidecars in XML format generated'
-    )
-    parser.add_argument('input', help='path to parent directory')
-    parser.add_argument('-object_extension_pattern', help='the filename extension that you would like to scan for')
-    parser.add_argument('-policy', help='the full path to the mediaconch XML policy')
-    parsed_args = parser.parse_args()
-    return parsed_args
-
-def main():
-    '''
-    Launches the main functions
-    '''
-    args = parse_args()
-    source_folder = args.input
-    for root, _, filenames in os.walk(source_folder):
-        for filename in filenames:
-            if filename[0] != '.':
-                if filename.endswith(args.object_extension_pattern):
-                    full_path = os.path.join(root, filename)
-                    sidecar = full_path + '_MediaConchReport.xml'
-                    mediaconch_cmd = ['mediaconch', full_path, '-p', args.policy, '-fx']
-                    # Running mediaconch twice is very lazy but it saves on XML parsing.
-                    mediaconch_overview_cmd = ['mediaconch', full_path, '-p', args.policy]
-                    mediaconch_output = subprocess.check_output(mediaconch_cmd)
-                    mediaconch_overview = subprocess.check_output(mediaconch_overview_cmd)
-                    if 'fail!' in str(mediaconch_overview):
-                        logging.info('%s does not validate against the policy - look at the sidecar XML for more info' % filename)
-                    elif 'pass!' in str(mediaconch_overview):
-                        logging.info('%s: No failure detected' % filename)
-                    if not os.path.isfile(sidecar):
-                        with open(sidecar, 'wb') as sidecar_object:
-                            sidecar_object.write(mediaconch_output)
-                            logging.info('Generating sidecar - %s' % sidecar)
-                    else:
-                        logging.info('%s already exists - skipping' % sidecar)
-                    if filename.endswith('.mkv'):
-                        mkv_implementation_overview_cmd = ['mediaconch', full_path]
-                        mkv_implementation_overview = subprocess.check_output(mkv_implementation_overview_cmd)
-                        if 'fail!' in str(mkv_implementation_overview):
-                            logging.info('%s does not validate against the implementation - look at the sidecar XML for more info' % filename)
-                        elif 'pass!' in str(mkv_implementation_overview):
-                            logging.info('%s: Valid implementation' % filename)
-                        mkv_sidecar_output = subprocess.check_output(['mediaconch', '-fx', full_path])
-                        if not os.path.isfile(full_path + '_implementation_report'):
-                            with open(full_path + '_ImplementationReport.xml', 'wb') as fo:
-                                fo.write(mkv_sidecar_output)
-                                logging.info('Generating implementation report sidecar: %s'% full_path + 'ImplementationReport.xml')
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+'''
+Generates Mediaconch xml reports
+Accepts a file extension pattern and a policy input
+Reports of fails are generated to the screen
+Sidecars in XML format generated
+'''
+import argparse
+import os
+import subprocess
+import logging
+
+logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
+def parse_args():
+    '''
+    Accept command line arguments
+    '''
+    parser = argparse.ArgumentParser(description='Generates Mediaconch xml reports'
+    'Accepts a file extension pattern and a policy input'
+    'Reports of fails are generated to the screen'
+    'Sidecars in XML format generated'
+    )
+    parser.add_argument('input', help='path to parent directory')
+    parser.add_argument('-object_extension_pattern', help='the filename extension that you would like to scan for')
+    parser.add_argument('-policy', help='the full path to the mediaconch XML policy')
+    parsed_args = parser.parse_args()
+    return parsed_args
+
+def main():
+    '''
+    Launches the main functions
+    '''
+    args = parse_args()
+    source_folder = args.input
+    for root, _, filenames in os.walk(source_folder):
+        for filename in filenames:
+            if filename[0] != '.':
+                if filename.endswith(args.object_extension_pattern):
+                    full_path = os.path.join(root, filename)
+                    sidecar = full_path + '_MediaConchReport.xml'
+                    mediaconch_cmd = ['mediaconch', full_path, '-p', args.policy, '-fx']
+                    # Running mediaconch twice is very lazy but it saves on XML parsing.
+                    mediaconch_overview_cmd = ['mediaconch', full_path, '-p', args.policy]
+                    mediaconch_output = subprocess.check_output(mediaconch_cmd)
+                    mediaconch_overview = subprocess.check_output(mediaconch_overview_cmd)
+                    if 'fail!' in str(mediaconch_overview):
+                        logging.info('%s does not validate against the policy - look at the sidecar XML for more info' % filename)
+                    elif 'pass!' in str(mediaconch_overview):
+                        logging.info('%s: No failure detected' % filename)
+                    if not os.path.isfile(sidecar):
+                        with open(sidecar, 'wb') as sidecar_object:
+                            sidecar_object.write(mediaconch_output)
+                            logging.info('Generating sidecar - %s' % sidecar)
+                    else:
+                        logging.info('%s already exists - skipping' % sidecar)
+                    if filename.endswith('.mkv'):
+                        mkv_implementation_overview_cmd = ['mediaconch', full_path]
+                        mkv_implementation_overview = subprocess.check_output(mkv_implementation_overview_cmd)
+                        if 'fail!' in str(mkv_implementation_overview):
+                            logging.info('%s does not validate against the implementation - look at the sidecar XML for more info' % filename)
+                        elif 'pass!' in str(mkv_implementation_overview):
+                            logging.info('%s: Valid implementation' % filename)
+                        mkv_sidecar_output = subprocess.check_output(['mediaconch', '-fx', full_path])
+                        if not os.path.isfile(full_path + '_implementation_report'):
+                            with open(full_path + '_ImplementationReport.xml', 'wb') as fo:
+                                fo.write(mkv_sidecar_output)
+                                logging.info('Generating implementation report sidecar: %s'% full_path + 'ImplementationReport.xml')
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/makedip.py` & `ifiscripts-2023.7.3.2/scripts/makedip.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-#!/usr/bin/env python3
-'''
-Accept options from command line and make access copy.
-Use makedip.py -h for help
-'''
-import argparse
-import os
-import bitc
-import prores
-
-
-
-def set_options():
-    '''
-    Parse command line options.
-    '''
-    parser = argparse.ArgumentParser(
-        description='IFI Irish Film Institute batch h264/aac proxy creator. ProRes HQ optional.'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        'input'
-    )
-    parser.add_argument(
-        '-o',
-        help='Set output directory.'
-        'The default directory is the same directory as input.', required=True
-    )
-    parser.add_argument(
-        '-prores',
-        action='store_true',
-        help='Use ProRes HQ instead of h264'
-        'The default codec is h264'
-    )
-    parser.add_argument(
-        '-wide',
-        action='store_true', help='Adds 16:9 metadata flag'
-    )
-    parser.add_argument(
-        '-bitc',
-        action='store_true', help='Adds BITC and watermark'
-    )
-    return parser.parse_args()
-def main():
-    '''
-    Launch the various functions that will make a h264/mp4 access copy.
-    '''
-    args = set_options()
-    source = args.input
-    for root, _, filenames in os.walk(source):
-        for filename in filenames:
-            full_path = os.path.join(root, filename)
-            if full_path.endswith(('.mov', '.mkv', '.mxf', '.dv', '.m2t')):
-                if args.prores:
-                    if not args.wide:
-                        prores.main([full_path, '-o', args.o, '-hq'])
-                    else:
-                        prores.main([full_path, '-wide', '-o', args.o, '-hq'])
-                    proxy_filename = os.path.join(args.o, filename +'_prores.mov')
-                    if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('aaa'):
-                        os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_prores.mov')
-                    elif os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('oe'):
-                        os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_prores.mov')
-                else:
-                    if not (os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) in str(os.listdir(args.o)):
-                        bitc_cmd = [full_path, '-o', args.o]
-                        if not args.bitc:
-                            bitc_cmd.extend(['-clean'])
-                        if args.wide:
-                            bitc_cmd.extend(['-wide'])
-                        bitc.main(bitc_cmd)
-                        proxy_filename = os.path.join(args.o, filename +'_h264.mov')
-                        if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('aaa'):
-                            os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
-                        if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('oe'):
-                            os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
-                    else:
-                        print('Skipping %s as the proxy already exists' % os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python3
+'''
+Accept options from command line and make access copy.
+Use makedip.py -h for help
+'''
+import argparse
+import os
+import bitc
+import prores
+
+
+
+def set_options():
+    '''
+    Parse command line options.
+    '''
+    parser = argparse.ArgumentParser(
+        description='IFI Irish Film Institute batch h264/aac proxy creator. ProRes HQ optional.'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        'input'
+    )
+    parser.add_argument(
+        '-o',
+        help='Set output directory.'
+        'The default directory is the same directory as input.', required=True
+    )
+    parser.add_argument(
+        '-prores',
+        action='store_true',
+        help='Use ProRes HQ instead of h264'
+        'The default codec is h264'
+    )
+    parser.add_argument(
+        '-wide',
+        action='store_true', help='Adds 16:9 metadata flag'
+    )
+    parser.add_argument(
+        '-bitc',
+        action='store_true', help='Adds BITC and watermark'
+    )
+    return parser.parse_args()
+def main():
+    '''
+    Launch the various functions that will make a h264/mp4 access copy.
+    '''
+    args = set_options()
+    source = args.input
+    for root, _, filenames in os.walk(source):
+        for filename in filenames:
+            full_path = os.path.join(root, filename)
+            if full_path.endswith(('.mov', '.mkv', '.mxf', '.dv', '.m2t')):
+                if args.prores:
+                    if not args.wide:
+                        prores.main([full_path, '-o', args.o, '-hq'])
+                    else:
+                        prores.main([full_path, '-wide', '-o', args.o, '-hq'])
+                    proxy_filename = os.path.join(args.o, filename +'_prores.mov')
+                    if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('aaa'):
+                        os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_prores.mov')
+                    elif os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('oe'):
+                        os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_prores.mov')
+                else:
+                    if not (os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) in str(os.listdir(args.o)):
+                        bitc_cmd = [full_path, '-o', args.o]
+                        if not args.bitc:
+                            bitc_cmd.extend(['-clean'])
+                        if args.wide:
+                            bitc_cmd.extend(['-wide'])
+                        bitc.main(bitc_cmd)
+                        proxy_filename = os.path.join(args.o, filename +'_h264.mov')
+                        if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('aaa'):
+                            os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
+                        if os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path)))).startswith('oe'):
+                            os.rename(proxy_filename, os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
+                    else:
+                        print('Skipping %s as the proxy already exists' % os.path.join(args.o, os.path.basename(os.path.dirname(os.path.dirname(os.path.dirname(full_path))))) + '_h264.mov')
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/makeffv1.py` & `ifiscripts-2023.7.3.2/scripts/makeffv1.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-#!/usr/bin/env python
-
-# Written by Kieran O'Leary, with a major review and overhaul/cleanup by Zach Kelling aka @Zeekay
-# Makes a single ffv1.mkv
-
-import subprocess
-import sys
-import filecmp
-import os
-import shutil
-import csv
-import time
-import itertools
-import getpass
-from glob import glob
-try:
-    from ififuncs import set_environment
-    from ififuncs import hashlib_manifest
-    from ififuncs import make_mediatrace
-    from ififuncs import make_mediainfo
-    from ififuncs import get_mediainfo
-    from ififuncs import append_csv
-    from ififuncs import create_csv
-    from ififuncs import generate_log
-    from ififuncs import get_ffmpeg_fmt
-except ImportError:
-    print '*** ERROR - IFIFUNCS IS MISSING - *** \n'
-    'Makeffv1 requires that ififuncs.py is located in the same directory'
-    ' as some functions are located in that script -'
-    'https://github.com/kieranjol/IFIscripts/blob/master/ififuncs.py'
-    sys.exit()
-
-def read_non_comment_lines(infile):
-    # Adapted from Andrew Dalke - http://stackoverflow.com/a/8304087/2188572
-    for lineno, line in enumerate(infile):
-        #if line[:1] != "#":
-        yield lineno, line
-
-def get_input():
-    if len(sys.argv) < 2:
-        print 'IFI FFV1.MKV SCRIPT'
-        print 'USAGE: PYTHON makeffv1.py FILENAME'
-        print 'OR'
-        print 'USAGE: PYTHON makeffv1.py DirectoryNAME'
-        print 'If input is a directory, all files will be processed'
-        print 'If input is a file, only that file will be processed'
-        sys.exit()
-    else:
-        # Input, either file or firectory, that we want to process.
-        input = sys.argv[1]
-        # Store the directory containing the input file/directory.
-        wd = os.path.dirname(input)
-        # Change current working directory to the value stored as "wd"
-        os.chdir(os.path.abspath(wd))
-        # Store the actual file/directory name without the full path.
-        file_without_path = os.path.basename(input)
-        csv_report_filename = (
-            os.path.basename(input)
-            + 'makeffv1_results'
-            + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.csv'
-            )
-        # Check if input is a file.
-        # AFAIK, os.path.isfile only works if full path isn't present.
-        if os.path.isfile(file_without_path):
-            print "single file found"
-            video_files = []                       # Create empty list
-            video_files.append(file_without_path)  # Add filename to list
-        # Check if input is a directory.
-        elif os.path.isdir(file_without_path):
-            os.chdir(file_without_path)
-            video_files = (
-                glob('*.mov')
-                + glob('*.mp4')
-                + glob('*.mxf')
-                + glob('*.mkv')
-                + glob('*.avi')
-                + glob('*.y4m')
-                )
-        else:
-            print "Your input isn't a file or a directory."
-            print "What was it? I'm curious."
-        # temporary hack to stop makeffv1 from processing DV
-        dv_test = []
-        for test_files in video_files:
-            codec =  get_mediainfo(
-                'codec', '--inform=Video;%Codec%',
-                 test_files
-                 ).rstrip()
-            if codec == 'DV':
-                dv_test.append(test_files)
-                print 'DV file found, skipping'
-        for i in dv_test:
-            if i in video_files:
-                video_files.remove(i)
-        create_csv(
-            csv_report_filename,
-            (
-                'FILENAME', 'Lossless?',
-                'Source size in bits', 'FFV1 size in bits',
-                ' Compression ratio'
-                )
-            )
-        return video_files, csv_report_filename
-def make_ffv1(video_files, csv_report_filename):
-    for filename in video_files: #loop all files in directory
-        filenoext = os.path.splitext(filename)[0]
-        # Generate new directory names
-        metadata_dir = "%s/metadata" % filenoext
-        log_dir = "%s/logs" % filenoext
-        data_dir = "%s/objects" % filenoext
-        # Actually create the directories.
-        os.makedirs(metadata_dir)
-        os.makedirs(data_dir)
-        os.makedirs(log_dir)
-        #Generate filenames for new files.
-        inputxml = "%s/%s_source_mediainfo.xml" % (
-            metadata_dir, os.path.basename(filename)
-            )
-        inputtracexml = "%s/%s_source_mediatrace.xml" % (
-            metadata_dir, os.path.basename(filename)
-            )
-        output = "%s/%s.mkv" % (
-            data_dir, os.path.splitext(os.path.basename(filename))[0]
-            )
-        # Generate filename of ffv1.mkv without the path.
-        outputfilename = os.path.basename(output)
-        outputxml = "%s/%s_mediainfo.xml" % (metadata_dir, outputfilename)
-        outputtracexml = "%s/%s_mediatrace.xml" % (metadata_dir, outputfilename)
-        fmd5 = "%s/%s_source.framemd5" % (
-            metadata_dir, os.path.basename(filename)
-            )
-        fmd5ffv1 = "%s/%s_ffv1.framemd5" % (metadata_dir, outputfilename)
-        log = "%s/%s_log.log" %  (log_dir, filename)
-        generate_log(log, 'Input = %s' % filename)
-        generate_log(log, 'Output = %s' % output)
-        generate_log(
-            log, 'makeffv1.py transcode to FFV1 and framemd5 generation of source started.'
-            )
-        ffv1_logfile = log_dir + '/%s_ffv1_transcode.log' % filename
-        ffv1_env_dict = set_environment(ffv1_logfile)
-        par = subprocess.check_output(
-            [
-                'mediainfo', '--Language=raw', '--Full',
-                "--Inform=Video;%PixelAspectRatio%", filename
-            ]
-            ).rstrip()
-        field_order = subprocess.check_output(
-            [
-                'mediainfo', '--Language=raw',
-                '--Full', "--Inform=Video;%ScanType%", filename
-            ]
-            ).rstrip()
-        height = subprocess.check_output(
-            [
-                'mediainfo', '--Language=raw',
-                '--Full', "--Inform=Video;%Height%",
-                filename
-            ]
-            ).rstrip()
-        # Transcode video file writing frame md5 and output appropriately
-        ffv1_command = [
-            'ffmpeg',
-            '-i', filename,
-            '-c:v', 'ffv1',        # Use FFv1 codec
-            '-g', '1',              # Use intra-frame only aka ALL-I aka GOP=1
-            '-level', '3',          # Use Version 3 of FFv1
-            '-c:a', 'copy',         # Copy and paste audio bitsream with no transcoding
-            '-map', '0',
-            '-dn',
-            '-report',
-            '-slicecrc', '1',
-            '-slices', '16',
-            ]
-        # check for FCP7 lack of description and PAL
-        if par == '1.000':
-            if field_order == '':
-                if height == '576':
-                    ffv1_command += [
-                        '-vf',
-                        'setfield=tff, setdar=4/3'
-                        ]
-        ffv1_command += [
-            output,
-            '-f', 'framemd5', '-an',  # Create decoded md5 checksums for every frame of the input. -an ignores audio
-            fmd5
-            ]
-        print ffv1_command
-        subprocess.call(ffv1_command, env=ffv1_env_dict)
-        generate_log(
-            log, 'makeffv1.py transcode to FFV1 and framemd5 generation completed.'
-            )
-        generate_log(
-            log, 'makeffv1.py Framemd5 generation of output file started.'
-            )
-        fmd5_logfile = log_dir + '/%s_framemd5.log' % outputfilename
-        fmd5_env_dict = set_environment(fmd5_logfile)
-        pix_fmt = get_ffmpeg_fmt(filename, 'video')
-        fmd5_command = [
-            'ffmpeg',    # Create decoded md5 checksums for every frame
-            '-i', output,
-            '-report',
-            '-pix_fmt', pix_fmt,
-            '-f', 'framemd5', '-an',
-            fmd5ffv1
-            ]
-        print fmd5_command
-        subprocess.call(fmd5_command, env=fmd5_env_dict)
-        generate_log(
-            log,
-            'makeffv1.py Framemd5 generation of output file completed'
-            )
-        source_video_size = get_mediainfo(
-            'source_video_size', "--inform=General;%FileSize%", filename
-            )
-        ffv1_video_size = get_mediainfo(
-            'ffv1_video_size', '--inform=General;%FileSize%', output
-            )
-        compression_ratio = float(source_video_size) / float(ffv1_video_size)
-        if os.path.basename(sys.argv[0]) == 'makeffv1.py':
-            try:
-                shutil.copy(sys.argv[0], log_dir)
-            except IOError:
-                pass
-        print 'Generating mediainfo xml of input file and saving it in %s' % inputxml
-        make_mediainfo(inputxml, 'mediaxmlinput', filename)
-        print 'Generating mediainfo xml of output file and saving it in %s' % outputxml
-        make_mediainfo(outputxml, 'mediaxmloutput', output)
-        print 'Generating mediatrace xml of input file and saving it in %s' % inputtracexml
-        make_mediatrace(inputtracexml, 'mediatracexmlinput', filename)
-        print 'Generating mediatrace xml of output file and saving it in %s' % outputtracexml
-        make_mediatrace(outputtracexml, 'mediatracexmloutput', output)
-        source_parent_dir = os.path.dirname(os.path.abspath(filename))
-        manifest = '%s/%s_manifest.md5' % (source_parent_dir, filenoext)
-        generate_log(log, 'makeffv1.py MD5 manifest started')
-        checksum_mismatches = []
-        with open(fmd5) as f1:
-            with open(fmd5ffv1) as f2:
-                for (lineno1, line1), (lineno2, line2) in itertools.izip(
-                        read_non_comment_lines(f1),
-                        read_non_comment_lines(f2)
-                        ):
-                    if line1 != line2:
-                        if 'sar' in line1:
-                            checksum_mismatches = ['sar']
-                        else:
-                            checksum_mismatches.append(1)
-        if len(checksum_mismatches) == 0:
-            print 'LOSSLESS'
-            append_csv(
-                csv_report_filename, (
-                    output,
-                    'LOSSLESS', source_video_size,
-                    ffv1_video_size, compression_ratio
-                    )
-                )
-            generate_log(log, 'makeffv1.py Transcode was lossless')
-        elif len(checksum_mismatches) == 1:
-            if checksum_mismatches[0] == 'sar':
-                print 'Image content is lossless,'
-                ' Pixel Aspect Ratio has been altered.'
-                ' Update ffmpeg in order to resolve the PAR issue.'
-                append_csv(
-                    csv_report_filename,
-                    (
-                        output,
-                        'LOSSLESS - different PAR',
-                        source_video_size, ffv1_video_size, compression_ratio
-                        )
-                    )
-                generate_log(
-                    log,
-                    'makeffv1.py Image content is lossless but Pixel Aspect Ratio has been altered.Update ffmpeg in order to resolve the PAR issue.'
-                    )
-        elif len(checksum_mismatches) > 1:
-            print 'NOT LOSSLESS'
-            append_csv(
-                csv_report_filename,
-                (
-                    output, 'NOT LOSSLESS',
-                    source_video_size, ffv1_video_size, compression_ratio
-                    )
-                )
-            generate_log(log, 'makeffv1.py Not Lossless.')
-        hashlib_manifest(filenoext, manifest, source_parent_dir)
-        if filecmp.cmp(fmd5, fmd5ffv1, shallow=False):
-            print "YOUR FILES ARE LOSSLESS YOU SHOULD BE SO HAPPY!!!"
-        else:
-            print "The framemd5 text files are not completely identical."
-            " This may be because of a lossy transcode,"
-            " or a change in metadata, most likely pixel aspect ratio."
-            " Please analyse the framemd5 files for source and output."
-
-def main():
-    video_files, csv_report_filename = get_input()
-    make_ffv1(video_files, csv_report_filename)
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+
+# Written by Kieran O'Leary, with a major review and overhaul/cleanup by Zach Kelling aka @Zeekay
+# Makes a single ffv1.mkv
+
+import subprocess
+import sys
+import filecmp
+import os
+import shutil
+import csv
+import time
+import itertools
+import getpass
+from glob import glob
+try:
+    from ififuncs import set_environment
+    from ififuncs import hashlib_manifest
+    from ififuncs import make_mediatrace
+    from ififuncs import make_mediainfo
+    from ififuncs import get_mediainfo
+    from ififuncs import append_csv
+    from ififuncs import create_csv
+    from ififuncs import generate_log
+    from ififuncs import get_ffmpeg_fmt
+except ImportError:
+    print '*** ERROR - IFIFUNCS IS MISSING - *** \n'
+    'Makeffv1 requires that ififuncs.py is located in the same directory'
+    ' as some functions are located in that script -'
+    'https://github.com/kieranjol/IFIscripts/blob/master/ififuncs.py'
+    sys.exit()
+
+def read_non_comment_lines(infile):
+    # Adapted from Andrew Dalke - http://stackoverflow.com/a/8304087/2188572
+    for lineno, line in enumerate(infile):
+        #if line[:1] != "#":
+        yield lineno, line
+
+def get_input():
+    if len(sys.argv) < 2:
+        print 'IFI FFV1.MKV SCRIPT'
+        print 'USAGE: PYTHON makeffv1.py FILENAME'
+        print 'OR'
+        print 'USAGE: PYTHON makeffv1.py DirectoryNAME'
+        print 'If input is a directory, all files will be processed'
+        print 'If input is a file, only that file will be processed'
+        sys.exit()
+    else:
+        # Input, either file or firectory, that we want to process.
+        input = sys.argv[1]
+        # Store the directory containing the input file/directory.
+        wd = os.path.dirname(input)
+        # Change current working directory to the value stored as "wd"
+        os.chdir(os.path.abspath(wd))
+        # Store the actual file/directory name without the full path.
+        file_without_path = os.path.basename(input)
+        csv_report_filename = (
+            os.path.basename(input)
+            + 'makeffv1_results'
+            + time.strftime("_%Y_%m_%dT%H_%M_%S") + '.csv'
+            )
+        # Check if input is a file.
+        # AFAIK, os.path.isfile only works if full path isn't present.
+        if os.path.isfile(file_without_path):
+            print "single file found"
+            video_files = []                       # Create empty list
+            video_files.append(file_without_path)  # Add filename to list
+        # Check if input is a directory.
+        elif os.path.isdir(file_without_path):
+            os.chdir(file_without_path)
+            video_files = (
+                glob('*.mov')
+                + glob('*.mp4')
+                + glob('*.mxf')
+                + glob('*.mkv')
+                + glob('*.avi')
+                + glob('*.y4m')
+                )
+        else:
+            print "Your input isn't a file or a directory."
+            print "What was it? I'm curious."
+        # temporary hack to stop makeffv1 from processing DV
+        dv_test = []
+        for test_files in video_files:
+            codec =  get_mediainfo(
+                'codec', '--inform=Video;%Codec%',
+                 test_files
+                 ).rstrip()
+            if codec == 'DV':
+                dv_test.append(test_files)
+                print 'DV file found, skipping'
+        for i in dv_test:
+            if i in video_files:
+                video_files.remove(i)
+        create_csv(
+            csv_report_filename,
+            (
+                'FILENAME', 'Lossless?',
+                'Source size in bits', 'FFV1 size in bits',
+                ' Compression ratio'
+                )
+            )
+        return video_files, csv_report_filename
+def make_ffv1(video_files, csv_report_filename):
+    for filename in video_files: #loop all files in directory
+        filenoext = os.path.splitext(filename)[0]
+        # Generate new directory names
+        metadata_dir = "%s/metadata" % filenoext
+        log_dir = "%s/logs" % filenoext
+        data_dir = "%s/objects" % filenoext
+        # Actually create the directories.
+        os.makedirs(metadata_dir)
+        os.makedirs(data_dir)
+        os.makedirs(log_dir)
+        #Generate filenames for new files.
+        inputxml = "%s/%s_source_mediainfo.xml" % (
+            metadata_dir, os.path.basename(filename)
+            )
+        inputtracexml = "%s/%s_source_mediatrace.xml" % (
+            metadata_dir, os.path.basename(filename)
+            )
+        output = "%s/%s.mkv" % (
+            data_dir, os.path.splitext(os.path.basename(filename))[0]
+            )
+        # Generate filename of ffv1.mkv without the path.
+        outputfilename = os.path.basename(output)
+        outputxml = "%s/%s_mediainfo.xml" % (metadata_dir, outputfilename)
+        outputtracexml = "%s/%s_mediatrace.xml" % (metadata_dir, outputfilename)
+        fmd5 = "%s/%s_source.framemd5" % (
+            metadata_dir, os.path.basename(filename)
+            )
+        fmd5ffv1 = "%s/%s_ffv1.framemd5" % (metadata_dir, outputfilename)
+        log = "%s/%s_log.log" %  (log_dir, filename)
+        generate_log(log, 'Input = %s' % filename)
+        generate_log(log, 'Output = %s' % output)
+        generate_log(
+            log, 'makeffv1.py transcode to FFV1 and framemd5 generation of source started.'
+            )
+        ffv1_logfile = log_dir + '/%s_ffv1_transcode.log' % filename
+        ffv1_env_dict = set_environment(ffv1_logfile)
+        par = subprocess.check_output(
+            [
+                'mediainfo', '--Language=raw', '--Full',
+                "--Inform=Video;%PixelAspectRatio%", filename
+            ]
+            ).rstrip()
+        field_order = subprocess.check_output(
+            [
+                'mediainfo', '--Language=raw',
+                '--Full', "--Inform=Video;%ScanType%", filename
+            ]
+            ).rstrip()
+        height = subprocess.check_output(
+            [
+                'mediainfo', '--Language=raw',
+                '--Full', "--Inform=Video;%Height%",
+                filename
+            ]
+            ).rstrip()
+        # Transcode video file writing frame md5 and output appropriately
+        ffv1_command = [
+            'ffmpeg',
+            '-i', filename,
+            '-c:v', 'ffv1',        # Use FFv1 codec
+            '-g', '1',              # Use intra-frame only aka ALL-I aka GOP=1
+            '-level', '3',          # Use Version 3 of FFv1
+            '-c:a', 'copy',         # Copy and paste audio bitsream with no transcoding
+            '-map', '0',
+            '-dn',
+            '-report',
+            '-slicecrc', '1',
+            '-slices', '16',
+            ]
+        # check for FCP7 lack of description and PAL
+        if par == '1.000':
+            if field_order == '':
+                if height == '576':
+                    ffv1_command += [
+                        '-vf',
+                        'setfield=tff, setdar=4/3'
+                        ]
+        ffv1_command += [
+            output,
+            '-f', 'framemd5', '-an',  # Create decoded md5 checksums for every frame of the input. -an ignores audio
+            fmd5
+            ]
+        print ffv1_command
+        subprocess.call(ffv1_command, env=ffv1_env_dict)
+        generate_log(
+            log, 'makeffv1.py transcode to FFV1 and framemd5 generation completed.'
+            )
+        generate_log(
+            log, 'makeffv1.py Framemd5 generation of output file started.'
+            )
+        fmd5_logfile = log_dir + '/%s_framemd5.log' % outputfilename
+        fmd5_env_dict = set_environment(fmd5_logfile)
+        pix_fmt = get_ffmpeg_fmt(filename, 'video')
+        fmd5_command = [
+            'ffmpeg',    # Create decoded md5 checksums for every frame
+            '-i', output,
+            '-report',
+            '-pix_fmt', pix_fmt,
+            '-f', 'framemd5', '-an',
+            fmd5ffv1
+            ]
+        print fmd5_command
+        subprocess.call(fmd5_command, env=fmd5_env_dict)
+        generate_log(
+            log,
+            'makeffv1.py Framemd5 generation of output file completed'
+            )
+        source_video_size = get_mediainfo(
+            'source_video_size', "--inform=General;%FileSize%", filename
+            )
+        ffv1_video_size = get_mediainfo(
+            'ffv1_video_size', '--inform=General;%FileSize%', output
+            )
+        compression_ratio = float(source_video_size) / float(ffv1_video_size)
+        if os.path.basename(sys.argv[0]) == 'makeffv1.py':
+            try:
+                shutil.copy(sys.argv[0], log_dir)
+            except IOError:
+                pass
+        print 'Generating mediainfo xml of input file and saving it in %s' % inputxml
+        make_mediainfo(inputxml, 'mediaxmlinput', filename)
+        print 'Generating mediainfo xml of output file and saving it in %s' % outputxml
+        make_mediainfo(outputxml, 'mediaxmloutput', output)
+        print 'Generating mediatrace xml of input file and saving it in %s' % inputtracexml
+        make_mediatrace(inputtracexml, 'mediatracexmlinput', filename)
+        print 'Generating mediatrace xml of output file and saving it in %s' % outputtracexml
+        make_mediatrace(outputtracexml, 'mediatracexmloutput', output)
+        source_parent_dir = os.path.dirname(os.path.abspath(filename))
+        manifest = '%s/%s_manifest.md5' % (source_parent_dir, filenoext)
+        generate_log(log, 'makeffv1.py MD5 manifest started')
+        checksum_mismatches = []
+        with open(fmd5) as f1:
+            with open(fmd5ffv1) as f2:
+                for (lineno1, line1), (lineno2, line2) in itertools.izip(
+                        read_non_comment_lines(f1),
+                        read_non_comment_lines(f2)
+                        ):
+                    if line1 != line2:
+                        if 'sar' in line1:
+                            checksum_mismatches = ['sar']
+                        else:
+                            checksum_mismatches.append(1)
+        if len(checksum_mismatches) == 0:
+            print 'LOSSLESS'
+            append_csv(
+                csv_report_filename, (
+                    output,
+                    'LOSSLESS', source_video_size,
+                    ffv1_video_size, compression_ratio
+                    )
+                )
+            generate_log(log, 'makeffv1.py Transcode was lossless')
+        elif len(checksum_mismatches) == 1:
+            if checksum_mismatches[0] == 'sar':
+                print 'Image content is lossless,'
+                ' Pixel Aspect Ratio has been altered.'
+                ' Update ffmpeg in order to resolve the PAR issue.'
+                append_csv(
+                    csv_report_filename,
+                    (
+                        output,
+                        'LOSSLESS - different PAR',
+                        source_video_size, ffv1_video_size, compression_ratio
+                        )
+                    )
+                generate_log(
+                    log,
+                    'makeffv1.py Image content is lossless but Pixel Aspect Ratio has been altered.Update ffmpeg in order to resolve the PAR issue.'
+                    )
+        elif len(checksum_mismatches) > 1:
+            print 'NOT LOSSLESS'
+            append_csv(
+                csv_report_filename,
+                (
+                    output, 'NOT LOSSLESS',
+                    source_video_size, ffv1_video_size, compression_ratio
+                    )
+                )
+            generate_log(log, 'makeffv1.py Not Lossless.')
+        hashlib_manifest(filenoext, manifest, source_parent_dir)
+        if filecmp.cmp(fmd5, fmd5ffv1, shallow=False):
+            print "YOUR FILES ARE LOSSLESS YOU SHOULD BE SO HAPPY!!!"
+        else:
+            print "The framemd5 text files are not completely identical."
+            " This may be because of a lossy transcode,"
+            " or a change in metadata, most likely pixel aspect ratio."
+            " Please analyse the framemd5 files for source and output."
+
+def main():
+    video_files, csv_report_filename = get_input()
+    make_ffv1(video_files, csv_report_filename)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/makepbcore.py` & `ifiscripts-2023.7.3.2/scripts/makepbcore.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/manifest.py` & `ifiscripts-2023.7.3.2/scripts/manifest.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/env python3
-'''
-Generates sidecar MD5 or SHA512 checksum manifest.
-'''
-import sys
-import os
-import argparse
-import time
-import shutil
-import ififuncs
-from ififuncs import generate_log
-from ififuncs import manifest_file_count
-from ififuncs import hashlib_manifest
-from ififuncs import make_desktop_logs_dir, make_desktop_manifest_dir
-
-
-def remove_bad_files(root_dir, log_name_source):
-    '''
-    Removes unwanted files.
-    Verify if this is different than the same function in ififuncs.
-    '''
-    rm_these = ['.DS_Store', 'Thumbs.db', 'desktop.ini']
-    for root, _, files in os.walk(root_dir):
-        for name in files:
-            path = os.path.join(root, name)
-            for i in rm_these:
-                if name == i:
-                    print(('***********************' + 'removing: ' + path))
-                    generate_log(
-                        log_name_source,
-                        'EVENT = Unwanted file removal - %s was removed' % path
-                    )
-                    try:
-                        os.remove(path)
-                    except OSError:
-                        print('can\'t delete as source is read-only')
-def main(args_):
-    '''
-    Overly long main function that makes a sidecar manifest.
-    This needs to get broken up into smaller functions.
-    '''
-    parser = argparse.ArgumentParser(description='Generate manifest with'
-                                     ' checksums for a directory'
-                                     ' Written by Kieran O\'Leary.')
-    parser.add_argument(
-        'source',
-        help='Input directory'
-    )
-    parser.add_argument(
-        '-s', '-sidecar',
-        action='store_true',
-        help='Generates Sidecar'
-    )
-    parser.add_argument(
-        '-f', '-felix',
-        action='store_true',
-        help='Felix Meehan workflow - places manifest inside of source directory'
-    )
-    parser.add_argument(
-        '-sha512',
-        action='store_true',
-        help='Generates sha512 checksums instead of md5'
-    )
-    args = parser.parse_args(args_)
-    source = args.source
-    source_parent_dir = os.path.dirname(source)
-    normpath = os.path.normpath(source)
-    relative_path = normpath.split(os.sep)[-1]
-    log_name_source_ = os.path.basename(
-        args.source
-    )  + time.strftime("_%Y_%m_%dT%H_%M_%S")
-    if args.s:
-        if args.sha512:
-            manifest = source_parent_dir + '/%s_manifest-sha512.txt' % relative_path
-        else:
-            manifest = source_parent_dir + '/%s_manifest.md5' % relative_path
-        log_name_source = source_parent_dir + '/%s.log' % log_name_source_
-    elif args.f:
-        if args.sha512:
-            manifest = source_parent_dir + '/%s_manifest-sha512.txt' % relative_path
-        else:
-            manifest = source + '/%s_manifest.md5' % relative_path
-        log_name_source = source_parent_dir + '/%s.log' % log_name_source_
-    else:
-        if args.sha512:
-            manifest_ = manifest_ = '/%s_manifest-sha512.txt' % relative_path
-        else:
-            manifest_ = '/%s_manifest.md5' % relative_path
-        desktop_manifest_dir = make_desktop_manifest_dir()
-        manifest = "%s/%s" % (desktop_manifest_dir, manifest_)
-        desktop_logs_dir = make_desktop_logs_dir()
-        log_name_source = "%s/%s.log" % (desktop_logs_dir, log_name_source_)
-    if args.sha512:
-        module = 'hashlib.sha512'
-    else:
-        module = 'hashlib.md5'
-    generate_log(log_name_source, 'manifest.py started.')
-    if sys.platform == "win32":
-            generate_log(
-                log_name_source,
-                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=Windows' % module
-            )
-    if sys.platform == "darwin":
-            generate_log(
-                log_name_source,
-                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=OSX' % module
-            )
-    elif sys.platform == "linux2":
-        generate_log(
-                log_name_source,
-                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=Linux' % module
-            )
-    ififuncs.generate_log(
-        log_name_source,
-        'eventDetail=manifest.py %s' % ififuncs.get_script_version('manifest.py'))
-    generate_log(log_name_source, 'Source: %s' % source)
-    if os.path.isfile(source):
-        print('\nFile checksum is not currently supported, only directories.\n')
-        generate_log(log_name_source, 'Error: Attempted to generate manifest for file. Only Directories/Folders are currently supported')
-        generate_log(log_name_source, 'manifest.py exit')
-        sys.exit()
-    elif not os.path.isdir(source):
-        print((' %s is either not a directory or it does not exist' % source))
-        generate_log(log_name_source, ' %s is either not a directory or it does not exist' % source)
-        generate_log(log_name_source, 'manifest.py exit')
-        sys.exit()
-    remove_bad_files(source, log_name_source)
-    source_count = 0
-    for _, _, filenames in os.walk(source):
-        # There has to be a better way to count the files..
-        for _ in filenames:
-            source_count += 1 #works in windows at least
-    if os.path.isfile(manifest):
-        count_in_manifest = manifest_file_count(manifest)
-        if source_count != count_in_manifest:
-            print('This manifest may be outdated as the number of files in your directory does not match the number of files in the manifest')
-            generate_log(log_name_source, 'EVENT = Existing source manifest check - Failure - The number of files in the source directory is not equal to the number of files in the source manifest ')
-            sys.exit()
-    if not os.path.isfile(manifest):
-        try:
-            print('Generating source manifest')
-            generate_log(log_name_source, 'EVENT = Generating source manifest')
-            if args.f:
-                if args.sha512:
-                    ififuncs.sha512_manifest(source, manifest, source)
-                else:
-                    hashlib_manifest(source, manifest, source)
-                shutil.move(log_name_source, source)
-            else:
-                if args.sha512:
-                    ififuncs.sha512_manifest(source, manifest, source_parent_dir)
-                else:
-                    hashlib_manifest(source, manifest, source_parent_dir)
-        except OSError:
-            print('You do not have access to this directory. Perhaps it is read only, or the wrong file system\n')
-            sys.exit()
-    else:
-        generate_log(log_name_source, 'EVENT = Existing source manifest check - Source manifest already exists. Script will exit. ')
-    print(('Manifest created in %s' % manifest))
-    generate_log(log_name_source, 'Manifest created in %s' % manifest)
-    return log_name_source
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Generates sidecar MD5 or SHA512 checksum manifest.
+'''
+import sys
+import os
+import argparse
+import time
+import shutil
+import ififuncs
+from ififuncs import generate_log
+from ififuncs import manifest_file_count
+from ififuncs import hashlib_manifest
+from ififuncs import make_desktop_logs_dir, make_desktop_manifest_dir
+
+
+def remove_bad_files(root_dir, log_name_source):
+    '''
+    Removes unwanted files.
+    Verify if this is different than the same function in ififuncs.
+    '''
+    rm_these = ['.DS_Store', 'Thumbs.db', 'desktop.ini']
+    for root, _, files in os.walk(root_dir):
+        for name in files:
+            path = os.path.join(root, name)
+            for i in rm_these:
+                if name == i:
+                    print(('***********************' + 'removing: ' + path))
+                    generate_log(
+                        log_name_source,
+                        'EVENT = Unwanted file removal - %s was removed' % path
+                    )
+                    try:
+                        os.remove(path)
+                    except OSError:
+                        print('can\'t delete as source is read-only')
+def main(args_):
+    '''
+    Overly long main function that makes a sidecar manifest.
+    This needs to get broken up into smaller functions.
+    '''
+    parser = argparse.ArgumentParser(description='Generate manifest with'
+                                     ' checksums for a directory'
+                                     ' Written by Kieran O\'Leary.')
+    parser.add_argument(
+        'source',
+        help='Input directory'
+    )
+    parser.add_argument(
+        '-s', '-sidecar',
+        action='store_true',
+        help='Generates Sidecar'
+    )
+    parser.add_argument(
+        '-f', '-felix',
+        action='store_true',
+        help='Felix Meehan workflow - places manifest inside of source directory'
+    )
+    parser.add_argument(
+        '-sha512',
+        action='store_true',
+        help='Generates sha512 checksums instead of md5'
+    )
+    args = parser.parse_args(args_)
+    source = args.source
+    source_parent_dir = os.path.dirname(source)
+    normpath = os.path.normpath(source)
+    relative_path = normpath.split(os.sep)[-1]
+    log_name_source_ = os.path.basename(
+        args.source
+    )  + time.strftime("_%Y_%m_%dT%H_%M_%S")
+    if args.s:
+        if args.sha512:
+            manifest = source_parent_dir + '/%s_manifest-sha512.txt' % relative_path
+        else:
+            manifest = source_parent_dir + '/%s_manifest.md5' % relative_path
+        log_name_source = source_parent_dir + '/%s.log' % log_name_source_
+    elif args.f:
+        if args.sha512:
+            manifest = source_parent_dir + '/%s_manifest-sha512.txt' % relative_path
+        else:
+            manifest = source + '/%s_manifest.md5' % relative_path
+        log_name_source = source_parent_dir + '/%s.log' % log_name_source_
+    else:
+        if args.sha512:
+            manifest_ = manifest_ = '/%s_manifest-sha512.txt' % relative_path
+        else:
+            manifest_ = '/%s_manifest.md5' % relative_path
+        desktop_manifest_dir = make_desktop_manifest_dir()
+        manifest = "%s/%s" % (desktop_manifest_dir, manifest_)
+        desktop_logs_dir = make_desktop_logs_dir()
+        log_name_source = "%s/%s.log" % (desktop_logs_dir, log_name_source_)
+    if args.sha512:
+        module = 'hashlib.sha512'
+    else:
+        module = 'hashlib.md5'
+    generate_log(log_name_source, 'manifest.py started.')
+    if sys.platform == "win32":
+            generate_log(
+                log_name_source,
+                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=Windows' % module
+            )
+    if sys.platform == "darwin":
+            generate_log(
+                log_name_source,
+                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=OSX' % module
+            )
+    elif sys.platform == "linux2":
+        generate_log(
+                log_name_source,
+                'EVENT = Generating manifest: status=started, eventType=message digest calculation, module=%s, agent=Linux' % module
+            )
+    ififuncs.generate_log(
+        log_name_source,
+        'eventDetail=manifest.py %s' % ififuncs.get_script_version('manifest.py'))
+    generate_log(log_name_source, 'Source: %s' % source)
+    if os.path.isfile(source):
+        print('\nFile checksum is not currently supported, only directories.\n')
+        generate_log(log_name_source, 'Error: Attempted to generate manifest for file. Only Directories/Folders are currently supported')
+        generate_log(log_name_source, 'manifest.py exit')
+        sys.exit()
+    elif not os.path.isdir(source):
+        print((' %s is either not a directory or it does not exist' % source))
+        generate_log(log_name_source, ' %s is either not a directory or it does not exist' % source)
+        generate_log(log_name_source, 'manifest.py exit')
+        sys.exit()
+    remove_bad_files(source, log_name_source)
+    source_count = 0
+    for _, _, filenames in os.walk(source):
+        # There has to be a better way to count the files..
+        for _ in filenames:
+            source_count += 1 #works in windows at least
+    if os.path.isfile(manifest):
+        count_in_manifest = manifest_file_count(manifest)
+        if source_count != count_in_manifest:
+            print('This manifest may be outdated as the number of files in your directory does not match the number of files in the manifest')
+            generate_log(log_name_source, 'EVENT = Existing source manifest check - Failure - The number of files in the source directory is not equal to the number of files in the source manifest ')
+            sys.exit()
+    if not os.path.isfile(manifest):
+        try:
+            print('Generating source manifest')
+            generate_log(log_name_source, 'EVENT = Generating source manifest')
+            if args.f:
+                if args.sha512:
+                    ififuncs.sha512_manifest(source, manifest, source)
+                else:
+                    hashlib_manifest(source, manifest, source)
+                shutil.move(log_name_source, source)
+            else:
+                if args.sha512:
+                    ififuncs.sha512_manifest(source, manifest, source_parent_dir)
+                else:
+                    hashlib_manifest(source, manifest, source_parent_dir)
+        except OSError:
+            print('You do not have access to this directory. Perhaps it is read only, or the wrong file system\n')
+            sys.exit()
+    else:
+        generate_log(log_name_source, 'EVENT = Existing source manifest check - Source manifest already exists. Script will exit. ')
+    print(('Manifest created in %s' % manifest))
+    generate_log(log_name_source, 'Manifest created in %s' % manifest)
+    return log_name_source
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/masscopy.py` & `ifiscripts-2023.7.3.2/scripts/masscopy.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-#!/usr/bin/env python3
-'''
-Launches copyit.py for subfolders that have md5 anifests.
-'''
-import os
-import argparse
-import time
-import copyit
-from ififuncs import make_desktop_logs_dir
-
-
-def analyze_log(logfile):
-    '''
-    Analyzes logfiles on the desktop and summarises the outcome.
-    '''
-    outcome = ''
-    with open(logfile, 'r', encoding='utf-8') as fo:
-        log_lines = fo.readlines()
-        for line in log_lines:
-            if 'EVENT = File Transfer Judgement - Success' in line:
-                outcome = 'success'
-            if 'EVENT = File Transfer Outcome - Failure' in line:
-                outcome = 'failure'
-            if 'EVENT = Existing source manifest check - Failure' in line:
-                outcome = 'failure - might be outdated manifests in use'
-        return outcome
-
-def parse_args():
-    '''
-    Accepts command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Performs moveit.py in a batch'
-        ' Written by Kieran O\'Leary.')
-    parser.add_argument(
-        'input',
-        help='full path of input directory'
-    )
-    parser.add_argument(
-        '-o',
-        help='full path of output directory',
-        required=True)
-    parser.add_argument(
-        '-l', '-lto',
-        action='store_true',
-        help='use gcp instead of rsync on osx for SPEED on LTO')
-    parser.add_argument(
-        '-y',
-        action='store_true',
-        help='Answers YES to the question: Not enough free space, would you like to continue?'
-    )
-    args = parser.parse_args()
-    return args
-
-
-def find_manifest(args):
-    '''
-    This function tries to find a manifest.
-    It looks one folder beneath the input folder for a checksum manifest
-    with a folder that has a matching name.
-    '''
-    # Creates an empty list called dirlist.
-    dirlist = []
-    # Creates a list of items in your input called directory_contents.
-    directory_contents = sorted(os.listdir(args.input))
-    # lists all contents of your input and analyzes each one in a `for loop`.
-    for item in directory_contents:
-        full_path = os.path.join(args.input, item)
-        manifest = os.path.join(
-            args.input, item
-        ) + '_manifest.md5'
-        # checks if the manifest exists
-        if os.path.isfile(manifest):
-            #if the manifest exists, add to dirlist
-            dirlist.append(full_path)
-        # checks if each item is a directory.
-        if os.path.isdir(full_path):
-            directories = os.listdir(full_path)
-            for subdirectories in directories:
-                full_subdirectory_path = os.path.join(
-                    full_path, subdirectories
-                )
-                if os.path.isdir(full_subdirectory_path):
-                    manifest = os.path.join(
-                        os.path.dirname(
-                            full_subdirectory_path
-                        ), subdirectories + '_manifest.md5'
-                        )
-                    if os.path.isfile(manifest):
-                        dirlist.append(os.path.dirname(full_subdirectory_path))
-    return dirlist # the dirlist is sent back out to the rest of the script.
-
-
-def analyze_reports(log_names, desktop_logs_dir):
-    '''
-    Tries to locate copyit.py logs on the desktop and analyzes them.
-    '''
-    print(' - SUMMARY REPORT')
-    for i in log_names:
-        if os.path.isfile(i):
-            print(" - %-*s   : %s" % (50, os.path.basename(i)[:-24], analyze_log(i)))
-        else:
-            print(' - %s can\'t find log file, trying again...' % i)
-            for logs in os.listdir(desktop_logs_dir):
-                # look at log filename minus the seconds and '.log'
-                if os.path.basename(i)[:-7] in logs:
-                    # make sure that the alternate log filename is more recent
-                    if int(
-                            os.path.basename(logs)[-12:-4].replace('_', '')) > int(os.path.basename(i)[-12:-4].replace('_', '')):
-                        print(' - trying to analyze %s' % logs)
-                        print(" - %-*s   : %s" % (50, os.path.basename(logs)[:-24], analyze_log(os.path.join(desktop_logs_dir, logs))))
-
-
-def main():
-    '''
-    Launches the other functions wihch attempt to run multiple copyit.py
-    instances if manifests and matching sidecar directories are found
-    inside of the input directory.
-    '''
-    args = parse_args()
-    all_files = find_manifest(args)
-    processed_dirs = []
-    log_names = []
-    print('\n\n - **** All of these folders will be copied to %s\n' % args.o)
-    for i in all_files:
-        absolute_path = os.path.join(args.o, os.path.basename(i))
-        if os.path.isdir(absolute_path):
-            print(' - %s already exists, skipping' % absolute_path)
-        else:
-            print(' - %s will be copied' % i)
-    time.sleep(2)
-    for i in all_files:
-        absolute_path = os.path.join(args.o, os.path.basename(i))
-        if os.path.isdir(absolute_path):
-            print(' - %s already exists, skipping' % absolute_path)
-        else:
-            desktop_logs_dir = make_desktop_logs_dir()
-            copyit_cmd = [os.path.join(args.input, i), args.o]
-            if args.l:
-                copyit_cmd.append('-l')
-            elif args.y:
-                copyit_cmd.append('-y')
-            log_name = copyit.main(copyit_cmd)
-            log_names.append(log_name)
-            processed_dirs.append(os.path.basename(os.path.join(args.input, i)))
-            print(' - ********\nWARNING - Please check the ifiscripts_logs directory on your Desktop to verify if ALL of your transfers were successful')
-            analyze_reports(log_names, desktop_logs_dir)
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+'''
+Launches copyit.py for subfolders that have md5 anifests.
+'''
+import os
+import argparse
+import time
+import copyit
+from ififuncs import make_desktop_logs_dir
+
+
+def analyze_log(logfile):
+    '''
+    Analyzes logfiles on the desktop and summarises the outcome.
+    '''
+    outcome = ''
+    with open(logfile, 'r', encoding='utf-8') as fo:
+        log_lines = fo.readlines()
+        for line in log_lines:
+            if 'EVENT = File Transfer Judgement - Success' in line:
+                outcome = 'success'
+            if 'EVENT = File Transfer Outcome - Failure' in line:
+                outcome = 'failure'
+            if 'EVENT = Existing source manifest check - Failure' in line:
+                outcome = 'failure - might be outdated manifests in use'
+        return outcome
+
+def parse_args():
+    '''
+    Accepts command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Performs moveit.py in a batch'
+        ' Written by Kieran O\'Leary.')
+    parser.add_argument(
+        'input',
+        help='full path of input directory'
+    )
+    parser.add_argument(
+        '-o',
+        help='full path of output directory',
+        required=True)
+    parser.add_argument(
+        '-l', '-lto',
+        action='store_true',
+        help='use gcp instead of rsync on osx for SPEED on LTO')
+    parser.add_argument(
+        '-y',
+        action='store_true',
+        help='Answers YES to the question: Not enough free space, would you like to continue?'
+    )
+    args = parser.parse_args()
+    return args
+
+
+def find_manifest(args):
+    '''
+    This function tries to find a manifest.
+    It looks one folder beneath the input folder for a checksum manifest
+    with a folder that has a matching name.
+    '''
+    # Creates an empty list called dirlist.
+    dirlist = []
+    # Creates a list of items in your input called directory_contents.
+    directory_contents = sorted(os.listdir(args.input))
+    # lists all contents of your input and analyzes each one in a `for loop`.
+    for item in directory_contents:
+        full_path = os.path.join(args.input, item)
+        manifest = os.path.join(
+            args.input, item
+        ) + '_manifest.md5'
+        # checks if the manifest exists
+        if os.path.isfile(manifest):
+            #if the manifest exists, add to dirlist
+            dirlist.append(full_path)
+        # checks if each item is a directory.
+        if os.path.isdir(full_path):
+            directories = os.listdir(full_path)
+            for subdirectories in directories:
+                full_subdirectory_path = os.path.join(
+                    full_path, subdirectories
+                )
+                if os.path.isdir(full_subdirectory_path):
+                    manifest = os.path.join(
+                        os.path.dirname(
+                            full_subdirectory_path
+                        ), subdirectories + '_manifest.md5'
+                        )
+                    if os.path.isfile(manifest):
+                        dirlist.append(os.path.dirname(full_subdirectory_path))
+    return dirlist # the dirlist is sent back out to the rest of the script.
+
+
+def analyze_reports(log_names, desktop_logs_dir):
+    '''
+    Tries to locate copyit.py logs on the desktop and analyzes them.
+    '''
+    print(' - SUMMARY REPORT')
+    for i in log_names:
+        if os.path.isfile(i):
+            print(" - %-*s   : %s" % (50, os.path.basename(i)[:-24], analyze_log(i)))
+        else:
+            print(' - %s can\'t find log file, trying again...' % i)
+            for logs in os.listdir(desktop_logs_dir):
+                # look at log filename minus the seconds and '.log'
+                if os.path.basename(i)[:-7] in logs:
+                    # make sure that the alternate log filename is more recent
+                    if int(
+                            os.path.basename(logs)[-12:-4].replace('_', '')) > int(os.path.basename(i)[-12:-4].replace('_', '')):
+                        print(' - trying to analyze %s' % logs)
+                        print(" - %-*s   : %s" % (50, os.path.basename(logs)[:-24], analyze_log(os.path.join(desktop_logs_dir, logs))))
+
+
+def main():
+    '''
+    Launches the other functions wihch attempt to run multiple copyit.py
+    instances if manifests and matching sidecar directories are found
+    inside of the input directory.
+    '''
+    args = parse_args()
+    all_files = find_manifest(args)
+    processed_dirs = []
+    log_names = []
+    print('\n\n - **** All of these folders will be copied to %s\n' % args.o)
+    for i in all_files:
+        absolute_path = os.path.join(args.o, os.path.basename(i))
+        if os.path.isdir(absolute_path):
+            print(' - %s already exists, skipping' % absolute_path)
+        else:
+            print(' - %s will be copied' % i)
+    time.sleep(2)
+    for i in all_files:
+        absolute_path = os.path.join(args.o, os.path.basename(i))
+        if os.path.isdir(absolute_path):
+            print(' - %s already exists, skipping' % absolute_path)
+        else:
+            desktop_logs_dir = make_desktop_logs_dir()
+            copyit_cmd = [os.path.join(args.input, i), args.o]
+            if args.l:
+                copyit_cmd.append('-l')
+            elif args.y:
+                copyit_cmd.append('-y')
+            log_name = copyit.main(copyit_cmd)
+            log_names.append(log_name)
+            processed_dirs.append(os.path.basename(os.path.join(args.input, i)))
+            print(' - ********\nWARNING - Please check the ifiscripts_logs directory on your Desktop to verify if ALL of your transfers were successful')
+            analyze_reports(log_names, desktop_logs_dir)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/massqc.py` & `ifiscripts-2023.7.3.2/scripts/massqc.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/mergepbcore.py` & `ifiscripts-2023.7.3.2/scripts/mergepbcore.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/multicopy.py` & `ifiscripts-2023.7.3.2/scripts/multicopy.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python3
-'''
-Launches multiple copyit jobs. This is different to masscopy.py,
-which takes a single directory as input and launches multiple copyit jobs.
-This script takes multiple inputs and copies them to the output directory.
-Make God have mercy on us all
-'''
-
-import argparse
-import copyit
-import masscopy
-import ififuncs
-
-def parse_args():
-    '''
-    Accepts command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Performs copyit.py in a batch'
-        'Launches multiple copyit jobs. This is different to masscopy.py,'
-        'which takes a single directory as input and launches multiple copyit jobs.'
-        'This script takes multiple inputs and copies them to the output directory.'
-        ' Written by Kieran O\'Leary.')
-    parser.add_argument(
-        '-i', nargs='+',
-        help='full path of input directory',
-        required=True
-    )
-    parser.add_argument(
-        '-o',
-        help='full path of output directory',
-        required=True)
-    parser.add_argument(
-        '-l', '-lto',
-        action='store_true',
-        help='use gcp instead of rsync on osx for SPEED on LTO')
-    parser.add_argument(
-        '-y',
-        action='store_true',
-        help='Answers YES to the question: Not enough free space, would you like to continue?'
-    )
-    args = parser.parse_args()
-    return args
-
-
-def main():
-    '''
-    Launches functions
-    '''
-    log_names = []
-    args = parse_args()
-    desktop_logs_dir = ififuncs.make_desktop_logs_dir()
-    for i in args.i:
-        copyit_cmd = [i, args.o]
-        if args.l:
-            copyit_cmd.append('-l')
-        elif args.y:
-            copyit_cmd.append('-y')
-        log_names.append(copyit.main(copyit_cmd))
-    print('********\nWARNING - Please check the ifiscripts_logs directory on your Desktop to verify if ALL of your transfers were successful')
-    masscopy.analyze_reports(log_names, desktop_logs_dir)
-
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+'''
+Launches multiple copyit jobs. This is different to masscopy.py,
+which takes a single directory as input and launches multiple copyit jobs.
+This script takes multiple inputs and copies them to the output directory.
+Make God have mercy on us all
+'''
+
+import argparse
+import copyit
+import masscopy
+import ififuncs
+
+def parse_args():
+    '''
+    Accepts command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Performs copyit.py in a batch'
+        'Launches multiple copyit jobs. This is different to masscopy.py,'
+        'which takes a single directory as input and launches multiple copyit jobs.'
+        'This script takes multiple inputs and copies them to the output directory.'
+        ' Written by Kieran O\'Leary.')
+    parser.add_argument(
+        '-i', nargs='+',
+        help='full path of input directory',
+        required=True
+    )
+    parser.add_argument(
+        '-o',
+        help='full path of output directory',
+        required=True)
+    parser.add_argument(
+        '-l', '-lto',
+        action='store_true',
+        help='use gcp instead of rsync on osx for SPEED on LTO')
+    parser.add_argument(
+        '-y',
+        action='store_true',
+        help='Answers YES to the question: Not enough free space, would you like to continue?'
+    )
+    args = parser.parse_args()
+    return args
+
+
+def main():
+    '''
+    Launches functions
+    '''
+    log_names = []
+    args = parse_args()
+    desktop_logs_dir = ififuncs.make_desktop_logs_dir()
+    for i in args.i:
+        copyit_cmd = [i, args.o]
+        if args.l:
+            copyit_cmd.append('-l')
+        elif args.y:
+            copyit_cmd.append('-y')
+        log_names.append(copyit.main(copyit_cmd))
+    print('********\nWARNING - Please check the ifiscripts_logs directory on your Desktop to verify if ALL of your transfers were successful')
+    masscopy.analyze_reports(log_names, desktop_logs_dir)
+
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/normalise.py` & `ifiscripts-2023.7.3.2/scripts/normalise.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-#!/usr/bin/env python3
-'''
-Performs normalisation to FFV1/Matroska.
-This performs a basic normalisation and does not enforce any folder structure.
-This supercedes makeffv1 within our workflows. This is mostly because makeffv1 imposes a specific, outdated
-folder structure, and it's best to let SIPCREATOR handle the folder structure and let normalise.py handle
-the actual normalisation.
-'''
-import sys
-import os
-import subprocess
-import argparse
-import shutil
-import time
-import ififuncs
-import sipcreator
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Performs normalisation to FFV1/Matroska.'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        '-i',
-        help='full path of input file or directory', required=True
-    )
-    parser.add_argument(
-        '-o', '-output',
-        help='full path of output directory', required=True
-    )
-    parser.add_argument(
-        '-sip',
-        help='Run sipcreator.py on the resulting file.', action='store_true'
-    )
-    parser.add_argument(
-        '-user',
-        help='Declare who you are. If this is not set, you will be prompted.')
-    parser.add_argument(
-        '-oe',
-        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
-    )
-    parser.add_argument(
-        '-supplement', nargs='+',
-        help='Enter the full path of files or folders that are to be added to the supplemental subfolder within the metadata folder. Use this for information that supplements your preservation objects but is not to be included in the objects folder.'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def normalise_process(filename, output_folder):
-    '''
-    Begins the actual normalisation process using FFmpeg
-    '''
-    output_uuid = ififuncs.create_uuid()
-    print(' - The following UUID has been generated: %s' % output_uuid)
-    output = "%s/%s.mkv" % (
-        output_folder, output_uuid
-        )
-    print(' - The normalised file will have this filename: %s' % output)
-    fmd5 = "%s/%s_source.framemd5" % (
-        output_folder, os.path.basename(filename)
-        )
-    print(' - Framemd5s for each frame of your input file will be stored in: %s' % fmd5)
-
-    ffv1_logfile = os.path.join(output_folder, '%s_normalise.log' % output_uuid)
-    print(' - The FFmpeg logfile for the transcode will be stored in: %s' % ffv1_logfile)
-    print(' - FFmpeg will begin normalisation now.')
-    ffv1_env_dict = ififuncs.set_environment(ffv1_logfile)
-    ffv1_command = [
-        'ffmpeg',
-        '-i', filename,
-        '-c:v', 'ffv1',         # Use FFv1 codec
-        '-g', '1',              # Use intra-frame only aka ALL-I aka GOP=1
-        '-level', '3',          # Use Version 3 of FFv1
-        '-c:a', 'copy',         # Copy and paste audio bitsream with no transcoding
-        '-map', '0',
-        '-dn',
-        '-report',
-        '-slicecrc', '1',
-        '-slices', '16',
-    ]
-    if ififuncs.check_for_fcp(filename) is True:
-        print(' - A 720/576 file with no Pixel Aspect Ratio and scan type metadata has been detected.')
-        ffv1_command += [
-            '-vf',
-            'setfield=tff, setdar=4/3'
-            ]
-        print(' - -vf setfield=tff, setdar=4/3 will be added to the FFmpeg command.')
-        ffprobe_dict = ififuncs.get_ffprobe_dict(filename)
-        # let's stipulate the colour metadata if not present for SD PAL material.
-        if not ififuncs.get_colour_metadata(ffprobe_dict):
-            ffv1_command += ['-color_primaries', 'bt470bg', '-color_trc', 'bt709', '-colorspace', 'bt470bg' ]
-    elif ififuncs.check_for_blackmagic(filename) is True:
-        print(' - A 720/576  with TFF scan type, clap atom featuring 702 width and a PAR of 1.093 has been detected.')
-        ffv1_command += ['-vf', 'setdar=4/3', '-color_primaries', 'bt470bg', '-color_trc', 'bt709', '-colorspace', 'bt470bg']
-    ffv1_command += [
-        output,
-        '-f', 'framemd5', '-an',  # Create decoded md5 checksums for every frame of the input. -an ignores audio
-        fmd5
-        ]
-    print(ffv1_command)
-    subprocess.call(ffv1_command, env=ffv1_env_dict)
-    return output, output_uuid, fmd5, ffv1_logfile
-
-def verify_losslessness(output_folder, output, output_uuid, fmd5):
-    '''
-    Verify the losslessness of the process using framemd5.
-    An additional metadata check should also occur.
-    '''
-    verdict = 'undeclared'
-    fmd5_logfile = os.path.join(output_folder, '%s_framemd5.log' % output_uuid)
-    fmd5ffv1 = "%s/%s.framemd5" % (output_folder, output_uuid)
-    print(' - Framemd5s for each frame of your output file will be stored in: %s' % fmd5ffv1)
-    fmd5_env_dict = ififuncs.set_environment(fmd5_logfile)
-    print(' - FFmpeg will attempt to verify the losslessness of the normalisation by using Framemd5s.')
-    fmd5_command = [
-        'ffmpeg',    # Create decoded md5 checksums for every frame
-        '-i', output,
-        '-report',
-        '-f', 'framemd5', '-an',
-        fmd5ffv1
-        ]
-    print(fmd5_command)
-    subprocess.call(fmd5_command, env=fmd5_env_dict)
-    checksum_mismatches = ififuncs.diff_framemd5s(fmd5, fmd5ffv1)
-    if len(checksum_mismatches) == 1:
-        if checksum_mismatches[0] == 'sar':
-            print('Image is lossless, but the Pixel Aspect Ratio is different than the source - this may have been intended.')
-            verdict = 'Image is lossless, but the Pixel Aspect Ratio is different than the source - this may have been intended.'
-        else:
-            print('not lossless')
-            verdict = 'not lossless'
-    elif len(checksum_mismatches) > 1:
-        print('not lossless')
-        verdict = 'not lossless'
-    elif len(checksum_mismatches) == 0:
-        print('YOUR FILES ARE LOSSLESS YOU SHOULD BE SO HAPPY!!!')
-        verdict = 'lossless'
-    return fmd5_logfile, fmd5ffv1, verdict
-
-def main(args_):
-    ififuncs.check_existence(['ffmpeg', 'mediainfo'])
-    print('\n - Normalise.py started')
-    args = parse_args(args_)
-    print(args)
-    source = args.i
-    output_folder = args.o
-    file_list = sorted(ififuncs.get_video_files(source))
-    if args.sip:
-        if args.user:
-            user = args.user
-        else:
-            user = ififuncs.get_user()
-        if args.oe:
-            if args.oe[:2] != 'oe':
-                print('First two characters must be \'oe\' and last four characters must be four digits')
-                object_entry = ififuncs.get_object_entry()
-            elif len(args.oe[2:]) not in range(4, 6):
-                print('First two characters must be \'oe\' and last four characters must be four digits')
-                object_entry = ififuncs.get_object_entry()
-            elif not args.oe[2:].isdigit():
-               object_entry = ififuncs.get_object_entry()
-               print('First two characters must be \'oe\' and last four characters must be four digits')
-            else:
-                object_entry = args.oe
-        else:
-            object_entry = ififuncs.get_object_entry()
-    if args.sip:
-        oe_digits = int(object_entry.replace('oe', ''))
-    for filename in file_list:
-        log_name_source = os.path.join(args.o, '%s_normalise_log.log' % time.strftime("_%Y_%m_%dT%H_%M_%S"))
-        ififuncs.generate_log(log_name_source, 'normalise.py started.')
-        ififuncs.generate_log(
-            log_name_source,
-            'Command line arguments: %s' % args
-        )
-        if args.sip:
-            ififuncs.generate_log(
-                log_name_source,
-                'EVENT = agentName=%s' % user
-            )
-        print('\n - Processing: %s' % filename)
-        ififuncs.generate_log(
-            log_name_source,
-            'EVENT = Normalization, status=started, eventType=Normalization, agentName=ffmpeg, eventDetail=Source object to be normalised=%s' % filename)
-        output, output_uuid, fmd5, ffv1_logfile = normalise_process(filename, output_folder)
-        ififuncs.generate_log(
-            log_name_source,
-            'EVENT = Normalization, status=finished, eventType=Normalization, agentName=ffmpeg, eventDetail=Source object normalised into=%s' % output)
-        inputxml, inputtracexml, dfxml = ififuncs.generate_mediainfo_xmls(filename, output_folder, output_uuid, log_name_source)
-        fmd5_logfile, fmd5ffv1, verdict = verify_losslessness(output_folder, output, output_uuid, fmd5)
-        ififuncs.generate_log(
-            log_name_source,
-            'EVENT = losslessness verification, status=finished, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation, eventOutcome=%s' % verdict)
-        if args.sip:
-            object_entry_complete = 'oe' + str(oe_digits)
-            supplement_cmd = ['-supplement', inputxml, inputtracexml, dfxml]
-            sipcreator_cmd = ['-i', output, '-move', '-u', output_uuid, '-user', user, '-oe', object_entry_complete, '-o', args.o]
-            if args.supplement:
-                supplement_cmd.extend(args.supplement)
-            sipcreator_cmd.extend(supplement_cmd)
-            sipcreator_log, sipcreator_manifest = sipcreator.main(sipcreator_cmd)
-            metadata_dir  = os.path.join(os.path.dirname(os.path.dirname(sipcreator_log)), 'metadata')
-            shutil.move(fmd5, metadata_dir)
-            shutil.move(fmd5_logfile, os.path.dirname(sipcreator_log))
-            shutil.move(fmd5ffv1, metadata_dir)
-            shutil.move(ffv1_logfile.replace('\\\\', '\\').replace('\:', ':'), os.path.dirname(sipcreator_log))
-            logs_dir = os.path.dirname(sipcreator_log)
-            ififuncs.manifest_update(sipcreator_manifest, os.path.join(metadata_dir, os.path.basename(fmd5)))
-            ififuncs.manifest_update(sipcreator_manifest, os.path.join(metadata_dir, os.path.basename(fmd5ffv1)))
-            ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(ffv1_logfile.replace('\\\\', '\\').replace('\:', ':'))))
-            ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(fmd5_logfile.replace('\\\\', '\\').replace('\:', ':'))))
-            ififuncs.merge_logs(log_name_source, sipcreator_log, sipcreator_manifest)
-            os.remove(dfxml)
-            os.remove(inputxml)
-            os.remove(inputtracexml)
-            print('The judgement above only refers to the copyit job, the losslessness judgement is: %s' % verdict)
-            oe_digits += 1
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Performs normalisation to FFV1/Matroska.
+This performs a basic normalisation and does not enforce any folder structure.
+This supercedes makeffv1 within our workflows. This is mostly because makeffv1 imposes a specific, outdated
+folder structure, and it's best to let SIPCREATOR handle the folder structure and let normalise.py handle
+the actual normalisation.
+'''
+import sys
+import os
+import subprocess
+import argparse
+import shutil
+import time
+import ififuncs
+import sipcreator
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Performs normalisation to FFV1/Matroska.'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        '-i',
+        help='full path of input file or directory', required=True
+    )
+    parser.add_argument(
+        '-o', '-output',
+        help='full path of output directory', required=True
+    )
+    parser.add_argument(
+        '-sip',
+        help='Run sipcreator.py on the resulting file.', action='store_true'
+    )
+    parser.add_argument(
+        '-user',
+        help='Declare who you are. If this is not set, you will be prompted.')
+    parser.add_argument(
+        '-oe',
+        help='Enter the Object Entry number for the representation.SIP will be placed in a folder with this name.'
+    )
+    parser.add_argument(
+        '-supplement', nargs='+',
+        help='Enter the full path of files or folders that are to be added to the supplemental subfolder within the metadata folder. Use this for information that supplements your preservation objects but is not to be included in the objects folder.'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def normalise_process(filename, output_folder):
+    '''
+    Begins the actual normalisation process using FFmpeg
+    '''
+    output_uuid = ififuncs.create_uuid()
+    print(' - The following UUID has been generated: %s' % output_uuid)
+    output = "%s/%s.mkv" % (
+        output_folder, output_uuid
+        )
+    print(' - The normalised file will have this filename: %s' % output)
+    fmd5 = "%s/%s_source.framemd5" % (
+        output_folder, os.path.basename(filename)
+        )
+    print(' - Framemd5s for each frame of your input file will be stored in: %s' % fmd5)
+
+    ffv1_logfile = os.path.join(output_folder, '%s_normalise.log' % output_uuid)
+    print(' - The FFmpeg logfile for the transcode will be stored in: %s' % ffv1_logfile)
+    print(' - FFmpeg will begin normalisation now.')
+    ffv1_env_dict = ififuncs.set_environment(ffv1_logfile)
+    ffv1_command = [
+        'ffmpeg',
+        '-i', filename,
+        '-c:v', 'ffv1',         # Use FFv1 codec
+        '-g', '1',              # Use intra-frame only aka ALL-I aka GOP=1
+        '-level', '3',          # Use Version 3 of FFv1
+        '-c:a', 'copy',         # Copy and paste audio bitsream with no transcoding
+        '-map', '0',
+        '-dn',
+        '-report',
+        '-slicecrc', '1',
+        '-slices', '16',
+    ]
+    if ififuncs.check_for_fcp(filename) is True:
+        print(' - A 720/576 file with no Pixel Aspect Ratio and scan type metadata has been detected.')
+        ffv1_command += [
+            '-vf',
+            'setfield=tff, setdar=4/3'
+            ]
+        print(' - -vf setfield=tff, setdar=4/3 will be added to the FFmpeg command.')
+        ffprobe_dict = ififuncs.get_ffprobe_dict(filename)
+        # let's stipulate the colour metadata if not present for SD PAL material.
+        if not ififuncs.get_colour_metadata(ffprobe_dict):
+            ffv1_command += ['-color_primaries', 'bt470bg', '-color_trc', 'bt709', '-colorspace', 'bt470bg' ]
+    elif ififuncs.check_for_blackmagic(filename) is True:
+        print(' - A 720/576  with TFF scan type, clap atom featuring 702 width and a PAR of 1.093 has been detected.')
+        ffv1_command += ['-vf', 'setdar=4/3', '-color_primaries', 'bt470bg', '-color_trc', 'bt709', '-colorspace', 'bt470bg']
+    ffv1_command += [
+        output,
+        '-f', 'framemd5', '-an',  # Create decoded md5 checksums for every frame of the input. -an ignores audio
+        fmd5
+        ]
+    print(ffv1_command)
+    subprocess.call(ffv1_command, env=ffv1_env_dict)
+    return output, output_uuid, fmd5, ffv1_logfile
+
+def verify_losslessness(output_folder, output, output_uuid, fmd5):
+    '''
+    Verify the losslessness of the process using framemd5.
+    An additional metadata check should also occur.
+    '''
+    verdict = 'undeclared'
+    fmd5_logfile = os.path.join(output_folder, '%s_framemd5.log' % output_uuid)
+    fmd5ffv1 = "%s/%s.framemd5" % (output_folder, output_uuid)
+    print(' - Framemd5s for each frame of your output file will be stored in: %s' % fmd5ffv1)
+    fmd5_env_dict = ififuncs.set_environment(fmd5_logfile)
+    print(' - FFmpeg will attempt to verify the losslessness of the normalisation by using Framemd5s.')
+    fmd5_command = [
+        'ffmpeg',    # Create decoded md5 checksums for every frame
+        '-i', output,
+        '-report',
+        '-f', 'framemd5', '-an',
+        fmd5ffv1
+        ]
+    print(fmd5_command)
+    subprocess.call(fmd5_command, env=fmd5_env_dict)
+    checksum_mismatches = ififuncs.diff_framemd5s(fmd5, fmd5ffv1)
+    if len(checksum_mismatches) == 1:
+        if checksum_mismatches[0] == 'sar':
+            print('Image is lossless, but the Pixel Aspect Ratio is different than the source - this may have been intended.')
+            verdict = 'Image is lossless, but the Pixel Aspect Ratio is different than the source - this may have been intended.'
+        else:
+            print('not lossless')
+            verdict = 'not lossless'
+    elif len(checksum_mismatches) > 1:
+        print('not lossless')
+        verdict = 'not lossless'
+    elif len(checksum_mismatches) == 0:
+        print('YOUR FILES ARE LOSSLESS YOU SHOULD BE SO HAPPY!!!')
+        verdict = 'lossless'
+    return fmd5_logfile, fmd5ffv1, verdict
+
+def main(args_):
+    ififuncs.check_existence(['ffmpeg', 'mediainfo'])
+    print('\n - Normalise.py started')
+    args = parse_args(args_)
+    print(args)
+    source = args.i
+    output_folder = args.o
+    file_list = sorted(ififuncs.get_video_files(source))
+    if args.sip:
+        if args.user:
+            user = args.user
+        else:
+            user = ififuncs.get_user()
+        if args.oe:
+            if args.oe[:2] != 'oe':
+                print('First two characters must be \'oe\' and last four characters must be four digits')
+                object_entry = ififuncs.get_object_entry()
+            elif len(args.oe[2:]) not in range(4, 6):
+                print('First two characters must be \'oe\' and last four characters must be four digits')
+                object_entry = ififuncs.get_object_entry()
+            elif not args.oe[2:].isdigit():
+               object_entry = ififuncs.get_object_entry()
+               print('First two characters must be \'oe\' and last four characters must be four digits')
+            else:
+                object_entry = args.oe
+        else:
+            object_entry = ififuncs.get_object_entry()
+    if args.sip:
+        oe_digits = int(object_entry.replace('oe', ''))
+    for filename in file_list:
+        log_name_source = os.path.join(args.o, '%s_normalise_log.log' % time.strftime("_%Y_%m_%dT%H_%M_%S"))
+        ififuncs.generate_log(log_name_source, 'normalise.py started.')
+        ififuncs.generate_log(
+            log_name_source,
+            'Command line arguments: %s' % args
+        )
+        if args.sip:
+            ififuncs.generate_log(
+                log_name_source,
+                'EVENT = agentName=%s' % user
+            )
+        print('\n - Processing: %s' % filename)
+        ififuncs.generate_log(
+            log_name_source,
+            'EVENT = Normalization, status=started, eventType=Normalization, agentName=ffmpeg, eventDetail=Source object to be normalised=%s' % filename)
+        output, output_uuid, fmd5, ffv1_logfile = normalise_process(filename, output_folder)
+        ififuncs.generate_log(
+            log_name_source,
+            'EVENT = Normalization, status=finished, eventType=Normalization, agentName=ffmpeg, eventDetail=Source object normalised into=%s' % output)
+        inputxml, inputtracexml, dfxml = ififuncs.generate_mediainfo_xmls(filename, output_folder, output_uuid, log_name_source)
+        fmd5_logfile, fmd5ffv1, verdict = verify_losslessness(output_folder, output, output_uuid, fmd5)
+        ififuncs.generate_log(
+            log_name_source,
+            'EVENT = losslessness verification, status=finished, eventType=messageDigestCalculation, agentName=ffmpeg, eventDetail=MD5s of AV streams of output file generated for validation, eventOutcome=%s' % verdict)
+        if args.sip:
+            object_entry_complete = 'oe' + str(oe_digits)
+            supplement_cmd = ['-supplement', inputxml, inputtracexml, dfxml]
+            sipcreator_cmd = ['-i', output, '-move', '-u', output_uuid, '-user', user, '-oe', object_entry_complete, '-o', args.o]
+            if args.supplement:
+                supplement_cmd.extend(args.supplement)
+            sipcreator_cmd.extend(supplement_cmd)
+            sipcreator_log, sipcreator_manifest = sipcreator.main(sipcreator_cmd)
+            metadata_dir  = os.path.join(os.path.dirname(os.path.dirname(sipcreator_log)), 'metadata')
+            shutil.move(fmd5, metadata_dir)
+            shutil.move(fmd5_logfile, os.path.dirname(sipcreator_log))
+            shutil.move(fmd5ffv1, metadata_dir)
+            shutil.move(ffv1_logfile.replace('\\\\', '\\').replace('\:', ':'), os.path.dirname(sipcreator_log))
+            logs_dir = os.path.dirname(sipcreator_log)
+            ififuncs.manifest_update(sipcreator_manifest, os.path.join(metadata_dir, os.path.basename(fmd5)))
+            ififuncs.manifest_update(sipcreator_manifest, os.path.join(metadata_dir, os.path.basename(fmd5ffv1)))
+            ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(ffv1_logfile.replace('\\\\', '\\').replace('\:', ':'))))
+            ififuncs.manifest_update(sipcreator_manifest, os.path.join(logs_dir, os.path.basename(fmd5_logfile.replace('\\\\', '\\').replace('\:', ':'))))
+            ififuncs.merge_logs(log_name_source, sipcreator_log, sipcreator_manifest)
+            os.remove(dfxml)
+            os.remove(inputxml)
+            os.remove(inputtracexml)
+            print('The judgement above only refers to the copyit job, the losslessness judgement is: %s' % verdict)
+            oe_digits += 1
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/order.py` & `ifiscripts-2023.7.3.2/scripts/order.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/package_update.py` & `ifiscripts-2023.7.3.2/scripts/package_update.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-#!/usr/bin/env python
-'''
-Moves files into subfolders, updates logfiles and manifests.
-'''
-import os
-import argparse
-import sys
-import datetime
-import shutil
-import ififuncs
-import copyit
-import sipcreator
-
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Moves files into subfolders, updates logfiles and manifests.'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        '-i', nargs='+',
-        help='full path of files to be moved', required=True
-    )
-    parser.add_argument(
-        '-new_folder',
-        help='full path of the new destination folder', required=True
-    )
-    parser.add_argument(
-        'input',
-        help='full path of \'sipcreator\' Object Entry package'
-    )
-    parser.add_argument(
-        '-user',
-        help='Declare who you are. If this is not set, you will be prompted.')
-    parser.add_argument(
-        '-copy', action='store_true',
-        help='Copies a file into a package instead of moving it. This should be used when adding files that originate outside of the package.')
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def update_manifest(manifest, old_path, new_path, new_log_textfile):
-    '''
-    Updates the path in a checksum manifest to reflect the new location.
-    '''
-    updated_lines = []
-    with open(manifest, 'r') as file_object:
-        checksums = file_object.readlines()
-        for line in checksums:
-            if old_path in line:
-                line = line.replace(old_path, new_path)
-                print(('the following path: %s has been updated with %s in the package manifest' % (old_path, new_path)))
-                ififuncs.generate_log(
-                    new_log_textfile,
-                    'EVENT = eventType=metadata modification,'
-                    ' agentName=package_update.py,'
-                    ' eventDetail=the following path: %s has been updated with %s in the package manifest' % (old_path, new_path)
-                )
-                updated_lines.append(line)
-            else:
-                updated_lines.append(line)
-    with open(manifest, 'w') as updated_manifest:
-        for updated_line in updated_lines:
-            updated_manifest.write(updated_line)
-
-
-def main(args_):
-    '''
-    Launch all the functions for creating an IFI SIP.
-    '''
-    args = parse_args(args_)
-    source = args.input
-    sip_path = ififuncs.check_for_sip([source])
-    if sip_path is not None:
-        oe_path = os.path.dirname(sip_path)
-        uuid = os.path.basename(sip_path)
-        sip_manifest = os.path.join(
-            oe_path, uuid
-            ) + '_manifest.md5'
-    else:
-        # this is assuming that the other workflow will be the 
-        # special collections workflow that has the uuid as the parent.
-        # some real checks should exist for this whole if/else flow.
-        sip_path = args.input
-        oe_path = os.path.dirname(args.input)
-        uuid = os.path.basename(sip_path)
-        sip_manifest = os.path.join(
-            oe_path, uuid + '_manifest.md5'
-            )
-    start = datetime.datetime.now()
-    print(args)
-    if args.user:
-        user = args.user
-    else:
-        user = ififuncs.get_user()
-    new_log_textfile = os.path.join(sip_path, 'logs' + '/' + uuid + '_sip_log.log')
-    ififuncs.generate_log(
-        new_log_textfile,
-        'EVENT = package_update.py started'
-    )
-    ififuncs.generate_log(
-        new_log_textfile,
-        'eventDetail=package_update.py %s' % ififuncs.get_script_version('package_update.py')
-    )
-    ififuncs.generate_log(
-        new_log_textfile,
-        'Command line arguments: %s' % args
-    )
-    ififuncs.generate_log(
-        new_log_textfile,
-        'EVENT = agentName=%s' % user
-    )
-    if not os.path.isdir(args.new_folder):
-        os.makedirs(args.new_folder)
-    if isinstance(args.i[0], (list,)):
-        args.i = args.i[0]
-    for filenames in args.i:
-        if args.copy:
-            copyit.main([filenames, args.new_folder])
-            ififuncs.generate_log(
-                new_log_textfile,
-                'EVENT = eventType=file movement,'
-                ' eventOutcomeDetailNote=%s has been moved into %s'
-                ' agentName=copyit.py'
-                % (filenames, args.new_folder)
-            )
-            # this is hardcoded - pick this apart so that any folder can be added to.
-            # this must be fixed in normalise.py as well.
-            relative_new_path = args.new_folder.replace(sip_path, '')
-            print((relative_new_path, 'relative'))
-            if (relative_new_path[0] == '/') or relative_new_path[0] == '\\':
-                relative_new_path = relative_new_path[1:].replace('\\', '/')
-            sipcreator.consolidate_manifests(sip_path, relative_new_path, new_log_textfile)
-            log_manifest = os.path.join(os.path.dirname(new_log_textfile), os.path.basename(filenames) + '_manifest.md5')
-            ififuncs.manifest_update(sip_manifest, log_manifest)
-            ififuncs.sort_manifest(sip_manifest)
-        else:
-            # add test to see if it actually deleted - what if read only?
-            shutil.move(filenames, args.new_folder)
-            ififuncs.generate_log(
-                new_log_textfile,
-                'EVENT = eventType=file movement,'
-                ' eventOutcomeDetailNote=%s has been moved into %s'
-                ' agentName=shutil.move()'
-                % (filenames, args.new_folder)
-            )
-            print(('%s has been moved into %s' % (filenames, args.new_folder)))
-            relative_filename = filenames.replace(os.path.dirname(args.input) + '/', '').replace('\\', '/')
-            relative_filename = filenames.replace(os.path.dirname(args.input) + '\\', '').replace('\\', '/')
-            relative_new_folder = args.new_folder.replace(os.path.dirname(args.input) + '/', '').replace('\\', '/')
-            relative_new_folder = args.new_folder.replace(os.path.dirname(args.input) + '\\', '').replace('\\', '/')
-            update_manifest(
-                sip_manifest,
-                relative_filename,
-                os.path.join(relative_new_folder, os.path.basename(relative_filename)).replace('\\', '/'),
-                new_log_textfile
-            )
-    ififuncs.generate_log(
-        new_log_textfile,
-        'EVENT = package_update.py finished'
-    )
-    ififuncs.checksum_replace(sip_manifest, new_log_textfile, 'md5')
-    finish = datetime.datetime.now()
-    print('\n- %s ran this script at %s and it finished at %s' % (user, start, finish))
-
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python
+'''
+Moves files into subfolders, updates logfiles and manifests.
+'''
+import os
+import argparse
+import sys
+import datetime
+import shutil
+import ififuncs
+import copyit
+import sipcreator
+
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Moves files into subfolders, updates logfiles and manifests.'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        '-i', nargs='+',
+        help='full path of files to be moved', required=True
+    )
+    parser.add_argument(
+        '-new_folder',
+        help='full path of the new destination folder', required=True
+    )
+    parser.add_argument(
+        'input',
+        help='full path of \'sipcreator\' Object Entry package'
+    )
+    parser.add_argument(
+        '-user',
+        help='Declare who you are. If this is not set, you will be prompted.')
+    parser.add_argument(
+        '-copy', action='store_true',
+        help='Copies a file into a package instead of moving it. This should be used when adding files that originate outside of the package.')
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def update_manifest(manifest, old_path, new_path, new_log_textfile):
+    '''
+    Updates the path in a checksum manifest to reflect the new location.
+    '''
+    updated_lines = []
+    with open(manifest, 'r') as file_object:
+        checksums = file_object.readlines()
+        for line in checksums:
+            if old_path in line:
+                line = line.replace(old_path, new_path)
+                print(('the following path: %s has been updated with %s in the package manifest' % (old_path, new_path)))
+                ififuncs.generate_log(
+                    new_log_textfile,
+                    'EVENT = eventType=metadata modification,'
+                    ' agentName=package_update.py,'
+                    ' eventDetail=the following path: %s has been updated with %s in the package manifest' % (old_path, new_path)
+                )
+                updated_lines.append(line)
+            else:
+                updated_lines.append(line)
+    with open(manifest, 'w') as updated_manifest:
+        for updated_line in updated_lines:
+            updated_manifest.write(updated_line)
+
+
+def main(args_):
+    '''
+    Launch all the functions for creating an IFI SIP.
+    '''
+    args = parse_args(args_)
+    source = args.input
+    sip_path = ififuncs.check_for_sip([source])
+    if sip_path is not None:
+        oe_path = os.path.dirname(sip_path)
+        uuid = os.path.basename(sip_path)
+        sip_manifest = os.path.join(
+            oe_path, uuid
+            ) + '_manifest.md5'
+    else:
+        # this is assuming that the other workflow will be the 
+        # special collections workflow that has the uuid as the parent.
+        # some real checks should exist for this whole if/else flow.
+        sip_path = args.input
+        oe_path = os.path.dirname(args.input)
+        uuid = os.path.basename(sip_path)
+        sip_manifest = os.path.join(
+            oe_path, uuid + '_manifest.md5'
+            )
+    start = datetime.datetime.now()
+    print(args)
+    if args.user:
+        user = args.user
+    else:
+        user = ififuncs.get_user()
+    new_log_textfile = os.path.join(sip_path, 'logs' + '/' + uuid + '_sip_log.log')
+    ififuncs.generate_log(
+        new_log_textfile,
+        'EVENT = package_update.py started'
+    )
+    ififuncs.generate_log(
+        new_log_textfile,
+        'eventDetail=package_update.py %s' % ififuncs.get_script_version('package_update.py')
+    )
+    ififuncs.generate_log(
+        new_log_textfile,
+        'Command line arguments: %s' % args
+    )
+    ififuncs.generate_log(
+        new_log_textfile,
+        'EVENT = agentName=%s' % user
+    )
+    if not os.path.isdir(args.new_folder):
+        os.makedirs(args.new_folder)
+    if isinstance(args.i[0], (list,)):
+        args.i = args.i[0]
+    for filenames in args.i:
+        if args.copy:
+            copyit.main([filenames, args.new_folder])
+            ififuncs.generate_log(
+                new_log_textfile,
+                'EVENT = eventType=file movement,'
+                ' eventOutcomeDetailNote=%s has been moved into %s'
+                ' agentName=copyit.py'
+                % (filenames, args.new_folder)
+            )
+            # this is hardcoded - pick this apart so that any folder can be added to.
+            # this must be fixed in normalise.py as well.
+            relative_new_path = args.new_folder.replace(sip_path, '')
+            print((relative_new_path, 'relative'))
+            if (relative_new_path[0] == '/') or relative_new_path[0] == '\\':
+                relative_new_path = relative_new_path[1:].replace('\\', '/')
+            sipcreator.consolidate_manifests(sip_path, relative_new_path, new_log_textfile)
+            log_manifest = os.path.join(os.path.dirname(new_log_textfile), os.path.basename(filenames) + '_manifest.md5')
+            ififuncs.manifest_update(sip_manifest, log_manifest)
+            ififuncs.sort_manifest(sip_manifest)
+        else:
+            # add test to see if it actually deleted - what if read only?
+            shutil.move(filenames, args.new_folder)
+            ififuncs.generate_log(
+                new_log_textfile,
+                'EVENT = eventType=file movement,'
+                ' eventOutcomeDetailNote=%s has been moved into %s'
+                ' agentName=shutil.move()'
+                % (filenames, args.new_folder)
+            )
+            print(('%s has been moved into %s' % (filenames, args.new_folder)))
+            relative_filename = filenames.replace(os.path.dirname(args.input) + '/', '').replace('\\', '/')
+            relative_filename = filenames.replace(os.path.dirname(args.input) + '\\', '').replace('\\', '/')
+            relative_new_folder = args.new_folder.replace(os.path.dirname(args.input) + '/', '').replace('\\', '/')
+            relative_new_folder = args.new_folder.replace(os.path.dirname(args.input) + '\\', '').replace('\\', '/')
+            update_manifest(
+                sip_manifest,
+                relative_filename,
+                os.path.join(relative_new_folder, os.path.basename(relative_filename)).replace('\\', '/'),
+                new_log_textfile
+            )
+    ififuncs.generate_log(
+        new_log_textfile,
+        'EVENT = package_update.py finished'
+    )
+    ififuncs.checksum_replace(sip_manifest, new_log_textfile, 'md5')
+    finish = datetime.datetime.now()
+    print('\n- %s ran this script at %s and it finished at %s' % (user, start, finish))
+
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/packagecheck.py` & `ifiscripts-2023.7.3.2/scripts/packagecheck.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-#!/usr/bin/env python
-'''
-Checks packages for correct structure.
-Also returns a dictionary containing important varibles such as
-folder paths and identifiers.
-'''
-import os
-import argparse
-import sys
-import ififuncs
-
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Check packages for correct structure.'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        'input',
-        help='full path of package'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def analyse_package(sip_path):
-    '''
-    Return a dictionary full of folder and file path variables
-    '''
-    package_info = {}
-    package_info['sip_path'] = sip_path
-    uuid = os.path.basename(sip_path)
-    if ififuncs.validate_uuid4(uuid) is not False:
-        package_info['uuid'] = uuid
-        package_info['oe_path'] = os.path.dirname(sip_path)
-        package_info['parent_identifier'] = os.path.basename(package_info['oe_path']) # can be OE or aaa
-        package_info['manifest'] = os.path.join(package_info['oe_path'], uuid + '_manifest.md5')
-        package_info['logs_dir'] = os.path.join(sip_path, 'logs')
-        package_info['metadata_dir'] = os.path.join(sip_path, 'metadata')
-        package_info['objects_dir'] = os.path.join(sip_path, 'objects')
-        package_info['sip_log'] = os.path.join(package_info['logs_dir'], uuid + '_sip_log.log')
-        package_info['objects'] = os.listdir(package_info['objects_dir'])
-    else:
-        return False
-    return package_info
-
-def test_package(package_info):
-    '''
-    Test if key files or folders exist.
-    '''
-    error_list = []
-    question_list = []
-    folder_list = [
-        package_info['oe_path'],
-        package_info['logs_dir'],
-        package_info['objects_dir'],
-        package_info['metadata_dir'],
-        package_info['sip_path']
-    ]
-    file_list = [
-        package_info['manifest'],
-        package_info['sip_log']
-    ]
-    for folder in folder_list:
-        if not os.path.isdir(folder):
-            error_list.append(folder)
-    for filename in file_list:
-        if not os.path.isfile(filename):
-            error_list.append(filename)
-    metadata_files = os.listdir(package_info['metadata_dir'])
-    for metadata_file in metadata_files:
-        full_path = os.path.join(package_info['metadata_dir'], metadata_file)
-        if os.path.getsize(full_path) == 0:
-            question_list.append(full_path)
-    for object_files in package_info['objects']:
-        mediainfo = os.path.join(package_info['metadata_dir'], object_files + '_mediainfo.xml')
-        if not os.path.isfile(mediainfo):
-             question_list.append(mediainfo)
-        mediatrace= os.path.join(package_info['metadata_dir'], object_files + '_mediatrace.xml')
-        if not os.path.isfile(mediatrace):
-             question_list.append(mediatrace)
-    if not error_list:
-        print('Key files and folders all exist')
-    else:
-        for error in error_list:
-            print((('%s does not exist') % error))
-    if not question_list:
-        print('No further errors detected')
-    else:
-        for error in question_list:
-            print((('%s requires investigation') % error))
-    return error_list, question_list
-
-
-def main(args_):
-    '''
-    Launch all the functions for determining folder and file paths.
-    '''
-    args = parse_args(args_)
-    source = args.input
-    sip_path = ififuncs.check_for_sip([source])
-    if sip_path is not None:
-        package_info = analyse_package(sip_path)
-    if package_info is False:
-        print('Valid UUID not found in folder path')
-    else:
-        print(package_info)
-    error_list, question_list = test_package(package_info)
-    return package_info, error_list, question_list
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python
+'''
+Checks packages for correct structure.
+Also returns a dictionary containing important varibles such as
+folder paths and identifiers.
+'''
+import os
+import argparse
+import sys
+import ififuncs
+
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Check packages for correct structure.'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        'input',
+        help='full path of package'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def analyse_package(sip_path):
+    '''
+    Return a dictionary full of folder and file path variables
+    '''
+    package_info = {}
+    package_info['sip_path'] = sip_path
+    uuid = os.path.basename(sip_path)
+    if ififuncs.validate_uuid4(uuid) is not False:
+        package_info['uuid'] = uuid
+        package_info['oe_path'] = os.path.dirname(sip_path)
+        package_info['parent_identifier'] = os.path.basename(package_info['oe_path']) # can be OE or aaa
+        package_info['manifest'] = os.path.join(package_info['oe_path'], uuid + '_manifest.md5')
+        package_info['logs_dir'] = os.path.join(sip_path, 'logs')
+        package_info['metadata_dir'] = os.path.join(sip_path, 'metadata')
+        package_info['objects_dir'] = os.path.join(sip_path, 'objects')
+        package_info['sip_log'] = os.path.join(package_info['logs_dir'], uuid + '_sip_log.log')
+        package_info['objects'] = os.listdir(package_info['objects_dir'])
+    else:
+        return False
+    return package_info
+
+def test_package(package_info):
+    '''
+    Test if key files or folders exist.
+    '''
+    error_list = []
+    question_list = []
+    folder_list = [
+        package_info['oe_path'],
+        package_info['logs_dir'],
+        package_info['objects_dir'],
+        package_info['metadata_dir'],
+        package_info['sip_path']
+    ]
+    file_list = [
+        package_info['manifest'],
+        package_info['sip_log']
+    ]
+    for folder in folder_list:
+        if not os.path.isdir(folder):
+            error_list.append(folder)
+    for filename in file_list:
+        if not os.path.isfile(filename):
+            error_list.append(filename)
+    metadata_files = os.listdir(package_info['metadata_dir'])
+    for metadata_file in metadata_files:
+        full_path = os.path.join(package_info['metadata_dir'], metadata_file)
+        if os.path.getsize(full_path) == 0:
+            question_list.append(full_path)
+    for object_files in package_info['objects']:
+        mediainfo = os.path.join(package_info['metadata_dir'], object_files + '_mediainfo.xml')
+        if not os.path.isfile(mediainfo):
+             question_list.append(mediainfo)
+        mediatrace= os.path.join(package_info['metadata_dir'], object_files + '_mediatrace.xml')
+        if not os.path.isfile(mediatrace):
+             question_list.append(mediatrace)
+    if not error_list:
+        print('Key files and folders all exist')
+    else:
+        for error in error_list:
+            print((('%s does not exist') % error))
+    if not question_list:
+        print('No further errors detected')
+    else:
+        for error in question_list:
+            print((('%s requires investigation') % error))
+    return error_list, question_list
+
+
+def main(args_):
+    '''
+    Launch all the functions for determining folder and file paths.
+    '''
+    args = parse_args(args_)
+    source = args.input
+    sip_path = ififuncs.check_for_sip([source])
+    if sip_path is not None:
+        package_info = analyse_package(sip_path)
+    if package_info is False:
+        print('Valid UUID not found in folder path')
+    else:
+        print(package_info)
+    error_list, question_list = test_package(package_info)
+    return package_info, error_list, question_list
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/scripts/prores.py` & `ifiscripts-2023.7.3.2/scripts/prores.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/seq2ffv1.py` & `ifiscripts-2023.7.3.2/scripts/seq2ffv1.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/sipcreator.py` & `ifiscripts-2023.7.3.2/scripts/sipcreator.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/strongbox_fixity.py` & `ifiscripts-2023.7.3.2/scripts/strongbox_fixity.py`

 * *Files identical despite different names*

### Comparing `ifiscripts-2023.7.3.1/scripts/subfolders.py` & `ifiscripts-2023.7.3.2/scripts/subfolders.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python3
-'''
-Generates subfolders based on filenames within the input directory
-and if -move is used, moves the relevant files into these new directories.
-Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml
-This will result in directories called file1 and file2 being created, and
-file1.mkv and file1.xml will be moved into the file1 directory, with a similar action
-for file2
-'''
-import os
-import sys
-import shutil
-import argparse
-
-def parse_args():
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Generates subfolders based on filenames within the input directory'
-        'and if -move is used, moves the relevant files into these new directories.'
-        'Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml'
-        'This will result in directories called file1 and file2 being created, and'
-        'file1.mkv and file1.xml will be moved into the file1 directory, with a similar action'
-        'for file2'
-    )
-    parser.add_argument(
-        '-i',
-        help='full path of input directory', required=True
-    )
-    parser.add_argument(
-        '-move',
-        help='Moves files into the newly created subfolders', action='store_true'
-    )
-    parsed_args = parser.parse_args()
-    return parsed_args
-
-def main():
-    '''
-    Generates subfolders based on filenames within the input directory
-    and if -move is used, moves the relevant files into these new directories.
-    Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml
-    This will result in directories called file1 and file2 being created, and
-    file1.mkv and file1.xml will be moved into the file1 directory, with a similar action
-    for file2
-    '''
-    args = parse_args()
-    inputs = args.i
-    if not os.path.isdir(inputs):
-        print(' - Input must be a directory/folder - exiting!')
-        sys.exit()
-    for dirs in os.listdir(inputs):
-        if dirs[0] != '.':
-            full_path = os.path.join(inputs, dirs)
-            new_dir, _ = (os.path.splitext(full_path))
-            if not os.path.isdir(new_dir):
-                os.makedirs(new_dir)
-                if os.path.isdir(new_dir):
-                    print(' - The following directory has been created: %s' % new_dir)
-            else:
-                print(' - %s already exists' % new_dir)
-            if args.move:
-                if new_dir in full_path:
-                    if os.path.isfile(full_path):
-                        print(' - %s will be moved into %s' % (full_path, new_dir))
-                        shutil.move(full_path, new_dir)
-
-if __name__ == '__main__':
+#!/usr/bin/env python3
+'''
+Generates subfolders based on filenames within the input directory
+and if -move is used, moves the relevant files into these new directories.
+Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml
+This will result in directories called file1 and file2 being created, and
+file1.mkv and file1.xml will be moved into the file1 directory, with a similar action
+for file2
+'''
+import os
+import sys
+import shutil
+import argparse
+
+def parse_args():
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Generates subfolders based on filenames within the input directory'
+        'and if -move is used, moves the relevant files into these new directories.'
+        'Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml'
+        'This will result in directories called file1 and file2 being created, and'
+        'file1.mkv and file1.xml will be moved into the file1 directory, with a similar action'
+        'for file2'
+    )
+    parser.add_argument(
+        '-i',
+        help='full path of input directory', required=True
+    )
+    parser.add_argument(
+        '-move',
+        help='Moves files into the newly created subfolders', action='store_true'
+    )
+    parsed_args = parser.parse_args()
+    return parsed_args
+
+def main():
+    '''
+    Generates subfolders based on filenames within the input directory
+    and if -move is used, moves the relevant files into these new directories.
+    Eg. An input directory contains file1.mkv, file1.xml file2.mkv, file2.xml
+    This will result in directories called file1 and file2 being created, and
+    file1.mkv and file1.xml will be moved into the file1 directory, with a similar action
+    for file2
+    '''
+    args = parse_args()
+    inputs = args.i
+    if not os.path.isdir(inputs):
+        print(' - Input must be a directory/folder - exiting!')
+        sys.exit()
+    for dirs in os.listdir(inputs):
+        if dirs[0] != '.':
+            full_path = os.path.join(inputs, dirs)
+            new_dir, _ = (os.path.splitext(full_path))
+            if not os.path.isdir(new_dir):
+                os.makedirs(new_dir)
+                if os.path.isdir(new_dir):
+                    print(' - The following directory has been created: %s' % new_dir)
+            else:
+                print(' - %s already exists' % new_dir)
+            if args.move:
+                if new_dir in full_path:
+                    if os.path.isfile(full_path):
+                        print(' - %s will be moved into %s' % (full_path, new_dir))
+                        shutil.move(full_path, new_dir)
+
+if __name__ == '__main__':
     main()
```

### Comparing `ifiscripts-2023.7.3.1/scripts/testfiles.py` & `ifiscripts-2023.7.3.2/scripts/testfiles.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-#!/usr/bin/env python3
-'''
-Creates some test video files via ffmpeg.
-Usage: testfiles.py -o path/to/dir
-Run testfiles.py -h for help.
-Written by Kieran O'Leary.
-'''
-import subprocess
-import os
-import argparse
-import sys
-import ififuncs
-
-def parse_args(args_):
-    '''
-    Parse command line arguments.
-    '''
-    parser = argparse.ArgumentParser(
-        description='Creates some test video files via ffmpeg'
-        ' Written by Kieran O\'Leary.'
-    )
-    parser.add_argument(
-        '-o', '-output',
-        help='full path of output directory', required=True
-    )
-    parser.add_argument(
-        '-onlyvideo',
-        help='Only creates video, no image sequences', action='store_true'
-    )
-    parsed_args = parser.parse_args(args_)
-    return parsed_args
-
-
-def main(args_):
-    '''
-    Creates three v210/mov tesfiles in a test_files subdirectory
-    '''
-    ififuncs.check_existence(['ffmpeg'])
-    args = parse_args(args_)
-    output_dir = os.path.join(os.path.abspath(args.o), 'test_files')
-    ten_bit_dpx_dir = os.path.join(output_dir, 'ten_bit_dpx')
-    sixteen_bit_dpx_dir = os.path.join(output_dir, 'sixteen_bit_dpx')
-    multi_reel_dir = os.path.join(output_dir, 'multi_reel')
-    reel1 = os.path.join(multi_reel_dir, 'whatever_reel1')
-    reel2 = os.path.join(multi_reel_dir, 'whatever_reel2')
-    reel3 = os.path.join(multi_reel_dir, 'whatever_reel3')
-    bars_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc', '-n',
-        '-f', 'lavfi', '-i', 'sine', '-c:v', 'v210', '-ac', '2', '-c:a', 'pcm_s24le',
-        '-t', '20', os.path.join(output_dir, 'bars_v210_pcm24le_stereo_20sec.mov')
-        ]
-    mandel_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'mandelbrot', '-n',
-        '-c:v', 'v210', '-t', '5', os.path.join(output_dir, 'mandel_silent.mov')
-        ]
-
-    life_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc',
-        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(ten_bit_dpx_dir, 'ten_bit_%06d.dpx'),
-        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(ten_bit_dpx_dir, 'ten_bit.wav')
-        ]
-    reel1_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc',
-        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel1, 'ten_bit_reel1_%06d.dpx'),
-        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel1, 'ten_bit_reel1.wav')
-        ]
-    reel2_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc2',
-        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel2, 'ten_bit_reel2_%06d.dpx'),
-        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel2, 'ten_bit_reel2.wav')
-        ]
-    reel3_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'mandelbrot',
-        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel3, 'ten_bit_reel3_%06d.dpx'),
-        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel3, 'ten_bit_reel3.wav')
-        ]
-    dpx16_cmd = [
-        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc2',
-        '-pix_fmt', 'rgb48le', '-t', '20', os.path.join(sixteen_bit_dpx_dir, 'sixteen_bit_%06d.dpx')
-        ]
-    if not os.path.isdir(output_dir):
-        os.makedirs(output_dir)
-    subprocess.call(bars_cmd)
-    subprocess.call(mandel_cmd)
-    if not args.onlyvideo:
-        if not os.path.isdir(ten_bit_dpx_dir):
-            os.makedirs(ten_bit_dpx_dir)
-        if not os.path.isdir(sixteen_bit_dpx_dir):
-            os.makedirs(sixteen_bit_dpx_dir)
-        if not os.path.isdir(reel1):
-            os.makedirs(reel1)
-        if not os.path.isdir(reel2):
-            os.makedirs(reel2)
-        if not os.path.isdir(reel3):
-            os.makedirs(reel3)
-        subprocess.call(dpx16_cmd)
-        subprocess.call(reel1_cmd)
-        subprocess.call(reel2_cmd)
-        subprocess.call(reel3_cmd)
-        subprocess.call(life_cmd)
-
-if __name__ == '__main__':
-    main(sys.argv[1:])
+#!/usr/bin/env python3
+'''
+Creates some test video files via ffmpeg.
+Usage: testfiles.py -o path/to/dir
+Run testfiles.py -h for help.
+Written by Kieran O'Leary.
+'''
+import subprocess
+import os
+import argparse
+import sys
+import ififuncs
+
+def parse_args(args_):
+    '''
+    Parse command line arguments.
+    '''
+    parser = argparse.ArgumentParser(
+        description='Creates some test video files via ffmpeg'
+        ' Written by Kieran O\'Leary.'
+    )
+    parser.add_argument(
+        '-o', '-output',
+        help='full path of output directory', required=True
+    )
+    parser.add_argument(
+        '-onlyvideo',
+        help='Only creates video, no image sequences', action='store_true'
+    )
+    parsed_args = parser.parse_args(args_)
+    return parsed_args
+
+
+def main(args_):
+    '''
+    Creates three v210/mov tesfiles in a test_files subdirectory
+    '''
+    ififuncs.check_existence(['ffmpeg'])
+    args = parse_args(args_)
+    output_dir = os.path.join(os.path.abspath(args.o), 'test_files')
+    ten_bit_dpx_dir = os.path.join(output_dir, 'ten_bit_dpx')
+    sixteen_bit_dpx_dir = os.path.join(output_dir, 'sixteen_bit_dpx')
+    multi_reel_dir = os.path.join(output_dir, 'multi_reel')
+    reel1 = os.path.join(multi_reel_dir, 'whatever_reel1')
+    reel2 = os.path.join(multi_reel_dir, 'whatever_reel2')
+    reel3 = os.path.join(multi_reel_dir, 'whatever_reel3')
+    bars_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc', '-n',
+        '-f', 'lavfi', '-i', 'sine', '-c:v', 'v210', '-ac', '2', '-c:a', 'pcm_s24le',
+        '-t', '20', os.path.join(output_dir, 'bars_v210_pcm24le_stereo_20sec.mov')
+        ]
+    mandel_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'mandelbrot', '-n',
+        '-c:v', 'v210', '-t', '5', os.path.join(output_dir, 'mandel_silent.mov')
+        ]
+
+    life_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc',
+        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(ten_bit_dpx_dir, 'ten_bit_%06d.dpx'),
+        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(ten_bit_dpx_dir, 'ten_bit.wav')
+        ]
+    reel1_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc',
+        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel1, 'ten_bit_reel1_%06d.dpx'),
+        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel1, 'ten_bit_reel1.wav')
+        ]
+    reel2_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc2',
+        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel2, 'ten_bit_reel2_%06d.dpx'),
+        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel2, 'ten_bit_reel2.wav')
+        ]
+    reel3_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'mandelbrot',
+        '-pix_fmt', 'gbrp10le', '-t', '20', os.path.join(reel3, 'ten_bit_reel3_%06d.dpx'),
+        '-f', 'lavfi', '-i', 'sine', '-ac', '2', '-c:a', 'pcm_s24le', '-t', '20', os.path.join(reel3, 'ten_bit_reel3.wav')
+        ]
+    dpx16_cmd = [
+        'ffmpeg', '-f', 'lavfi', '-i', 'testsrc2',
+        '-pix_fmt', 'rgb48le', '-t', '20', os.path.join(sixteen_bit_dpx_dir, 'sixteen_bit_%06d.dpx')
+        ]
+    if not os.path.isdir(output_dir):
+        os.makedirs(output_dir)
+    subprocess.call(bars_cmd)
+    subprocess.call(mandel_cmd)
+    if not args.onlyvideo:
+        if not os.path.isdir(ten_bit_dpx_dir):
+            os.makedirs(ten_bit_dpx_dir)
+        if not os.path.isdir(sixteen_bit_dpx_dir):
+            os.makedirs(sixteen_bit_dpx_dir)
+        if not os.path.isdir(reel1):
+            os.makedirs(reel1)
+        if not os.path.isdir(reel2):
+            os.makedirs(reel2)
+        if not os.path.isdir(reel3):
+            os.makedirs(reel3)
+        subprocess.call(dpx16_cmd)
+        subprocess.call(reel1_cmd)
+        subprocess.call(reel2_cmd)
+        subprocess.call(reel3_cmd)
+        subprocess.call(life_cmd)
+
+if __name__ == '__main__':
+    main(sys.argv[1:])
```

### Comparing `ifiscripts-2023.7.3.1/setup.py` & `ifiscripts-2023.7.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,10 +74,10 @@
         'dicttoxml',
         'future',
         'clairmeta'
     ],
     data_files=[('', ['film_scan_aip_documentation.txt', '26_XYZ-22_Rec709.cube'])],
     include_package_data=True,
     name='ifiscripts',
-    version='2023.07.03.1',
+    version='2023.07.03.2',
     python_requires='>=3.8'
 )
```

