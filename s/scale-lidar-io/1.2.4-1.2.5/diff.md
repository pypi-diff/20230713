# Comparing `tmp/scale_lidar_io-1.2.4.tar.gz` & `tmp/scale_lidar_io-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scale_lidar_io-1.2.4.tar", last modified: Wed Jun  7 14:51:10 2023, max compression
+gzip compressed data, was "scale_lidar_io-1.2.5.tar", last modified: Thu Jul 13 15:34:10 2023, max compression
```

## Comparing `scale_lidar_io-1.2.4.tar` & `scale_lidar_io-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/LICENSE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.369967 scale_lidar_io-1.2.4/scale_lidar_io/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16749 2023-06-07 14:49:18.000000 scale_lidar_io-1.2.4/scale_lidar_io/camera.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1710 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/color_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3136 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/connectors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20267 2023-06-07 14:49:18.000000 scale_lidar_io-1.2.4/scale_lidar_io/frame.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-06-07 14:49:11.000000 scale_lidar_io-1.2.4/scale_lidar_io/helper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3482 2023-06-07 14:49:11.000000 scale_lidar_io-1.2.4/scale_lidar_io/image.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1406 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/interpolate_transforms.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8290 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/lidar_frame_1_pb2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14947 2023-03-02 20:24:08.000000 scale_lidar_io-1.2.4/scale_lidar_io/nucleus_scene.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/protobuf_helper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12220 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/scene.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9439 2023-06-07 14:49:15.000000 scale_lidar_io-1.2.4/scale_lidar_io/task.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7879 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/scale_lidar_io/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      443 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-07 14:51:10.000000 scale_lidar_io-1.2.4/scale_lidar_io.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1070 2023-06-07 14:50:52.000000 scale_lidar_io-1.2.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 14:51:10.373968 scale_lidar_io-1.2.4/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6270 2022-07-14 17:56:36.000000 scale_lidar_io-1.2.4/test/test_scale_lidar_io.py
+drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-07-13 15:34:10.460991 scale_lidar_io-1.2.5/
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)    11357 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/LICENSE.md
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)      443 2023-07-13 15:34:10.460815 scale_lidar_io-1.2.5/PKG-INFO
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)       30 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/README.md
+drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-07-13 15:34:10.459325 scale_lidar_io-1.2.5/scale_lidar_io/
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)      192 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/__init__.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)    16749 2023-07-13 15:29:37.000000 scale_lidar_io-1.2.5/scale_lidar_io/camera.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     1710 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/color_utils.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     3136 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/connectors.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)    20268 2023-07-13 15:29:37.000000 scale_lidar_io-1.2.5/scale_lidar_io/frame.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     2439 2023-07-13 15:33:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/helper.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     3482 2023-07-13 15:33:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/image.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     1406 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/interpolate_transforms.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     8290 2023-03-16 17:36:13.000000 scale_lidar_io-1.2.5/scale_lidar_io/lidar_frame_1_pb2.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)    14947 2023-03-16 17:36:13.000000 scale_lidar_io-1.2.5/scale_lidar_io/nucleus_scene.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     2723 2023-03-16 17:36:13.000000 scale_lidar_io-1.2.5/scale_lidar_io/protobuf_helper.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)    12220 2023-07-13 15:33:14.000000 scale_lidar_io-1.2.5/scale_lidar_io/scene.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     9439 2023-03-16 17:36:13.000000 scale_lidar_io-1.2.5/scale_lidar_io/task.py
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     7880 2023-04-19 16:10:37.000000 scale_lidar_io-1.2.5/scale_lidar_io/transform.py
+drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-07-13 15:34:10.460291 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)      443 2023-07-13 15:34:10.000000 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)      648 2023-07-13 15:34:10.000000 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)        1 2023-07-13 15:34:10.000000 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)      191 2023-07-13 15:34:10.000000 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/requires.txt
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)       15 2023-07-13 15:34:10.000000 scale_lidar_io-1.2.5/scale_lidar_io.egg-info/top_level.txt
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)       38 2023-07-13 15:34:10.461050 scale_lidar_io-1.2.5/setup.cfg
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     1070 2023-07-13 15:33:14.000000 scale_lidar_io-1.2.5/setup.py
+drwxr-xr-x   0 ivan.roumec   (503) staff       (20)        0 2023-07-13 15:34:10.460450 scale_lidar_io-1.2.5/test/
+-rw-r--r--   0 ivan.roumec   (503) staff       (20)     6270 2023-02-23 19:42:14.000000 scale_lidar_io-1.2.5/test/test_scale_lidar_io.py
```

### Comparing `scale_lidar_io-1.2.4/LICENSE.md` & `scale_lidar_io-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/camera.py` & `scale_lidar_io-1.2.5/scale_lidar_io/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     world2cam = Transform.from_euler([-90, 0, -90], degrees=True)
 
     def __init__(self, camera_id):
         self.id = camera_id
         self.pose = Transform(self.world2cam)
         self.world_poses = None
         self.K = np.eye(3, dtype=np.float32)
-        self.D = np.zeros(6, dtype=np.float32)
+        self.D = np.zeros(7, dtype=np.float32)
         self.model = "brown_conrady"
         self.scale_factor = 1
         self.skew = 0
 
     @property
     def position(self) -> np.ndarray:
         """Camera position
```

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/color_utils.py` & `scale_lidar_io-1.2.5/scale_lidar_io/color_utils.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/connectors.py` & `scale_lidar_io-1.2.5/scale_lidar_io/connectors.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/frame.py` & `scale_lidar_io-1.2.5/scale_lidar_io/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       - transform: Pose/ transform of this frame
     """
 
     def __init__(self, frame_id, cameras):
         self.id = frame_id
         self.cameras: pd.Series[Any, LidarCamera] = cameras
         self.images: pd.Series[Any, LidarImage] = pd.Series(dtype=object)
-        self.points: np.ndarray = np.zeros((0, 6), dtype=float)
+        self.points: np.ndarray = np.zeros((0, 5), dtype=float)
         self.radar_points: np.ndarray = np.zeros((0, 3), dtype=float)
         self.colors: np.ndarray = np.zeros((0, 3), dtype=float)
         self.transform = Transform()
 
     def get_image(self, camera_id) -> LidarImage:
         """Get image by camera_id or create one if it does not exist
 
@@ -144,14 +144,15 @@
                 [points, np.ones((points.shape[0], 1)) * intensity])
         if points.shape[1] == 4:
             if sensor_id != 0:
                 points = np.hstack(
                     [points, np.ones((points.shape[0], 1)) * sensor_id])
             else:
                 points = np.hstack([points, np.zeros((points.shape[0], 1))])
+
         if points.shape[1] == 5:
             if sensor_id != 0:
                 points = np.hstack(
                     [points, np.ones((points.shape[0], 1)) * sensor_id])
             else:
                 points = np.hstack([points, np.zeros((points.shape[0], 1))])
         if transform is not None:
```

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/helper.py` & `scale_lidar_io-1.2.5/scale_lidar_io/helper.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/image.py` & `scale_lidar_io-1.2.5/scale_lidar_io/image.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/interpolate_transforms.py` & `scale_lidar_io-1.2.5/scale_lidar_io/interpolate_transforms.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/lidar_frame_1_pb2.py` & `scale_lidar_io-1.2.5/scale_lidar_io/lidar_frame_1_pb2.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/nucleus_scene.py` & `scale_lidar_io-1.2.5/scale_lidar_io/nucleus_scene.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/protobuf_helper.py` & `scale_lidar_io-1.2.5/scale_lidar_io/protobuf_helper.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/scene.py` & `scale_lidar_io-1.2.5/scale_lidar_io/scene.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/task.py` & `scale_lidar_io-1.2.5/scale_lidar_io/task.py`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io/transform.py` & `scale_lidar_io-1.2.5/scale_lidar_io/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         :type degrees: boolean
         :returns: Transform created from euler angles
         :rtype: Transform
 
         """
         if degrees:
             angles = np.deg2rad(angles)
+
         return Transform(t3d.euler.euler2mat(*angles, axes=axes))
 
     @staticmethod
     def from_transformed_points(A, B):
         """Create a transform from two points
 
         :param A: Point A (x,y,z)
```

### Comparing `scale_lidar_io-1.2.4/scale_lidar_io.egg-info/SOURCES.txt` & `scale_lidar_io-1.2.5/scale_lidar_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scale_lidar_io-1.2.4/setup.py` & `scale_lidar_io-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scale_lidar_io",
-    version="1.2.4",
+    version="1.2.5",
     author="Scale AI",
     author_email="rodrigo.belfiore@scale.com, ivan.roumec@scale.com",
     description="Lidar data conversion helpers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scale_lidar_io"],
     install_requires=[
```

### Comparing `scale_lidar_io-1.2.4/test/test_scale_lidar_io.py` & `scale_lidar_io-1.2.5/test/test_scale_lidar_io.py`

 * *Files identical despite different names*

