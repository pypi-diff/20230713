# Comparing `tmp/Presage Physiology Preprocessing-1.2.2.tar.gz` & `tmp/Presage Physiology Preprocessing-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Presage Physiology Preprocessing-1.2.2.tar", last modified: Tue Jul 11 16:39:31 2023, max compression
+gzip compressed data, was "Presage Physiology Preprocessing-1.2.3.tar", last modified: Thu Jul 13 16:20:21 2023, max compression
```

## Comparing `Presage Physiology Preprocessing-1.2.2.tar` & `Presage Physiology Preprocessing-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/
--rw-r--r--   0 root         (0) root         (0)     5759 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.207368 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5759 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-11 16:39:31.000000 Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/mediapipefunctions.py
--rw-rw-rw-   0 root         (0) root         (0)    18335 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 16:39:29.000000 Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/version.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-11 16:39:31.211368 Presage Physiology Preprocessing-1.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-11 16:37:28.000000 Presage Physiology Preprocessing-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:20:21.801452 Presage Physiology Preprocessing-1.2.3/
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-07-13 16:20:21.801452 Presage Physiology Preprocessing-1.2.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:20:21.801452 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5759 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-13 16:20:21.000000 Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-13 16:18:19.000000 Presage Physiology Preprocessing-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:20:21.801452 Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-13 16:18:19.000000 Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-13 16:18:19.000000 Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/mediapipefunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)    18344 2023-07-13 16:18:19.000000 Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-13 16:20:20.000000 Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-13 16:20:21.805452 Presage Physiology Preprocessing-1.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-13 16:18:19.000000 Presage Physiology Preprocessing-1.2.3/setup.py
```

### Comparing `Presage Physiology Preprocessing-1.2.2/PKG-INFO` & `Presage Physiology Preprocessing-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage Physiology Preprocessing
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python helper package used for preprocessing video before sending it to Presage Technologies Physiology API.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_physiology_preprocessing/issues
 Description: # presage_physiology_preprocessing
```

### Comparing `Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/PKG-INFO` & `Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Presage-Physiology-Preprocessing
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python helper package used for preprocessing video before sending it to Presage Technologies Physiology API.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_physiology_preprocessing/issues
 Description: # presage_physiology_preprocessing
```

### Comparing `Presage Physiology Preprocessing-1.2.2/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt` & `Presage Physiology Preprocessing-1.2.3/Presage_Physiology_Preprocessing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.2/README.md` & `Presage Physiology Preprocessing-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/mediapipefunctions.py` & `Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/mediapipefunctions.py`

 * *Files identical despite different names*

### Comparing `Presage Physiology Preprocessing-1.2.2/presage_physiology_preprocessing/preprocessing.py` & `Presage Physiology Preprocessing-1.2.3/presage_physiology_preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
     """
     rr_fps_ideal = 5
     mod_rr = frame_skipper(fps, rr_fps_ideal)
     # mod_rr = round(mod_rr / mod_hr)
     return mod_rr
 
 
-def video_preprocess(path, HR_FPS = 10, DN_SAMPLE = 1):
+def video_preprocess(path, HR_FPS=30, DN_SAMPLE=1):
     """
     Video_preprocess reads in a video from source (path) and subsequently processes each frame into a set of variables stored in traces
     - internally used parameter variables are stored in settings
     - traces a python dict which is then serialized into a json object and returned
      - traces can be post processed to extract absolute vital measurements
     """
 
@@ -374,15 +374,15 @@
         frame_index_last_rr = None
         # traces[frame_index_last] = None
         # traces[frame_index_last_rr] = None
         fake_time = 0.0
         for frame_index in range(0, vid_length):
             save_time = False
             if frame_index > 0:
-                fake_time+=1/fps_orig
+                fake_time += 1.0/fps_orig
             frame_data = {}
             ret, frame = cap.read()
             if not ret:
                 continue
             if not orientation_done:
                 vid_height, vid_width = frame.shape[:2]
 
@@ -412,19 +412,19 @@
                         print(f"Processing error in HR analysis at frame: {frame_index}, error: {e}")
                         pass
 
                 try:
                     # here we compute all metrics associated with RR analysis, tracked points of body
                     if frame_index % mod_amount_rr == 0:
                         if frame_last_rr is None and frame_index_last_rr is None:
-                            frame_data.update(process_frame_rr(frame, None, None))
+                            frame_data.update(process_frame_rr(dn_frame, None, None))
                         else:
-                            frame_data.update(process_frame_rr(frame, frame_last_rr, traces["frames"][frame_index_last_rr]))
+                            frame_data.update(process_frame_rr(dn_frame, frame_last_rr, traces["frames"][frame_index_last_rr]))
                         frame_index_last_rr = len(traces["frames"])
-                        frame_last_rr = frame
+                        frame_last_rr = dn_frame
 
                 except Exception as e:
                     print(f"Processing error in RR analysis at frame: {frame_index}, error: {e}")
                     pass
 
                 if save_time:
                     frame_data.update({'time_now': round(fake_time, 3)})
```

### Comparing `Presage Physiology Preprocessing-1.2.2/setup.py` & `Presage Physiology Preprocessing-1.2.3/setup.py`

 * *Files identical despite different names*

