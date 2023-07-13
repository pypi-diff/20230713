# Comparing `tmp/PyFlyt-0.7.3.tar.gz` & `tmp/PyFlyt-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.7.3.tar", last modified: Tue May 30 17:28:19 2023, max compression
+gzip compressed data, was "PyFlyt-0.7.4.tar", last modified: Thu Jul 13 14:58:39 2023, max compression
```

## Comparing `PyFlyt-0.7.3.tar` & `PyFlyt-0.7.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.349257 PyFlyt-0.7.3/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.7.3/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-05-30 17:28:19.349257 PyFlyt-0.7.3/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.337257 PyFlyt-0.7.3/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.7.3/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.337257 PyFlyt-0.7.3/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.7.3/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-12 15:29:31.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-04-27 19:26:46.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15799 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-12 15:30:45.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.7.3/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.7.3/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-01 18:23:35.000000 PyFlyt-0.7.3/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.7.3/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.341257 PyFlyt-0.7.3/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.7.3/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.7.3/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.7.3/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.7.3/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.337257 PyFlyt-0.7.3/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.345257 PyFlyt-0.7.3/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.7.3/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.337257 PyFlyt-0.7.3/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-05-30 17:28:19.000000 PyFlyt-0.7.3/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-30 17:28:19.000000 PyFlyt-0.7.3/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-30 17:28:19.000000 PyFlyt-0.7.3/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       49 2023-05-30 17:28:19.000000 PyFlyt-0.7.3/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-30 17:28:19.000000 PyFlyt-0.7.3/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1242 2023-05-30 17:28:05.000000 PyFlyt-0.7.3/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.7.3/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-30 17:28:19.349257 PyFlyt-0.7.3/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.7.3/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-30 17:28:19.349257 PyFlyt-0.7.3/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-12 23:01:51.000000 PyFlyt-0.7.3/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-05-29 18:32:17.000000 PyFlyt-0.7.3/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-11-23 13:24:51.000000 PyFlyt-0.7.4/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-01 18:16:37.000000 PyFlyt-0.7.4/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-06 19:51:22.000000 PyFlyt-0.7.4/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-12 20:44:00.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-05-12 19:45:35.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-12 20:30:07.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-12 22:54:11.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12141 2023-06-07 19:07:52.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-12 15:30:11.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-06-07 19:10:09.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-06-07 19:14:24.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-06-07 19:08:30.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-10 22:15:27.000000 PyFlyt-0.7.4/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-07 22:16:41.000000 PyFlyt-0.7.4/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2345 2023-07-13 14:58:06.000000 PyFlyt-0.7.4/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-12 21:08:07.000000 PyFlyt-0.7.4/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-08 22:30:13.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:01:10.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:01:10.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-13 17:50:38.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-12 15:34:33.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-05-29 18:39:28.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-08 01:12:26.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-18 14:26:29.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-06 11:28:39.000000 PyFlyt-0.7.4/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-26 21:57:19.000000 PyFlyt-0.7.4/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-11-23 13:24:51.000000 PyFlyt-0.7.4/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-24 22:55:32.000000 PyFlyt-0.7.4/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-23 13:24:51.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-12 22:15:04.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-12 22:19:56.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-10 23:51:03.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-08 21:54:50.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-12 22:15:09.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-12 22:17:02.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-11 08:07:00.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-11 08:07:00.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-02 23:10:49.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-12 14:42:21.000000 PyFlyt-0.7.4/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.319317 PyFlyt-0.7.4/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-07-13 14:58:39.000000 PyFlyt-0.7.4/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-07-13 14:58:39.000000 PyFlyt-0.7.4/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-13 14:58:39.000000 PyFlyt-0.7.4/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       49 2023-07-13 14:58:39.000000 PyFlyt-0.7.4/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-13 14:58:39.000000 PyFlyt-0.7.4/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1242 2023-07-13 14:58:23.000000 PyFlyt-0.7.4/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 19:14:33.000000 PyFlyt-0.7.4/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-01 19:59:08.000000 PyFlyt-0.7.4/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-13 14:58:39.323317 PyFlyt-0.7.4/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-12 23:01:51.000000 PyFlyt-0.7.4/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-05-29 18:32:17.000000 PyFlyt-0.7.4/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.7.3/LICENSE.txt` & `PyFlyt-0.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PKG-INFO` & `PyFlyt-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.3
+Version: 0.7.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/boosters.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,16 +126,21 @@
         )
         self.throttle = np.zeros((self.num_boosters,), dtype=np.float64)
         self.ignition_state = np.zeros((self.num_boosters,), dtype=bool)
 
     def get_states(self) -> np.ndarray:
         """Gets the current state of the components.
 
+        Returns a (a0, a1, ..., an, b0, b1, ... bn, c0, c1, ... cn) array where:
+        - (a0, a1, ..., an) represent the ignition state
+        - (b0, b1, ..., bn) represent the remaining fuel ratio
+        - (c0, c1, ..., cn) represent the current throttle state
+
         Returns:
-            np.ndarray:
+            np.ndarray: A (3 * num_boosters, ) array
         """
         return np.concatenate(
             [
                 self.ignition_state.flatten(),  # [n]
                 self.ratio_fuel_remaining.flatten(),  # [n]
                 self.throttle.flatten(),  # [n]
             ]
```

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/gimbals.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.rotation1 = np.array([np.eye(3)] * self.num_gimbals, dtype=np.float64)
         self.rotation2 = np.array([np.eye(3)] * self.num_gimbals, dtype=np.float64)
 
     def get_states(self) -> np.ndarray:
         """Gets the current state of the components.
 
         Returns:
-            np.ndarray:
+            np.ndarray: a (2 * num_gimbals, ) array where every pair of values represents the current state of the gimbal
         """
         return np.concatenate(
             [
                 self.gimbal_state.flatten(),  # [n, 2]
             ]
         )
```

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """Resets all lifting surfaces."""
         [surface.reset() for surface in self.surfaces]
 
     def get_states(self) -> np.ndarray:
         """Gets the current state of the components.
 
         Returns:
-            np.ndarray:
+            np.ndarray: a (num_surfaces, ) array representing the actuation state for each surface
         """
         return np.array([surface.actuation for surface in self.surfaces])
 
     def physics_update(self, cmd: np.ndarray):
         """Converts actuation commands into forces on the lifting surfaces.
 
         Args:
```

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/motors.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         """Reset the motors."""
         self.throttle = np.zeros((self.num_motors,))
 
     def get_states(self) -> np.ndarray:
         """Gets the current state of the components.
 
         Returns:
-            np.ndarray:
+            np.ndarray: an (num_motors, ) array for the current throttle level of each motor
         """
         return self.throttle.flatten()
 
     def state_update(self):
         """This does not need to be called for motors."""
         warnings.warn("`state_update` does not need to be called for motors.")
```

### Comparing `PyFlyt-0.7.3/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.7.4/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/aviary.py` & `PyFlyt-0.7.4/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.7.4/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.7.4/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.7.4/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/core/load_objs.py` & `PyFlyt-0.7.4/PyFlyt/core/load_objs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Convenience function to load an obj into the pybullet environment."""
 from __future__ import annotations
 
 import numpy as np
-
-from .aviary import Aviary
+from pybullet_utils import bullet_client
 
 
 def loadOBJ(
-    env: Aviary,
+    env: bullet_client.BulletClient,
     fileName: str = "null",
     visualId: int = -1,
     collisionId: int = -1,
     baseMass: float = 0.0,
     meshScale: list[float] | np.ndarray = [1.0, 1.0, 1.0],
     basePosition: list[float] | np.ndarray = [0.0, 0.0, 0.0],
     baseOrientation: list[float] | np.ndarray = [0.0, 0.0, 0.0],
@@ -44,15 +43,17 @@
 
     env.register_all_new_bodies()
 
     return body_id
 
 
 def obj_visual(
-    env: Aviary, fileName: str, meshScale: list[float] | np.ndarray = [1.0, 1.0, 1.0]
+    env: bullet_client.BulletClient,
+    fileName: str,
+    meshScale: list[float] | np.ndarray = [1.0, 1.0, 1.0],
 ):
     """Loads an object visual model.
 
     Args:
         env (Aviary): env
         fileName (str): fileName
         meshScale (list[float] | np.ndarray): meshScale
@@ -63,15 +64,17 @@
         rgbaColor=[1, 1, 1, 1],
         specularColor=[0.0, 0.0, 0.0],
         meshScale=meshScale,
     )
 
 
 def obj_collision(
-    env: Aviary, fileName: str, meshScale: list[float] | np.ndarray = [1.0, 1.0, 1.0]
+    env: bullet_client.BulletClient,
+    fileName: str,
+    meshScale: list[float] | np.ndarray = [1.0, 1.0, 1.0],
 ):
     """Loads an object collision model.
 
     Args:
         env (Aviary): env
         fileName (str): fileName
         meshScale (list[float] | np.ndarray): meshScale
```

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.7.4/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.7.4/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.7.4/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.7.4/PyFlyt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.3
+Version: 0.7.4
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.7.3/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.7.4/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/pyproject.toml` & `PyFlyt-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PyFlyt-0.7.3/readme.md` & `PyFlyt-0.7.4/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/tests/test_core.py` & `PyFlyt-0.7.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.3/tests/test_gym_envs.py` & `PyFlyt-0.7.4/tests/test_gym_envs.py`

 * *Files identical despite different names*

