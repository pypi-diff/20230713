# Comparing `tmp/lqs-client-0.1.3.tar.gz` & `tmp/lqs-client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqs-client-0.1.3.tar", last modified: Thu Jul 13 16:54:00 2023, max compression
+gzip compressed data, was "lqs-client-0.1.4.tar", last modified: Thu Jul 13 17:15:03 2023, max compression
```

## Comparing `lqs-client-0.1.3.tar` & `lqs-client-0.1.4.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.695423 lqs-client-0.1.3/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       42 2023-05-10 21:11:32.000000 lqs-client-0.1.3/MANIFEST.in
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 16:54:00.695423 lqs-client-0.1.3/PKG-INFO
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     3946 2023-05-10 21:11:32.000000 lqs-client-0.1.3/README.md
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.635423 lqs-client-0.1.3/lqs_client/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5721 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/__init__.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      247 2023-05-16 20:59:43.000000 lqs-client-0.1.3/lqs_client/__main__.py
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/__init__.py
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      334 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1626 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      127 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      180 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      426 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       93 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.651423 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Accel.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      235 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       30 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       84 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Point.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      367 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Point32.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       98 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      107 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      104 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      868 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       79 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      323 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      122 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      108 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      118 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Transform.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      115 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Twist.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       82 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      326 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      382 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      103 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.655423 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      113 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/GridCells.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      374 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      291 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      385 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/Odometry.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      112 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/Path.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.655423 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      184 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      457 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      722 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.667423 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2596 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6284 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1008 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      640 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      517 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      986 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1362 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Image.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1206 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Imu.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      995 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JointState.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      286 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Joy.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      413 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      238 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1519 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1150 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1151 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1685 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1596 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      753 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      553 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1039 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      425 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointField.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2027 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Range.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      872 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      618 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      331 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      321 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.671423 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      196 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/Mesh.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       63 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      153 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/Plane.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1138 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/std_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Bool.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Byte.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Char.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       40 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       14 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Duration.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Empty.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float32.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float64.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      551 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Header.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int16.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int32.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int64.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int8.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      141 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      911 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/String.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Time.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt16.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt32.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt64.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt8.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1137 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       65 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      476 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.687423 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      827 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      808 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2586 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1256 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      475 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      228 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      950 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1935 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/Marker.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       17 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1586 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.687423 lqs-client-0.1.3/lqs_client/gen/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9365 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/gen/__init__.py
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.691423 lqs-client-0.1.3/lqs_client/interface/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      239 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/__init__.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     8658 2023-06-16 15:39:07.000000 lqs-client-0.1.3/lqs_client/interface/ark_deserialization.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5572 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/common.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6158 2023-06-14 16:27:27.000000 lqs-client-0.1.3/lqs_client/interface/creator.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1817 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/deleter.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9312 2023-06-01 14:32:08.000000 lqs-client-0.1.3/lqs_client/interface/fs.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1959 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/getter.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    11610 2023-05-16 17:09:57.000000 lqs-client-0.1.3/lqs_client/interface/input_stream.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18199 2023-06-05 20:40:55.000000 lqs-client-0.1.3/lqs_client/interface/lister.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    16489 2023-05-22 21:04:59.000000 lqs-client-0.1.3/lqs_client/interface/message_converter.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6849 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/node.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18266 2023-07-13 15:55:09.000000 lqs-client-0.1.3/lqs_client/interface/ros_deserialization.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    28686 2023-07-13 16:45:29.000000 lqs-client-0.1.3/lqs_client/interface/s3.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15734 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/terminal.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2221 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/updater.py
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15935 2023-07-13 15:57:22.000000 lqs-client-0.1.3/lqs_client/interface/utils.py
-drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client.egg-info/
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/PKG-INFO
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     7647 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/SOURCES.txt
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        1 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/dependency_links.txt
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      181 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/requires.txt
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/top_level.txt
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      206 2023-05-10 21:11:32.000000 lqs-client-0.1.3/pyproject.toml
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       38 2023-07-13 16:54:00.695423 lqs-client-0.1.3/setup.cfg
--rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1261 2023-07-13 16:47:33.000000 lqs-client-0.1.3/setup.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.274748 lqs-client-0.1.4/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       42 2023-05-10 21:11:32.000000 lqs-client-0.1.4/MANIFEST.in
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 17:15:03.274748 lqs-client-0.1.4/PKG-INFO
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     3946 2023-05-10 21:11:32.000000 lqs-client-0.1.4/README.md
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.234748 lqs-client-0.1.4/lqs_client/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5721 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/__init__.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      247 2023-05-16 20:59:43.000000 lqs-client-0.1.4/lqs_client/__main__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.238748 lqs-client-0.1.4/lqs_client/definitions/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/__init__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.238748 lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      334 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1626 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      127 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/diagnostic_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.238748 lqs-client-0.1.4/lqs_client/definitions/diagnostic_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      180 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      426 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       93 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.246748 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Accel.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      235 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       30 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       84 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Point.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      367 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Point32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       98 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      107 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      104 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Pose.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      868 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       79 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      323 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      122 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      108 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      118 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Transform.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      115 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Twist.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       82 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      326 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      382 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      103 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.246748 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      113 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/GridCells.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      374 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      291 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      385 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/Odometry.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      112 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/nav_msgs/msg/Path.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.250748 lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      184 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      457 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      722 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.254748 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2596 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6284 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1008 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      640 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      517 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      986 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1362 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Image.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1206 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Imu.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      995 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/JointState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      286 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Joy.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      413 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      238 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1519 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1150 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1151 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1685 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1596 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      753 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      553 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1039 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      425 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/PointField.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2027 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Range.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      872 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      618 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      331 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      321 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.254748 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      196 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/Mesh.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       63 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      153 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/Plane.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1138 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/std_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.266749 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Bool.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Byte.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Char.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       40 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       14 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Duration.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Empty.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Float32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Float64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      551 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Header.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int16.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int8.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      141 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      911 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/String.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Time.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt16.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt8.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/stereo_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.266749 lqs-client-0.1.4/lqs_client/definitions/stereo_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1137 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.230748 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.266749 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       65 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      476 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.234748 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.270748 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      827 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      808 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2586 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1256 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      475 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      228 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      950 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1935 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/Marker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       17 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1586 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.270748 lqs-client-0.1.4/lqs_client/gen/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9365 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/gen/__init__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.274748 lqs-client-0.1.4/lqs_client/interface/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      239 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/__init__.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     8658 2023-06-16 15:39:07.000000 lqs-client-0.1.4/lqs_client/interface/ark_deserialization.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5572 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/common.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6158 2023-06-14 16:27:27.000000 lqs-client-0.1.4/lqs_client/interface/creator.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1817 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/deleter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9312 2023-06-01 14:32:08.000000 lqs-client-0.1.4/lqs_client/interface/fs.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1959 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/getter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    11610 2023-05-16 17:09:57.000000 lqs-client-0.1.4/lqs_client/interface/input_stream.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18199 2023-06-05 20:40:55.000000 lqs-client-0.1.4/lqs_client/interface/lister.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    16489 2023-05-22 21:04:59.000000 lqs-client-0.1.4/lqs_client/interface/message_converter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6849 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/node.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18266 2023-07-13 15:55:09.000000 lqs-client-0.1.4/lqs_client/interface/ros_deserialization.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    28686 2023-07-13 16:45:29.000000 lqs-client-0.1.4/lqs_client/interface/s3.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15734 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/terminal.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2221 2023-05-10 21:11:32.000000 lqs-client-0.1.4/lqs_client/interface/updater.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15935 2023-07-13 15:57:22.000000 lqs-client-0.1.4/lqs_client/interface/utils.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 17:15:03.234748 lqs-client-0.1.4/lqs_client.egg-info/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 17:15:03.000000 lqs-client-0.1.4/lqs_client.egg-info/PKG-INFO
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     7647 2023-07-13 17:15:03.000000 lqs-client-0.1.4/lqs_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        1 2023-07-13 17:15:03.000000 lqs-client-0.1.4/lqs_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      195 2023-07-13 17:15:03.000000 lqs-client-0.1.4/lqs_client.egg-info/requires.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-07-13 17:15:03.000000 lqs-client-0.1.4/lqs_client.egg-info/top_level.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      206 2023-05-10 21:11:32.000000 lqs-client-0.1.4/pyproject.toml
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       38 2023-07-13 17:15:03.274748 lqs-client-0.1.4/setup.cfg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1285 2023-07-13 17:10:19.000000 lqs-client-0.1.4/setup.py
```

### Comparing `lqs-client-0.1.3/PKG-INFO` & `lqs-client-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.3/README.md` & `lqs-client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/__init__.py` & `lqs-client-0.1.4/lqs_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg` & `lqs-client-0.1.4/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg` & `lqs-client-0.1.4/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg` & `lqs-client-0.1.4/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Image.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Image.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Imu.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Imu.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JointState.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/JointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Range.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/Range.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg` & `lqs-client-0.1.4/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg` & `lqs-client-0.1.4/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Header.msg` & `lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/Header.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg` & `lqs-client-0.1.4/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg` & `lqs-client-0.1.4/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/Marker.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/Marker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg` & `lqs-client-0.1.4/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/gen/__init__.py` & `lqs-client-0.1.4/lqs_client/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/ark_deserialization.py` & `lqs-client-0.1.4/lqs_client/interface/ark_deserialization.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/common.py` & `lqs-client-0.1.4/lqs_client/interface/common.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/creator.py` & `lqs-client-0.1.4/lqs_client/interface/creator.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/deleter.py` & `lqs-client-0.1.4/lqs_client/interface/deleter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/fs.py` & `lqs-client-0.1.4/lqs_client/interface/fs.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/getter.py` & `lqs-client-0.1.4/lqs_client/interface/getter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/input_stream.py` & `lqs-client-0.1.4/lqs_client/interface/input_stream.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/lister.py` & `lqs-client-0.1.4/lqs_client/interface/lister.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/message_converter.py` & `lqs-client-0.1.4/lqs_client/interface/message_converter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/node.py` & `lqs-client-0.1.4/lqs_client/interface/node.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/ros_deserialization.py` & `lqs-client-0.1.4/lqs_client/interface/ros_deserialization.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/s3.py` & `lqs-client-0.1.4/lqs_client/interface/s3.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/terminal.py` & `lqs-client-0.1.4/lqs_client/interface/terminal.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/updater.py` & `lqs-client-0.1.4/lqs_client/interface/updater.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client/interface/utils.py` & `lqs-client-0.1.4/lqs_client/interface/utils.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/lqs_client.egg-info/PKG-INFO` & `lqs-client-0.1.4/lqs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.3/lqs_client.egg-info/SOURCES.txt` & `lqs-client-0.1.4/lqs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.3/setup.py` & `lqs-client-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqs-client",
-    version="0.1.3",
+    version="0.1.4",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="LogQS Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS-Client",
     project_urls={
@@ -38,9 +38,10 @@
         "tqdm==4.*",
         "boto3==1.26.*",
         "Pillow==9.0.*",
         "numpy==1.22.*",
         "av==9.2.*",
         "lz4==4.0.*",
         "zstd==1.5.*",
+        "s3path==0.4.*"
     ],
 )
```

