# Comparing `tmp/logol-0.0.5.tar.gz` & `tmp/logol-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logol-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "logol-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `logol-0.0.5.tar` & `logol-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3161 2022-02-11 11:53:48.259908 logol-0.0.5/.gitignore
--rw-r--r--   0        0        0     1105 2022-12-26 16:09:44.368041 logol-0.0.5/LICENSE
--rw-r--r--   0        0        0        0 2022-12-26 12:31:09.358622 logol-0.0.5/README.md
--rw-r--r--   0        0        0     4374 2023-05-19 17:51:14.960008 logol-0.0.5/logol.py
--rw-r--r--   0        0        0      417 2023-05-19 18:18:36.913952 logol-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      555 2023-05-19 17:11:02.794317 logol-0.0.5/test.py
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 logol-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3161 2022-02-11 11:53:48.259908 logol-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1105 2022-12-26 16:09:44.368041 logol-0.0.6/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-26 12:31:09.358622 logol-0.0.6/README.md
+-rw-r--r--   0        0        0     4389 2023-07-13 16:02:07.378616 logol-0.0.6/logol.py
+-rw-r--r--   0        0        0      417 2023-05-19 18:18:36.913952 logol-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-05-19 17:11:02.794317 logol-0.0.6/test.py
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 logol-0.0.6/PKG-INFO
```

### Comparing `logol-0.0.5/.gitignore` & `logol-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `logol-0.0.5/LICENSE` & `logol-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `logol-0.0.5/logol.py` & `logol-0.0.6/logol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Pre-configured logs"""
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 import logging
 from logging.handlers import RotatingFileHandler
 from logging import Logger
 from typing import Dict, Optional
 from time import time_ns
 from pathlib import Path
@@ -45,15 +45,15 @@
     filename = Path(filename)
     logpath = Path(BASE_PATH) / filename.relative_to(filename.anchor)
     logpath.parent.mkdir(parents=True, exist_ok=True)
 
     logpath = logpath.with_suffix('.log')
     
     formatter = logging.Formatter(fmt=FORMAT_PRINTER, datefmt='%d/%b/%y %H:%M:%S')
-    logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024)
+    logfile = RotatingFileHandler(logpath, mode='a', encoding='utf-8', maxBytes=filesize_mb*1024*1024, backupCount=1)
 
     logfile.setLevel(logging.DEBUG)
     logfile.setFormatter(formatter)
     logger.addHandler(logfile)
     
     console = logging.StreamHandler()
     console.setLevel(logging.INFO)
```

### Comparing `logol-0.0.5/test.py` & `logol-0.0.6/test.py`

 * *Files identical despite different names*

