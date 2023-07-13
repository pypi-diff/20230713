# Comparing `tmp/mocap-0.1.1.tar.gz` & `tmp/mocap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocap-0.1.1.tar", last modified: Wed Jul 12 19:56:59 2023, max compression
+gzip compressed data, was "mocap-0.1.2.tar", last modified: Thu Jul 13 03:40:27 2023, max compression
```

## Comparing `mocap-0.1.1.tar` & `mocap-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:56:59.114475 mocap-0.1.1/
--rw-rw-rw-   0        0        0       26 2023-07-11 02:53:40.000000 mocap-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      462 2023-07-12 19:56:59.113475 mocap-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      137 2023-07-11 02:57:09.000000 mocap-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 19:56:59.114475 mocap-0.1.1/mocap/
--rw-rw-rw-   0        0        0      883 2023-07-11 06:23:44.000000 mocap-0.1.1/mocap/ArucoBot.py
--rw-rw-rw-   0        0        0     2408 2023-07-11 06:23:44.000000 mocap-0.1.1/mocap/ArucoDevice.py
--rw-rw-rw-   0        0        0    11863 2023-07-12 02:14:54.000000 mocap-0.1.1/mocap/ArucoHelper.py
--rw-rw-rw-   0        0        0      381 2023-07-11 06:27:23.000000 mocap-0.1.1/mocap/__init__.py
--rw-rw-rw-   0        0        0       79 2023-07-12 19:56:59.114475 mocap-0.1.1/mocap/_static_version.py
--rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 mocap-0.1.1/mocap/_version.py
--rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 mocap-0.1.1/mocap/calibration.yml
--rw-rw-rw-   0        0        0      218 2023-07-03 23:33:43.000000 mocap-0.1.1/mocap/run_test.py
--rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 mocap-0.1.1/mocap/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:56:59.113475 mocap-0.1.1/mocap.egg-info/
--rw-rw-rw-   0        0        0      462 2023-07-12 19:56:59.000000 mocap-0.1.1/mocap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-12 19:56:59.000000 mocap-0.1.1/mocap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:56:59.000000 mocap-0.1.1/mocap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-12 19:56:59.000000 mocap-0.1.1/mocap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 19:56:59.000000 mocap-0.1.1/mocap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 23:26:58.000000 mocap-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 19:56:59.114475 mocap-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1748 2023-07-12 19:56:56.000000 mocap-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.790027 mocap-0.1.2/
+-rw-rw-rw-   0        0        0       26 2023-07-11 02:53:40.000000 mocap-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      462 2023-07-13 03:40:27.790027 mocap-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2023-07-11 02:57:09.000000 mocap-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.790027 mocap-0.1.2/mocap/
+-rw-rw-rw-   0        0        0      883 2023-07-11 06:23:44.000000 mocap-0.1.2/mocap/ArucoBot.py
+-rw-rw-rw-   0        0        0     2408 2023-07-11 06:23:44.000000 mocap-0.1.2/mocap/ArucoDevice.py
+-rw-rw-rw-   0        0        0    11825 2023-07-13 03:40:08.000000 mocap-0.1.2/mocap/ArucoHelper.py
+-rw-rw-rw-   0        0        0      381 2023-07-11 06:27:23.000000 mocap-0.1.2/mocap/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-07-13 03:40:27.790027 mocap-0.1.2/mocap/_static_version.py
+-rw-rw-rw-   0        0        0     6071 2023-07-03 04:13:13.000000 mocap-0.1.2/mocap/_version.py
+-rw-rw-rw-   0        0        0      425 2023-07-03 02:24:52.000000 mocap-0.1.2/mocap/calibration.yml
+-rw-rw-rw-   0        0        0      218 2023-07-03 23:33:43.000000 mocap-0.1.2/mocap/run_test.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 02:24:52.000000 mocap-0.1.2/mocap/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-07-13 03:40:27.789027 mocap-0.1.2/mocap.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-13 03:40:27.000000 mocap-0.1.2/mocap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 23:26:58.000000 mocap-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 03:40:27.790027 mocap-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1748 2023-07-13 03:39:55.000000 mocap-0.1.2/setup.py
```

### Comparing `mocap-0.1.1/mocap/ArucoBot.py` & `mocap-0.1.2/mocap/ArucoBot.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.1/mocap/ArucoDevice.py` & `mocap-0.1.2/mocap/ArucoDevice.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.1/mocap/ArucoHelper.py` & `mocap-0.1.2/mocap/ArucoHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.camera_id = camera_id
         self.frames = {}   # tracking ids and respective frames
         if env is None:
             env = ENV()
         self.arena_corner = np.array([[0.0, 0.0], [env.WIDTH, 0.0], [0.0, env.LENGTH], [env.WIDTH, env.LENGTH]], np.float32) * 1000
         self.arena_corner_actual =  np.array([[0.0, 0.0], [env.WIDTH, 0.0], [0.0, env.LENGTH], [env.WIDTH, env.LENGTH]], np.float32) * 1000
         self.arena_origin_offset =[-env.WIDTH/2,-env.LENGTH/2,0,0,0,0] #World origin to World tag
-        print(env.WIDTH, env.LENGTH)
         #calibration setting
         self.criteria = (cv2.TERM_CRITERIA_EPS + cv2.TERM_CRITERIA_MAX_ITER, 30, 0.001)
         self.t = 0.0
 
     def get_camera(self):
 
         self.camera = cv2.VideoCapture(self.camera_id)
```

### Comparing `mocap-0.1.1/mocap/_version.py` & `mocap-0.1.2/mocap/_version.py`

 * *Files identical despite different names*

### Comparing `mocap-0.1.1/setup.py` & `mocap-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='mocap',
-    version='0.1.1',
+    version='0.1.2',
     cmdclass=cmdclass,
     description=get_metadata('description'),
     url=get_metadata("url"),
     project_urls={'GitHub': 'https://github.com/rems-ucla/mocap'},
     author=get_metadata('author'),
     license='LGPLv3',
     packages=find_packages(include=['mocap', 'mocap.*']),
```

