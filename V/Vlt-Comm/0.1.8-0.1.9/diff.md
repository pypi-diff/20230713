# Comparing `tmp/Vlt-Comm-0.1.8.tar.gz` & `tmp/Vlt-Comm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\work\tools\vlt\dist\.tmp-tme264on\Vlt-Comm-0.1.8.tar", last modified: Thu Feb 23 01:45:16 2023, max compression
+gzip compressed data, was "C:\work\tools\vlt\dist\.tmp-u7kudc1_\Vlt-Comm-0.1.9.tar", last modified: Wed Mar 22 03:31:37 2023, max compression
```

## Comparing `Vlt-Comm-0.1.8.tar` & `Vlt-Comm-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 01:45:16.901146 Vlt-Comm-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-02-23 01:45:16.804726 Vlt-Comm-0.1.8/FcBus/
--rw-rw-rw-   0        0        0     1432 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.8/FcBus/Message.py
--rw-rw-rw-   0        0        0     3382 2022-11-17 03:14:54.000000 Vlt-Comm-0.1.8/FcBus/ParaOp.py
--rw-rw-rw-   0        0        0     3627 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.8/FcBus/Parameters.py
--rw-rw-rw-   0        0        0    10284 2023-02-21 07:16:23.000000 Vlt-Comm-0.1.8/FcBus/PnuOp.py
--rw-rw-rw-   0        0        0     3576 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.8/FcBus/RecMsg.py
--rw-rw-rw-   0        0        0     1297 2022-10-31 08:11:37.000000 Vlt-Comm-0.1.8/FcBus/SndMsg.py
--rw-rw-rw-   0        0        0      811 2022-10-09 02:02:30.000000 Vlt-Comm-0.1.8/FcBus/Support.py
--rw-rw-rw-   0        0        0     5220 2022-10-08 07:49:00.000000 Vlt-Comm-0.1.8/FcBus/VltMonitor.py
--rw-rw-rw-   0        0        0    11571 2023-02-22 23:59:08.000000 Vlt-Comm-0.1.8/FcBus/VltOp.py
--rw-rw-rw-   0        0        0      203 2023-02-21 07:22:04.000000 Vlt-Comm-0.1.8/FcBus/__init__.py
--rw-rw-rw-   0        0        0     7141 2023-02-23 00:51:12.000000 Vlt-Comm-0.1.8/FcBus/boot.py
--rw-rw-rw-   0        0        0     1764 2023-01-10 00:46:05.000000 Vlt-Comm-0.1.8/FcBus/commands.json
--rw-rw-rw-   0        0        0     2072 2022-12-13 06:15:27.000000 Vlt-Comm-0.1.8/FcBus/dbglog.py
-drwxrwxrwx   0        0        0        0 2023-02-23 01:45:16.820730 Vlt-Comm-0.1.8/FcBus/test/
--rw-rw-rw-   0        0        0      567 2022-11-14 01:21:35.000000 Vlt-Comm-0.1.8/FcBus/test/e38.py
--rw-rw-rw-   0        0        0    13458 2022-11-01 03:58:21.000000 Vlt-Comm-0.1.8/FcBus/tmcmds.json
--rw-rw-rw-   0        0        0     2013 2023-02-23 00:51:18.000000 Vlt-Comm-0.1.8/FcBus/tmcmds.py
--rw-rw-rw-   0        0        0      371 2023-02-21 07:06:40.000000 Vlt-Comm-0.1.8/FcBus/tools.py
-drwxrwxrwx   0        0        0        0 2023-02-23 01:45:16.845235 Vlt-Comm-0.1.8/FcBus/ymodem/
--rw-rw-rw-   0        0        0    32322 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.8/FcBus/ymodem/Modem.py
--rw-rw-rw-   0        0        0      963 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.8/FcBus/ymodem/Protocol.py
--rw-rw-rw-   0        0        0        0 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.8/FcBus/ymodem/__init__.py
--rw-rw-rw-   0        0        0     1091 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       20 2022-10-09 01:39:24.000000 Vlt-Comm-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3372 2023-02-23 01:45:16.898624 Vlt-Comm-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2023-02-21 07:21:05.000000 Vlt-Comm-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 01:45:16.889682 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/
--rw-rw-rw-   0        0        0     3372 2023-02-23 01:45:16.000000 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-02-23 01:45:16.000000 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 01:45:16.000000 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-02-23 01:45:16.000000 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-23 01:45:16.000000 Vlt-Comm-0.1.8/Vlt_Comm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      619 2023-02-21 07:21:30.000000 Vlt-Comm-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-23 01:45:16.901146 Vlt-Comm-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-22 03:31:37.074225 Vlt-Comm-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-03-22 03:31:36.936610 Vlt-Comm-0.1.9/FcBus/
+-rw-rw-rw-   0        0        0     1432 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.9/FcBus/Message.py
+-rw-rw-rw-   0        0        0     3382 2022-11-17 03:14:54.000000 Vlt-Comm-0.1.9/FcBus/ParaOp.py
+-rw-rw-rw-   0        0        0     3627 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.9/FcBus/Parameters.py
+-rw-rw-rw-   0        0        0    10284 2023-03-22 03:30:25.000000 Vlt-Comm-0.1.9/FcBus/PnuOp.py
+-rw-rw-rw-   0        0        0     3576 2022-05-26 13:17:17.000000 Vlt-Comm-0.1.9/FcBus/RecMsg.py
+-rw-rw-rw-   0        0        0     1297 2022-10-31 08:11:37.000000 Vlt-Comm-0.1.9/FcBus/SndMsg.py
+-rw-rw-rw-   0        0        0      811 2022-10-09 02:02:30.000000 Vlt-Comm-0.1.9/FcBus/Support.py
+-rw-rw-rw-   0        0        0     5220 2022-10-08 07:49:00.000000 Vlt-Comm-0.1.9/FcBus/VltMonitor.py
+-rw-rw-rw-   0        0        0    11012 2023-03-19 03:55:02.000000 Vlt-Comm-0.1.9/FcBus/VltOp.py
+-rw-rw-rw-   0        0        0      203 2023-02-21 07:22:04.000000 Vlt-Comm-0.1.9/FcBus/__init__.py
+-rw-rw-rw-   0        0        0     7149 2023-03-19 03:54:58.000000 Vlt-Comm-0.1.9/FcBus/boot.py
+-rw-rw-rw-   0        0        0     1763 2023-03-01 07:11:53.000000 Vlt-Comm-0.1.9/FcBus/commands.json
+-rw-rw-rw-   0        0        0     2072 2022-12-13 06:15:27.000000 Vlt-Comm-0.1.9/FcBus/dbglog.py
+drwxrwxrwx   0        0        0        0 2023-03-22 03:31:36.955469 Vlt-Comm-0.1.9/FcBus/test/
+-rw-rw-rw-   0        0        0      567 2022-11-14 01:21:35.000000 Vlt-Comm-0.1.9/FcBus/test/e38.py
+-rw-rw-rw-   0        0        0    13458 2022-11-01 03:58:21.000000 Vlt-Comm-0.1.9/FcBus/tmcmds.json
+-rw-rw-rw-   0        0        0     2013 2023-02-23 00:51:18.000000 Vlt-Comm-0.1.9/FcBus/tmcmds.py
+-rw-rw-rw-   0        0        0      371 2023-02-21 07:06:40.000000 Vlt-Comm-0.1.9/FcBus/tools.py
+drwxrwxrwx   0        0        0        0 2023-03-22 03:31:37.000001 Vlt-Comm-0.1.9/FcBus/ymodem/
+-rw-rw-rw-   0        0        0    32322 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.9/FcBus/ymodem/Modem.py
+-rw-rw-rw-   0        0        0      963 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.9/FcBus/ymodem/Protocol.py
+-rw-rw-rw-   0        0        0        0 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.9/FcBus/ymodem/__init__.py
+-rw-rw-rw-   0        0        0     1091 2022-10-08 06:59:43.000000 Vlt-Comm-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       20 2022-10-09 01:39:24.000000 Vlt-Comm-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3372 2023-03-22 03:31:37.072100 Vlt-Comm-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2023-02-21 07:21:05.000000 Vlt-Comm-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-22 03:31:37.065789 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/
+-rw-rw-rw-   0        0        0     3372 2023-03-22 03:31:36.000000 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-03-22 03:31:36.000000 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-22 03:31:36.000000 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-03-22 03:31:36.000000 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-03-22 03:31:36.000000 Vlt-Comm-0.1.9/Vlt_Comm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      619 2023-03-22 03:26:48.000000 Vlt-Comm-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-22 03:31:37.076532 Vlt-Comm-0.1.9/setup.cfg
```

### Comparing `Vlt-Comm-0.1.8/FcBus/Message.py` & `Vlt-Comm-0.1.9/FcBus/Message.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/ParaOp.py` & `Vlt-Comm-0.1.9/FcBus/ParaOp.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/Parameters.py` & `Vlt-Comm-0.1.9/FcBus/Parameters.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/PnuOp.py` & `Vlt-Comm-0.1.9/FcBus/PnuOp.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/RecMsg.py` & `Vlt-Comm-0.1.9/FcBus/RecMsg.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/SndMsg.py` & `Vlt-Comm-0.1.9/FcBus/SndMsg.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/Support.py` & `Vlt-Comm-0.1.9/FcBus/Support.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/VltMonitor.py` & `Vlt-Comm-0.1.9/FcBus/VltMonitor.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/commands.json` & `Vlt-Comm-0.1.9/FcBus/commands.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'FC360'": "{'pud': {insert: [(0, 'dtm timeout -t 5000')], delete: [0]}}"}*

```diff
@@ -21,15 +21,15 @@
         "moc": [
             "dtm timeout -t 20000",
             "dtm moc flash_block_erase -s 4 -e 6",
             "dtm timeout -t 500",
             "load moc -m yMODEM -b 0x08010000"
         ],
         "pud": [
-            " dtm timeout -t 5000",
+            "dtm timeout -t 5000",
             "dtm moc flash_block_erase -s 2 -e 2",
             "dtm timeout -t 1000",
             "load moc -m yMODEM -b 0x08008000"
         ]
     },
     "commands": {
         "ee": {
```

### Comparing `Vlt-Comm-0.1.8/FcBus/dbglog.py` & `Vlt-Comm-0.1.9/FcBus/dbglog.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/test/e38.py` & `Vlt-Comm-0.1.9/FcBus/test/e38.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/tmcmds.json` & `Vlt-Comm-0.1.9/FcBus/tmcmds.json`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/tmcmds.py` & `Vlt-Comm-0.1.9/FcBus/tmcmds.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/ymodem/Modem.py` & `Vlt-Comm-0.1.9/FcBus/ymodem/Modem.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/FcBus/ymodem/Protocol.py` & `Vlt-Comm-0.1.9/FcBus/ymodem/Protocol.py`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/LICENSE` & `Vlt-Comm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/PKG-INFO` & `Vlt-Comm-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Vlt-Comm
-Version: 0.1.8
+Version: 0.1.9
 Summary: FcBus library for Vlt drives
 Author-email: tangfei <fei.tang@danfoss.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `Vlt-Comm-0.1.8/README.md` & `Vlt-Comm-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/Vlt_Comm.egg-info/PKG-INFO` & `Vlt-Comm-0.1.9/Vlt_Comm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Vlt-Comm
-Version: 0.1.8
+Version: 0.1.9
 Summary: FcBus library for Vlt drives
 Author-email: tangfei <fei.tang@danfoss.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `Vlt-Comm-0.1.8/Vlt_Comm.egg-info/SOURCES.txt` & `Vlt-Comm-0.1.9/Vlt_Comm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Vlt-Comm-0.1.8/pyproject.toml` & `Vlt-Comm-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Vlt-Comm"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="tangfei", email="fei.tang@danfoss.com" },
 ]
 description = "FcBus library for Vlt drives"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

