# Comparing `tmp/SpecLab-4.2.2.tar.gz` & `tmp/SpecLab-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpecLab-4.2.2.tar", last modified: Wed Jul 12 15:23:27 2023, max compression
+gzip compressed data, was "SpecLab-4.2.3.tar", last modified: Thu Jul 13 16:16:06 2023, max compression
```

## Comparing `SpecLab-4.2.2.tar` & `SpecLab-4.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:23:27.964980 SpecLab-4.2.2/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:23:09.000000 SpecLab-4.2.2/README.md
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.960980 SpecLab-4.2.2/SpecLab/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/aux/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/aux/param_files/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.default.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.2/SpecLab/aux/pyqtgraph_modifications.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2183 2023-07-12 15:02:27.000000 SpecLab-4.2.2/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-12 15:22:43.000000 SpecLab-4.2.2/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1385 2023-07-12 14:56:42.000000 SpecLab-4.2.2/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5047 2023-07-12 15:22:57.000000 SpecLab-4.2.2/SpecLab/doc/README.md
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/doc/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/SpecLabFunctions.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/__init__.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/gen/myfunc.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.2/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49849 2023-07-12 15:22:22.000000 SpecLab-4.2.2/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-12 15:23:27.964980 SpecLab-4.2.2/SpecLab.egg-info/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5301 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/requires.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-12 15:23:27.000000 SpecLab-4.2.2/SpecLab.egg-info/top_level.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-12 15:23:27.964980 SpecLab-4.2.2/setup.cfg
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-12 15:20:08.000000 SpecLab-4.2.2/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-13 16:16:06.864657 SpecLab-4.2.3/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-13 16:13:13.000000 SpecLab-4.2.3/README.md
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/aux/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/aux/param_files/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    36736 2023-07-12 15:12:23.000000 SpecLab-4.2.3/SpecLab/aux/pyqtgraph_modifications.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2186 2023-07-13 16:12:45.000000 SpecLab-4.2.3/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1020 2023-07-13 16:11:49.000000 SpecLab-4.2.3/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1509 2023-07-13 16:11:31.000000 SpecLab-4.2.3/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5409 2023-07-13 16:10:48.000000 SpecLab-4.2.3/SpecLab/doc/README.md
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/doc/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53081 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/SpecLabFunctions.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/__init__.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/gen/myfunc.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-07-10 20:06:38.000000 SpecLab-4.2.3/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    49863 2023-07-13 16:00:58.000000 SpecLab-4.2.3/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-07-13 16:16:06.864657 SpecLab-4.2.3/SpecLab.egg-info/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     5663 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      760 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        1 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      138 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/requires.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        8 2023-07-13 16:16:06.000000 SpecLab-4.2.3/SpecLab.egg-info/top_level.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)       38 2023-07-13 16:16:06.864657 SpecLab-4.2.3/setup.cfg
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1299 2023-07-13 16:13:05.000000 SpecLab-4.2.3/setup.py
```

### Comparing `SpecLab-4.2.2/PKG-INFO` & `SpecLab-4.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.2
+Version: 4.2.3
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.2 (Latest)
+# imXam:  v4.2.3 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 12, 2023)
+author: Adam F Kowalski (July 13, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have
+Create a conda environment to install into (recommended).  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
-From a terminal window:
+In a terminal window, type
 
 `conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
@@ -52,14 +52,15 @@
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
 `python SpecLab_config.py`
 
+If SpecLab_config.py fails, it is likely a permissions issue.  Please check to make sure that you can write and untar to your site-packages/ directory.
 
 ### Basic Usage
 
 You will then be able to run imXam.py from anywhere (it is located in .../anaconda3/envs/your_env_name/bin/).
 
 Basic usage (or create an alias for `imXam.py -f` in your .bash_profile):
 
@@ -88,15 +89,15 @@
 Please see KNOWN_ISSUES.
 
 Enjoy!
 
 
 ## Interactive Commands
 
-Will need to left mouse click on pyqtgraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQTGraph display window.
+Will need to left mouse click on PyQtGraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQtGraph display window.
 
 click 'h' key to print this to screen from within imXam:
 
 The default parameters used to do the calculations are in imXam_param.dat.  You can edit this file from command line by typing `epar_imXam.py'
 
 
 q:  quit imXam.
@@ -138,28 +139,25 @@
 
 `pip install SpecLab --upgrade`
 
 # To Uninstall
 
 `pip uninstall SpecLab`
 
-Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
-
 # Acknowledgments
 
-Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
-Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
-Thanks to Gordon MacDonald for helpful suggestions.
+Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.  Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  Thanks to Gordon MacDonald for helpful suggestions.
 
 # Troubleshooting
-On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+On a Linux, one may have to try these commands if one gets an `xcb` [error](https://stackoverflow.com/questions/68036484/qt6-qt-qpa-plugin-could-not-load-the-qt-platform-plugin-xcb-in-even-thou/68058308#68058308) during `pip install SpecLab`:
 
 `sudo apt install libxcb-cursor0`
 
 or
 
 `sudo apt install --reinstall libxcb-cursor0`
 
 or
 
 `sudo apt-get install --reinstall libxcb-xinerama0`
 
+On Mac, there should be no problem with Intel processors.  For M1/2 processors, a build for PyQt6 will become available shortly.
```

### Comparing `SpecLab-4.2.2/README.md` & `SpecLab-4.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# imXam:  v4.2.2 (Latest)
+# imXam:  v4.2.3 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 12, 2023)
+author: Adam F Kowalski (July 13, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have
+Create a conda environment to install into (recommended).  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
-From a terminal window:
+In a terminal window, type
 
 `conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
@@ -43,14 +43,15 @@
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
 `python SpecLab_config.py`
 
+If SpecLab_config.py fails, it is likely a permissions issue.  Please check to make sure that you can write and untar to your site-packages/ directory.
 
 ### Basic Usage
 
 You will then be able to run imXam.py from anywhere (it is located in .../anaconda3/envs/your_env_name/bin/).
 
 Basic usage (or create an alias for `imXam.py -f` in your .bash_profile):
 
@@ -79,15 +80,15 @@
 Please see KNOWN_ISSUES.
 
 Enjoy!
 
 
 ## Interactive Commands
 
-Will need to left mouse click on pyqtgraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQTGraph display window.
+Will need to left mouse click on PyQtGraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQtGraph display window.
 
 click 'h' key to print this to screen from within imXam:
 
 The default parameters used to do the calculations are in imXam_param.dat.  You can edit this file from command line by typing `epar_imXam.py'
 
 
 q:  quit imXam.
@@ -129,28 +130,25 @@
 
 `pip install SpecLab --upgrade`
 
 # To Uninstall
 
 `pip uninstall SpecLab`
 
-Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
-
 # Acknowledgments
 
-Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
-Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
-Thanks to Gordon MacDonald for helpful suggestions.
+Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.  Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  Thanks to Gordon MacDonald for helpful suggestions.
 
 # Troubleshooting
-On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+On a Linux, one may have to try these commands if one gets an `xcb` [error](https://stackoverflow.com/questions/68036484/qt6-qt-qpa-plugin-could-not-load-the-qt-platform-plugin-xcb-in-even-thou/68058308#68058308) during `pip install SpecLab`:
 
 `sudo apt install libxcb-cursor0`
 
 or
 
 `sudo apt install --reinstall libxcb-cursor0`
 
 or
 
 `sudo apt-get install --reinstall libxcb-xinerama0`
 
+On Mac, there should be no problem with Intel processors.  For M1/2 processors, a build for PyQt6 will become available shortly.
```

### Comparing `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.2.3/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/aux/pyqtgraph_modifications.tar.gz` & `SpecLab-4.2.3/SpecLab/aux/pyqtgraph_modifications.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.2.3/SpecLab/cfg/SpecLab_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 
-import os
+# import os
 import site
 import tarfile
 
 
 try:
     your_site_packages_location = site.getsitepackages()
     tar_fname = your_site_packages_location[0]+'/'+'SpecLab/aux/pyqtgraph_modifications.tar.gz'
-    current_dir = os.getcwd()+'/'
+#    current_dir = os.getcwd()+'/'
 
  #   if not os.path.exists(your_site_packages_location[0]+'/pyqtgraph10_speclab/'):
 #        print('Extracting PyQTGraph v10 tarfile (pyqtgraph10_speclab.tar.gz) contents to ', your_site_packages_location[0]+'/pyqtgraph10_speclab/')
  #       print('If uninstall SpecLab through pip (pip uninstall SpecLab), you may also want to rm -r pyqtgraph10_speclab/ from within your site-packages/ directory. ** Please be careful with the rm -r command **')
```

### Comparing `SpecLab-4.2.2/SpecLab/doc/CHANGELOG.txt` & `SpecLab-4.2.3/SpecLab/doc/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 - updates for python 3.6 and 3.7
 
 4.1.1 
 
 - updates to PyQtGraph, photutils module call for Python 3.8, Numpy 1.
 
-4.2.2
+4.2.3
 
 Updated everything to PyQtGraph 0.13, PyQt6, and Python 3.11.4.  All other packages were updated to latest version.
 No longer packages up the PyQtGraph into a tar, now only packages up the modified routines (ROI, GraphicsScene, ImageView).
 
 install_requires=['numpy>=1.25.0', 'plotly>=5.15.0', 'pandas>=2.0.3','astropy>=5.3.1','scipy>=1.11.1','matplotlib>=3.7.2','PyQt6==6.5.1', 'photutils>=1.8.0','pyqtgraph==0.13.3',]
```

### Comparing `SpecLab-4.2.2/SpecLab/doc/KNOWN_ISSUES.txt` & `SpecLab-4.2.3/SpecLab/doc/KNOWN_ISSUES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 or
 sudo apt-get install --reinstall libxcb-xinerama0
 
 Note 4: The default version of PyQtGraph encounters a problem with Python 3.11:
 https://github.com/python/cpython/issues/105497
 This fix won't get pushed until August 2023.  In the meantime, I've made the necessary
 fixes to ROI.py in PyQtGraph.
+
+Note 5: This should work with Intel processors on a Mac.  For M1/2 processors, a build for PyQt6 should be available soon.
```

### Comparing `SpecLab-4.2.2/SpecLab/doc/LICENSE.txt` & `SpecLab-4.2.3/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/doc/README.md` & `SpecLab-4.2.3/SpecLab/doc/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# imXam:  v4.2.2 (Latest)
+# imXam:  v4.2.3 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 12, 2023)
+author: Adam F Kowalski (July 13, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have
+Create a conda environment to install into (recommended).  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
-From a terminal window:
+In a terminal window, type
 
 `conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
@@ -43,14 +43,15 @@
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
 `python SpecLab_config.py`
 
+If SpecLab_config.py fails, it is likely a permissions issue.  Please check to make sure that you can write and untar to your site-packages/ directory.
 
 ### Basic Usage
 
 You will then be able to run imXam.py from anywhere (it is located in .../anaconda3/envs/your_env_name/bin/).
 
 Basic usage (or create an alias for `imXam.py -f` in your .bash_profile):
 
@@ -79,15 +80,15 @@
 Please see KNOWN_ISSUES.
 
 Enjoy!
 
 
 ## Interactive Commands
 
-Will need to left mouse click on pyqtgraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQTGraph display window.
+Will need to left mouse click on PyQtGraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQtGraph display window.
 
 click 'h' key to print this to screen from within imXam:
 
 The default parameters used to do the calculations are in imXam_param.dat.  You can edit this file from command line by typing `epar_imXam.py'
 
 
 q:  quit imXam.
@@ -129,28 +130,25 @@
 
 `pip install SpecLab --upgrade`
 
 # To Uninstall
 
 `pip uninstall SpecLab`
 
-Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
-
 # Acknowledgments
 
-Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
-Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
-Thanks to Gordon MacDonald for helpful suggestions.
+Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.  Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  Thanks to Gordon MacDonald for helpful suggestions.
 
 # Troubleshooting
-On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+On a Linux, one may have to try these commands if one gets an `xcb` [error](https://stackoverflow.com/questions/68036484/qt6-qt-qpa-plugin-could-not-load-the-qt-platform-plugin-xcb-in-even-thou/68058308#68058308) during `pip install SpecLab`:
 
 `sudo apt install libxcb-cursor0`
 
 or
 
 `sudo apt install --reinstall libxcb-cursor0`
 
 or
 
 `sudo apt-get install --reinstall libxcb-xinerama0`
 
+On Mac, there should be no problem with Intel processors.  For M1/2 processors, a build for PyQt6 will become available shortly.
```

### Comparing `SpecLab-4.2.2/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.2.3/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/gen/globals.py` & `SpecLab-4.2.3/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/gen/myfunc.py` & `SpecLab-4.2.3/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/SpecLab/imXam/imXam.py` & `SpecLab-4.2.3/SpecLab/imXam/imXam.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: v4.2.2 (July 12, 2023)')
-print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
-print(' You may have to click on gui with left mouse button in order to use interactive commands')
+print('imXam: v4.2.3 (July 13, 2023)')
+print(' To shut down gui, type q in display window, type h for interactive commands, use middle mouse wheel to zoom in and out')
+print(' You may have to click on image display with left mouse button in order to use interactive commands')
 print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
 print('--> To edit imXam_param.dat with vim, type epar_imXam.py from a terminal.')
 print('======================================================')
```

### Comparing `SpecLab-4.2.2/SpecLab.egg-info/PKG-INFO` & `SpecLab-4.2.3/SpecLab.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: SpecLab
-Version: 4.2.2
+Version: 4.2.3
 Summary: IRAF imexam+DS9 alternative for Python
 Home-page: http://pypi.python.org/pypi/SpecLab/
 Author: A. F. Kowalski
 Author-email: adam.f.kowalski@colorado.edu
 Description-Content-Type: text/markdown
 
-# imXam:  v4.2.2 (Latest)
+# imXam:  v4.2.3 (Latest)
 
 **imXam** is the first interactive program finished for the **SpecLab** python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (PyQtGraph + Plotly) in the future as these get finished.
 
-This uses [PyQTGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically.  
+This uses [PyQtGraph](https://www.pyqtgraph.org/) 0.13.3, which will be installed automatically below.  
 A customized version of a few routines (`ROI.py`, `GraphicsScene.py`, `ImageView.py`) will be copied
 to your site-packages/pyqtgraph/ by running the config below.  The installation below will install PyQt6 (6.5.1).
 
-author: Adam F Kowalski (July 12, 2023)
+author: Adam F Kowalski (July 13, 2023)
 
 ## Installing imXam 
 
 ### Step 1
 
 From terminal (if you want to install to your current conda environment; if not, go to Step 2):
 
 `pip install SpecLab`
 
 
 ### Step 2
 
-Create a conda environment to install into.  If you already have
+Create a conda environment to install into (recommended).  If you already have
 run `pip install SpecLab` in that environment, then skip to Step 3 below.
 
 To set up a fresh conda environment:
 
-From a terminal window:
+In a terminal window, type
 
 `conda create --name your_env_name python=3.11`
 
 `conda activate your_env_name`
 
 `pip install SpecLab`
 
@@ -52,14 +52,15 @@
 
 You may have to open a fresh tab in your terminal for your system to see the new routines in .../your_env_name/bin/.  You can also:
 
 `cd /location_of_your_anaconda/anaconda3/envs/your_env_name/bin/`
 
 `python SpecLab_config.py`
 
+If SpecLab_config.py fails, it is likely a permissions issue.  Please check to make sure that you can write and untar to your site-packages/ directory.
 
 ### Basic Usage
 
 You will then be able to run imXam.py from anywhere (it is located in .../anaconda3/envs/your_env_name/bin/).
 
 Basic usage (or create an alias for `imXam.py -f` in your .bash_profile):
 
@@ -88,15 +89,15 @@
 Please see KNOWN_ISSUES.
 
 Enjoy!
 
 
 ## Interactive Commands
 
-Will need to left mouse click on pyqtgraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQTGraph display window.
+Will need to left mouse click on PyQtGraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the PyQtGraph display window.
 
 click 'h' key to print this to screen from within imXam:
 
 The default parameters used to do the calculations are in imXam_param.dat.  You can edit this file from command line by typing `epar_imXam.py'
 
 
 q:  quit imXam.
@@ -138,28 +139,25 @@
 
 `pip install SpecLab --upgrade`
 
 # To Uninstall
 
 `pip uninstall SpecLab`
 
-Will have to remove pyqtgraph10_speclab/ from your environment site-packages by hand.
-
 # Acknowledgments
 
-Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
-Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
-Thanks to Gordon MacDonald for helpful suggestions.
+Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.  Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  Thanks to Gordon MacDonald for helpful suggestions.
 
 # Troubleshooting
-On a Linux, one may have to try these commands if one gets an error during `pip install Speclab`:
+On a Linux, one may have to try these commands if one gets an `xcb` [error](https://stackoverflow.com/questions/68036484/qt6-qt-qpa-plugin-could-not-load-the-qt-platform-plugin-xcb-in-even-thou/68058308#68058308) during `pip install SpecLab`:
 
 `sudo apt install libxcb-cursor0`
 
 or
 
 `sudo apt install --reinstall libxcb-cursor0`
 
 or
 
 `sudo apt-get install --reinstall libxcb-xinerama0`
 
+On Mac, there should be no problem with Intel processors.  For M1/2 processors, a build for PyQt6 will become available shortly.
```

### Comparing `SpecLab-4.2.2/SpecLab.egg-info/SOURCES.txt` & `SpecLab-4.2.3/SpecLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.2.2/setup.py` & `SpecLab-4.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from pathlib import Path
 
 setup(
     name='SpecLab',
-    version='4.2.2',
+    version='4.2.3',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat', '*.md', '*.rst'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
```

