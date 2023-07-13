# Comparing `tmp/QCharted-1.1.2.tar.gz` & `tmp/QCharted-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/QCharted-1.1.2.tar", last modified: Wed Sep 23 12:33:42 2020, max compression
+gzip compressed data, was "QCharted-1.1.3.tar", last modified: Thu Jul 13 12:20:02 2023, max compression
```

## Comparing `QCharted-1.1.2.tar` & `QCharted-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 arnold    (1000) arnold    (1000)        0 2020-09-23 12:33:42.000000 QCharted-1.1.2/
--rw-r--r--   0 arnold    (1000) arnold    (1000)      600 2020-09-23 12:32:53.000000 QCharted-1.1.2/setup.py
--rw-r--r--   0 arnold    (1000) arnold    (1000)     3315 2020-09-23 12:33:42.000000 QCharted-1.1.2/PKG-INFO
-drwxr-xr-x   0 arnold    (1000) arnold    (1000)        0 2020-09-23 12:33:42.000000 QCharted-1.1.2/QCharted.egg-info/
--rw-r--r--   0 arnold    (1000) arnold    (1000)        9 2020-09-23 12:33:41.000000 QCharted-1.1.2/QCharted.egg-info/top_level.txt
--rw-r--r--   0 arnold    (1000) arnold    (1000)      189 2020-09-23 12:33:42.000000 QCharted-1.1.2/QCharted.egg-info/SOURCES.txt
--rw-r--r--   0 arnold    (1000) arnold    (1000)        1 2020-09-23 12:33:41.000000 QCharted-1.1.2/QCharted.egg-info/dependency_links.txt
--rw-r--r--   0 arnold    (1000) arnold    (1000)     3315 2020-09-23 12:33:41.000000 QCharted-1.1.2/QCharted.egg-info/PKG-INFO
--rw-r--r--   0 arnold    (1000) arnold    (1000)       40 2020-09-23 12:33:41.000000 QCharted-1.1.2/QCharted.egg-info/requires.txt
--rw-r--r--   0 arnold    (1000) arnold    (1000)    20029 2020-09-23 12:32:53.000000 QCharted-1.1.2/QCharted.py
--rw-r--r--   0 arnold    (1000) arnold    (1000)       38 2020-09-23 12:33:42.000000 QCharted-1.1.2/setup.cfg
--rw-r--r--   0 arnold    (1000) arnold    (1000)     2210 2020-09-23 12:32:53.000000 QCharted-1.1.2/README.md
+drwxrwxr-x   0 arnold    (1002) arnold    (1002)        0 2023-07-13 12:20:02.634485 QCharted-1.1.3/
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)    35149 2023-07-13 12:00:00.000000 QCharted-1.1.3/LICENSE
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)     2506 2023-07-13 12:20:02.634485 QCharted-1.1.3/PKG-INFO
+drwxrwxr-x   0 arnold    (1002) arnold    (1002)        0 2023-07-13 12:20:02.634485 QCharted-1.1.3/QCharted.egg-info/
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)     2506 2023-07-13 12:20:02.000000 QCharted-1.1.3/QCharted.egg-info/PKG-INFO
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)      197 2023-07-13 12:20:02.000000 QCharted-1.1.3/QCharted.egg-info/SOURCES.txt
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)        1 2023-07-13 12:20:02.000000 QCharted-1.1.3/QCharted.egg-info/dependency_links.txt
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)       40 2023-07-13 12:20:02.000000 QCharted-1.1.3/QCharted.egg-info/requires.txt
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)        9 2023-07-13 12:20:02.000000 QCharted-1.1.3/QCharted.egg-info/top_level.txt
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)    20117 2023-07-13 12:02:31.000000 QCharted-1.1.3/QCharted.py
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)     2210 2023-07-13 12:00:00.000000 QCharted-1.1.3/README.md
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)       38 2023-07-13 12:20:02.634485 QCharted-1.1.3/setup.cfg
+-rw-rw-r--   0 arnold    (1002) arnold    (1002)      600 2023-07-13 12:18:37.000000 QCharted-1.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `QCharted-1.1.2/setup.py` & `QCharted-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='QCharted',
-    version='1.1.2',
+    version='1.1.3',
     author="Bernhard Arnold",
     author_email="bernhard.arnold@oeaw.ac.at",
     url = "https://github.com/arnobaer/QCharted",
     description="Plotting large data series using PyQtChart.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=['QCharted'],
```

### Comparing `QCharted-1.1.2/QCharted.py` & `QCharted-1.1.3/QCharted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import math
 import re
 
 import numpy as np
 
 from PyQt5 import QtCore, QtGui, QtWidgets, QtChart
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 __all__ = ['ChartView', 'Chart']
 
-milliseconds = 1000.
+milliseconds = 1e3
 
-def toDateTime(seconds):
+def toDateTime(seconds: float) -> QtCore.QDateTime:
     """Returns seconds as QDateTime object."""
-    return QtCore.QDateTime.fromMSecsSinceEpoch(seconds * milliseconds)
+    return QtCore.QDateTime.fromMSecsSinceEpoch(int(seconds * milliseconds))
 
-def toSecs(datetime):
+def toSecs(datetime: QtCore.QDateTime) -> float:
     """Returns QDateTime object as seconds."""
     return datetime.toMSecsSinceEpoch() / milliseconds
 
-def toMSecs(seconds):
+def toMSecs(seconds: float) -> int:
     """Returns QDateTime object as milli seconds."""
-    return seconds * milliseconds
+    return int(seconds * milliseconds)
 
-def stripHtml(html):
+def stripHtml(html: str) -> str:
     html = re.sub(r'<[^>]+>', ' ', html)
     html = re.sub(r'&[^;]*;', ' ', html)
     html = re.sub(r'\s+', ' ', html)
     return html
 
 class DataSeries:
     """2D data series using numpy arrays.
```

### Comparing `QCharted-1.1.2/README.md` & `QCharted-1.1.3/README.md`

 * *Files identical despite different names*

