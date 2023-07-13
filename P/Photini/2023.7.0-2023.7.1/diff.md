# Comparing `tmp/Photini-2023.7.0.tar.gz` & `tmp/Photini-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmp_te6b7bu/Photini-2023.7.0.tar", last modified: Thu Jul  6 08:02:10 2023, max compression
+gzip compressed data, was "/home/jim/Documents/projects/Photini/main/dist/tmpz8fxg595/Photini-2023.7.1.tar", last modified: Thu Jul 13 10:34:48 2023, max compression
```

## Comparing `Photini-2023.7.0.tar` & `Photini-2023.7.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/
--rw-r--r--   0 jim       (1026) users      (100)    16225 2023-07-06 07:57:56.000000 Photini-2023.7.0/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.7.0/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      529 2023-07-06 07:57:56.000000 Photini-2023.7.0/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)     8956 2023-07-06 08:02:10.000000 Photini-2023.7.0/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     7859 2023-05-22 14:34:16.000000 Photini-2023.7.0/README.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/custom_build/
--rw-r--r--   0 jim       (1026) users      (100)     2178 2023-07-06 07:57:56.000000 Photini-2023.7.0/custom_build/backend.py
--rw-r--r--   0 jim       (1026) users      (100)     3469 2023-07-06 07:57:56.000000 Photini-2023.7.0/pyproject.toml
--rw-r--r--   0 jim       (1026) users      (100)       38 2023-07-06 08:02:10.000000 Photini-2023.7.0/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     2558 2023-07-06 07:57:56.000000 Photini-2023.7.0/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)     1746 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/Photini.egg-info/SOURCES.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)     1021 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)      148 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/_version.py
--rw-r--r--   0 jim       (1026) users      (100)    19538 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22083 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    32893 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    47745 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    29058 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    10685 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    42960 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)    55597 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2026 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    21228 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    10258 2023-07-06 08:02:09.000000 Photini-2023.7.0/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      321 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/linux/photini.desktop
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/map/
--rw-r--r--   0 jim       (1026) users      (100)     7507 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/bingmap.js
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     6211 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/googlemap.js
--rw-r--r--   0 jim       (1026) users      (100)     5687 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/mapboxmap.js
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/data/map/pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-06 08:02:10.000000 Photini-2023.7.0/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    23314 2023-05-22 14:34:16.000000 Photini-2023.7.0/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     8435 2023-05-17 06:57:34.000000 Photini-2023.7.0/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    32853 2023-05-22 14:34:16.000000 Photini-2023.7.0/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40229 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    36703 2023-05-29 10:44:57.000000 Photini-2023.7.0/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25512 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10708 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    36607 2023-05-22 14:34:16.000000 Photini-2023.7.0/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     7887 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.7.0/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40948 2023-05-22 14:34:16.000000 Photini-2023.7.0/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    72475 2023-05-22 14:34:16.000000 Photini-2023.7.0/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    47789 2023-05-17 06:57:34.000000 Photini-2023.7.0/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    35993 2023-07-06 07:57:56.000000 Photini-2023.7.0/src/photini/widgets.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/
+-rw-r--r--   0 jim       (1026) users      (100)    16304 2023-07-13 10:32:50.000000 Photini-2023.7.1/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.7.1/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      529 2023-07-06 07:57:56.000000 Photini-2023.7.1/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)     8956 2023-07-13 10:34:48.000000 Photini-2023.7.1/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     7859 2023-05-22 14:34:16.000000 Photini-2023.7.1/README.rst
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/custom_build/
+-rw-r--r--   0 jim       (1026) users      (100)     2294 2023-07-13 10:32:50.000000 Photini-2023.7.1/custom_build/backend.py
+-rw-r--r--   0 jim       (1026) users      (100)     3469 2023-07-06 07:57:56.000000 Photini-2023.7.1/pyproject.toml
+-rw-r--r--   0 jim       (1026) users      (100)       38 2023-07-13 10:34:48.000000 Photini-2023.7.1/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     2558 2023-07-06 07:57:56.000000 Photini-2023.7.1/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)     1746 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/Photini.egg-info/SOURCES.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)     1021 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)      148 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/_version.py
+-rw-r--r--   0 jim       (1026) users      (100)    19538 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22083 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    32893 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    47745 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    29058 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10685 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    42960 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)    55597 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2026 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    21228 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10258 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      321 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/linux/photini.desktop
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/map/
+-rw-r--r--   0 jim       (1026) users      (100)     7507 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/bingmap.js
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     6211 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/googlemap.js
+-rw-r--r--   0 jim       (1026) users      (100)     5687 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/mapboxmap.js
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/data/map/pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-07-13 10:34:48.000000 Photini-2023.7.1/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    23314 2023-05-22 14:34:16.000000 Photini-2023.7.1/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     8435 2023-05-17 06:57:34.000000 Photini-2023.7.1/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    32853 2023-05-22 14:34:16.000000 Photini-2023.7.1/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40643 2023-07-13 10:32:50.000000 Photini-2023.7.1/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    36703 2023-05-29 10:44:57.000000 Photini-2023.7.1/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25512 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10708 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    36607 2023-05-22 14:34:16.000000 Photini-2023.7.1/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     7887 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.7.1/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40948 2023-05-22 14:34:16.000000 Photini-2023.7.1/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    72475 2023-05-22 14:34:16.000000 Photini-2023.7.1/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    47789 2023-05-17 06:57:34.000000 Photini-2023.7.1/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    35993 2023-07-06 07:57:56.000000 Photini-2023.7.1/src/photini/widgets.py
```

### Comparing `Photini-2023.7.0/CHANGELOG.txt` & `Photini-2023.7.1/CHANGELOG.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see
 <http://www.gnu.org/licenses/>.
 
+Changes in v2023.7.1:
+  1/ Fix bug setting file dates before 1970 on Windows.
+
 Changes in v2023.7.0:
   1/ Enabled installation of PyQt5 & PyQt6 with pip and photini-configure.
   2/ Fix crash if using arrow key navigation when no pictures loaded.
   3/ Other minor improvements and bug fixes.
   4/ Improved and modernised package building process.
 
 Changes in v2023.5.2:
```

### Comparing `Photini-2023.7.0/LICENSE.txt` & `Photini-2023.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/MANIFEST.in` & `Photini-2023.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/PKG-INFO` & `Photini-2023.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Photini-2023.7.0/README.rst` & `Photini-2023.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/custom_build/backend.py` & `Photini-2023.7.1/custom_build/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,20 @@
         if not os.path.exists(src_file):
             continue
         dst_file = os.path.join(dst_dir, 'photini.' + lang + '.qm')
         if (os.path.exists(dst_file) and
                 os.stat(dst_file).st_mtime >= os.stat(src_file).st_mtime):
             continue
         print('compiling {} -> {}'.format(src_file, dst_file))
-        subprocess.check_call([
-            'lrelease-qt5', '-silent', src_file, '-qm', dst_file])
+        try:
+            subprocess.check_call([
+                'lrelease-qt5', '-silent', src_file, '-qm', dst_file])
+        except FileNotFoundError as ex:
+            print('FAIL:', str(ex))
+            return
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
     build_lang()
     return _orig.build_wheel(wheel_directory, config_settings=config_settings,
                              metadata_directory=metadata_directory)
```

### Comparing `Photini-2023.7.0/pyproject.toml` & `Photini-2023.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/setup.py` & `Photini-2023.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/Photini.egg-info/SOURCES.txt` & `Photini-2023.7.1/src/Photini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/__init__.py` & `Photini-2023.7.1/src/photini/__init__.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/__main__.py` & `Photini-2023.7.1/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/address.py` & `Photini-2023.7.1/src/photini/address.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/bingmap.py` & `Photini-2023.7.1/src/photini/bingmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/configstore.py` & `Photini-2023.7.1/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/cv.py` & `Photini-2023.7.1/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/LICENSE.txt` & `Photini-2023.7.1/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/icons/photini_128.png` & `Photini-2023.7.1/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/icons/photini_48.png` & `Photini-2023.7.1/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/icons/photini_win.ico` & `Photini-2023.7.1/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/keys.txt` & `Photini-2023.7.1/src/photini/data/keys.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.ca.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.cs.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.de.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.de.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.en.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.en.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.es.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.fr.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.it.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.ko.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.nb.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/lang/photini.pl.qm` & `Photini-2023.7.1/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/map/bingmap.js` & `Photini-2023.7.1/src/photini/data/map/bingmap.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/map/googlemap.js` & `Photini-2023.7.1/src/photini/data/map/googlemap.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/map/mapboxmap.js` & `Photini-2023.7.1/src/photini/data/map/mapboxmap.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/map/pin_grey.png` & `Photini-2023.7.1/src/photini/data/map/pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/map/pin_red.png` & `Photini-2023.7.1/src/photini/data/map/pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2023.7.1/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/descriptive.py` & `Photini-2023.7.1/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/editor.py` & `Photini-2023.7.1/src/photini/editor.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/editsettings.py` & `Photini-2023.7.1/src/photini/editsettings.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/exiv2.py` & `Photini-2023.7.1/src/photini/exiv2.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/ffmpeg.py` & `Photini-2023.7.1/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/flickr.py` & `Photini-2023.7.1/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/googlemap.py` & `Photini-2023.7.1/src/photini/googlemap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/googlephotos.py` & `Photini-2023.7.1/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/gpximporter.py` & `Photini-2023.7.1/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/imagelist.py` & `Photini-2023.7.1/src/photini/imagelist.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
 import io
 import logging
 import os
+import time
 
 try:
     import PIL.Image as PIL
 except ImportError:
     PIL = None
 
 from photini.ffmpeg import FFmpeg
@@ -909,17 +910,24 @@
             # old config format
             keep_time = ('now', 'keep')[keep_time]
         if not images:
             images = self.images
         with Busy():
             for image in images:
                 if keep_time == 'taken' and image.metadata.date_taken:
-                    file_times = (
-                        image.file_times[0],
-                        image.metadata.date_taken['datetime'].timestamp())
+                    date_taken = image.metadata.date_taken['datetime']
+                    try:
+                        date_taken = date_taken.timestamp()
+                    except Exception:
+                        # probably a negative value on Windows
+                        epoch = time.gmtime(0)
+                        epoch = datetime(
+                            epoch.tm_year, epoch.tm_mon, epoch.tm_mday)
+                        date_taken = (date_taken - epoch).total_seconds()
+                    file_times = image.file_times[0], date_taken
                 elif keep_time == 'keep':
                     file_times = image.file_times
                 else:
                     file_times = None
                 image.metadata.save(
                     if_mode=if_mode, sc_mode=sc_mode,
                     iptc_mode=iptc_mode, file_times=file_times)
```

### Comparing `Photini-2023.7.0/src/photini/importer.py` & `Photini-2023.7.1/src/photini/importer.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/ipernity.py` & `Photini-2023.7.1/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/loggerwindow.py` & `Photini-2023.7.1/src/photini/loggerwindow.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/mapboxmap.py` & `Photini-2023.7.1/src/photini/mapboxmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/metadata.py` & `Photini-2023.7.1/src/photini/metadata.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/ownership.py` & `Photini-2023.7.1/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/photinimap.py` & `Photini-2023.7.1/src/photini/photinimap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/pixelfed.py` & `Photini-2023.7.1/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/pyqt.py` & `Photini-2023.7.1/src/photini/pyqt.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/regions.py` & `Photini-2023.7.1/src/photini/regions.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/scripts.py` & `Photini-2023.7.1/src/photini/scripts.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/spelling.py` & `Photini-2023.7.1/src/photini/spelling.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/technical.py` & `Photini-2023.7.1/src/photini/technical.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/types.py` & `Photini-2023.7.1/src/photini/types.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/uploader.py` & `Photini-2023.7.1/src/photini/uploader.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.7.0/src/photini/widgets.py` & `Photini-2023.7.1/src/photini/widgets.py`

 * *Files identical despite different names*

