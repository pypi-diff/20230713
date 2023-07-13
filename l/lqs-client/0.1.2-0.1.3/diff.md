# Comparing `tmp/lqs-client-0.1.2.tar.gz` & `tmp/lqs-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqs-client-0.1.2.tar", last modified: Thu Jun 22 18:57:17 2023, max compression
+gzip compressed data, was "lqs-client-0.1.3.tar", last modified: Thu Jul 13 16:54:00 2023, max compression
```

## Comparing `lqs-client-0.1.2.tar` & `lqs-client-0.1.3.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.256765 lqs-client-0.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2022-12-19 19:59:13.000000 lqs-client-0.1.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2023-06-22 18:57:17.256765 lqs-client-0.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3946 2023-03-31 19:13:53.000000 lqs-client-0.1.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.232766 lqs-client-0.1.2/lqs_client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5721 2023-04-25 20:40:06.000000 lqs-client-0.1.2/lqs_client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.1.2/lqs_client/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.232766 lqs-client-0.1.2/lqs_client/definitions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-19 19:48:58.000000 lqs-client-0.1.2/lqs_client/definitions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.232766 lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2022-12-20 19:36:05.000000 lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1626 2022-12-20 19:36:05.000000 lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2022-12-20 19:36:05.000000 lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/diagnostic_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.232766 lqs-client-0.1.2/lqs_client/definitions/diagnostic_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2022-12-20 19:36:25.000000 lqs-client-0.1.2/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      426 2022-12-20 19:36:25.000000 lqs-client-0.1.2/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2022-12-20 19:36:25.000000 lqs-client-0.1.2/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.240765 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Accel.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Point.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      367 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Point32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       98 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Pose.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      868 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      122 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      118 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Transform.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Twist.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      382 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      103 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      117 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2022-12-20 19:36:28.000000 lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.240765 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2022-12-20 19:36:31.000000 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/GridCells.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2022-12-20 19:36:31.000000 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-12-20 19:36:31.000000 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      385 2022-12-20 19:36:31.000000 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/Odometry.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2022-12-20 19:36:31.000000 lqs-client-0.1.2/lqs_client/definitions/nav_msgs/msg/Path.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.240765 lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      184 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      722 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.244765 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6284 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1008 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      640 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      986 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1362 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Image.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1206 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Imu.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/JointState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Joy.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1519 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1685 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1596 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      753 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      425 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/PointField.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Range.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      618 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      331 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-20 19:36:33.000000 lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.244765 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      196 2022-12-20 19:36:36.000000 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/Mesh.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-12-20 19:36:36.000000 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2022-12-20 19:36:36.000000 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/Plane.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2022-12-20 19:36:36.000000 lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/std_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.248765 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Bool.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Byte.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Char.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Duration.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Empty.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Float32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Float64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      551 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Header.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int16.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int8.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      911 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/String.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Time.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt16.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt32.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt64.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt8.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2022-11-28 20:46:11.000000 lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/stereo_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.248765 lqs-client-0.1.2/lqs_client/definitions/stereo_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-12-20 19:36:39.000000 lqs-client-0.1.2/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.252766 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2022-12-20 19:36:42.000000 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      337 2022-12-20 19:36:42.000000 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      476 2022-12-20 19:36:42.000000 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2022-12-20 19:36:42.000000 lqs-client-0.1.2/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.228765 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.252766 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      827 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      808 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2586 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1256 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1935 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/Marker.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1586 2022-12-20 19:36:44.000000 lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.252766 lqs-client-0.1.2/lqs_client/gen/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9365 2023-04-26 13:56:12.000000 lqs-client-0.1.2/lqs_client/gen/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.256765 lqs-client-0.1.2/lqs_client/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      239 2023-04-11 20:07:37.000000 lqs-client-0.1.2/lqs_client/interface/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8696 2023-06-05 19:22:37.000000 lqs-client-0.1.2/lqs_client/interface/ark_deserialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2023-03-31 19:14:09.000000 lqs-client-0.1.2/lqs_client/interface/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6158 2023-06-22 18:52:49.000000 lqs-client-0.1.2/lqs_client/interface/creator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.1.2/lqs_client/interface/deleter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9312 2023-05-19 14:25:06.000000 lqs-client-0.1.2/lqs_client/interface/fs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.1.2/lqs_client/interface/getter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11610 2023-05-19 14:25:06.000000 lqs-client-0.1.2/lqs_client/interface/input_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18199 2023-06-08 16:18:38.000000 lqs-client-0.1.2/lqs_client/interface/lister.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16489 2023-06-05 19:22:37.000000 lqs-client-0.1.2/lqs_client/interface/message_converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6849 2023-05-09 21:11:30.000000 lqs-client-0.1.2/lqs_client/interface/node.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18266 2023-06-22 18:55:55.000000 lqs-client-0.1.2/lqs_client/interface/ros_deserialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27304 2023-05-19 14:25:06.000000 lqs-client-0.1.2/lqs_client/interface/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15734 2023-04-24 20:09:51.000000 lqs-client-0.1.2/lqs_client/interface/terminal.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.1.2/lqs_client/interface/updater.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15935 2023-06-12 14:47:41.000000 lqs-client-0.1.2/lqs_client/interface/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 18:57:17.232766 lqs-client-0.1.2/lqs_client.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4445 2023-06-22 18:57:17.000000 lqs-client-0.1.2/lqs_client.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7647 2023-06-22 18:57:17.000000 lqs-client-0.1.2/lqs_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-22 18:57:17.000000 lqs-client-0.1.2/lqs_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-06-22 18:57:17.000000 lqs-client-0.1.2/lqs_client.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-22 18:57:17.000000 lqs-client-0.1.2/lqs_client.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.1.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-22 18:57:17.256765 lqs-client-0.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1261 2023-06-22 18:55:36.000000 lqs-client-0.1.2/setup.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.695423 lqs-client-0.1.3/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       42 2023-05-10 21:11:32.000000 lqs-client-0.1.3/MANIFEST.in
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 16:54:00.695423 lqs-client-0.1.3/PKG-INFO
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     3946 2023-05-10 21:11:32.000000 lqs-client-0.1.3/README.md
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.635423 lqs-client-0.1.3/lqs_client/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5721 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/__init__.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      247 2023-05-16 20:59:43.000000 lqs-client-0.1.3/lqs_client/__main__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/__init__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      334 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalID.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1626 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      127 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatusArray.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      180 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      426 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/DiagnosticStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       93 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/diagnostic_msgs/msg/KeyValue.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.651423 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Accel.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/AccelWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      235 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Inertia.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       30 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/InertiaStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       84 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Point.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      367 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Point32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       98 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PointStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      107 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Polygon.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      104 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PolygonStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      119 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      868 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       79 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      323 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      122 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/PoseWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      108 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Quaternion.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/QuaternionStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      118 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Transform.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TransformStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      115 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Twist.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       82 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      326 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistWithCovariance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      124 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/TwistWithCovarianceStamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      382 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Vector3.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      103 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Vector3Stamped.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      117 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Wrench.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       85 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/WrenchStamped.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.627423 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.655423 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      113 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/GridCells.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      374 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/MapMetaData.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      291 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/OccupancyGrid.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      385 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/Odometry.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      112 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/nav_msgs/msg/Path.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.655423 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      184 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/Clock.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      457 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/Log.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      722 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.667423 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2596 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6284 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1008 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      640 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      517 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      986 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1362 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Image.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1206 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Imu.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      995 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JointState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      286 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Joy.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      413 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JoyFeedback.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       83 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JoyFeedbackArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      238 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserEcho.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1519 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1150 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1151 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1685 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1596 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      753 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      553 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1039 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      425 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointField.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2027 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Range.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      872 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      618 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      331 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Temperature.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      321 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/TimeReference.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.671423 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      196 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/Mesh.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       63 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/MeshTriangle.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      153 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/Plane.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1138 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/std_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Bool.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Byte.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/ByteMultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        9 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Char.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       40 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/ColorRGBA.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       14 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Duration.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Empty.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Float64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      551 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Header.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int16.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int16MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int8.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Int8MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      141 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayDimension.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      911 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/String.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       10 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Time.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       12 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt16.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt16MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt32.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt32MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt64.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt64MultiArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt8.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      210 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/UInt8MultiArray.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1137 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.683423 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       65 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/JointTrajectory.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      337 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/JointTrajectoryPoint.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      476 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectory.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      330 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/trajectory_msgs/msg/MultiDOFJointTrajectoryPoint.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.631423 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.687423 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      827 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      808 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2586 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1256 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      475 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerInit.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      228 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerPose.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      950 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1935 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/Marker.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       17 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MarkerArray.msg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1586 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.687423 lqs-client-0.1.3/lqs_client/gen/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9365 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/gen/__init__.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.691423 lqs-client-0.1.3/lqs_client/interface/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      239 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/__init__.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     8658 2023-06-16 15:39:07.000000 lqs-client-0.1.3/lqs_client/interface/ark_deserialization.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     5572 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/common.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6158 2023-06-14 16:27:27.000000 lqs-client-0.1.3/lqs_client/interface/creator.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1817 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/deleter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     9312 2023-06-01 14:32:08.000000 lqs-client-0.1.3/lqs_client/interface/fs.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1959 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/getter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    11610 2023-05-16 17:09:57.000000 lqs-client-0.1.3/lqs_client/interface/input_stream.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18199 2023-06-05 20:40:55.000000 lqs-client-0.1.3/lqs_client/interface/lister.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    16489 2023-05-22 21:04:59.000000 lqs-client-0.1.3/lqs_client/interface/message_converter.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     6849 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/node.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    18266 2023-07-13 15:55:09.000000 lqs-client-0.1.3/lqs_client/interface/ros_deserialization.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    28686 2023-07-13 16:45:29.000000 lqs-client-0.1.3/lqs_client/interface/s3.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15734 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/terminal.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     2221 2023-05-10 21:11:32.000000 lqs-client-0.1.3/lqs_client/interface/updater.py
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)    15935 2023-07-13 15:57:22.000000 lqs-client-0.1.3/lqs_client/interface/utils.py
+drwxrwxr-x   0 amalmattyantony  (1001) amalmattyantony  (1002)        0 2023-07-13 16:54:00.639423 lqs-client-0.1.3/lqs_client.egg-info/
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     4445 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/PKG-INFO
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     7647 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)        1 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      181 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/requires.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       11 2023-07-13 16:54:00.000000 lqs-client-0.1.3/lqs_client.egg-info/top_level.txt
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)      206 2023-05-10 21:11:32.000000 lqs-client-0.1.3/pyproject.toml
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)       38 2023-07-13 16:54:00.695423 lqs-client-0.1.3/setup.cfg
+-rw-rw-r--   0 amalmattyantony  (1001) amalmattyantony  (1002)     1261 2023-07-13 16:47:33.000000 lqs-client-0.1.3/setup.py
```

### Comparing `lqs-client-0.1.2/PKG-INFO` & `lqs-client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.2/README.md` & `lqs-client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/__init__.py` & `lqs-client-0.1.3/lqs_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg` & `lqs-client-0.1.3/lqs_client/definitions/actionlib_msgs/msg/GoalStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg` & `lqs-client-0.1.3/lqs_client/definitions/geometry_msgs/msg/Pose2D.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg` & `lqs-client-0.1.3/lqs_client/definitions/rosgraph_msgs/msg/TopicStatistics.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/BatteryState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CameraInfo.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/ChannelFloat32.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/CompressedImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/FluidPressure.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Illuminance.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Image.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Image.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Imu.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Imu.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/JointState.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/JointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/LaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MagneticField.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiDOFJointState.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/MultiEchoLaserScan.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatFix.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/NavSatStatus.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/PointCloud2.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/Range.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/Range.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RegionOfInterest.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg` & `lqs-client-0.1.3/lqs_client/definitions/sensor_msgs/msg/RelativeHumidity.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg` & `lqs-client-0.1.3/lqs_client/definitions/shape_msgs/msg/SolidPrimitive.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/Header.msg` & `lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/Header.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg` & `lqs-client-0.1.3/lqs_client/definitions/std_msgs/msg/MultiArrayLayout.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg` & `lqs-client-0.1.3/lqs_client/definitions/stereo_msgs/msg/DisparityImage.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/ImageMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerControl.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerFeedback.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/InteractiveMarkerUpdate.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/Marker.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/Marker.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg` & `lqs-client-0.1.3/lqs_client/definitions/visualization_msgs/msg/MenuEntry.msg`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/gen/__init__.py` & `lqs-client-0.1.3/lqs_client/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/ark_deserialization.py` & `lqs-client-0.1.3/lqs_client/interface/ark_deserialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
             field_value = read_fn()
             # find size of field
             field_size = sys.getsizeof(field_value)
             if trim and field_size >= trim_size:
                 field_value = None
             res[field_name] = field_value
 
-        # import pdb; pdb.set_trace()
         while input_stream.has_more_sections:
             group_id, group_size = input_stream.read_optional_group_header()
             # check if we have a group with this id
             if group_id not in schema["groups"]:
                 input_stream.advance(group_size)
             else:
                 # process it
```

### Comparing `lqs-client-0.1.2/lqs_client/interface/common.py` & `lqs-client-0.1.3/lqs_client/interface/common.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/creator.py` & `lqs-client-0.1.3/lqs_client/interface/creator.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/deleter.py` & `lqs-client-0.1.3/lqs_client/interface/deleter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/fs.py` & `lqs-client-0.1.3/lqs_client/interface/fs.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/getter.py` & `lqs-client-0.1.3/lqs_client/interface/getter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/input_stream.py` & `lqs-client-0.1.3/lqs_client/interface/input_stream.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/lister.py` & `lqs-client-0.1.3/lqs_client/interface/lister.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/message_converter.py` & `lqs-client-0.1.3/lqs_client/interface/message_converter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/node.py` & `lqs-client-0.1.3/lqs_client/interface/node.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/ros_deserialization.py` & `lqs-client-0.1.3/lqs_client/interface/ros_deserialization.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/s3.py` & `lqs-client-0.1.3/lqs_client/interface/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from urllib.parse import unquote
 
 import lzma
 import zstd
 import lz4.block
 import bz2
 import struct
+import s3path
 
 from .fs import FileSystemManager
 
 
 class S3Method(str, Enum):
     abort_multipart_upload = "abort_multipart_upload"
     complete_multipart_upload = "complete_multipart_upload"
@@ -678,25 +679,41 @@
 
     def get_message_data_for_ark_record(
         self, record, s3_bucket=None, s3_key=None, ingestion_id=None
     ):
         if s3_bucket is None or s3_key is None:
             s3_bucket = record["s3_bucket"]
             s3_key = record["s3_key"]
+
             if s3_bucket is None or s3_key is None:
                 ingestion_id = record["ingestion_id"]
                 if ingestion_id is None:
                     raise ValueError("Missing ingestion_id and s3_bucket/s3_key")
                 ingestion = self._getter.ingestion(ingestion_id=ingestion_id)["data"]
                 s3_bucket = ingestion["s3_bucket"]
-                s3_key = ingestion["s3_key"]
+                if s3_key is None:
+                    s3_key = ingestion["s3_key"]
+        split_id = None
+        if record["context"]:
+            split_id = record["context"].get("split_id", None)
 
-        split_id = record["context"].get("split_id", None)
         if split_id:
             s3_key = self.get_split_s3_key(s3_key, split_id)
+        else:
+            assert record["s3_key"] is not None
+            relative_s3_key = record["s3_key"]
+            # get the manifest s3 key from the ingestion
+            ingestion_id = record["ingestion_id"]
+            ingestion = self._getter.ingestion(ingestion_id=ingestion_id)["data"]
+            s3_key = ingestion["s3_key"]
+            # combine the manifest s3 key with the relative s3 key
+            s3_key = self._get_split_s3_key_for_record(
+                manifest_s3_key=s3_key, relative_split_path=relative_s3_key,
+                s3_bucket=s3_bucket
+            )
 
         compression = record["chunk_compression"]
         chunk_start_offset = record["chunk_offset"]
         # the offset is inclusive, so we need to subtract 1
         chunk_end_offset = record["chunk_offset"] + record["chunk_length"] - 1
         bytes = self.fs.get_data(
             s3_bucket=s3_bucket,
@@ -757,7 +774,22 @@
                 raise Exception(f"Unsupported compression type {compression_type}")
         return decompressed_bytes
 
     def get_split_s3_key(self, manifest_s3_key: str, split_id: str) -> str:
         parent_path = manifest_s3_key.rsplit("/manifests", 1)[0]
         split_file_path = f"{parent_path}/splits/{split_id}"
         return self.fs.prepare_s3_key(split_file_path)
+
+    def _get_split_s3_key_for_record(
+        self, manifest_s3_key: str, relative_split_path: str, s3_bucket: str
+    ) -> str:
+        log_prefix = manifest_s3_key.rsplit("/manifests", 1)[0]
+        split_s3_key = s3path.PureS3Path.from_bucket_key(
+            bucket=s3_bucket, key=manifest_s3_key + "/" + relative_split_path
+        ).key
+        # if the split_s3_key doesn't start with the log_prefix, then something funky is going on
+        if not split_s3_key.startswith(log_prefix):
+            raise Exception(
+                f"Split s3 key {split_s3_key} does not start with log prefix {log_prefix}"
+            )
+
+        return self.fs.prepare_s3_key(split_s3_key)
```

### Comparing `lqs-client-0.1.2/lqs_client/interface/terminal.py` & `lqs-client-0.1.3/lqs_client/interface/terminal.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/updater.py` & `lqs-client-0.1.3/lqs_client/interface/updater.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client/interface/utils.py` & `lqs-client-0.1.3/lqs_client/interface/utils.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/lqs_client.egg-info/PKG-INFO` & `lqs-client-0.1.3/lqs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.1.2/lqs_client.egg-info/SOURCES.txt` & `lqs-client-0.1.3/lqs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lqs-client-0.1.2/setup.py` & `lqs-client-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqs-client",
-    version="0.1.2",
+    version="0.1.3",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="LogQS Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS-Client",
     project_urls={
```

