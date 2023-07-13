# Comparing `tmp/blendersynth-0.0.3.tar.gz` & `tmp/blendersynth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendersynth-0.0.3.tar", last modified: Wed Jul  5 10:09:56 2023, max compression
+gzip compressed data, was "blendersynth-0.0.4.tar", last modified: Thu Jul 13 08:17:49 2023, max compression
```

## Comparing `blendersynth-0.0.3.tar` & `blendersynth-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.168607 blendersynth-0.0.3/
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.158096 blendersynth-0.0.3/BlenderSynth.egg-info/
--rw-r--r--   0 ollie      (501) staff       (20)     1907 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1654 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/SOURCES.txt
--rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/dependency_links.txt
--rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-05 10:09:56.000000 blendersynth-0.0.3/BlenderSynth.egg-info/top_level.txt
--rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.3/LICENSE
--rw-r--r--   0 ollie      (501) staff       (20)     1907 2023-07-05 10:09:56.168439 blendersynth-0.0.3/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1632 2023-07-03 17:47:18.000000 blendersynth-0.0.3/README.md
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.158520 blendersynth-0.0.3/blendersynth/
--rw-r--r--   0 ollie      (501) staff       (20)     1458 2023-07-03 17:09:00.000000 blendersynth-0.0.3/blendersynth/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.159825 blendersynth-0.0.3/blendersynth/annotations/
--rw-r--r--   0 ollie      (501) staff       (20)       87 2023-06-27 20:17:42.000000 blendersynth-0.0.3/blendersynth/annotations/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     1979 2023-06-27 20:17:42.000000 blendersynth-0.0.3/blendersynth/annotations/bbox.py
--rw-r--r--   0 ollie      (501) staff       (20)      272 2023-06-27 20:05:19.000000 blendersynth-0.0.3/blendersynth/annotations/keypoints.py
--rw-r--r--   0 ollie      (501) staff       (20)     1185 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/annotations/utils.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.162162 blendersynth-0.0.3/blendersynth/blender/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/blender/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     8420 2023-06-14 19:52:56.000000 blendersynth-0.0.3/blendersynth/blender/aov.py
--rw-r--r--   0 ollie      (501) staff       (20)     4193 2023-07-05 08:58:47.000000 blendersynth-0.0.3/blendersynth/blender/camera.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.163713 blendersynth-0.0.3/blendersynth/blender/compositor/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/blender/compositor/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     9543 2023-07-03 17:32:33.000000 blendersynth-0.0.3/blendersynth/blender/compositor/compositor.py
--rw-r--r--   0 ollie      (501) staff       (20)     3677 2023-06-27 20:31:49.000000 blendersynth-0.0.3/blendersynth/blender/compositor/image_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/blender/compositor/mask_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)      887 2023-06-27 21:00:21.000000 blendersynth-0.0.3/blendersynth/blender/compositor/node_group.py
--rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-06-27 21:00:00.000000 blendersynth-0.0.3/blendersynth/blender/compositor/visuals.py
--rw-r--r--   0 ollie      (501) staff       (20)     1218 2023-07-05 08:49:09.000000 blendersynth-0.0.3/blendersynth/blender/curve.py
--rw-r--r--   0 ollie      (501) staff       (20)     1256 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/blender/light.py
--rw-r--r--   0 ollie      (501) staff       (20)    12586 2023-07-03 17:02:53.000000 blendersynth-0.0.3/blendersynth/blender/mesh.py
--rw-r--r--   0 ollie      (501) staff       (20)      700 2023-07-03 17:45:30.000000 blendersynth-0.0.3/blendersynth/blender/render.py
--rw-r--r--   0 ollie      (501) staff       (20)     1940 2023-06-27 20:08:32.000000 blendersynth-0.0.3/blendersynth/blender/utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     1755 2023-06-16 17:58:30.000000 blendersynth-0.0.3/blendersynth/blender/world.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.165524 blendersynth-0.0.3/blendersynth/file/
--rw-r--r--   0 ollie      (501) staff       (20)       84 2023-07-05 09:14:27.000000 blendersynth-0.0.3/blendersynth/file/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      839 2023-06-14 20:54:24.000000 blendersynth-0.0.3/blendersynth/file/dataset_inputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      159 2023-06-09 15:47:06.000000 blendersynth-0.0.3/blendersynth/file/dataset_outputs.py
--rw-r--r--   0 ollie      (501) staff       (20)     2929 2023-07-05 10:03:41.000000 blendersynth-0.0.3/blendersynth/file/frames_to_video.py
--rw-r--r--   0 ollie      (501) staff       (20)      412 2023-06-27 20:38:09.000000 blendersynth-0.0.3/blendersynth/file/tempfiles.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.166608 blendersynth-0.0.3/blendersynth/run/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/run/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.3/blendersynth/run/blender_interface.py
--rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.3/blendersynth/run/blender_threading.py
--rw-r--r--   0 ollie      (501) staff       (20)     3002 2023-06-27 21:08:18.000000 blendersynth-0.0.3/blendersynth/run/run.py
--rw-r--r--   0 ollie      (501) staff       (20)      722 2023-07-05 10:01:27.000000 blendersynth-0.0.3/blendersynth/run_this_script.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.166880 blendersynth-0.0.3/blendersynth/utils/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.3/blendersynth/utils/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-05 10:09:56.167894 blendersynth-0.0.3/blendersynth/utils/blender_setup/
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     3885 2023-06-14 21:00:10.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_locator.py
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_python_path.py
--rw-r--r--   0 ollie      (501) staff       (20)     2744 2023-07-05 09:07:26.000000 blendersynth-0.0.3/blendersynth/utils/blender_setup/check_blender_install.py
--rw-r--r--   0 ollie      (501) staff       (20)     3359 2023-06-13 09:36:59.000000 blendersynth-0.0.3/blendersynth/utils/node_arranger.py
--rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-05 10:09:32.000000 blendersynth-0.0.3/pyproject.toml
--rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-05 10:09:56.168668 blendersynth-0.0.3/setup.cfg
--rw-r--r--   0 ollie      (501) staff       (20)      173 2023-07-05 10:09:32.000000 blendersynth-0.0.3/setup.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.907982 blendersynth-0.0.4/
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.891185 blendersynth-0.0.4/BlenderSynth.egg-info/
+-rw-r--r--   0 ollie      (501) staff       (20)     2034 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1835 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/SOURCES.txt
+-rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/dependency_links.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       40 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/requires.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-13 08:17:49.000000 blendersynth-0.0.4/BlenderSynth.egg-info/top_level.txt
+-rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.4/LICENSE
+-rw-r--r--   0 ollie      (501) staff       (20)     2034 2023-07-13 08:17:49.907807 blendersynth-0.0.4/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1759 2023-07-12 13:02:47.000000 blendersynth-0.0.4/README.md
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.890748 blendersynth-0.0.4/blendersynth/
+-rw-r--r--   0 ollie      (501) staff       (20)     1650 2023-07-10 19:24:35.000000 blendersynth-0.0.4/blendersynth/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.894613 blendersynth-0.0.4/blendersynth/annotations/
+-rw-r--r--   0 ollie      (501) staff       (20)      133 2023-07-10 22:37:06.000000 blendersynth-0.0.4/blendersynth/annotations/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2066 2023-07-10 22:37:46.000000 blendersynth-0.0.4/blendersynth/annotations/axes.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2440 2023-07-09 12:11:14.000000 blendersynth-0.0.4/blendersynth/annotations/bbox.py
+-rw-r--r--   0 ollie      (501) staff       (20)      656 2023-07-09 12:11:14.000000 blendersynth-0.0.4/blendersynth/annotations/keypoints.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1387 2023-07-09 12:13:20.000000 blendersynth-0.0.4/blendersynth/annotations/utils.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.899966 blendersynth-0.0.4/blendersynth/blender/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-07-05 14:54:19.000000 blendersynth-0.0.4/blendersynth/blender/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     8664 2023-07-05 14:37:51.000000 blendersynth-0.0.4/blendersynth/blender/aov.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1525 2023-07-07 11:07:54.000000 blendersynth-0.0.4/blendersynth/blender/bsyn_object.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6288 2023-07-07 12:50:10.000000 blendersynth-0.0.4/blendersynth/blender/camera.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.902098 blendersynth-0.0.4/blendersynth/blender/compositor/
+-rw-r--r--   0 ollie      (501) staff       (20)       34 2023-07-05 13:24:45.000000 blendersynth-0.0.4/blendersynth/blender/compositor/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)    11373 2023-07-10 22:37:06.000000 blendersynth-0.0.4/blendersynth/blender/compositor/compositor.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6574 2023-07-10 22:39:48.000000 blendersynth-0.0.4/blendersynth/blender/compositor/image_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.4/blendersynth/blender/compositor/mask_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)      887 2023-07-10 22:40:32.000000 blendersynth-0.0.4/blendersynth/blender/compositor/node_group.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-07-05 12:25:55.000000 blendersynth-0.0.4/blendersynth/blender/compositor/visuals.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1218 2023-07-05 12:25:55.000000 blendersynth-0.0.4/blendersynth/blender/curve.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1843 2023-07-05 15:30:58.000000 blendersynth-0.0.4/blendersynth/blender/light.py
+-rw-r--r--   0 ollie      (501) staff       (20)    17430 2023-07-12 14:35:28.000000 blendersynth-0.0.4/blendersynth/blender/mesh.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1491 2023-07-05 15:36:05.000000 blendersynth-0.0.4/blendersynth/blender/render.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3191 2023-07-12 14:28:48.000000 blendersynth-0.0.4/blendersynth/blender/utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2444 2023-07-10 21:23:07.000000 blendersynth-0.0.4/blendersynth/blender/world.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.904062 blendersynth-0.0.4/blendersynth/file/
+-rw-r--r--   0 ollie      (501) staff       (20)      152 2023-07-07 19:23:23.000000 blendersynth-0.0.4/blendersynth/file/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1005 2023-07-05 13:57:01.000000 blendersynth-0.0.4/blendersynth/file/dataset_inputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      318 2023-07-09 12:14:45.000000 blendersynth-0.0.4/blendersynth/file/dataset_outputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      497 2023-07-07 19:24:14.000000 blendersynth-0.0.4/blendersynth/file/ffmpeg_utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3001 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/file/frames_to_video.py
+-rw-r--r--   0 ollie      (501) staff       (20)      618 2023-07-05 13:54:50.000000 blendersynth-0.0.4/blendersynth/file/tempfiles.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.905496 blendersynth-0.0.4/blendersynth/run/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.4/blendersynth/run/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.4/blendersynth/run/blender_interface.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.4/blendersynth/run/blender_threading.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3278 2023-07-09 12:37:15.000000 blendersynth-0.0.4/blendersynth/run/run.py
+-rw-r--r--   0 ollie      (501) staff       (20)      859 2023-07-12 13:54:07.000000 blendersynth-0.0.4/blendersynth/run/run_this_script.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.906266 blendersynth-0.0.4/blendersynth/utils/
+-rw-r--r--   0 ollie      (501) staff       (20)       43 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      713 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/blender_importer.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-13 08:17:49.907446 blendersynth-0.0.4/blendersynth/utils/blender_setup/
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4475 2023-07-07 10:33:19.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_locator.py
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_python_path.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2956 2023-07-12 13:58:45.000000 blendersynth-0.0.4/blendersynth/utils/blender_setup/check_blender_install.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3604 2023-07-09 12:37:15.000000 blendersynth-0.0.4/blendersynth/utils/node_arranger.py
+-rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-13 08:17:27.000000 blendersynth-0.0.4/pyproject.toml
+-rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-13 08:17:49.908049 blendersynth-0.0.4/setup.cfg
+-rw-r--r--   0 ollie      (501) staff       (20)      245 2023-07-13 08:17:27.000000 blendersynth-0.0.4/setup.py
```

### Comparing `blendersynth-0.0.3/BlenderSynth.egg-info/PKG-INFO` & `blendersynth-0.0.4/BlenderSynth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
 
 ![](docs/splash.png)
 
+[Documentation](https://ollieboyne.github.io/BlenderSynth/) | 
+
 Synthetic Blender pipeline - aimed at generating large synthetic datasets.
 
 [BlenderProc](https://github.com/DLR-RM/BlenderProc) is an incredibly useful tool for synthetic dataset generation. We aim here to provide an alternative that is (a) more specialised for uncommon data forms, and (b) runs faster for creating large scale datasets.
 
 We produce support for:
 - Custom Shader [AOVs](https://docs.blender.org/manual/en/latest/render/shader_nodes/output/aov.html) (eg. UVs, Normals, etc.)
-- Multi-threading support
+- Fine-grained node control
+- Multi-threading
 - Efficient run-speed
 
 ## Installation
 
 1) Install [Blender](https://www.blender.org)
 
 2) Install blendersynth
@@ -36,21 +39,21 @@
 ```
 
 Or from local clone:
 
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
-python setup.py install
+pip install .
 python -c "import blendersynth" --local
 ```
 
 ## Examples
 
-[See here](examples) for usage examples.
+[See here](https://github.com/OllieBoyne/BlenderSynth/tree/main/examples) for usage examples.
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
```

### Comparing `blendersynth-0.0.3/BlenderSynth.egg-info/SOURCES.txt` & `blendersynth-0.0.4/BlenderSynth.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 pyproject.toml
 setup.py
 BlenderSynth.egg-info/PKG-INFO
 BlenderSynth.egg-info/SOURCES.txt
 BlenderSynth.egg-info/dependency_links.txt
 BlenderSynth.egg-info/top_level.txt
 blendersynth/__init__.py
-blendersynth/run_this_script.py
 blendersynth.egg-info/PKG-INFO
 blendersynth.egg-info/SOURCES.txt
 blendersynth.egg-info/dependency_links.txt
+blendersynth.egg-info/requires.txt
 blendersynth.egg-info/top_level.txt
 blendersynth/annotations/__init__.py
+blendersynth/annotations/axes.py
 blendersynth/annotations/bbox.py
 blendersynth/annotations/keypoints.py
 blendersynth/annotations/utils.py
 blendersynth/blender/__init__.py
 blendersynth/blender/aov.py
+blendersynth/blender/bsyn_object.py
 blendersynth/blender/camera.py
 blendersynth/blender/curve.py
 blendersynth/blender/light.py
 blendersynth/blender/mesh.py
 blendersynth/blender/render.py
 blendersynth/blender/utils.py
 blendersynth/blender/world.py
@@ -30,19 +32,22 @@
 blendersynth/blender/compositor/image_overlay.py
 blendersynth/blender/compositor/mask_overlay.py
 blendersynth/blender/compositor/node_group.py
 blendersynth/blender/compositor/visuals.py
 blendersynth/file/__init__.py
 blendersynth/file/dataset_inputs.py
 blendersynth/file/dataset_outputs.py
+blendersynth/file/ffmpeg_utils.py
 blendersynth/file/frames_to_video.py
 blendersynth/file/tempfiles.py
 blendersynth/run/__init__.py
 blendersynth/run/blender_interface.py
 blendersynth/run/blender_threading.py
 blendersynth/run/run.py
+blendersynth/run/run_this_script.py
 blendersynth/utils/__init__.py
+blendersynth/utils/blender_importer.py
 blendersynth/utils/node_arranger.py
 blendersynth/utils/blender_setup/__init__.py
 blendersynth/utils/blender_setup/blender_locator.py
 blendersynth/utils/blender_setup/blender_python_path.py
 blendersynth/utils/blender_setup/check_blender_install.py
```

### Comparing `blendersynth-0.0.3/LICENSE` & `blendersynth-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/PKG-INFO` & `blendersynth-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
 
 ![](docs/splash.png)
 
+[Documentation](https://ollieboyne.github.io/BlenderSynth/) | 
+
 Synthetic Blender pipeline - aimed at generating large synthetic datasets.
 
 [BlenderProc](https://github.com/DLR-RM/BlenderProc) is an incredibly useful tool for synthetic dataset generation. We aim here to provide an alternative that is (a) more specialised for uncommon data forms, and (b) runs faster for creating large scale datasets.
 
 We produce support for:
 - Custom Shader [AOVs](https://docs.blender.org/manual/en/latest/render/shader_nodes/output/aov.html) (eg. UVs, Normals, etc.)
-- Multi-threading support
+- Fine-grained node control
+- Multi-threading
 - Efficient run-speed
 
 ## Installation
 
 1) Install [Blender](https://www.blender.org)
 
 2) Install blendersynth
@@ -36,21 +39,21 @@
 ```
 
 Or from local clone:
 
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
-python setup.py install
+pip install .
 python -c "import blendersynth" --local
 ```
 
 ## Examples
 
-[See here](examples) for usage examples.
+[See here](https://github.com/OllieBoyne/BlenderSynth/tree/main/examples) for usage examples.
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
```

### Comparing `blendersynth-0.0.3/README.md` & `blendersynth-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # BlenderSynth
 
 ![](docs/splash.png)
 
+[Documentation](https://ollieboyne.github.io/BlenderSynth/) | 
+
 Synthetic Blender pipeline - aimed at generating large synthetic datasets.
 
 [BlenderProc](https://github.com/DLR-RM/BlenderProc) is an incredibly useful tool for synthetic dataset generation. We aim here to provide an alternative that is (a) more specialised for uncommon data forms, and (b) runs faster for creating large scale datasets.
 
 We produce support for:
 - Custom Shader [AOVs](https://docs.blender.org/manual/en/latest/render/shader_nodes/output/aov.html) (eg. UVs, Normals, etc.)
-- Multi-threading support
+- Fine-grained node control
+- Multi-threading
 - Efficient run-speed
 
 ## Installation
 
 1) Install [Blender](https://www.blender.org)
 
 2) Install blendersynth
@@ -27,21 +30,21 @@
 ```
 
 Or from local clone:
 
 ```
 git clone https://github.com/OllieBoyne/BlenderSynth
 cd BlenderSynth
-python setup.py install
+pip install .
 python -c "import blendersynth" --local
 ```
 
 ## Examples
 
-[See here](examples) for usage examples.
+[See here](https://github.com/OllieBoyne/BlenderSynth/tree/main/examples) for usage examples.
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Contributions
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
```

### Comparing `blendersynth-0.0.3/blendersynth/annotations/bbox.py` & `blendersynth-0.0.4/blendersynth/annotations/bbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from ..blender.mesh import Mesh
 from typing import List
 
 BBOX_FMTS = ['x1y1x2y2', 'xywh']
 
 def bounding_box(object: Mesh, camera: bpy.types.Camera = None,
 				 scene:bpy.types.Scene=None,
-				 return_fmt='x1y1x2y2', normalized=False, invert_y=True):
+				 return_fmt:str='x1y1x2y2', normalized:bool=False, invert_y:bool=True) -> tuple:
 	"""Get the bounding box of an object in camera space.
 	Achieve this by projecting all vertices of the object to the image plane,
 	and taking the min/max of the resulting coordinates.
 
 	:param object: Mesh
 	:param camera: bpy.types.Camera (if None, use bpy.context.scene.camera)
 	:param scene: bpy.types.Scene (if None, use bpy.context.scene)
-	:param return_fmt: str, one of ['x1y1x2y2', 'xywh']
-	:param normalized: bool, if True, return normalized coordinates (0-1) instead of pixel coordinates
-	:param invert_y: bool, if True, y is measured from the top of the image, otherwise from the bottom (Blender measures from bottom)
+	:param return_fmt: one of ['x1y1x2y2', 'xywh']
+	:param normalized: if True, return normalized coordinates (0-1) instead of pixel coordinates
+	:param invert_y: if True, y is measured from the top of the image, otherwise from the bottom (Blender measures from bottom)
 	"""
 
 	if camera is None:
 		camera = bpy.context.scene.camera
 
 	if scene is None:
 		scene = bpy.context.scene
@@ -46,12 +46,20 @@
 		return xmin, ymin, xmax - xmin, ymax - ymin
 
 	else:
 		raise ValueError(f'Invalid return_fmt: {return_fmt}. Must be one of {BBOX_FMTS}')
 
 def bounding_boxes(objects: List[Mesh], camera: bpy.types.Camera = None,
 				 scene:bpy.types.Scene=None,
-				 return_fmt='x1y1x2y2', normalized=False, invert_y=True):
-	"""Get the bounding boxes of multiple objects in image space."""
+				 return_fmt:str='x1y1x2y2', normalized:bool=False, invert_y:bool=True) -> List[tuple]:
+	"""Run `bounding_box` for multiple objects
+
+	:param objects: List of Mesh objects
+	:param camera: bpy.types.Camera (if None, use bpy.context.scene.camera)
+	:param scene: bpy.types.Scene (if None, use bpy.context.scene)
+	:param return_fmt: one of ['x1y1x2y2', 'xywh']
+	:param normalized: if True, return normalized coordinates (0-1) instead of pixel coordinates
+	:param invert_y: if True, y is measured from the top of the image, otherwise from the bottom (Blender measures from bottom)
+	"""
 
 	return [bounding_box(obj, camera=camera, scene=scene, return_fmt=return_fmt,
 						   normalized=normalized, invert_y=invert_y) for obj in objects]
```

### Comparing `blendersynth-0.0.3/blendersynth/annotations/utils.py` & `blendersynth-0.0.4/blendersynth/annotations/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import bpy
 from bpy_extras.object_utils import world_to_camera_view
 import mathutils
 import numpy as np
 
 
-def project_point_to_image(P: mathutils.Vector, scene, camera, invert_y=True):
+def project_point_to_image(P: mathutils.Vector, scene:bpy.types.Scene,
+						   camera:bpy.types.Camera, invert_y:bool=True):
 	"""Return 2D (x, y) image coordinates of a 3D point P.
 
-	invert_y: if True, y is measured from the top of the image, otherwise from the bottom
-	(Blender measures from bottom)"""
+	:param P: 3D point
+	:param scene: Blender scene
+	:param camera: Camera to project through
+	:param invert_y: if True, y is measured from the top of the image, otherwise from the bottom (Blender measures from bottom)"""
+
 	ndc_x, ndc_y, ndc_depth = world_to_camera_view(scene, camera, P)  # normalized device coords
 	imgx = scene.render.resolution_x * ndc_x
 
 	if invert_y:
 		imgy = scene.render.resolution_y * (1 - ndc_y)  # ndc_y measured from bottom
 	else:
 		imgy = scene.render.resolution_y * ndc_y
 
 
 	return imgx, imgy
 
 
-def project_points(points, scene, camera, invert_y=True):
+def project_points(points:np.ndarray, scene:bpy.types.Scene, camera:bpy.types.Camera, invert_y:bool=True):
 	"""Project points to image plane.
+
 	:param points: Nx3 matrix of points
-	:param scene: bpy.types.Scene
-	:param camera: bpy.types.Camera
+	:param scene: Blender scene
+	:param camera: Camera to project through
 	:param invert_y: if True, y is measured from the top of the image, otherwise from the bottom
 
 	:return: Nx2 matrix of 2D image coordinates"""
 	coords_2d = []
 	for p in points:
 		p_vec = mathutils.Vector(*(p,))
 		coords_2d.append(project_point_to_image(p_vec, scene, camera, invert_y=invert_y))
```

### Comparing `blendersynth-0.0.3/blendersynth/blender/aov.py` & `blendersynth-0.0.4/blendersynth/blender/aov.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 import bpy
 from ..utils.node_arranger import tidy_tree
 
 ref_frames = ['CAMERA', 'WORLD', 'OBJECT']
 
 class AOV:
+	"""A generic Arbitrary Output Value.
+	An AOV is a float or color value that can be output from a shader to the renderer.
+	See `Blender docs <https://docs.blender.org/manual/en/latest/render/shader_nodes/output/aov.html>`_ for more info.
+	"""
+
 	AOV_TYPE = 'COLOR'
 	def __init__(self, name=None, **kwargs):
 		if name is None:
 			name = self.__class__.__name__
 
 		self.name = name
 		self._add_to_view_layer()
```

### Comparing `blendersynth-0.0.3/blendersynth/blender/compositor/compositor.py` & `blendersynth-0.0.4/blendersynth/blender/compositor/compositor.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import shutil
 from ..render import render, render_depth
 from .node_group import CompositorNodeGroup
 from ..aov import AOV
 from ..mesh import Mesh
 from .mask_overlay import MaskOverlay
 from .visuals import DepthVis
-from .image_overlay import KeypointsOverlay, BoundingBoxOverlay
+from .image_overlay import KeypointsOverlay, BoundingBoxOverlay, AlphaImageOverlay, AxesOverlay
 
 
 from typing import Union, List
 from ...utils.node_arranger import tidy_tree
 
 # Mapping of file formats to extensions
 format_to_extension = {
@@ -121,30 +121,75 @@
 			raise ValueError("Only allowed one BBox overlay (it can contain multiple objects).")
 
 		self.overlays['BBox'] = cng
 
 		self.tidy_tree()
 		return cng
 
-	def get_keypoints_visual(self) -> KeypointsOverlay:
+	def get_keypoints_visual(self, marker:str='x', color:tuple=(0, 0, 255), size:int=5,
+							 thickness:int=2) -> KeypointsOverlay:
 		"""
-		Initialize a keypoints overlay node
+		Initialize a keypoints overlay node.
+
+		:param marker: Marker type, either [c/circle], [s/square], [t/triangle] or [x]. Default 'x'
+		:param size: Size of marker. Default 5
+		:param color: Color of marker, RGB or RGBA, default (0, 0, 255) (red)
+		:param thickness: Thickness of marker. Default 2
 		"""
 
-		cng = KeypointsOverlay(f"Keypoints Visual", self.node_tree)
+		cng = KeypointsOverlay(f"Keypoints Visual", self.node_tree, marker=marker, color=color,
+							   size=size, thickness=thickness)
 		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
 
 		if 'Keypoints' in self.overlays:
 			raise ValueError("Only allowed one Keypoints overlay.")
 
 		self.overlays['Keypoints'] = cng
 
 		self.tidy_tree()
 		return cng
 
+	def get_axes_visual(self, size:int=1, thickness:int=2) -> AxesOverlay:
+		"""
+		Initialize an axes overlay node.
+
+		:param size: Size of axes. Default 100
+		:param thickness: Thickness of axes. Default 2
+		"""
+
+		cng = AxesOverlay(f"Axes Visual", self.node_tree,
+							   size=size, thickness=thickness)
+		self.node_tree.links.new(self.render_layers_node.outputs['Image'], cng.input('Image'))
+
+		if 'Axes' in self.overlays:
+			raise ValueError("Only allowed one Axes overlay.")
+
+		self.overlays['Axes'] = cng
+		self.tidy_tree()
+		return cng
+
+	def stack_visuals(self, *visuals: AlphaImageOverlay) -> AlphaImageOverlay:
+		"""Given a series of image overlays, stack them and return to be used as a single output node.
+
+		:param *visuals: Stack of overlays to add."""
+
+		if len(visuals) < 2:
+			raise ValueError("Requires at least 2 visuals to stack")
+
+		# No need to store these overlays separately in self.overlays, but need to check they're all present
+		for overlay in visuals:
+			if overlay not in self.overlays.values():
+				raise ValueError(f"Visual {overlay} not found in Compositor. Make sure it was obtained via the Compositor.")
+
+		# Stack the output of the previous to the input of the next
+		for va, vb in zip(visuals, visuals[1:]):
+			self.node_tree.links.new(va.output('Image'), vb.input('Image'))
+
+		return visuals[-1]
+
 	def get_depth_visual(self, max_depth=1, col=(255, 255, 255)):
 		"""Get depth visual, which normalizes depth values so max_depth = col,
 		and any values below that are depth/max_depth * col.
 
 		Col = 0-255 RGB or RGBA"""
 
 		if 'Depth' not in self.render_layers_node.outputs:
@@ -163,21 +208,23 @@
 					  file_format='PNG', color_mode='RGBA', jpeg_quality=90,
 					  png_compression=15, color_depth='8', EXR_color_depth='32',
 					  name=None):
 		"""Add a connection between a valid render output, and a file output node.
 		Supports changing view output.
 
 		This should only be called once per output (NOT inside a loop).
-		Inside the loop, only
+		Inside the loop, only call `update_filename` or `update_directory`
 
 		:mode: if 'image', export in sRGB color space. If 'data', export in raw linear color space
 
-		:input_node: if string, will get the input_data from that key in the render_layers_node
-		:input_data: if CompositorNodeGroup, will use that node as input
-		:input_data: if AOV, will use that AOV as input (storing AOV)
+		:input_data: Can take one of three forms:
+			- `string`, will get the input_data from that key in the render_layers_node
+			- `CompositorNodeGroup`, will use that node as input
+			- `AOV`, will use that AOV as input (storing AOV)
+
 		:name: Name of output. If not given, will take the str representation of input_data
 		"""
 
 		if isinstance(input_data, AOV):
 			self.aovs.append(input_data)
 			input_data = input_data.name  # name is sufficient to pull from render_layers_node
```

### Comparing `blendersynth-0.0.3/blendersynth/blender/compositor/mask_overlay.py` & `blendersynth-0.0.4/blendersynth/blender/compositor/mask_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/blendersynth/blender/compositor/node_group.py` & `blendersynth-0.0.4/blendersynth/blender/compositor/node_group.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/blendersynth/blender/compositor/visuals.py` & `blendersynth-0.0.4/blendersynth/blender/compositor/visuals.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/blendersynth/blender/curve.py` & `blendersynth-0.0.4/blendersynth/blender/curve.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/blendersynth/blender/mesh.py` & `blendersynth-0.0.4/blendersynth/blender/mesh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os.path
 
 import bpy
-from .utils import GetNewObject, SelectObjects, handle_vec
+from .utils import GetNewObject, SelectObjects, handle_vec, SetMode
+from .bsyn_object import BsynObject, animatable_property
 from .aov import AOV
 import numpy as np
 import mathutils
 from mathutils import Vector, Euler
+from typing import Union, List
+from copy import deepcopy
 
-_primitives ={
+_primitives = {
 	"cube": bpy.ops.mesh.primitive_cube_add,
 	"sphere": bpy.ops.mesh.primitive_uv_sphere_add,
 	"cylinder": bpy.ops.mesh.primitive_cylinder_add,
 	"plane": bpy.ops.mesh.primitive_plane_add,
 	"cone": bpy.ops.mesh.primitive_cone_add,
 	"monkey": bpy.ops.mesh.primitive_monkey_add,
 	"torus": bpy.ops.mesh.primitive_torus_add,
@@ -24,58 +27,45 @@
 	'prim_cylinder': 3,
 	'prim_plane': 4,
 	'prim_cone': 5,
 	'prim_monkey': 6,
 	'prim_torus': 7,
 }
 
-def get_child_meshes(obj):
+
+def _get_child_meshes(obj):
 	"""Given an object, return all meshes that are children of it. Recursively searches children of children.
 	Also returns any child objects that aren't meshes"""
 	if obj.type == 'MESH':
 		return [obj], []
 	else:
 		meshes, other = [], [obj]
 		for child in obj.children:
-			child_meshes, child_other = get_child_meshes(child)
+			child_meshes, child_other = _get_child_meshes(child)
 			meshes += child_meshes
 			other += child_other
 
 		return meshes, other
 
-def bounds_center(mesh):
-	"""Get center of bounding box in world space"""
-	local_bbox_center = 0.125 * sum((mathutils.Vector(b) for b in mesh.bound_box), mathutils.Vector())
-	global_bbox_center = mesh.matrix_world @ local_bbox_center
-	return np.array(global_bbox_center)
-
-def vertex_center(mesh):
-	"""Get center of vertices in world space"""
-	verts = np.array([mesh.matrix_world @ v.co for v in mesh.data.vertices])
-	return verts.mean(axis=0)
-
-def set_origin(mesh, vec):
-	if mesh.type == 'MESH':
-		delta = mesh.location - mathutils.Vector(vec)
-		delta_object = mesh.matrix_world.inverted() @ delta
-		mesh.data.transform(mathutils.Matrix.Translation(delta_object))  # Move the mesh vertices in the opposite direction
-		mesh.location -= delta_object
-		bpy.context.view_layer.update()
-
 
-def euler_from(a: mathutils.Euler, b: mathutils.Euler):
+def _euler_from(a: mathutils.Euler, b: mathutils.Euler):
 	"""Get euler rotation from a to b"""
 	return (b.to_matrix() @ a.to_matrix().inverted()).to_euler()
 
-def euler_add(a: mathutils.Euler, b: mathutils.Euler):
+
+def _euler_add(a: mathutils.Euler, b: mathutils.Euler):
 	"""Compute euler rotation of a, followed by b"""
 	return (a.to_matrix() @ b.to_matrix()).to_euler()
 
 
-class Mesh:
+class Mesh(BsynObject):
+	"""A mesh object. Can be a single mesh, or a hierarchy of meshes."""
+	primitive_list = list(_primitives.keys())
+	"""List of available primitives"""
+
 	def __init__(self, obj, material=None, scene=None, class_id=None):
 		"""
 		:param obj: Receives either a single mesh, or an empty with children empty & meshes
 		:param material:
 		:param scene:
 
 		If obj contains multiple meshes, they will all be assigned the same material, and must act as a single object
@@ -83,27 +73,27 @@
 
 		"""
 
 		if scene is None:
 			scene = bpy.context.scene
 
 		self.scene = scene
-		self.obj = obj
-		self._meshes, self._other_objects = get_child_meshes(obj)
+		self._object = obj
+		self._meshes, self._other_objects = _get_child_meshes(obj)
 
 		# Must have a material, create if not passed
 		if material is None:
 			material = bpy.data.materials.new(name='Material')
 			material.use_nodes = True
 
 			for mesh in self._meshes:
 				mesh.data.materials.append(material)
 
 		# INSTANCING - Define InstanceID based on number of meshes in scene
-		self.obj['instance_id'] = scene.get('NUM_MESHES', 0)
+		self._object['instance_id'] = scene.get('NUM_MESHES', 0)
 		scene['NUM_MESHES'] = scene.get('NUM_MESHES', 0) + 1  # Increment number of meshes in scene
 
 		# CLASS - Define class based on type of object (e.g. primitive)
 		# can be overriden at any point
 		self.set_class_id(class_id)
 
 		self.assigned_aovs = []
@@ -113,27 +103,43 @@
 		self._rotation_euler = Euler((0, 0, 0))
 		self._location = Vector((0, 0, 0))
 
 	def set_class_id(self, class_id):
 		assert isinstance(class_id, int), f"Class ID must be an integer, not {type(class_id)}"
 		assert class_id >= 0, f"Class ID must be >= 0, not {class_id}"
 
-		self.obj['class_id'] = class_id
+		self._object['class_id'] = class_id
 		self.scene['MAX_CLASSES'] = max(self.scene.get('MAX_CLASSES', 0), class_id)
 
-
 	@classmethod
-	def from_scene(cls, key, class_id=None):
-		"""Create object from scene"""
+	def from_scene(cls, key, class_id=0) -> 'Mesh':
+		"""Create object from named object in scene.
+
+		:param key: Name of object in scene
+		:param class_id: Class ID to assign to object
+
+		:return: Mesh loaded from scene"""
 		obj = bpy.data.objects[key]
 		return cls(obj, class_id=class_id)
 
 	@classmethod
-	def from_primitive(cls, name='cube', scale=None, location=None, rotation_euler=None, class_id=None, **kwargs):
-		"""Create object from primitive"""
+	def from_primitive(cls, name='cube', scale=None, location=None, rotation_euler=None, class_id=None,
+					   **kwargs) -> 'Mesh':
+		"""Create Mesh from primitive.
+		
+		:param name: Name of primitive to create. See :attr:`~blendersynth.blender.Mesh.primitive_list` for options
+		:param scale: Scale of object
+		:param location: Location of object
+		:param rotation_euler: Rotation of object
+		:param class_id: Class ID to assign to object
+		:param kwargs: Additional arguments to pass to primitive (see `bpy.ops.mesh.primitive_cube_add <https://docs.blender.org/api/current/bpy.ops.mesh.html#bpy.ops.mesh.primitive_cube_add>`_, etc.)
+
+		:return: Mesh object created from primitive
+		"""
+
 		assert name in _primitives, f"Primitive `{name}` not found. Options are: {list(_primitives.keys())}"
 
 		importer = GetNewObject(bpy.context.scene)
 		with importer:
 			prim = _primitives[name](**kwargs)  # Create primitive
 
 		if class_id is None:
@@ -143,50 +149,51 @@
 
 		if scale is not None: obj.scale = scale
 		if location is not None: obj.location = location
 		if rotation_euler is not None: obj.rotation_euler = rotation_euler
 
 		return obj
 
-
 	@classmethod
 	def from_obj(cls, obj_loc, class_id=None,
 				 forward_axis='-Z', up_axis='Y'):
 		"""Load object from .obj file.
 
 		Note: we use bpy.ops.wm.obj_import instead of bpy.ops.import_scene.obj because the latter
 		causes issues with materials & vertex ordering.
 		(Changing vertex ordering makes the use of keypoints difficult.)
 		"""
 		for axis in (forward_axis, up_axis):
-			assert axis in ('X', 'Y', 'Z', '-X', '-Y', '-Z'), f"Axis `{axis}` not valid, must be one of X, Y, Z, -X, -Y, -Z"
+			assert axis in (
+			'X', 'Y', 'Z', '-X', '-Y', '-Z'), f"Axis `{axis}` not valid, must be one of X, Y, Z, -X, -Y, -Z"
 
-		forward_axis = axis.replace('-', 'NEGATIVE_') # e.g. -X -> NEGATIVE_X
-		up_axis = axis.replace('-', 'NEGATIVE_')
+		forward_axis = forward_axis.replace('-', 'NEGATIVE_')  # e.g. -X -> NEGATIVE_X
+		up_axis = up_axis.replace('-', 'NEGATIVE_')
 
 		assert os.path.isfile(obj_loc) and obj_loc.endswith('.obj'), f"File `{obj_loc}` not a valid .obj file"
 
 		directory, fname = os.path.split(obj_loc)
 		directory = os.path.abspath(directory)  # ensure absolute path for clean loading
 
 		importer = GetNewObject(bpy.context.scene)
 		with importer:
 			bpy.ops.wm.obj_import(filepath=fname, directory=directory, filter_image=False,
-									 files=[{"name": fname}], forward_axis=forward_axis, up_axis=up_axis)
+								  files=[{"name": fname}], forward_axis=forward_axis, up_axis=up_axis)
 
 		if class_id is None:
 			class_id = default_ids['loaded_mesh']
 
 		obj = importer.imported_obj
 		return cls(obj, class_id=class_id)
 
 	@classmethod
 	def from_glb(cls, glb_loc, class_id=None):
 		"""Load object from .glb file"""
-		assert os.path.isfile(glb_loc) and glb_loc.endswith(('.glb', '.gtlf')), f"File `{glb_loc}` not a valid .glb file"
+		assert os.path.isfile(glb_loc) and glb_loc.endswith(
+			('.glb', '.gtlf')), f"File `{glb_loc}` not a valid .glb file"
 
 		directory, fname = os.path.split(glb_loc)
 		importer = GetNewObject(bpy.context.scene)
 		with importer:
 			bpy.ops.import_scene.gltf(filepath=glb_loc, files=[{"name": fname}])
 
 		if class_id is None:
@@ -194,24 +201,62 @@
 
 		return cls(importer.imported_obj, class_id=class_id)
 
 	@classmethod
 	def from_gltf(cls, gltf_loc, class_id=None):
 		return cls.from_glb(gltf_loc, class_id=class_id)
 
+	@classmethod
+	def from_fbx(cls, fbx_loc, class_id=None):
+		"""Load object from .fbx file"""
+		assert os.path.isfile(fbx_loc) and fbx_loc.endswith('.fbx'), f"File `{fbx_loc}` not a valid .fbx file"
+
+		directory, fname = os.path.split(fbx_loc)
+		importer = GetNewObject(bpy.context.scene)
+		with importer:
+			bpy.ops.import_scene.fbx(filepath=fbx_loc, files=[{"name": fname}])
+
+		if class_id is None:
+			class_id = default_ids['loaded_mesh']
+
+		return cls(importer.imported_obj, class_id=class_id)
 
 	@property
-	def origin(self):
-		"""Get origin as origin of first mesh"""
-		return self._meshes[0].location
+	def origin(self) -> Union[Vector, List[Vector]]:
+		"""
+		If single mesh, return Vector of origin.
+		If multiple meshes, return list of Vectors of centroid of each mesh."""
+		if len(self._meshes) == 1:
+			return self._meshes[0].location
+
+		else:
+			return [m.location for m in self._meshes]
 
 	@origin.setter
 	def origin(self, origin):
-		"""Set origin of object"""
-		self._meshes[0].location = origin
+		"""Set origin of object.
+		If single mesh, expects Vector.
+		If multiple meshes, expects list of Vectors"""
+
+		if len(self._meshes) == 1:
+			try:
+				vec = handle_vec(origin)
+			except ValueError:
+				raise ValueError(f"Error with setting origin. Expects a 3 long Vector. Received: {origin}")
+
+			self._meshes[0].location = vec
+
+		else:
+			for i in range(len(self._meshes)):
+				try:
+					vec = handle_vec(origin[i])
+					self._meshes[i].location = vec
+				except:
+					raise ValueError(
+						f"Error with setting origin. Expects a list of {len(self._meshes)} 3-long Vector. Received: {origin}")
 
 	def get_all_vertices(self, ref_frame='WORLD'):
 		verts = np.array([vert.co[:] + (1,) for mesh in self._meshes for vert in mesh.data.vertices]).T
 
 		if ref_frame == 'LOCAL':
 			pass
 
@@ -221,15 +266,14 @@
 
 		else:
 			raise ValueError(f"Invalid ref_frame: {ref_frame}. Must be one of ['LOCAL', 'WORLD']")
 
 		verts = verts[:3, :] / verts[3, :]  # convert from homogeneous coordinates
 		return verts.T
 
-
 	@property
 	def materials(self):
 		return {m for mesh in self._meshes for m in mesh.data.materials}
 
 	def assign_pass_index(self, index: int):
 		"""Assign pass index to object. This can be used when mask rendering."""
 		for mesh in self._meshes:
@@ -242,108 +286,120 @@
 			for material in self.materials:
 				shader_node_tree = material.node_tree
 				assert shader_node_tree is not None, "Material must have a node tree"
 				aov.add_to_shader(shader_node_tree)
 
 		self.assigned_aovs.append(aov)
 
-
 	def set_minimum_to(self, axis='Z', pos=0):
 		"""Set minimum of object to a given position"""
 		min_pos = self.get_all_vertices('WORLD')[:, 'XYZ'.index(axis)].min()
 		trans_vec = np.zeros(3)
 		trans_vec['XYZ'.index(axis)] = pos - min_pos
 		self.translate(trans_vec)
 
-	# @property
-	# def bound_box(self):
-	# 	"""Return bounding box of object(s)"""
-	# 	return self.obj.bound_box
-
 	@property
 	def matrix_world(self):
 		"""Return world matrix of object(s).
 		"""
-		bpy.context.evaluated_depsgraph_get() # required to update object matrix
+		bpy.context.evaluated_depsgraph_get()  # required to update object matrix
 		return self._meshes[0].matrix_world
 
 	@property
+	def axes(self) -> np.ndarray:
+		"""Return 3x3 rotation matrix (normalized) to represent axes"""
+		mat = np.array(self.matrix_world)[:3, :3]
+		mat = mat / np.linalg.norm(mat, axis=0)
+		return mat
+
+	@property
+	def location(self):
+		return self._location
+
+	@location.setter
+	def location(self, location):
+		self.set_location(location)
+
+	@property
+	def rotation_euler(self):
+		return self._rotation_euler
+
+	@rotation_euler.setter
+	def rotation_euler(self, rotation):
+		self.set_rotation_euler(rotation)
+
+	@property
 	def scale(self):
-		"""Return scale of primary mesh."""
 		return self._scale
 
 	@scale.setter
 	def scale(self, scale):
-		"""Set scale of all meshes (scales about origin)"""
-		if isinstance(scale, (int, float)):
-			scale = (scale, scale, scale)
+		self.set_scale(scale)
 
-		resize_fac = np.array(scale) / np.array(self.scale)
+	@animatable_property('location')
+	def set_location(self, location):
+		"""Set location of object"""
+		location = handle_vec(location, 3)
 
+		translation = location - self.location
 		with SelectObjects(self._meshes + self._other_objects):
-			bpy.ops.transform.resize(value=resize_fac)
-
-		self._scale = scale
+			bpy.ops.transform.translate(value=translation)
 
-	@property
-	def rotation_euler(self):
-		"""Return euler rotation of object"""
-		return self._rotation_euler
+		self._location = location
 
-	@rotation_euler.setter
-	def rotation_euler(self, rotation):
+	@animatable_property('rotation_euler')
+	def set_rotation_euler(self, rotation):
 		"""Set euler rotation of object"""
 		assert len(rotation) == 3, f"Rotation must be a tuple of length 3, got {len(rotation)}"
 		rotation = Euler(rotation, 'XYZ')
-		diff = euler_from(self.rotation_euler, rotation)
+		diff = _euler_from(self.rotation_euler, rotation)
 
 		with SelectObjects(self._meshes + self._other_objects):
 			for ax, val in zip('XYZ', diff):
 				if val != 0:
 					bpy.ops.transform.rotate(value=val, orient_axis=ax)
 
 		self._rotation_euler = rotation
 
-	@property
-	def location(self):
-		"""Return location of object"""
-		return self._location
+	@animatable_property('scale')
+	def set_scale(self, scale):
+		"""Set scale of object"""
+		if isinstance(scale, (int, float)):
+			scale = (scale, scale, scale)
 
-	@location.setter
-	def location(self, location):
-		"""Set location of object"""
-		location = handle_vec(location, 3)
+		resize_fac = np.array(scale) / np.array(self.scale)
 
-		translation = location - self.location
 		with SelectObjects(self._meshes + self._other_objects):
-			bpy.ops.transform.translate(value=translation)
+			bpy.ops.transform.resize(value=resize_fac)
 
-		self._location = location
+		self._scale = scale
 
 	def translate(self, translation):
 		"""Translate object"""
 		translation = handle_vec(translation, 3)
 		self.location = self.location + translation
 
 	def rotate_by(self, rotation):
 		"""Add a rotation to the object. Must be in XYZ order, euler angles, radians."""
 		rotation = handle_vec(rotation, 3)
-		new_rotation = euler_add(self.rotation_euler, Euler(rotation, 'XYZ'))
+		new_rotation = _euler_add(self.rotation_euler, Euler(rotation, 'XYZ'))
 		self.rotation_euler = new_rotation
 
 	def scale_by(self, scale):
 		"""Scale object"""
 		if isinstance(scale, (int, float)):
 			scale = (scale, scale, scale)
 
 		scale = handle_vec(scale, 3)
 		self.scale = self._scale * scale
 
-	def delete(self, delete_materials=True):
-		"""Clear mesh from scene & mesh data"""
+	def delete(self, delete_materials: bool = True):
+		"""Clear mesh from scene & mesh data.
+
+		:param delete_materials: Also delete object materials from scene"""
 		mesh_names = [m.name for m in self._meshes]
 		for mesh in self._meshes:
 			bpy.data.objects.remove(mesh, do_unlink=True)
 
 		# remove any non-mesh objects
 		for obj in self._other_objects:
 			bpy.data.objects.remove(obj, do_unlink=True)
@@ -357,56 +413,140 @@
 
 		self._meshes = []  # clear mesh list
 
 		if delete_materials:
 			for material in self.materials:
 				bpy.data.materials.remove(material, do_unlink=True)
 
-	def centroid(self, method='vertex'):
+	def centroid(self, method: str = 'median') -> Vector:
 		"""
-		:param method: 'vertex' or 'bounds'
-		:return:
+		Return the centroid of the mesh(es)
+
+		:param method: See :attr:`~blendersynth.blender.mesh.Mesh.origin_to_centroid` for options.
+		:return: Centroid of the mesh(es). If multiple meshes, will average the centroids.
 		"""
-		centroids = []
 
-		for mesh in self._meshes:
-			if method == 'vertex':
-				centroids.append(vertex_center(mesh))
+		original_origins = deepcopy(self.origin)
+		self.origin_to_centroid(method=method)
+		centroid = deepcopy(self.origin)
+		self.origin = original_origins
+
+		if len(self._meshes) > 1:
+			return sum(centroid) / len(self._meshes)
+
+		return centroid
+
+	def _set_origin_manual(self, origin: Vector, all_meshes=True):
+		"""Override to set origin manually. Should only be used by internal functions."""
+		if all_meshes:
+			for mesh in self._meshes:
+				mesh.location = origin
+		else:
+			self._meshes[0].location = origin
 
-			elif method == 'bounds':
-				centroids.append(bounds_center(mesh))
+	def origin_to_centroid(self, method: str = 'bounds'):
+		"""Move object origin to centroid.
 
-			else:
-				raise ValueError(f"Invalid method: {method}. Must be one of ['vertex', 'bounds']")
+		Four methods available:
 
-		return np.mean(centroids, axis=0)
+		* 'bounds' - move the origin to the center of the bounds of the mesh
+		* 'median' - move the origin to the median point of the mesh
+		* 'com_volume' - move to the centre of mass of the volume of the mesh
+		* 'com_area' - Move to the centre of mass of the surface of the mesh
 
-	def origin_to_centroid(self, method='bounds'):
-		"""Move object origin to centroid"""
-		centroid = self.centroid(method=method)
-		for mesh in self._meshes:
-			set_origin(mesh, centroid)
+		:param method: Selected method to move origin to centroid
+		"""
+
+		_valid_methods = ['bounds', 'median', 'com_volume', 'com_area']
+
+		_type_lookup = dict(bounds='ORIGIN_GEOMETRY', median='ORIGIN_GEOMETRY',
+							com_volume='ORIGIN_CENTER_OF_VOLUME',
+							com_area='ORIGIN_CENTER_OF_MASS')
 
-	def get_keypoints(self, idxs=None, position=None):
+		center = 'BOUNDS' if method == 'bounds' else 'MEDIAN'
+
+		with SelectObjects(self._meshes + self._other_objects):
+			bpy.ops.object.origin_set(type=_type_lookup[method], center=center)
+
+	def get_keypoints(self, idxs: list = None, position: Union[np.ndarray, List[Vector]] = None) -> List[Vector]:
 		"""Return 3D keypoint positions in world coordinates, given either:
 
-		idxs: list of indices or ndarray of keypoints to project (only valid for single-mesh objects)
-		position: 3D position of keypoints to project - in LOCAL object coordinates
+		:param idxs: list of indices or ndarray of keypoints to project (only valid for single-mesh objects)
+		:param position: 3D position of keypoints to project - in LOCAL object coordinates
 
-		:return N list of Vectors of keypoints in world space, where N is the number of keypoints:
+		:return: N list of Vectors of keypoints in world space, where N is the number of keypoints
 		"""
 
 		assert (idxs is not None) ^ (position is not None), "Must provide either idxs or position, but not both."
 
-
 		if idxs is not None:
 			assert len(self._meshes) == 1, "Can only project keypoints by index for single-mesh objects."
 			kps3d = [self.matrix_world @ self._meshes[0].data.vertices[i].co for i in idxs]
 
 		elif position is not None:
 			kps3d = [self.matrix_world @ p for p in position]
 
 		return kps3d
 
 	@property
 	def name(self):
-		return self._meshes[0].name
+		return self._meshes[0].name
+
+	def get_armature(self, armature_name: str = None) -> bpy.types.Object:
+		"""Get armature.
+		If no name given, return first armature found.
+
+		:param armature_name: Name of armature to load."""
+
+		armatures = [obj for obj in self._other_objects if obj.type == 'ARMATURE']
+
+		if armature_name:
+			for arm in armatures:
+				if arm.name == armature_name:
+					return arm
+
+			raise KeyError(f"Armature `{armature_name}` not found.")
+
+		else:
+			if len(armatures) == 0:
+				raise ValueError("No armatures found.")
+
+			return armatures[0]
+
+	def get_bone(self, bone_name: str, armature_name: str = None) -> bpy.types.PoseBone:
+		"""
+		Get bone from armature.
+		:param bone_name:
+		:param armature_name: If not given, will load first available armature found
+		:return:
+		"""
+
+		armature = self.get_armature(armature_name)
+		try:
+			bone = armature.pose.bones[bone_name]
+		except KeyError:
+			raise KeyError(f"Bone `{bone_name}` not found in armature `{armature.name}`")
+		return bone
+
+	def pose_bone(self, bone_name: str, armature_name: str = None, rotation: Vector = None, location: Vector = None,
+				  frame: int = None):
+		"""Set the pose of a bone by giving a Euler XYZ rotation and/or location.
+
+		:param bone_name: Name of bone to pose
+		:param armature_name: Name of armature to use. If not given, will use first armature found.
+		:param rotation: Euler XYZ rotation in radians
+		:param location: Location in object space
+		:param frame: Frame to set pose on. If given, will insert keyframe here.
+		"""
+
+		with SetMode('POSE'):
+			bone = self.get_bone(bone_name, armature_name)
+			bone.rotation_mode = 'XYZ'
+			if rotation is not None:
+				bone.rotation_euler = rotation
+				if frame is not None:
+					bone.keyframe_insert(data_path='rotation_euler', frame=frame)
+
+			if location is not None:
+				bone.location = location
+				if frame is not None:
+					bone.keyframe_insert(data_path='location', frame=frame)
```

### Comparing `blendersynth-0.0.3/blendersynth/blender/utils.py` & `blendersynth-0.0.4/blendersynth/blender/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+"""Context managers and operations for handling Blender"""
+
 import bpy
 import numpy as np
 import mathutils
 
-from bpy_extras.object_utils import world_to_camera_view
-
 
 class GetNewObject():
+	"""Context manager for getting the newly imported object(s) to the scene.
+
+	On exit, will return the newly imported object(s).
+
+	Assumes that either (1) only one object is imported, or (2) there is a hierarchy to the imported objects, and the top level object is the one to return."""
+
 	def __init__(self, scene):
 		self.scene = scene
 		self.imported_obj = None
 
 	def __enter__(self):
 		self.old_objs = set(self.scene.objects)
 
@@ -28,17 +34,22 @@
 				if obj.parent is None:
 					parent_obj = obj
 					break
 
 			assert parent_obj is not None, "Multiple objects loaded,  but no parent object found..."
 			self.imported_obj = parent_obj
 
-class SelectObjects():
-	"""Context manager for selecting objects"""
-	def __init__(self, objects):
+
+class SelectObjects:
+	"""Context manager for selecting objects.
+	On exit, will reselect the objects that were selected before entering the context."""
+
+	def __init__(self, objects: list = ()):
+		"""Initialize with a list of objects to select
+		:param objects: list of bpy.types.Object"""
 		self.objects = objects
 
 	def __enter__(self):
 		self.old_objs = bpy.context.selected_objects
 		# deselect all
 		bpy.ops.object.select_all(action='DESELECT')
 
@@ -49,25 +60,54 @@
 	def __exit__(self, *args):
 		for obj in self.objects:
 			obj.select_set(False)
 
 		for obj in self.old_objs:
 			obj.select_set(True)
 
-def get_node_by_name(node_tree: bpy.types.NodeTree, key: str, raise_error=False):
-	"""Given a nodetree and a key, return the first node found with label matching key"""
+
+class SetMode:
+	"""Context manager for changing the mode of Blender (e.g.) to 'Pose',
+	returning to the original mode on exit."""
+	def __init__(self, target_mode):
+		self.target_mode = target_mode.upper()
+		self.original_mode = None
+
+	def __enter__(self):
+		self.original_mode = bpy.context.object.mode
+		bpy.ops.object.mode_set(mode=self.target_mode)
+
+	def __exit__(self, type, value, traceback):
+		bpy.ops.object.mode_set(mode=self.original_mode)
+
+
+def get_node_by_name(node_tree: bpy.types.NodeTree, key: str, raise_error=False) -> bpy.types.Node:
+	"""Given a nodetree and a key, return the first node found with label matching key.
+
+	:param node_tree: Node tree to search
+	:param key: Key to search for
+	:param raise_error: If True, raise KeyError if key not found
+	:return: Node with matching label"""
 	for node in node_tree.nodes:
 		if node.name == key:
 			return node
 
 	if raise_error:
 		raise KeyError(f"Key {key} not found in node tree!\nLabels are: {[n.name for n in node_tree.nodes]}")
 
 
-def handle_vec(vec, expected_length=3):
-	"""Check ven is expected_length. Convert from tuple or ndarray to mathutils.Vector """
+def handle_vec(vec, expected_length: int = 3) -> mathutils.Vector:
+	"""Check `vec` is expected_length. Convert from tuple or ndarray to mathutils.Vector.
+
+	:param vec: Vector to check
+	:param expected_length: Expected length of vector
+	"""
+
 	if isinstance(vec, (tuple, list)):
 		vec = mathutils.Vector(vec)
 	elif isinstance(vec, np.ndarray):
 		vec = mathutils.Vector(vec.tolist())
-	assert len(vec) == expected_length, "Vector must be length {}".format(expected_length)
-	return vec
+
+	if len(vec) != expected_length:
+		raise ValueError("Vector must be length {}".format(expected_length))
+
+	return vec
```

### Comparing `blendersynth-0.0.3/blendersynth/file/dataset_inputs.py` & `blendersynth-0.0.4/blendersynth/file/dataset_inputs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """When constructing a dataset, the INPUTS object below will
 return an iterable with read's in sys.argv's `--jobs` jsons."""
+
 import sys
 import json
 import os
 
 import logging
 
 class INPUTS:
+	"""This class is used to iterate over the JSONs passed in via `--jobs` in sys.argv."""
+	jsons = None
+	"""List of JSON files passed in via `--jobs` in sys.argv."""
+
 	def __init__(self):
 		self.jsons = sys.argv[sys.argv.index('--jobs') + 1].split(',')
 		log_loc = sys.argv[sys.argv.index('--log') + 1]
 
 		# Set up logging
 		logging.basicConfig(filename=log_loc, level=logging.INFO, filemode='w',
 							format='%(asctime)s - %(levelname)s - %(message)s')
```

### Comparing `blendersynth-0.0.3/blendersynth/file/frames_to_video.py` & `blendersynth-0.0.4/blendersynth/file/frames_to_video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import ffmpeg
 import os
 import glob
 import re
 from .tempfiles import create_temp_file
 
+from ..utils import import_module
+ffmpeg = import_module('ffmpeg', 'ffmpeg-python')
+
+
 valid_frames_exts = ('png', 'jpg', 'jpeg', 'bmp', 'tiff', 'tif')
 
 
 def get_frames_from_directory(directory, exts=valid_frames_exts, sort=True):
 	"""Return a list of all paths to files in directory which have a valid frame extension"""
 	files = [os.path.join(directory, f) for f in os.listdir(directory) if os.path.splitext(f)[-1][1:] in exts]
 	if sort:
```

### Comparing `blendersynth-0.0.3/blendersynth/run/blender_threading.py` & `blendersynth-0.0.4/blendersynth/run/blender_threading.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.3/blendersynth/run/run.py` & `blendersynth-0.0.4/blendersynth/run/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 
 from .blender_threading import BlenderThreadManager, list_split
 from ..utils.blender_setup.blender_locator import get_blender_path
-from copy import deepcopy
 from ..file.tempfiles import cleanup_temp_files as cleanup
+from typing import Union
 
 from sys import platform
+
 if platform == "linux" or platform == "linux2" or platform == "darwin":
 	nul_text = '/dev/null'
 elif platform == "win32":
 	nul_text = 'nul'
 
 
-
-
-
 class BlenderCommand:
 	"""Construct command for running blender script"""
+
 	def __init__(self, blender_loc, background=True):
 		self.blender_loc = blender_loc
 		self.background = background
 		self._command = [blender_loc, "--background" if background else ""]
 
 	def compose(self, script, args=(), **kwargs):
 		command = self._command + ["--python", script]
@@ -51,14 +50,15 @@
 
 	def set_logger(self, log_loc):
 		"""Set file for logging"""
 		cmd = self.copy()
 		cmd._command += ["--log", log_loc]
 		return cmd
 
+
 class Runner:
 	def __init__(self, script, jsons, output_directory, num_threads=1,
 				 print_to_stdout=False,
 				 **script_kwargs):
 		"""
 		:param jsons: N sized list of .json files, each with info about the given job
 		:param num_threads: threads to run in parallel (default = 1)
@@ -74,26 +74,32 @@
 		command.compose(script=script, **script_kwargs)
 
 		thread_manager = BlenderThreadManager(command, json_chunks, print_to_stdout=print_to_stdout,
 											  output_directory=output_directory)
 
 		thread_manager.start()
 
-def execute_jobs(script, json_src, output_directory, num_threads=1,
-				 print_to_stdout=False, **script_kwargs):
+
+def execute_jobs(script: str, json_src: Union[list, str], output_directory: str, num_threads: int = 1,
+				 print_to_stdout: bool = False, **script_kwargs):
 	"""
+	Execute a script, given a list of jobs to execute.
+
+	:param script: path to script to execute
 	:param json_src: N sized list of .json files, each with info about the given job. OR a directory containing .json files,
 		which will be used as the jsons
+	:param output_directory: directory to save output files
 	:param num_threads: threads to run in parallel (default = 1)
+	:param print_to_stdout: If True, print to stdout instead of saving to file
 	"""
 
-	assert not(num_threads> 1 and print_to_stdout), "Cannot print to stdout with multiple threads"
+	assert not (num_threads > 1 and print_to_stdout), "Cannot print to stdout with multiple threads"
 	if print_to_stdout:
 		raise NotImplementedError("Print to stdout not supported yet.")
 
 	if isinstance(json_src, str):
 		json_src = sorted([os.path.join(json_src, f) for f in os.listdir(json_src) if f.endswith(".json")])
 
 	Runner(script, json_src, output_directory, num_threads, print_to_stdout=print_to_stdout,
-			**script_kwargs)
+		   **script_kwargs)
 
-	cleanup()
+	cleanup()
```

### Comparing `blendersynth-0.0.3/blendersynth/utils/blender_setup/blender_locator.py` & `blendersynth-0.0.4/blendersynth/utils/blender_setup/blender_locator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,71 +6,87 @@
 import warnings
 
 appname = "blendersynth"
 appauthor = "BlenderSynth"
 config_dir = appdirs.user_config_dir(appname, appauthor)
 config_file = os.path.join(config_dir, "config.ini")
 
-def is_blender_in_path():
+
+def is_blender_in_path() -> bool:
+	"""Check if blender is in the PATH (i.e. can be run from the command line with 'blender')"""
 	return shutil.which("blender") is not None
 
-def find_blender_python(blender_path):
 
-	if read_from_config('BLENDER_PYTHON_PATH') is not None:
-		return read_from_config('BLENDER_PYTHON_PATH')
+def find_blender_python(blender_path: str) -> str:
+	"""Given a blender executable, find the python interpreter it uses
 
-	targ_script = os.path.abspath(os.path.join(os.path.dirname(__file__), 'blender_python_path.py'))
+	:param blender_path: path to blender executable"""
 
-	# open file as read & write
-	with open('___python.txt', 'w') as f:
-		try:
-			subprocess.check_call([blender_path, "--background", "--python",
-							  targ_script], stdout=f)
-		except subprocess.CalledProcessError as e:
-			raise Exception(f"Issues with finding blender python path. Error: {e}")
+	if read_from_config('BLENDER_PYTHON_PATH') is not None:
+		return read_from_config('BLENDER_PYTHON_PATH')
 
+	# get blender to run script to find python path
+	try:
+		targ_script = os.path.abspath(os.path.join(os.path.dirname(__file__), 'blender_python_path.py'))
+		output = subprocess.check_output([blender_path, "--background", "--python", targ_script])
+	except subprocess.CalledProcessError as e:
+		raise Exception(f"Issues with finding blender python path. Error: {e}")
 
+	# read output to find python path
 	out = None
-	with open('___python.txt', 'r') as f:
-		for l in f.readlines():
-			if "PYTHON INTERPRETER" in l:
-				out = l.split(": ")[1].strip()
-				break
-
-	os.remove('___python.txt')
+	for l in output.decode('utf-8').split('\n'):
+		if "PYTHON INTERPRETER" in l:
+			out = l.split(": ")[1].strip()
+			break
 
 	if out is not None:
 		write_to_config('BLENDER_PYTHON_PATH', out)
 		return out
 
 	raise Exception("Could not find Python interpreter for Blender.")
 
-def validate_blender_path(blender_path):
+
+def validate_blender_path(blender_path: str) -> bool:
+	"""Check if `blender_path` is a valid blender executable.
+
+	:param blender_path: path to blender executable"""
 	if os.access(blender_path, os.X_OK):
 		return True
 
 	return False
 
-def get_blender_path(_blender_path=None):
-	"""Get blender path in following order of precedence:
-	1. Input arg to function
-	2. In config file
-	3. Environment variable BLENDER_PATH
-	4. Blender in PATH
-	5. Ask user for path
+
+def get_blender_path(_blender_path: str = None) -> str:
+	"""Get a valid blender executable path.
+
+	To achieve this, checks in the following locations:
+
+	1) Input argument `_blender_path` (if given)
+
+	2) Config file stored in user's `appdirs.user_config_dir`
+
+	3) Environment variable `BLENDER_PATH`
+
+	4) Blender in PATH
+
+	5) Ask user for path
+
+	It will end as soon as a valid path is found. If the input path is not valid, it will raise an error.
+
+	:param _blender_path: path to blender executable
 	"""
 
 	cfg_result = read_from_config('BLENDER_PATH')
 
 	if _blender_path is not None:
 
 		if validate_blender_path(_blender_path):
 			blender_path = _blender_path
 
-		elif validate_blender_path(_blender_path + '.exe'): # add .exe if not there (helps os.access checking)
+		elif validate_blender_path(_blender_path + '.exe'):  # add .exe if not there (helps os.access checking)
 			blender_path = _blender_path + '.exe'
 
 		else:
 			raise ValueError(f"Provided Blender path, {_blender_path}, is not executable.")
 
 	elif cfg_result is not None:
 		blender_path = cfg_result
@@ -78,29 +94,30 @@
 	elif os.environ.get('BLENDER_PATH') is not None:
 		blender_path = os.environ.get('BLENDER_PATH')
 
 	elif is_blender_in_path():
 		blender_path = shutil.which("blender")
 
 	else:
-		blender_path = input("Blender not found in PATH or Environment Variable.\n"
-							 "Please provide path to blender executable: ")
+		blender_path = input(
+			"Blender not found in PATH or Environment Variable.\nPlease provide path to blender executable: ")
 
 	blender_path = os.path.abspath(blender_path)  # make sure it's absolute path
 
 	if not validate_blender_path(blender_path):
 		if validate_blender_path(blender_path + '.exe'):
 			blender_path += '.exe'
 
 		else:
 			raise ValueError(f"Provided Blender path, {blender_path}, is not valid as a Blender executable.")
 
 	write_to_config('BLENDER_PATH', blender_path)
 	return blender_path
 
+
 def write_to_config(key, value, section='BLENDER_SETUP'):
 	"""Load config, and write key value pair to cfg[section]"""
 	config = configparser.ConfigParser()
 
 	if os.path.exists(config_file):
 		config.read(config_file)
 
@@ -108,14 +125,15 @@
 		config[section] = {}
 
 	config[section][key] = value
 
 	with open(config_file, 'w') as configfile:
 		config.write(configfile)
 
+
 def read_from_config(key, section='BLENDER_SETUP'):
 	"""Load config, and read value from cfg[section]"""
 	config = configparser.ConfigParser()
 
 	if os.path.exists(config_file):
 		config.read(config_file)
 
@@ -123,14 +141,15 @@
 		return None
 
 	if key not in config[section]:
 		return None
 
 	return config[section][key]
 
+
 def remove_from_config(key, section='BLENDER_SETUP'):
 	"""Load config, and remove key from cfg[section]"""
 	config = configparser.ConfigParser()
 
 	if os.path.exists(config_file):
 		config.read(config_file)
 
@@ -141,11 +160,12 @@
 		return None
 
 	del config[section][key]
 
 	with open(config_file, 'w') as configfile:
 		config.write(configfile)
 
+
 def remove_config():
 	"""Remove config file"""
 	if os.path.exists(config_file):
 		os.remove(config_file)
```

### Comparing `blendersynth-0.0.3/blendersynth/utils/blender_setup/check_blender_install.py` & `blendersynth-0.0.4/blendersynth/utils/blender_setup/check_blender_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,20 +55,24 @@
 
 	if not read_from_config('DEPENDENCIES_INSTALLED') == 'True':
 		# check if blender's python has all necessary packages
 		for dependency in dependencies:
 			if not check_module(python_path, dependency):
 				install_module(python_path, dependency)
 
+		# First uninstall blendersynth if present (in case of updates)
+		if check_module(python_path, 'blendersynth'):
+			subprocess.check_call([python_path, '-m', 'pip', 'uninstall', '-y', 'blendersynth'])
+
 		# Install blendersynth package to blender's python
 		if blendersynth_from_local:
 			# Install from local setup.py
-			setup_py_loc = os.path.join(os.path.dirname(__file__), '..', '..', 'setup.py')
-			if not os.path.isfile('setup.py'):
+			setup_py_loc = os.path.join(os.path.dirname(__file__), '..', '..', '..', 'setup.py')
+			if not os.path.isfile(setup_py_loc):
 				raise Exception(f"Could not find setup.py at {setup_py_loc}.")
-			subprocess.check_call([python_path, 'setup.py', 'install'])
+			subprocess.check_call([python_path, setup_py_loc, 'install'])
 
 		else:
 			# Install from pypi
 			install_module(python_path, 'blendersynth', upgrade=True)
 
 		write_to_config('DEPENDENCIES_INSTALLED', 'True')
```

### Comparing `blendersynth-0.0.3/blendersynth/utils/node_arranger.py` & `blendersynth-0.0.4/blendersynth/utils/node_arranger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-"""Space out nodes in the node editor."""
+"""Utilities for neatly arranging nodes in the node editor,
+to make debugging easier."""
+
 import bpy
 from collections import defaultdict
 from copy import copy
 
 
 def get_source_nodes(node):
 	for i in node.inputs:
 		for link in i.links:
 			yield link.from_node
 
+
 def get_sink_nodes(node):
 	for o in node.outputs:
 		for link in o.links:
 			yield link.to_node
 
+
 def split_to_islands(nodes):
 	"""Given a node list, return a list of sets, each one being a fully disconnected island"""
 
 	def dfs(node, island):
 		"""Depth-first search from node."""
 		node['visited'] = True
 		islands[node] = island
@@ -82,39 +86,40 @@
 			sources = [s for s in get_source_nodes(node) if s in node_island]
 			if sources:
 				new_depth = max(node['depth'] for node in sources) + 1
 				if node['depth'] != new_depth:
 					node['depth'] = new_depth
 					depth_changed = True
 
-
 	# Normalize depths
 	min_depth = min(node['depth'] for node in node_island)
 	for node in node_island:
 		node['depth'] -= min_depth
 
 	return node_island
 
 
-def tidy_tree(node_tree, dX = 400, dY = 200):
-	"""Search through tree, and position nodes in a grid"""
+def tidy_tree(node_tree: bpy.types.NodeTree, dX: int = 400, dY: int = 200):
+	"""Search through tree, positioning nodes in a grid based on their depth and connectivity.
+
+	:param node_tree: node tree to tidy
+	:param dX: horizontal distance between nodes
+	:param dY: vertical distance between nodes"""
 
 	nodes = node_tree.nodes
 	islands = split_to_islands(nodes)
 
-	y = 0 # track running height to manage multiple islands
+	y = 0  # track running height to manage multiple islands
 
-	height = defaultdict(int) # track height of each depth level
+	height = defaultdict(int)  # track height of each depth level
 	for island in islands:
 		island = calc_depth(island)
 
 		# want to centre each depth level, so set heights accordingly
 		for i in range(max(node['depth'] for node in island) + 1):
 			height[i] = - dY * sum(node['depth'] == i for node in island) / 2
 
 		for node in island:
 			node.location = (node['depth'] * dX, y + height[node['depth']])
 			height[node['depth']] += dY
 
 		y += max(height.values()) + dY
-
-
```

