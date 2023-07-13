# Comparing `tmp/mocap-0.1.2.tar.gz` & `tmp/mocap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocap-0.1.2.tar", last modified: Thu Jul 13 03:40:27 2023, max compression
+gzip compressed data, was "mocap-0.1.3.tar", last modified: Thu Jul 13 07:27:01 2023, max compression
```

## Comparing `mocap-0.1.2.tar` & `mocap-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.790027 mocap-0.1.2/
--rw-rw-rw-   0        0        0       26 2023-07-11 02:53:40.000000 mocap-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      462 2023-07-13 03:40:27.790027 mocap-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-07-11 02:57:09.000000 mocap-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.790027 mocap-0.1.2/mocap/
--rw-rw-rw-   0        0        0      883 2023-07-11 06:23:44.000000 mocap-0.1.2/mocap/ArucoBot.py
--rw-rw-rw-   0        0        0     2408 2023-07-11 06:23:44.000000 mocap-0.1.2/mocap/ArucoDevice.py
--rw-rw-rw-   0        0        0    11825 2023-07-13 03:40:08.000000 mocap-0.1.2/mocap/ArucoHelper.py
--rw-rw-rw-   0        0        0      381 2023-07-11 06:27:23.000000 mocap-0.1.2/mocap/__init__.py
--rw-rw-rw-   0        0        0       73 2023-07-13 03:40:27.790027 mocap-0.1.2/mocap/_static_version.py
--rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 mocap-0.1.2/mocap/_version.py
--rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 mocap-0.1.2/mocap/calibration.yml
--rw-rw-rw-   0        0        0      218 2023-07-03 23:33:43.000000 mocap-0.1.2/mocap/run_test.py
--rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 mocap-0.1.2/mocap/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.789027 mocap-0.1.2/mocap.egg-info/
--rw-rw-rw-   0        0        0      462 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 23:26:58.000000 mocap-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 03:40:27.790027 mocap-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1748 2023-07-13 03:39:55.000000 mocap-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:27:01.124308 mocap-0.1.3/
+-rw-rw-rw-   0        0        0       26 2023-07-11 02:53:40.000000 mocap-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      462 2023-07-13 07:27:01.123308 mocap-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2023-07-11 02:57:09.000000 mocap-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 07:27:01.124308 mocap-0.1.3/mocap/
+-rw-rw-rw-   0        0        0      883 2023-07-11 06:23:44.000000 mocap-0.1.3/mocap/ArucoBot.py
+-rw-rw-rw-   0        0        0     2408 2023-07-11 06:23:44.000000 mocap-0.1.3/mocap/ArucoDevice.py
+-rw-rw-rw-   0        0        0    12267 2023-07-13 07:09:11.000000 mocap-0.1.3/mocap/ArucoHelper.py
+-rw-rw-rw-   0        0        0      413 2023-07-13 07:02:17.000000 mocap-0.1.3/mocap/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-07-13 07:27:01.124308 mocap-0.1.3/mocap/_static_version.py
+-rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 mocap-0.1.3/mocap/_version.py
+-rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 mocap-0.1.3/mocap/calibration.yml
+-rw-rw-rw-   0        0        0      459 2023-07-13 07:20:06.000000 mocap-0.1.3/mocap/run_test.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 mocap-0.1.3/mocap/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:27:01.123308 mocap-0.1.3/mocap.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-07-13 07:27:01.000000 mocap-0.1.3/mocap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-13 07:27:01.000000 mocap-0.1.3/mocap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:27:01.000000 mocap-0.1.3/mocap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-13 07:27:01.000000 mocap-0.1.3/mocap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 07:27:01.000000 mocap-0.1.3/mocap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 23:26:58.000000 mocap-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:27:01.124308 mocap-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1748 2023-07-13 07:26:17.000000 mocap-0.1.3/setup.py
```

### Comparing `mocap-0.1.2/mocap/ArucoBot.py` & `mocap-0.1.3/mocap/ArucoBot.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.2/mocap/ArucoDevice.py` & `mocap-0.1.3/mocap/ArucoDevice.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.2/mocap/ArucoHelper.py` & `mocap-0.1.3/mocap/ArucoHelper.py`

 * *Files 7% similar despite different names*

```diff
@@ -186,18 +186,25 @@
         return ret_frames
 
     @staticmethod
     def _rvec_2_euler(rvec):
         euler_rvec = R.from_rotvec(rvec).as_euler(ARUCO.EULER)
         return euler_rvec
 
-    def run(self, track_ids):
+    def run(self, track_ids, duration=-1):
         """run function is to test run the aruco tag detection standalone
         No need to use this in the simulation implementation"""
-        while True:
+        def is_time(duration, start_time):
+            if duration < 0: # indefinite run
+                return True
+            else:
+                return (time.perf_counter() - start_time) <= duration
+
+        start_time =time.perf_counter()
+        while is_time(duration, start_time):
             fs = self.get_frames(track_ids)
             print(fs)
             # Wait 3 milisecoonds for an interaction. Check the key and do the corresponding job.
             key = cv2.waitKey(int(1000/self.fps)) & 0xFF
             if key == ord('q'):  # Quit
                 break
         self.close()
@@ -258,14 +265,18 @@
 
         # note we also have to specify the type to retrieve otherwise we only get a
         # FileNode object back instead of a matrixR
         camera_matrix = cv_file.getNode("Camera").mat()
         dist_matrix = cv_file.getNode("Distortion").mat()
 
         cv_file.release()
+        if camera_matrix is None:
+            camera_matrix = np.eye(3)
+        if dist_matrix is None:
+            dist_matrix = np.zeros((1, 5))
         self.camera_matrix = camera_matrix
         self.distortion_matrix = dist_matrix
 
     def __del__(self):
         self.close()
 
     def close(self):
```

### Comparing `mocap-0.1.2/mocap/_version.py` & `mocap-0.1.3/mocap/_version.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.2/setup.py` & `mocap-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='mocap',
-    version='0.1.2',
+    version='0.1.3',
     cmdclass=cmdclass,
     description=get_metadata('description'),
     url=get_metadata("url"),
     project_urls={'GitHub': 'https://github.com/rems-ucla/mocap'},
     author=get_metadata('author'),
     license='LGPLv3',
     packages=find_packages(include=['mocap', 'mocap.*']),
```

