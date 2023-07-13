# Comparing `tmp/flashcam-1.5.3.tar.gz` & `tmp/flashcam-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.5.3.tar", last modified: Wed Jul 12 13:26:08 2023, max compression
+gzip compressed data, was "flashcam-1.5.4.tar", last modified: Thu Jul 13 20:59:03 2023, max compression
```

## Comparing `flashcam-1.5.3.tar` & `flashcam-1.5.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.468169 flashcam-1.5.3/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 13:26:08.468169 flashcam-1.5.3/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-04-17 13:40:53.000000 flashcam-1.5.3/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24826 2023-04-20 12:20:29.000000 flashcam-1.5.3/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-06 11:29:38.000000 flashcam-1.5.3/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-06 11:29:38.000000 flashcam-1.5.3/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-06 11:48:21.000000 flashcam-1.5.3/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8079 2023-04-17 13:40:53.000000 flashcam-1.5.3/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.468169 flashcam-1.5.3/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-20 08:33:53.000000 flashcam-1.5.3/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-06 11:29:38.000000 flashcam-1.5.3/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-12 09:16:16.000000 flashcam-1.5.3/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-20 12:14:15.000000 flashcam-1.5.3/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102690 2023-07-12 13:24:22.000000 flashcam-1.5.3/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-06 11:51:33.000000 flashcam-1.5.3/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-12 09:16:16.000000 flashcam-1.5.3/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-12 13:08:09.000000 flashcam-1.5.3/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-12 13:26:08.464169 flashcam-1.5.3/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      830 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-12 13:26:08.000000 flashcam-1.5.3/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-12 13:26:08.468169 flashcam-1.5.3/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-18 08:31:29.000000 flashcam-1.5.3/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-13 20:59:03.689931 flashcam-1.5.4/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      569 2023-07-13 20:58:58.000000 flashcam-1.5.4/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.685931 flashcam-1.5.4/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    24865 2023-07-13 20:59:00.000000 flashcam-1.5.4/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      311 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      551 2023-04-17 20:01:01.000000 flashcam-1.5.4/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5255 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8106 2023-07-13 20:56:38.000000 flashcam-1.5.4/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4178 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40421 2023-07-11 20:11:58.000000 flashcam-1.5.4/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    35953 2023-04-28 18:56:55.000000 flashcam-1.5.4/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   102717 2023-07-13 20:54:51.000000 flashcam-1.5.4/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11302 2023-04-17 20:01:01.000000 flashcam-1.5.4/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    27692 2023-07-11 20:09:40.000000 flashcam-1.5.4/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30433 2023-07-13 20:52:49.000000 flashcam-1.5.4/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-07-13 20:59:03.689931 flashcam-1.5.4/flashcam.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      850 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      820 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      157 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2023-07-13 20:59:03.000000 flashcam-1.5.4/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-07-13 20:59:03.689931 flashcam-1.5.4/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2008 2023-04-17 20:44:28.000000 flashcam-1.5.4/setup.py
```

### Comparing `flashcam-1.5.3/PKG-INFO` & `flashcam-1.5.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.3
+Version: 1.5.4
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project flashcam
 ================
 
 `FLASk supported webCAM`
 
@@ -33,7 +34,9 @@
 
 Usage
 =====
 
 See README.howto.org
 
 Or run with *-h*
+
+
```

### Comparing `flashcam-1.5.3/README.md` & `flashcam-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/bin/flashcam` & `flashcam-1.5.4/bin/flashcam`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
     main_defaults["kompress"] = 95
     main_defaults["save"] = False,  # for UNI
     main_defaults["qpassfile"] = "~/.pycamfw_userpass"
     main_defaults["otate"] = False # for UNI, also for CONFIG, also for show
     main_defaults["x"] = 0
     main_defaults["y"] = 0
     main_defaults["debug"]=False
-    main_defaults["vof"]="101,2"
+    main_defaults["vof"]="101,-1" # negative means uni will not display
     main_defaults["zoom"]=1
 
     main_defaults["XY"]="1x1"
 
     # ACTUALS - get from commandline
     main_actual={}
     main_actual["product"]=product
```

### Comparing `flashcam-1.5.3/bin/flashcamg` & `flashcam-1.5.4/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/base_camera2.py` & `flashcam-1.5.4/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/config.py` & `flashcam-1.5.4/flashcam/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
           'qpassfile':"~/.pycamfw_userpass",
 
           'otate':0, # rotate 0
           'x':0,
           'y':0,
           # debug
-          'vof':110, # field of view 110 degrees default (uniwrec only)
+          'vof':(110,-1), # field of view 110 degrees default (uniwrec only) and measured distance
           'zoom':1,
 
           'XY':'1x1',  # position (uppercase)
 
           'user':'aaa',
           'password':'aaa',
           'port':5000,
```

### Comparing `flashcam-1.5.3/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.5.4/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.5.4/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/DET_NRDY.jpg` & `flashcam-1.5.4/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/DET_RDY_.jpg` & `flashcam-1.5.4/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/digital-7.mono.ttf` & `flashcam-1.5.4/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/monoskop.jpg` & `flashcam-1.5.4/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/win_rain.jpg` & `flashcam-1.5.4/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/win_skull.jpg` & `flashcam-1.5.4/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/win_storm.jpg` & `flashcam-1.5.4/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/win_winter.jpg` & `flashcam-1.5.4/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/data/windows.jpg` & `flashcam-1.5.4/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/direct.py` & `flashcam-1.5.4/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/izmq_receiver.py` & `flashcam-1.5.4/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/mmapwr.py` & `flashcam-1.5.4/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/real_camera.py` & `flashcam-1.5.4/flashcam/real_camera.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/stream_enhancer.py` & `flashcam-1.5.4/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/uniwrec.py` & `flashcam-1.5.4/flashcam/uniwrec.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 
         # measurements (distance)
         measure = 0  # 1.7
 
         if str(vof).find(",") > 0:
             vof = str(vof).strip("(")
             vof = str(vof).strip(")")
-            measure_fov, measure = (float(vof.split(",")[0]),) # ??? BUG?
+            measure_fov, measure  = (float(vof.split(",")[0]), float(vof.split(",")[1]) ) # ??? BUG?
             print("D... measure == ", measure )
             float(vof.split(",")[1])
         else:
             measure_fov = float(vof)  # config.CONFIG['vof'] #
 
         cross = None
         greencross = False  # just tell if on/off
```

### Comparing `flashcam-1.5.3/flashcam/usbcheck.py` & `flashcam-1.5.4/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/v4lc.py` & `flashcam-1.5.4/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam/web.py` & `flashcam-1.5.4/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/flashcam.egg-info/PKG-INFO` & `flashcam-1.5.4/flashcam.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.5.3
+Version: 1.5.4
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project flashcam
 ================
 
 `FLASk supported webCAM`
 
@@ -33,7 +34,9 @@
 
 Usage
 =====
 
 See README.howto.org
 
 Or run with *-h*
+
+
```

### Comparing `flashcam-1.5.3/flashcam.egg-info/SOURCES.txt` & `flashcam-1.5.4/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.5.3/setup.py` & `flashcam-1.5.4/setup.py`

 * *Files identical despite different names*

