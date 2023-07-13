# Comparing `tmp/model-railway-signals-3.4.0.tar.gz` & `tmp/model-railway-signals-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/model-railway-signals-3.4.0.tar", last modified: Sun Jun 18 15:02:23 2023, max compression
+gzip compressed data, was "dist/model-railway-signals-3.4.1.tar", last modified: Thu Jul 13 09:50:14 2023, max compression
```

## Comparing `model-railway-signals-3.4.0.tar` & `model-railway-signals-3.4.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     6386 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     5042 2023-06-18 14:44:25.000000 model-railway-signals-3.4.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/
--rw-r--r--   0 pi        (1000) pi        (1000)     6829 2023-06-13 19:27:26.000000 model-railway-signals-3.4.0/model_railway_signals/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    49919 2023-05-17 19:17:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    17917 2023-06-12 20:31:04.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_instrument.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10609 2023-06-18 14:35:52.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_line.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21296 2023-05-17 19:02:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_point.py
--rw-r--r--   0 pi        (1000) pi        (1000)    22142 2023-06-04 18:46:34.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_section.py
--rw-r--r--   0 pi        (1000) pi        (1000)    58536 2023-05-17 19:02:52.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal.py
--rw-r--r--   0 pi        (1000) pi        (1000)    53376 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab1.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21732 2023-05-17 18:48:48.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab2.py
--rw-r--r--   0 pi        (1000) pi        (1000)    34207 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab3.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21192 2023-06-18 13:48:39.000000 model-railway-signals-3.4.0/model_railway_signals/editor/editor.py
--rw-r--r--   0 pi        (1000) pi        (1000)    22191 2023-06-18 14:03:21.000000 model-railway-signals-3.4.0/model_railway_signals/editor/menubar_windows.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/
--rw-r--r--   0 pi        (1000) pi        (1000)     6067 2023-04-30 08:41:38.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    32300 2023-06-17 07:57:59.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9959 2023-05-03 18:46:06.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13178 2023-05-17 19:28:08.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13260 2023-05-17 19:28:02.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_lines.py
--rw-r--r--   0 pi        (1000) pi        (1000)    20191 2023-05-03 18:38:12.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_points.py
--rw-r--r--   0 pi        (1000) pi        (1000)    18889 2023-04-30 05:47:14.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    50424 2023-06-13 19:24:44.000000 model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_signals.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2900 2023-05-03 17:52:46.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow1.png
--rw-r--r--   0 pi        (1000) pi        (1000)     2914 2023-05-03 17:54:08.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow2.png
--rw-r--r--   0 pi        (1000) pi        (1000)     2927 2023-05-03 17:55:10.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow3.png
--rw-r--r--   0 pi        (1000) pi        (1000)     2933 2023-05-03 17:55:54.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow4.png
--rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/colourlight.png
--rw-r--r--   0 pi        (1000) pi        (1000)     2858 2023-04-30 16:09:28.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/endstop.png
--rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/grounddisc.png
--rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/groundpos.png
--rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/instrument.png
--rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/lhpoint.png
--rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/line.png
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/rhpoint.png
--rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/section.png
--rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/editor/resources/semaphore.png
--rw-r--r--   0 pi        (1000) pi        (1000)    55559 2023-05-23 20:06:32.000000 model-railway-signals-3.4.0/model_railway_signals/editor/run_layout.py
--rw-r--r--   0 pi        (1000) pi        (1000)    42689 2023-06-17 07:57:38.000000 model-railway-signals-3.4.0/model_railway_signals/editor/schematic.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9149 2023-06-18 14:04:31.000000 model-railway-signals-3.4.0/model_railway_signals/editor/settings.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/library/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    56398 2023-06-04 19:20:01.000000 model-railway-signals-3.4.0/model_railway_signals/library/block_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6481 2023-05-17 20:19:26.000000 model-railway-signals-3.4.0/model_railway_signals/library/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    43946 2023-06-04 19:34:10.000000 model-railway-signals-3.4.0/model_railway_signals/library/dcc_control.py
--rw-r--r--   0 pi        (1000) pi        (1000)    23696 2023-05-17 20:22:42.000000 model-railway-signals-3.4.0/model_railway_signals/library/file_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    20005 2023-06-14 19:04:40.000000 model-railway-signals-3.4.0/model_railway_signals/library/mqtt_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    31597 2023-05-17 20:24:20.000000 model-railway-signals-3.4.0/model_railway_signals/library/pi_sprog_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    26152 2023-05-17 20:25:20.000000 model-railway-signals-3.4.0/model_railway_signals/library/points.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-02.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-03.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-04.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-04-22 17:13:00.000000 model-railway-signals-3.4.0/model_railway_signals/library/resources/telegraph-key-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    50923 2023-06-04 19:13:19.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals.py
--rw-r--r--   0 pi        (1000) pi        (1000)    46806 2023-06-14 19:51:48.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_colour_lights.py
--rw-r--r--   0 pi        (1000) pi        (1000)    39299 2023-06-14 20:26:52.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7712 2023-06-14 19:16:38.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_disc.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10104 2023-06-14 19:16:30.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_position.py
--rw-r--r--   0 pi        (1000) pi        (1000)    55797 2023-06-14 19:51:58.000000 model-railway-signals-3.4.0/model_railway_signals/library/signals_semaphores.py
--rw-r--r--   0 pi        (1000) pi        (1000)    27709 2023-06-04 19:12:12.000000 model-railway-signals-3.4.0/model_railway_signals/library/track_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13717 2023-05-17 20:33:06.000000 model-railway-signals-3.4.0/model_railway_signals/library/track_sensors.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6386 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3338 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-06-18 15:02:20.000000 model-railway-signals-3.4.0/model_railway_signals.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-18 15:02:23.000000 model-railway-signals-3.4.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-06-18 14:04:57.000000 model-railway-signals-3.4.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/MANIFEST.in
+-rw-r--r--   0 pi        (1000) pi        (1000)     6017 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     4705 2023-07-13 09:32:57.000000 model-railway-signals-3.4.1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6829 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/__main__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/editor/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/editor/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    49919 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    18172 2023-07-13 07:54:31.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_instrument.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10609 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_line.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21304 2023-07-13 07:54:44.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_point.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20603 2023-07-13 09:01:22.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_section.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    58573 2023-07-13 08:23:06.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    53936 2023-07-13 07:55:03.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab1.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    22190 2023-07-13 08:07:05.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab2.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    35324 2023-07-13 08:22:30.000000 model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab3.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21731 2023-07-12 14:58:24.000000 model-railway-signals-3.4.1/model_railway_signals/editor/editor.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    22191 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/menubar_windows.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6067 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    32377 2023-07-12 14:45:35.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9959 2023-07-12 16:48:51.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13015 2023-07-11 15:29:40.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13260 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_lines.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    17910 2023-07-11 15:29:40.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_points.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    18889 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    50424 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_signals.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2900 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow1.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2914 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow2.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2927 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow3.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2933 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow4.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/colourlight.png
+-rw-r--r--   0 pi        (1000) pi        (1000)     2858 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/endstop.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/grounddisc.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/groundpos.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/instrument.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/lhpoint.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/line.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/rhpoint.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/section.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/editor/resources/semaphore.png
+-rw-r--r--   0 pi        (1000) pi        (1000)    55559 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/editor/run_layout.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    42904 2023-07-12 13:34:40.000000 model-railway-signals-3.4.1/model_railway_signals/editor/schematic.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9149 2023-07-13 09:30:51.000000 model-railway-signals-3.4.1/model_railway_signals/editor/settings.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/library/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    55457 2023-07-11 17:02:39.000000 model-railway-signals-3.4.1/model_railway_signals/library/block_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6481 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    43946 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/dcc_control.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    23696 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/file_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20005 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/mqtt_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    31597 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/pi_sprog_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    28397 2023-07-11 15:29:40.000000 model-railway-signals-3.4.1/model_railway_signals/library/points.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-02.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-03.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-04.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-04-22 17:13:00.000000 model-railway-signals-3.4.1/model_railway_signals/library/resources/telegraph-key-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    50923 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    46806 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals_colour_lights.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    39299 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7712 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals_ground_disc.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10104 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals_ground_position.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    55797 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/signals_semaphores.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    27709 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/track_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13717 2023-06-18 15:38:55.000000 model-railway-signals-3.4.1/model_railway_signals/library/track_sensors.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6017 2023-07-13 09:50:12.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     3338 2023-07-13 09:50:12.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-13 09:50:12.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-07-13 09:50:12.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-07-13 09:50:12.000000 model-railway-signals-3.4.1/model_railway_signals.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-07-13 09:50:14.000000 model-railway-signals-3.4.1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-07-13 09:30:22.000000 model-railway-signals-3.4.1/setup.py
```

### Comparing `model-railway-signals-3.4.0/PKG-INFO` & `model-railway-signals-3.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.4.0
+Version: 3.4.1
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
@@ -25,26 +25,22 @@
         What's currently supported by the Editor:
         * Draw your schematic with lines, points, signals, track occupancy sections and block instruments
         * Define the DCC command sequences needed to drive the signals and points out on the layout
         * Configure the signals, points and block instruments for protototypical interlocking
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
         * Configure a level of automation for the signals as trains traverse the layout
         
-        What's New in Release 3.4.0:
-        * Point and line colour selections - to enable colour coding of routes
-        * Line end-style selections - end-stops and arrow styles can now be specified
-        * Enhanced error/warning reporting via popups - reduced reliance on logs
-        * Layout 'info' function (under Help) allows you to add notes for your layout
-        * Fixed issue when selecting objects if Canvas is scrolled within the main window
-        * Various window geometry improvements to keep key UI elements visible on resizing
-        * Track section occupancy logic corrected for passing shunt-ahead ground signals
+        What's new in Release 3.4.1:
+        * Minor bug fixes and enabling work for MQTT networking
+        * Improvements to the operation of single line block instruments
+        * Some block instrument library API functions have been DEPRECATED (see PUBLIC_API.md)
         
         What's coming soon:
         * MQTT networking (for linking layouts)
-        * Better pplication documentation
+        * Better application documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
         
         There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.4.0/README.md` & `model-railway-signals-3.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,22 @@
 What's currently supported by the Editor:
 * Draw your schematic with lines, points, signals, track occupancy sections and block instruments
 * Define the DCC command sequences needed to drive the signals and points out on the layout
 * Configure the signals, points and block instruments for protototypical interlocking
 * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
 * Configure a level of automation for the signals as trains traverse the layout
 
-What's New in Release 3.4.0:
-* Point and line colour selections - to enable colour coding of routes
-* Line end-style selections - end-stops and arrow styles can now be specified
-* Enhanced error/warning reporting via popups - reduced reliance on logs
-* Layout 'info' function (under Help) allows you to add notes for your layout
-* Fixed issue when selecting objects if Canvas is scrolled within the main window
-* Various window geometry improvements to keep key UI elements visible on resizing
-* Track section occupancy logic corrected for passing shunt-ahead ground signals
+What's new in Release 3.4.1:
+* Minor bug fixes and enabling work for MQTT networking
+* Improvements to the operation of single line block instruments
+* Some block instrument library API functions have been DEPRECATED (see PUBLIC_API.md)
 
 What's coming soon:
 * MQTT networking (for linking layouts)
-* Better pplication documentation
+* Better application documentation
 
 Any bug reports and feedback you may have would be gratefully appreciated - specifically:
 * What aspects are intuitive? What aspects aren't?
 * What aspects do you particularly like?
 * What aspects particularly irritate you?
 
 There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/__init__.py` & `model-railway-signals-3.4.1/model_railway_signals/__init__.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/common.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_instrument.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
 #    edit_instrument - Open the edit block instrument top level window
 #
 # Makes the following external API calls to other editor modules:
 #    objects.update_object(obj_id,new_obj) - Update the configuration on save
+#    objects.instrument_exists(id) - To see if the instrument exists (local or remote)
 #
 # Accesses the following external editor objects directly:
 #    objects.signal_index - To iterate through all the signal objects
 #    objects.schematic_objects - To load/save the object configuration
 #
 # Makes the following external API calls to library modules:
 #    block_instruments.instrument_exists(id) - To see if the instrument exists
@@ -155,16 +156,16 @@
 #    "set_value" - will set the current value of the entry box (str)
 #    "get_value" - will return the last "valid" value of the entry box (str)
 #    "validate" - Validates the instrument exists and not the current inst_id
 #------------------------------------------------------------------------------------
 
 class linked_to_selection(common.str_item_id_entry_box):
     def __init__(self, parent_frame, parent_object):
-        # These are the functions used to validate that the entered ID
-        # exists on the schematic and is different to the current ID
+        # The exists_function from the block_instruments module is used to validate that the
+        # entered ID  exists on the schematic or has been subscribed to via mqtt networking
         exists_function = block_instruments.instrument_exists
         current_id_function = parent_object.instid.get_value
         # Create the Label Frame for the "also switch" entry box
         self.frame = Tk.LabelFrame(parent_frame, text="Block section")
         # Call the common base class init function to create the EB
         self.label1 = Tk.Label(self.frame,text="Linked block instrument:")
         self.label1.pack(side=Tk.LEFT, padx=2, pady=2)
@@ -259,17 +260,18 @@
 #------------------------------------------------------------------------------------
 
 class instrument_configuration_tab():
     def __init__(self, parent_tab):
         # Create a Frame to hold the Inst ID and Inst Type Selections
         self.frame = Tk.Frame(parent_tab)
         self.frame.pack(padx=2, pady=2, fill='x')
-        # Create the UI Element for Inst ID selection
+        # Create the UI Element for Inst ID selection - Note that we use the instrument_exists
+        # function from the objects module - as we are only interested in local instruments
         self.instid = common.object_id_selection(self.frame, "Inst ID",
-                        exists_function = block_instruments.instrument_exists) 
+                        exists_function = objects.instrument_exists) 
         self.instid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
         # Create the UI Element for Inst Type selection
         self.insttype = common.selection_buttons(self.frame, "Point type",
                     "Select block Instrument Type", None, "Single line", "Double Line")
         self.insttype.frame.pack(padx=2, pady=2, fill='x')
         self.linkedto = linked_to_selection(parent_tab, self)
         self.linkedto.frame.pack(padx=2, pady=2, fill='x')
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_line.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_line.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_point.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
 #    edit_point - Open the edit point top level window
 #
 # Makes the following external API calls to other editor modules:
 #    objects.update_object(obj_id,new_obj) - Update the configuration on save
-#    objects.point_exists(point_id) - To see if a specified point ID exists
+#    objects.point_exists(point_id) - To see if a specified point ID exists (local)
 #    objects.point(point_id) - To get the object_id for a given point_id
 #
 # Accesses the following external editor objects directly:
 #    objects.point_index - To iterate through all the point objects
 #    objects.schematic_objects - To load/save the object configuration
 #
 # Inherits the following common editor base classes (from common):
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_section.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_section.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
 #    edit_section - Open the edit section top level window
 #
 # Makes the following external API calls to other editor modules:
 #    objects.update_object(obj_id,new_obj) - Update the configuration on save
-#    objects.section_exists(section_id) - To see if a specified section ID exists
+#    objects.section_exists(section_id) - To see if a specified section ID exists (local)
 #    objects.section(section_id) - To get the object_id for a given section ID
 #
 # Accesses the following external editor objects directly:
 #    objects.section_index - To iterate through all the section objects
 #    objects.schematic_objects - To load/save the object configuration
 #
+# Makes the following external API calls to library modules:
+#    track_sections.section_exists(id) - To see if the section exists (remote)
+#
 # Inherits the following common editor base classes (from common):
 #    common.check_box
 #    common.str_item_id_entry_box
 #    common.object_id_selection
 #    common.signal_route_selections
 #    common.window_controls
 #
@@ -27,29 +30,15 @@
 
 import tkinter as Tk
 from tkinter import ttk
 
 from . import common
 from . import objects
 
-#------------------------------------------------------------------------------------
-# Function to return the read-only "mirrored by" parameter. This is the back-reference
-# to the section that is configured to mirror the current section (else zero). This
-# is only used within the UI so doesn't need to be tracked in the section object dict
-# Note that the mirrored element is a string to support local and remote sections
-#------------------------------------------------------------------------------------
-
-def mirrored_by_section(object_id):
-    mirrored_by_section_id = ""
-    for section_id in objects.section_index:
-        mirrored_section_id = objects.schematic_objects[objects.section(section_id)]["mirror"]
-        if mirrored_section_id == str(objects.schematic_objects[object_id]["itemid"]):
-            mirrored_by_section_id = section_id
-    return(mirrored_by_section_id)
-
+from ..library import track_sections
 
 #------------------------------------------------------------------------------------
 # Helper Function to return the list of available signal routes for the signal ahead
 #------------------------------------------------------------------------------------
 
 def get_signal_routes(object_id):
     sig_routes = objects.schematic_objects[object_id]["sigroutes"]
@@ -109,15 +98,14 @@
     else:
         # Label the edit window with the Section ID
         section.window.title("Track Section "+str(objects.schematic_objects[object_id]["itemid"]))
         # Set the Initial UI state from the current object settings
         section.config.sectionid.set_value(objects.schematic_objects[object_id]["itemid"])
         section.config.readonly.set_value(not objects.schematic_objects[object_id]["editable"])
         section.config.mirror.set_value(objects.schematic_objects[object_id]["mirror"])
-        section.config.mirror.set_mirrored_by(mirrored_by_section(object_id))
         section.config.label.set_value(objects.schematic_objects[object_id]["defaultlabel"])
         section.automation.ahead.set_values(signals_ahead(object_id))
         section.automation.behind.set_values(signals_behind(object_id))
     return()
     
 #------------------------------------------------------------------------------------
 # Function to commit all configuration changes (Apply/OK Button)
@@ -172,49 +160,30 @@
 # Class instance methods provided by this class are:
 #    "validate" - Also validate the section is not mirrored by another section
 #    "set_mirrored_by" - to set the read-only value for the "mirrored_by" section
 #------------------------------------------------------------------------------------
 
 class mirrored_section(common.str_item_id_entry_box):
     def __init__(self, parent_frame, parent_object):
-        # These are the functions used to validate that the entered signal ID
-        # exists on the schematic and is different to the current signal ID
-        ##################################################################################
-        ### TODO - when we eventually support remote sections we can't use the current ###
-        ### section_exists function as that only checks if the section exists in the   ###
-        ### dictionary of schematic objects so won't pick up any sections subscribed   ###
-        ### to via the MQTT networking - we'll therefore have to use the internal      ###
-        ### library function or validate also against a list of subscribed sections    ###
-        ### Note that the validation function will also need to change                 ###
-        ##################################################################################
-        exists_function = objects.section_exists
+        # These are the functions used to validate that the entered section ID
+        # exists on the schematic and is different to the current section ID
+        exists_function = self.section_exists
         current_id_function = parent_object.sectionid.get_value
         # Create the Label Frame for the "mirrored section" entry box
         self.frame = Tk.LabelFrame(parent_frame, text="Link to other track section")
         # Create a frame for the "Section to mirror" elements
         self.subframe1 = Tk.Frame(self.frame)
         self.subframe1.pack()
         # Call the common base class init function to create the EB
         self.label1 = Tk.Label(self.subframe1,text="Section to mirror:")
         self.label1.pack(side=Tk.LEFT, padx=2, pady=2)
         super().__init__(self.subframe1, tool_tip = "Enter the ID of the track section to mirror - This can "+
                     "be a local section or a remote section (subscribed to via MQTT networking)",
                     exists_function=exists_function, current_id_function=current_id_function)
         self.pack(side=Tk.LEFT, padx=2, pady=2)
-        # Create a frame for the "Mirrored by" elements
-        self.subframe2 = Tk.Frame(self.frame)
-        self.subframe2.pack()
-        self.mirrored_by = Tk.StringVar(parent_frame, "")
-        self.label2 = Tk.Label(self.subframe2,text="Mirrored by section:")
-        self.label2.pack(side=Tk.LEFT, padx=2, pady=2)
-        self.mirrored_by_eb = Tk.Entry(self.subframe2, width=3, textvariable=self.mirrored_by,
-                                            justify='center',state="disabled")
-        self.mirrored_by_eb.pack(side=Tk.LEFT, padx=2, pady=2)
-        self.TT1 = common.CreateToolTip(self.mirrored_by_eb, "ID of the track "+
-                            "section that that will be mirrored by this section")
 
     def validate(self):
         # Do the basic item validation first (exists and not current item ID)
         valid = super().validate(update_validation_status=False)
         if valid and self.entry.get() != "":
             mirrored_section = int(self.entry.get())
             # Test to see if the entered section is already being mirrored by another section
@@ -226,37 +195,46 @@
                 else: other_mirrored = int(other_section)
                 if other_mirrored == mirrored_section and mirrored_section != initial_mirrored:
                     self.TT.text = ("Track section "+str(mirrored_section)+" is already "+
                                           "mirrored by section "+section_id)
                     valid = False       
         self.set_validation_status(valid)
         return(valid)
-
-    def set_mirrored_by(self, section_id:str):
-        # Strings are used as the mirrored element supports local or remote sections
-        self.mirrored_by.set(section_id)
+    
+    # We would normally use the library 'section_exists' function to determine if a track section
+    # either exists on the local schematic OR has been subscribed to via MQTT networking, but the
+    # local track section library objects don't exist when in edit mode (although the function
+    # will report that any remote sections subscribed to via MQTT networking do exist). We
+    # therefore need to create a hybrid 'exists' function using a combination of the exists
+    # functions from the objects module and the library modules
+    def section_exists(self, sec_id):
+        return (objects.section_exists(sec_id) or track_sections.section_exists(sec_id))
 
 #------------------------------------------------------------------------------------
 # Class for the Default lable entry box - builds on the common entry_box class
 # Inherited class methods are:
 #    "set_value" - set the initial value of the entry box (string) 
 #    "get_value" - get the last "validated" value of the entry box (string)
 # Overriden class methods are
 #    "validate" - Validates the length of the entered text (between 2-10 chars)
 #------------------------------------------------------------------------------------
 
 class default_label_entry(common.entry_box):
     def __init__(self, parent_frame):
         # Create the Label Frame for the "mirrored section" entry box
         self.frame = Tk.LabelFrame(parent_frame, text="Default section label")
+        self.packing1 = Tk.Label(self.frame, width=6)
+        self.packing1.pack(side=Tk.LEFT)
         super().__init__(self.frame, width=16, tool_tip = "Enter the default label to "+
                          "display when the section is occupied (this defines the default "+
                          "width of the Track Section object on the schematic). The default "+
                          "label should be between 4 and 10 characters")
-        self.pack(padx=2, pady=2)
+        self.pack(side=Tk.LEFT, padx=2, pady=2)
+        self.packing2 = Tk.Label(self.frame, width=6)
+        self.packing2.pack(side=Tk.LEFT)
 
     def validate(self):
         label = self.entry.get()
         if len(label) >= 4 and len(label) <=10:
             valid = True
         else:
             valid = False
@@ -368,18 +346,18 @@
         self.tabs.add(self.tab1, text="Configration")
         self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Automation")
         self.tabs.pack(fill='x')
         self.config = section_configuration_tab(self.tab1)
         self.automation = section_automation_tab(self.tab2)        
         # Create the common Apply/OK/Reset/Cancel buttons for the window
-        self.controls = common.window_controls(self.main_frame, self, load_state, save_state)
+        self.controls = common.window_controls(self.window, self, load_state, save_state)
         self.controls.frame.pack(padx=2, pady=2)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
-        self.validation_error = Tk.Label(self.main_frame, text="Errors on Form need correcting", fg="red")
+        self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
         # THIS IS STILL NOT WORKING AS IT LEAVES THE ENTRY BOX HIGHLIGHTED
         # self.window.focus()
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #------------------------------------------------------------------------------------
 # This module contains all the ui functions for configuring Signal objects
 #------------------------------------------------------------------------------------
 #
 # External API functions intended for use by other editor modules:
-#    edit_signal - Open the edit point wtop level window
+#    edit_signal - Open the edit point top level window
 #
 # Makes the following external API calls to other editor modules:
 #    objects.update_object(obj_id,new_obj) - Update the configuration of the signal object
-#    objects.signal_exists(point_id) - To see if a specified signal ID exists
-#    objects.signal(point_id) - To get the object_id for a given signal_id
 #
 # Accesses the following external editor objects directly:
-#    objects.signal_index - To iterate through all the point objects
 #    objects.schematic_objects - To load/save the object configuration
 #
+# Accesses the following types directly from the library modules:
+#    signals_common.sig_type - The sygnal type
+#    signals_colour_lights.signal_sub_type - colour light signal sub-type
+#    signals_semaphores.semaphore_sub_type - semaphore signal sub-type
+#
 # Uses the classes from the following modules for each configuration tab:
 #    configure_signal_tab1 - General signal configuration
 #    configure_signal_tab2 - Point and signal interlocking
 #    configure_signal_tab3 - signal automation
 #    common.window_controls - the common load/save/cancel/OK controls
 #------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab1.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 #------------------------------------------------------------------------------------
-# Functions and sub Classes for the Edit Signal "Configuration" Tab 
+# Functions and sub Classes for the Edit Signal "Configuration" Tab
+#
+# Makes the following external API calls to other editor modules:
+#    objects.signal_exists(id) - To see if the signal exists (local)
+#
+# Inherits the following common editor base classes (from common):
+#    common.int_item_id_entry_box
+#    common.entry_box
+#    common.check_box
+#    common.dcc_entry_box
+#    common.dcc_command_entry
+#    common.object_id_selection
+#    common.selection_buttons
 #------------------------------------------------------------------------------------
 
 import tkinter as Tk
 
-from . import common
 from . import objects
+from . import common
 
 #------------------------------------------------------------------------------------
 # Class for the General Settings UI Element - Builds on the common checkbox class
 # Public class instance methods inherited from the base check box class are:
 #    "set_value" - set the initial value of the Rotate checkbutton (int) 
 #    "get_value" - get the last "validated" value of the Rotate checkbutton (int) 
 #------------------------------------------------------------------------------------
@@ -1009,14 +1021,16 @@
 #------------------------------------------------------------------------------------
 
 class signal_configuration_tab:
     def __init__(self, parent_tab, sig_type_updated, sub_type_updated,
                 route_type_updated, route_selections_updated, sig_routes_updated,
                 sub_routes_updated, dist_routes_updated):
         # Create a Frame for the Sig ID and Signal Type Selections (always packed)
+        # Note that for the Sig ID selection we use the signal_exists function 
+        # from the objects module - as we are only interested in local signals
         self.frame1 = Tk.Frame(parent_tab)
         self.frame1.pack(padx=2, pady=2, fill='x')
         self.sigid = common.object_id_selection(self.frame1,"Signal ID",
                                 exists_function = objects.signal_exists)
         self.sigid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='both')
         self.sigtype = common.selection_buttons(self.frame1,"Signal Type",
                     "Select signal type",sig_type_updated,"Colour Light",
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab2.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 #------------------------------------------------------------------------------------
-# Functions and sub Classes for the Edit Signal "Interlocking" Tab 
+# Functions and sub Classes for the Edit Signal "Interlocking" Tab
+#
+# Makes the following external API calls to other editor modules:
+#    objects.point_exists(id) - To see if the point exists (local)
+#    objects.signal_exists(id) - To see if the point exists (local)
+#
+# Makes the following external API calls to library modules:
+#    signals_common.sig_exists(id) - To see if the instrument exists (local or remote)
+#    block_instruments.instrument_exists(id) - To see if the instrument exists (local or remote)
+#
+# Inherits the following common editor base classes (from common):
+#    common.check_box
+#    common.state_box
+#    common.int_item_id_entry_box
+#    common.str_item_id_entry_box
+#    common.signal_route_selections
 #------------------------------------------------------------------------------------
 
 import tkinter as Tk
 
 from . import common
 from . import objects
 
+from ..library import signals_common
+from ..library import block_instruments
+
 #------------------------------------------------------------------------------------
 # Class for a point interlocking entry element (point_id + point_state)
 # Uses the common int_item_id_entry_box and state_box classes
 # Public class instance methods provided are:
 #    "validate" - validate the current entry box value and return True/false
 #    "set_value" - will set the current value [point_id:int, state:bool]
 #    "get_value" - will return the last "valid" value [point_id:int, state:bool]
@@ -68,27 +86,21 @@
 #    "disable_sig_ahead" - disables the Sig ahead selections
 #    "enable_block_ahead" - enables the block ahead selections (if the route is enabled)
 #    "disable_block_ahead" - disables the block ahead selections
 #------------------------------------------------------------------------------------
 
 class interlocking_route_group: 
     def __init__(self, parent_frame, parent_object, label:str):
-        # These are the functions used to validate that the entered IDs exist
-        # on the schematic (and the sig ID is different to the current sig ID) 
-        #################################################################################
-        ### TODO - when we eventually support remote signals we can't use the current ###
-        ### signal_exists function as that only checks if the signal exists in the    ###
-        ### dictionary of schematic objects so won't pick up any signals subscribed   ###
-        ### to via the MQTT networking - we'll therefore have to use the internal     ###
-        ### library function or validate also against a list of subscribed signals    ###                
-        #################################################################################
-        instrument_exists_function = objects.instrument_exists
-        signal_exists_function = objects.signal_exists
+        # Note that for the interlocked point selections we validate using the point_exists function 
+        # from the objects module - as we are only interested in local points. For the signal ahead
+        # and block instrument ahead selections, we use the exists function from the library modules
+        # as to validate the items exist on the schematic or have been subscribed to via MQTT networking
+        signal_exists_function = signals_common.sig_exists
         current_id_function = parent_object.config.sigid.get_value
-        instrument_exists_function = objects.instrument_exists
+        instrument_exists_function = block_instruments.instrument_exists
         point_exists_function = objects.point_exists
         # Create a frame for this UI element (always packed into the parent frame)
         self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the lable and the point interlocking entry elements (these are
         # packed LEFT in the frame by the parent class when created)
         self.label = Tk.Label(self.frame, anchor='w', width=5, text=label)
@@ -267,16 +279,18 @@
 #    "enable_route" - Enables/loads all selections for the route
 #    "disable_route" - Disables/blanks all selections for the route
 #    "validate" - Validates all Entry boxes (Signals exist and not current ID) 
 #------------------------------------------------------------------------------------
 
 class conflicting_signals_element():
     def __init__(self, parent_frame, parent_object, label:str):
-        # These are the functions used to validate that the entered signal ID
-        # exists on the schematic and is different to the current signal ID
+        # These are the functions used to validate that the entered signal ID  exists on the
+        # schematic and is different to the current signal ID - note that we only allow
+        # interlocking with signals on the local schematic - so we use the signal_exists
+        # function from the objects module
         exists_function = objects.signal_exists
         current_id_function = parent_object.config.sigid.get_value
         # Create the Label Frame for the UI element (packed/unpacked on enable/disable) 
         self.frame = Tk.LabelFrame(parent_frame, text=label+" - interlocking with conflicting signals")
         self.frame.pack(padx=2, pady=2, fill='x')
         # create two frames - each frame will hold two conflicting signals
         self.subframe1 = Tk.Frame(self.frame)
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/configure_signal_tab3.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/configure_signal_tab3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 #------------------------------------------------------------------------------------
 # Functions and sub Classes for the Edit Signal "Automation" Tab
+#
+# Makes the following external API calls to other editor modules:
+#    objects.section_exists(id) - To see if the section exists (local)
+#    objects.signal_exists(id) - To see if the signal exists (local)
+#    objects.signal(id) - to get the object ID of a given item ID
+#
+# Accesses the following external editor objects directly:
+#    objects.signal_index - To iterate through all the signal objects
+#    objects.schematic_objects - To load/save the object configuration
+#
+# Inherits the following common editor base classes (from common):
+#    common.check_box
+#    common.integer_entry_box
+#    common.int_item_id_entry_box
+#    common.CreateToolTip
+#
 #------------------------------------------------------------------------------------
 
 import tkinter as Tk
 
 from . import common
 from . import objects
 
@@ -94,14 +110,18 @@
 # Public Class instance methods (inherited from the base class) are
 #    "disable" - disables/blanks the entry box 
 #    "enable"  enables/loads the entry box
 #    "set_value" - will set the current value (integer)
 #    "get_value" - will return the last "valid" value (integer)
 # Public Class instance methods provided by the section_ahead_frame class:
 #    "validate" - validate all 'section ahead' entry box values and return True/false
+#
+# Note that the software only supports automation of track sections on the local schematic
+# (local sections should be created to 'mirror' remote sections for networked layouts)
+# so we use the section_exists function from the objects module for entry validation
 #------------------------------------------------------------------------------------
 
 class section_behind_element(common.int_item_id_entry_box):
     def __init__(self, parent_frame):
         self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         self.label1 = Tk.Label(self.frame, width=1)
@@ -242,14 +262,17 @@
 # Class for a Timed signal route element comprising a route selection checkbox, a
 # signal ID entry box and two integer entry boxes for specifying the timed sequence
 # Public class instance methods provided by this class are 
 #    "disable" - disables/blanks all checkboxes and selection boxes 
 #    "enable"  enables/loads all checkboxes and selection boxes
 #    "set_values" - set the initial values for the check box and entry boxes) 
 #    "get_values" - get the last "validated" values of the check box and entry boxes
+#
+# Note that the software only supports triggering of signals on the local schematic
+# so we use the signal_exists function from the objects module for entry validation
 #------------------------------------------------------------------------------------
 
 #####################################################################################
 # TODO - consider better validation of the timed signal selections, namely:
 # 1) Should only be able to select a main semaphore or colour light signal type
 # 2) If triggering the current signal then the start delay should be Zero
 # Low priority enhancement as these things get handled gracefully at run time
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/editor.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,54 +104,66 @@
         self.help_menu.add_command(label =" Help...", command=lambda:menubar_windows.display_help(self.root))
         self.help_menu.add_command(label =" About...", command=lambda:menubar_windows.display_about(self.root))
         self.help_menu.add_command(label =" Info...", command=lambda:menubar_windows.edit_layout_info(self.root))
         self.mainmenubar.add_cascade(label = "Help  ", menu=self.help_menu)
         # Flag to track whether the new configuration has been saved or not
         # Used to enforce a "save as" dialog on the initial save of a new layout
         self.file_has_been_saved = False
-        # initialise the schematic editor
-        width, height, grid = settings.get_canvas()
-        schematic.initialise(self.root, self.handle_canvas_event, width, height, grid)
         # Initialise the editor configuration at startup
-        self.initialise_editor()
+        self.initialise_editor(startup=True)
         # Parse the command line arguments to get the filename (and load it)
         # The version is the third parameter provided by 'get_general'
         parser = ArgumentParser(description =  "Model railway signalling "+settings.get_general()[2])
         parser.add_argument("-f","--file",dest="filename",help="schematic file to load on startup",metavar="FILE")
         args = parser.parse_args()
         if args.filename is not None: self.load_schematic(args.filename)
-        
-    # Common initialisation function (called on editor start or layout load or new layout)
-    def initialise_editor(self):
+    
+    # --------------------------------------------------------------------------------------
+    # Common initialisation functions (called on editor start or layout load or new layout)
+    # --------------------------------------------------------------------------------------
+    
+    def initialise_editor(self,startup:bool=False):
         # Set the root window label to the name of the current file (split from the dir path)
         # The fully qualified filename is the first parameter provided by 'get_general'
         path, name = os.path.split(settings.get_general()[0])
         self.root.title(name)
-        # Set the edit mode (2nd param in the returned tuple)
-        if settings.get_general()[1]: self.edit_mode()
-        else: self.run_mode()
-        # Set the log level before creating the new layout objects
+        # Re-size the canvas to reflect the new schematic size
+        width, height, grid = settings.get_canvas()
+        if startup: schematic.initialise(self.root, self.handle_canvas_event, width, height, grid)
+        else: schematic.update_canvas(width, height, grid)
+        # Set the logging level before we start doing stuff
         initial_log_level = settings.get_logging()
         logging.basicConfig(format='%(levelname)s: %(message)s')
         if initial_log_level == 1: logging.getLogger().setLevel(logging.ERROR)
         elif initial_log_level == 2: logging.getLogger().setLevel(logging.WARNING)
         elif initial_log_level == 3: logging.getLogger().setLevel(logging.INFO)
         elif initial_log_level == 4: logging.getLogger().setLevel(logging.DEBUG)
         # Initialise the SPROG (if configured). Note that we use the menubar functions
         # for connection and the DCC power so these are correctly reflected in the UI
         port, baud, debug, startup, power = settings.get_sprog()
         if startup: self.sprog_connect()
         if power: self.dcc_power_on()
+        # Set the edit mode (2nd param in the returned tuple)
+        # Either of these calls will trigger a run layout update
+        if settings.get_general()[1]: self.edit_mode()
+        else: self.run_mode()
         
+    # --------------------------------------------------------------------------------------
+    # Callback function to handle the Toggle Mode Event ('m' key) from schematic.py
+    # --------------------------------------------------------------------------------------
+
     def handle_canvas_event(self, event=None):
-        # Handle the Toggle Mode Event ('m' key)
         if event.keysym == 'm':
             # the Edit mode flag is the second parameter returned
             if settings.get_general()[1]: self.run_mode()
             else: self.edit_mode()
+            
+    # --------------------------------------------------------------------------------------
+    # Callback functions to handle menubar selection events
+    # --------------------------------------------------------------------------------------
 
     def edit_mode(self):
         new_label = "Mode:Edit  "
         self.mainmenubar.entryconfigure(self.mode_label, label=new_label)
         self.mode_label = new_label
         settings.set_general(editmode=True)
         schematic.enable_editing()
@@ -230,17 +242,14 @@
                 message="Are you sure you want to discard all changes and create a new blank schematic"):
             # Delete all existing objects
             schematic.delete_all_objects()
             # Restore the default settings and update the editor config
             settings.restore_defaults()
             # Re-initialise the editor for the new settings to take effect
             self.initialise_editor()
-            # Re-size the canvas to reflect the new schematic size
-            width, height, grid = settings.get_canvas()
-            schematic.update_canvas(width, height, grid)
             # save the current state (for undo/redo) - deleting all previous history
             objects.save_schematic_state(reset_pointer=True)
         return()
 
     def save_schematic(self, save_as:bool=False):
         settings_to_save = settings.get_all()
         objects_to_save = objects.get_all()
@@ -276,18 +285,15 @@
                 # Create an empty list for any warning messages generated by the load
                 # Messages could be generated by settings.set_all or objects.set_all
                 warning_messages = []
                 # Store the newly loaded settings (getting any warnings)
                 warning_messages = settings.set_all(layout_state["settings"])
                 # Set the filename to reflect that actual name of the loaded file
                 settings.set_general(filename=file_loaded)
-                # Re-size the canvas to reflect the new schematic size
-                width, height, grid = settings.get_canvas()
-                schematic.update_canvas(width, height, grid)
-                # Re-initailise the editor with the new configuration
+                # Re-initialise the editor for the new settings to take effect
                 self.initialise_editor()
                 # Create the loaded layout objects then purge the loaded state information
                 warning_messages.extend(objects.set_all(layout_state["objects"]))
                 # Purge the loaded state (to stope it being erroneously inherited
                 # when items are deleted and then new items created with the same IDs)
                 file_interface.purge_loaded_state_information()
                 # Set the flag so we don't enforce a "save as" on next save
@@ -301,15 +307,15 @@
             else:
                 logging.error("LOAD LAYOUT - Selected file does not contain all required elements")
                 Tk.messagebox.showerror(parent=self.root, title="Load Error", 
                     message="File does not contain\nall required elements")
         return()
     
 #------------------------------------------------------------------------------------
-# Class for the window to display any file load warning messages  
+# Class for the pop-up window to display any file load warning messages  
 #------------------------------------------------------------------------------------
 
     class load_warnings_window():
         def __init__(self, root_window, warning_text):
             self.root_window = root_window
             # Create the top level window for the file load warnings
             winx = self.root_window.winfo_rootx() + 250
@@ -335,15 +341,15 @@
             self.label.pack(padx=2, pady=2, side=Tk.TOP)
             self.text.pack(padx=2, pady=2, fill=Tk.BOTH, expand=True)
             
         def ok(self):
             self.window.destroy()
         
 #------------------------------------------------------------------------------------
-# This is where the code begins  
+# This is the main function to run up the schematic editor application  
 #------------------------------------------------------------------------------------
 
 def run_editor():
     # Create the Main Root Window
     root = Tk.Tk()
     # Create the menubar and editor canvas (canvas size will be set on creation)
     main_window_menubar = main_menubar(root)
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/menubar_windows.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/menubar_windows.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/__init__.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,22 +306,22 @@
     return()
 
 #------------------------------------------------------------------------------------
 # Function to permanently Delete one or more objects from the schematic
 # Called from the Schematic Module when selected objects are deleted
 #------------------------------------------------------------------------------------
 
-def delete_objects(list_of_object_ids):
+def delete_objects(list_of_object_ids, initialise_layout_after_delete:bool=True):
     for object_id in list_of_object_ids:
         delete_object(object_id)
     # save the current state (for undo/redo)
     save_schematic_state()
     # Process any layout changes (interlocking, signal ahead etc)
     # that might need to change following objet deletion
-    run_layout.initialise_layout()
+    if initialise_layout_after_delete: run_layout.initialise_layout()
     return()
 
 #------------------------------------------------------------------------------------
 # Function to Rotate one or more objects on the schematic
 # Called from the Schematic Module when selected objects are rotated
 # Only Points and Signals can be rotated - all other objects are unchanged
 #------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_common.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_instruments.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_instruments.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 #    objects_common.default_object - The common dictionary element for all objects
 #    objects_common.object_type - The Enumeration of supported objects
 #    objects_common.canvas - Reference to the Tkinter drawing canvas
 #
 # Makes the following external API calls to library modules:
 #    block_instruments.delete_instrument(id) - delete library drawing object (part of soft delete)
 #    block_instruments.create_block_instrument(id) -  To create the library object (create or redraw)
+#    block_instruments.update_linked_to(old_id, new_id) - update the linked instrument reference
 #    block_instruments.get_tags(id) - get the canvas 'tags' for the instrument drawing objects
 #
 #------------------------------------------------------------------------------------
 
 import uuid
 import copy
 
@@ -61,33 +62,29 @@
 def update_references_to_instrument(old_inst_id:int, new_inst_id:int):
     # Iterate through all the instruments on the schematic
     for instrument_id in objects_common.instrument_index:
         # get the instrument object (so we can query the ID of the linked instrument)
         instrument_object = objects_common.instrument(instrument_id)
         if objects_common.schematic_objects[instrument_object]["linkedto"] == str(old_inst_id):
             objects_common.schematic_objects[instrument_object]["linkedto"] = str(new_inst_id)
-            # We have to delete and re-create the 'linked' instrument for changes to take effect
-            delete_instrument_object(instrument_object)
-            redraw_instrument_object(instrument_object)
+            block_instruments.update_linked_to(int(instrument_id), str(new_inst_id))
     return()
 
 #------------------------------------------------------------------------------------
 # Internal function to Remove references from instruments linked to this one
 #------------------------------------------------------------------------------------
 
 def remove_references_to_instrument(deleted_inst_id:int):
     # Iterate through all the instruments on the schematic
     for instrument_id in objects_common.instrument_index:
         # get the instrument object (so we can query the ID of the linked instrument)
         instrument_object = objects_common.instrument(instrument_id)
         if objects_common.schematic_objects[instrument_object]["linkedto"] == str(deleted_inst_id):
             objects_common.schematic_objects[instrument_object]["linkedto"] = ""
-            # We have to delete and re-create the 'linked' instrument for changes to take effect
-            delete_instrument_object(instrument_object)
-            redraw_instrument_object(instrument_object)
+            block_instruments.update_linked_to(int(instrument_id), None)
     return()
     
 #------------------------------------------------------------------------------------
 # Function to to update an instrument object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_instrument(object_id, new_object_configuration):
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_lines.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_lines.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_points.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #
 # Accesses the following external library objects directly:
 #    points.point_type - for setting the enum value when creating the object
 #
 # Makes the following external API calls to library modules:
 #    points.delete_point(id) - delete library drawing object (part of soft delete)
 #    points.create_point(id) -  To create the library object (create or redraw)
+#    points.update_autoswitch(id,autoswitch_id) - to change the config of an existing point
 #    points.get_tags(id) - get the canvas 'tags' for the point drawing objects
 #    points.point_switched(id) - test if a point is switched (when updating dependent objects)
 #    points.toggle_point_state(id) - to toggle point (when updating dependent objects)
 #    dcc_control.delete_point_mapping - delete mappings when deleting point / prior to recreating
 #    dcc_control.map_dcc_point - to create the new DCC mapping (creation or updating)
 #
 #------------------------------------------------------------------------------------
@@ -112,74 +113,46 @@
                         point_interlocked_by_signal = True
             if point_interlocked_by_signal:
                 interlocked_signal = [objects_common.schematic_objects[signal_object]["itemid"], interlocked_routes]
                 objects_common.schematic_objects[point_object]["siginterlock"].append(interlocked_signal)
     return()
 
 #------------------------------------------------------------------------------------
-# Internal function to update references from points that "also switch" this point
+# Internal function to update references from points that "also switch" this point.
+# Note that we use the non-public API function for updating the 'autoswitched' ID
+# rather than deleting the point and then re-creating it in its new state
 #------------------------------------------------------------------------------------
 
 def update_references_to_point(old_point_id:int, new_point_id:int):
     # Iterate through all the points on the schematic
     for point_id in objects_common.point_index:
         point_object = objects_common.point(point_id)
         if objects_common.schematic_objects[point_object]["alsoswitch"] == old_point_id:
             objects_common.schematic_objects[point_object]["alsoswitch"] = new_point_id
-            # We have to delete and re-create the 'parent' point for changes to take effect
-            # Note that when we delete and then re-draw the point it is created in its
-            # default state - so if it was switched before we need to switch it after
-            # Use the non-public-api call to bypass the validation for "toggle_point"
-            parent_point_switched = points.point_switched(point_id)
-            delete_point_object(point_object)
-            redraw_point_object(point_object)
-            if parent_point_switched:
-                points.toggle_point_state(point_id,True)
+            points.update_autoswitch(point_id=point_id, autoswitch_id=new_point_id)
     return()
 
 #------------------------------------------------------------------------------------
-# Internal function to Remove references from points that "also switch" this point.
+# Internal function to remove references to this point from points configured to "also
+# switch" the deleted point. Note that we use the non-public API function for updating
+# the 'autoswitched' ID rather than deleting the point and then re-creating it in its new
+# state. The main use case is when bulk deleting objects via the schematic editor, where
+# we want to avoid interleaving tkinter 'create' commands in amongst the 'delete' commands
+# outside of the main loop as this can result in with artefacts persisting on the canvas
 #------------------------------------------------------------------------------------
 
 def remove_references_to_point(deleted_point_id:int):
     for point_id in objects_common.point_index:
         point_object = objects_common.point(point_id)
         if objects_common.schematic_objects[point_object]["alsoswitch"] == deleted_point_id:
             objects_common.schematic_objects[point_object]["alsoswitch"] = 0
-            # We have to delete and re-create the 'parent' point for changes to take effect
-            # Note that when we delete and then re-draw the point it is created in its
-            # default state - so if it was switched before we need to switch it after
-            # Use the non-public-api call to bypass the validation for "toggle_point"
-            point_switched = points.point_switched(point_id)
-            delete_point_object(point_object)
-            redraw_point_object(point_object)
-            if point_switched:
-                points.toggle_point_state(point_id,True)    
+            points.update_autoswitch(point_id=point_id, autoswitch_id=0)
     return()
 
 #------------------------------------------------------------------------------------
-# Internal Function to update an autoswitched point chain by recursively working
-# through the chain to set any downstream points.
-#------------------------------------------------------------------------------------
-
-def update_downstream_points(object_id):
-    # Test to see if the current point is configured to "auto switch" another
-    # point and, if so, toggle the other (downstream) point to the same setting
-    point_id = objects_common.schematic_objects[object_id]["itemid"]
-    also_switch_id = objects_common.schematic_objects[object_id]["alsoswitch"]
-    if  also_switch_id > 0:
-        if points.point_switched(also_switch_id) != points.point_switched(point_id):
-            # Use the non-public-api call to bypass validation (can't toggle "auto" points)
-            points.toggle_point_state(also_switch_id,True)
-            # Recursively call back into the function with the object ID for the other point
-            update_downstream_points(objects_common.point(str(also_switch_id)))
-    return()
-
-
-#------------------------------------------------------------------------------------
 # Function to to update a point object after a configuration change
 #------------------------------------------------------------------------------------
 
 def update_point(object_id, new_object_configuration):
     # We need to track whether the Item ID has changed
     old_item_id = objects_common.schematic_objects[object_id]["itemid"]
     new_item_id = new_object_configuration["itemid"]
@@ -193,26 +166,14 @@
         # Update the type-specific index
         del objects_common.point_index[str(old_item_id)]
         objects_common.point_index[str(new_item_id)] = object_id
         # Update any other point that "also switches" this point to use the new ID
         update_references_to_point(old_item_id,new_item_id)
         # Update any affected signal interlocking tables to reference the new point ID
         objects_signals.update_references_to_point(old_item_id, new_item_id)
-    # We need to ensure that all points in an 'auto switch' chain are set
-    # to the same switched/not-switched state so they switch together correctly
-    # First, test to see if the current point is configured to "auto switch" with 
-    # another point and, if so, toggle the current point to the same setting
-    for point_id in objects_common.point_index:
-        point_object = objects_common.point(point_id)
-        if objects_common.schematic_objects[point_object]["alsoswitch"] == new_item_id:
-            if points.point_switched(point_id):
-                # Use the non-public-api call to bypass the validation for "toggle_point"
-                points.toggle_point_state(new_item_id,True)
-    # Next, update any downstream points that are configured to autoswitch with this one
-    update_downstream_points(object_id)
     return()
 
 #------------------------------------------------------------------------------------
 # Function to redraw a Point object on the schematic. Called when the object is first
 # created or after the object configuration has been updated.
 #------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_sections.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_sections.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/objects/objects_signals.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/objects/objects_signals.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow1.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow1.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow2.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow2.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow3.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow3.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/arrow4.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/arrow4.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/endstop.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/endstop.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/instrument.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/instrument.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/resources/section.png` & `model-railway-signals-3.4.1/model_railway_signals/editor/resources/section.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/run_layout.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/run_layout.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/schematic.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,18 @@
 # Internal function to delete all objects (for layout 'load' and layout 'new'
 #------------------------------------------------------------------------------------
 
 def delete_all_objects():
     global schematic_state
     # Select and delete all objects (also clear the selected objects list)
     select_all_objects()
-    delete_selected_objects()
+    # Delete the objects from the schematic
+    objects.delete_objects(schematic_state["selectedobjects"],initialise_layout_after_delete=False)
+    # Remove the objects from the list of selected objects
+    schematic_state["selectedobjects"]=[]
     # Belt and braces delete of all canvas objects as I've seen issues when
     # running the system tests (probably because I'm not using the mainloop)
     canvas.delete("all")
     # Set the select area box to 'None' so it gets created on first use
     schematic_state["selectareabox"] = None
     return()
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/editor/settings.py` & `model-railway-signals-3.4.1/model_railway_signals/editor/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # These are the default settings
 #------------------------------------------------------------------------------------
 
 default_settings = {}
 default_settings["general"] = {}
 default_settings["general"]["filename"] = "new_layout.sig"
 default_settings["general"]["editmode"] = True
-default_settings["general"]["version"] = "Version 3.4.0"
+default_settings["general"]["version"] = "Version 3.4.1"
 default_settings["general"]["info"] = "Document your layout here"
 default_settings["canvas"] = {}
 default_settings["canvas"]["width"] = 1000
 default_settings["canvas"]["height"] = 500
 default_settings["canvas"]["grid"] = 25
 default_settings["logging"] = {}
 default_settings["logging"]["level"] = 2   # Warning
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/block_instruments.py` & `model-railway-signals-3.4.1/model_railway_signals/library/block_instruments.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,28 @@
 # -------------------------------------------------------------------------
 # The default "External" callback for Block Instruments if one isn't specified
 # -------------------------------------------------------------------------
 
 def null_callback(block_id:int, callback_type):
     return(block_id, callback_type)
 
+# -------------------------------------------------------------------------
+# Helper function to return an instrument ID ofthe right python Type - depending
+# on whether it is a local (int) or remote (str) ID. We need to do this for the
+# editor as the editor will give us both local and remote IDs as a string
+# -------------------------------------------------------------------------
+
+def set_item_id_type(input_id:Union[int,str]):
+    if input_id is None or input_id == "":
+        output_id = None
+    else:
+        try: output_id = int(input_id)
+        except: output_id = str(input_id)
+    return(output_id)
+
 # --------------------------------------------------------------------------------
 # Internal Function to Open a window containing a list of common signal box bell
 # codes on the right click of the TELEGRAPH Button on any Block Instrument. The
 # window will always be displayed on top of the other Tkinter windows until closed.
 # Only one Telegraph Bell Codes window can be open at a time
 # --------------------------------------------------------------------------------
 
@@ -245,230 +259,185 @@
 # --------------------------------------------------------------------------------
 
 def set_repeater_blocked (block_id:int,make_callback:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists(block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to LINE BLOCKED - Block instrument doesn't exist")
-    elif instruments[str(block_id)]["singleline"]:
-        # If this is a single line instrument then we need to change the main instrument state
-        # We need to inhibit the update of the linked instrument in this call to prevent recursion
-        set_section_blocked(block_id,update_remote_instrument=False)
-        # As the change was initiated by a remote instrument we disable the local instrument
-        # buttons until the remote instrument has changed back to LINE BLOCKED
-        instruments[str(block_id)]["blockbutton"].config(state="normal")
-        instruments[str(block_id)]["clearbutton"].config(state="normal")
-        instruments[str(block_id)]["occupbutton"].config(state="normal")
     elif instruments[str(block_id)]["repeaterstate"] is not None:
         logging.info ("Block Instrument "+str(block_id)+": Changing block section repeater to LINE BLOCKED")
         # Set the internal repeater state and the repeater indicator to BLOCKED
         instruments[str(block_id)]["repeaterstate"] = None
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatoroccup"],state = "hidden")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorclear"],state = "hidden")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorblock"],state = "normal")
-    # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
-    # This enables full block section interlocking to be implemented for the starter signal in OUR block section
-    if make_callback: instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
+        # For single line instruments we set the local instrument buttons to mirror the remote instrument
+        # and also enable the local buttons (as the remote instrument has been returned to LINE BLOCKED)
+        if instruments[str(block_id)]["singleline"]:
+            instruments[str(block_id)]["blockbutton"].config(state="normal",relief="sunken",bg=common.bgsunken)
+            instruments[str(block_id)]["clearbutton"].config(state="normal",relief="raised",bg=common.bgraised)
+            instruments[str(block_id)]["occupbutton"].config(state="normal",relief="raised",bg=common.bgraised)
+        # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
+        # This enables full block section interlocking to be implemented for the starter signal in OUR block section
+        if make_callback:
+            instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
     return ()
 
 # --------------------------------------------------------------------------------
 # Function to set the repeater indicator (linked to another block section)
 # to LINE CLEAR - if its a single line instrument then we set the main indication
 # --------------------------------------------------------------------------------
 
 def set_repeater_clear (block_id:int,make_callback:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to LINE CLEAR - Block instrument doesn't exist")
-    elif instruments[str(block_id)]["singleline"]:
-        # If this is a single line instrument then we need to change the main instrument state
-        # We need to inhibit the update of the linked instrument in this call to prevent recursion
-        set_section_clear(block_id,update_remote_instrument=False)
-        # As the change was initiated by a remote instrument we disable the local instrument
-        # buttons until the remote instrument has changed back to LINE BLOCKED
-        instruments[str(block_id)]["blockbutton"].config(state="disabled")
-        instruments[str(block_id)]["clearbutton"].config(state="disabled")
-        instruments[str(block_id)]["occupbutton"].config(state="disabled")
     elif instruments[str(block_id)]["repeaterstate"] != True:
         logging.info ("Block Instrument "+str(block_id)+": Changing block section repeater to LINE CLEAR")
         # Set the internal repeater state and the repeater indicator to CLEAR
         instruments[str(block_id)]["repeaterstate"] = True
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatoroccup"],state = "hidden")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorclear"],state = "normal")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorblock"],state = "hidden")
-    # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
-    # This enables full block section interlocking to be implemented for the starter signal in OUR block section
-    if make_callback: instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
+        # For single line instruments we set the local instrument buttons to mirror the remote instrument
+        # and also inhibit the local buttons (until the remote instrument is returned to LINE BLOCKED)
+        if instruments[str(block_id)]["singleline"]:
+            instruments[str(block_id)]["blockbutton"].config(state="disabled",relief="raised",bg=common.bgraised)
+            instruments[str(block_id)]["clearbutton"].config(state="disabled",relief="sunken",bg=common.bgsunken)
+            instruments[str(block_id)]["occupbutton"].config(state="disabled",relief="raised",bg=common.bgraised)
+        # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
+        # This enables full block section interlocking to be implemented for the starter signal in OUR block section
+        if make_callback:
+            instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
     return ()
 
 # --------------------------------------------------------------------------------
 # Function to set the repeater indicator (linked to another block section)
 # to OCCUPIED - if its a single line instrument then we set the main indication
 # --------------------------------------------------------------------------------
 
 def set_repeater_occupied (block_id:int,make_callback:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set repeater to TRAIN ON LINE - Block instrument doesn't exist")
-    elif instruments[str(block_id)]["singleline"]:
-        # If this is a single line instrument then we need to change the main instrument state
-        # We need to inhibit the update of the linked instrument in this call to prevent recursion
-        set_section_occupied(block_id,update_remote_instrument=False)
-        # As the change was initiated by a remote instrument we disable the local instrument
-        # buttons until the remote instrument has changed back to LINE BLOCKED
-        instruments[str(block_id)]["blockbutton"].config(state="disabled")
-        instruments[str(block_id)]["clearbutton"].config(state="disabled")
-        instruments[str(block_id)]["occupbutton"].config(state="disabled")
     elif instruments[str(block_id)]["repeaterstate"] != False:
         logging.info ("Block Instrument "+str(block_id)+": Changing block section repeater to TRAIN ON LINE")
         # Set the internal repeater state and the repeater indicator to OCCUPIED
         instruments[str(block_id)]["repeaterstate"] = False
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatoroccup"],state = "normal")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorclear"],state = "hidden")
         instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["repeatindicatorblock"],state = "hidden")
-    # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
-    # This enables full block section interlocking to be implemented for the starter signal in OUR block section
-    if make_callback: instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
+        # For single line instruments we set the local instrument buttons to mirror the remote instrument
+        # and also inhibit the local buttons (until the remote instrument is returned to LINE BLOCKED)
+        if instruments[str(block_id)]["singleline"]:
+            instruments[str(block_id)]["blockbutton"].config(state="disabled",relief="raised",bg=common.bgraised)
+            instruments[str(block_id)]["clearbutton"].config(state="disabled",relief="raised",bg=common.bgraised)
+            instruments[str(block_id)]["occupbutton"].config(state="disabled",relief="sunken",bg=common.bgsunken)
+        # Make an external callback (if one was specified) to notify that the block section AHEAD has been updated
+        # This enables full block section interlocking to be implemented for the starter signal in OUR block section
+        if make_callback:
+            instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal Function to set the main block section indicator to BLOCKED
 # called when the "BLOCKED" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_blocked (block_id:int,update_remote_instrument:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to LINE BLOCKED - Block instrument doesn't exist")
-    else:
-        # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
-        # to deal with single line instruments being updated by a state change of the linked instrument
-        instruments[str(block_id)]["blockbutton"].config(relief="sunken")
-        instruments[str(block_id)]["blockbutton"].config(bg=common.bgsunken)
-        instruments[str(block_id)]["clearbutton"].config(relief="raised")
-        instruments[str(block_id)]["clearbutton"].config(bg=common.bgraised)
-        instruments[str(block_id)]["occupbutton"].config(relief="raised")
-        instruments[str(block_id)]["occupbutton"].config(bg=common.bgraised)
-        # Everything else is only processed on a state change
-        if instruments[str(block_id)]["sectionstate"] is not None:
-            logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to LINE BLOCKED")
-            # Set the internal state of the block instrument
-            instruments[str(block_id)]["sectionstate"] = None
-            # The repeater state is always the same as the main state for single line instruments
-            if instruments[str(block_id)]["singleline"]: instruments[str(block_id)]["repeaterstate"] = None
-            # Set the local block indication to reflect the state that has been set locally
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "normal")
-            # If linked to another instrument then update the repeater indicator on the other instrument or
-            # Publish the initial state to the broker (for other nodes to consume). Note that state will only
-            # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument:
-                if instruments[str(block_id)]["linkedto"] is not None:
-                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                    else: set_repeater_blocked(instruments[str(block_id)]["linkedto"])
-                # Handle the case of a single line instrument with no linked instrument - in this case we
-                # want to make a callback on block state change to allow interlocking to be processed
-                elif instruments[str(block_id)]["singleline"]:
-                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
+    elif instruments[str(block_id)]["sectionstate"] is not None:
+        logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to LINE BLOCKED")
+        # Set the state of the buttons accordingly
+        instruments[str(block_id)]["blockbutton"].config(relief="sunken",bg=common.bgsunken)
+        instruments[str(block_id)]["clearbutton"].config(relief="raised",bg=common.bgraised)
+        instruments[str(block_id)]["occupbutton"].config(relief="raised",bg=common.bgraised)
+        # Set the internal state of the block instrument and the local indicator
+        instruments[str(block_id)]["sectionstate"] = None
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "normal")
+        # If linked to another instrument then update the repeater indicator on the other instrument or
+        # Publish the initial state to the broker (for other nodes to consume). Note that state will only
+        # be published if the MQTT interface has been configured and we are connected to the broker
+        if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
+            linked_to_id = instruments[str(block_id)]["linkedto"]
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(block_id)
+            elif instrument_exists(linked_to_id): set_repeater_blocked(linked_to_id)
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal Function to set the main block section indicator to CLEAR
 # called when the "CLEAR" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_clear (block_id:int,update_remote_instrument:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to LINE CLEAR - Block instrument doesn't exist")
-    else:
-        # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
-        # to deal with single line instruments being updated by a state change of the linked instrument
-        instruments[str(block_id)]["blockbutton"].config(relief="raised")
-        instruments[str(block_id)]["blockbutton"].config(bg=common.bgraised)
-        instruments[str(block_id)]["clearbutton"].config(relief="sunken")
-        instruments[str(block_id)]["clearbutton"].config(bg=common.bgsunken)
-        instruments[str(block_id)]["occupbutton"].config(relief="raised")
-        instruments[str(block_id)]["occupbutton"].config(bg=common.bgraised)
-        # Everything else is only processed on a state change
-        if instruments[str(block_id)]["sectionstate"] != True:
-            logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to LINE CLEAR")
-            # Set the internal state of the block instrument
-            instruments[str(block_id)]["sectionstate"] = True
-            # The repeater state is always the same as the main state for single line instruments
-            if instruments[str(block_id)]["singleline"]: instruments[str(block_id)]["repeaterstate"] = True
-            # Set the local block indication to reflect the state that has been set locally
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "normal")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
-            # If linked to another instrument then update the repeater indicator on the other instrument or
-            # Publish the initial state to the broker (for other nodes to consume). Note that state will only
-            # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument:
-                if instruments[str(block_id)]["linkedto"] is not None:
-                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                    else: set_repeater_clear(instruments[str(block_id)]["linkedto"])
-                # Handle the case of a single line instrument with no linked instrument - in this case we
-                # want to make a callback on block state change to allow interlocking to be processed
-                elif instruments[str(block_id)]["singleline"]:
-                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
+    elif instruments[str(block_id)]["sectionstate"] != True:
+        logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to LINE CLEAR")
+        # Set the state of the buttons accordingly
+        instruments[str(block_id)]["blockbutton"].config(relief="raised",bg=common.bgraised)
+        instruments[str(block_id)]["clearbutton"].config(relief="sunken",bg=common.bgsunken)
+        instruments[str(block_id)]["occupbutton"].config(relief="raised",bg=common.bgraised)
+        # Set the internal state of the block instrument and the local indicator
+        instruments[str(block_id)]["sectionstate"] = True
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "normal")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
+        # If linked to another instrument then update the repeater indicator on the other instrument or
+        # Publish the initial state to the broker (for other nodes to consume). Note that state will only
+        # be published if the MQTT interface has been configured and we are connected to the broker
+        if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
+            linked_to_id = instruments[str(block_id)]["linkedto"]
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(block_id)
+            elif instrument_exists(linked_to_id): set_repeater_clear(linked_to_id)
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal Function to set the main block section indicator to OCCUPIED
 # called when the "OCCUP" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
 # --------------------------------------------------------------------------------
 
 def set_section_occupied (block_id:int,update_remote_instrument:bool=True):
     global instruments
     # do some basic validation on the block ID we've been given
     if not instrument_exists (block_id):
         logging.error ("Block Instrument "+str(block_id)+": Can't set section to TRAIN ON LINE - Block instrument doesn't exist")
-    else:
-        # Set the state of the buttons accordingly. We always do this (even if the state hasn't changed)
-        # to deal with single line instruments being updated by a state change of the linked instrument
-        instruments[str(block_id)]["blockbutton"].config(relief="raised")
-        instruments[str(block_id)]["blockbutton"].config(bg=common.bgraised)
-        instruments[str(block_id)]["clearbutton"].config(relief="raised")
-        instruments[str(block_id)]["clearbutton"].config(bg=common.bgraised)
-        instruments[str(block_id)]["occupbutton"].config(relief="sunken")
-        instruments[str(block_id)]["occupbutton"].config(bg=common.bgsunken)
-        # Everything else is only processed on a state change
-        if instruments[str(block_id)]["sectionstate"] != False:
-            logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to TRAIN ON LINE")
-            # Set the internal state of the block instrument and the buttons accordingly. We always do
-            instruments[str(block_id)]["sectionstate"] = False
-            # The repeater state is always the same as the main state for single line instruments
-            if instruments[str(block_id)]["singleline"]: instruments[str(block_id)]["repeaterstate"] = False
-            # Set the local block indication to reflect the state that has been set locally
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "normal")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
-            instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
-            # If linked to another instrument then update the repeater indicator on the other instrument or
-            # Publish the initial state to the broker (for other nodes to consume). Note that state will only
-            # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument:
-                if instruments[str(block_id)]["linkedto"] is not None:
-                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                    else: set_repeater_occupied(instruments[str(block_id)]["linkedto"])
-                # Handle the case of a single line instrument with no linked instrument - in this case we
-                # want to make a callback on block state change to allow interlocking to be processed
-                elif instruments[str(block_id)]["singleline"]:
-                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
+    elif instruments[str(block_id)]["sectionstate"] != False:
+        logging.info ("Block Instrument "+str(block_id)+": Changing block section indicator to TRAIN ON LINE")
+        # Set the state of the buttons accordingly
+        instruments[str(block_id)]["blockbutton"].config(relief="raised",bg=common.bgraised)
+        instruments[str(block_id)]["clearbutton"].config(relief="raised",bg=common.bgraised)
+        instruments[str(block_id)]["occupbutton"].config(relief="sunken",bg=common.bgsunken)
+        # Set the internal state of the block instrument and the local indicator
+        instruments[str(block_id)]["sectionstate"] = False
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "normal")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
+        instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
+        # If linked to another instrument then update the repeater indicator on the other instrument or
+        # Publish the initial state to the broker (for other nodes to consume). Note that state will only
+        # be published if the MQTT interface has been configured and we are connected to the broker
+        if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
+            linked_to_id = instruments[str(block_id)]["linkedto"]
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(block_id)
+            elif instrument_exists(linked_to_id): set_repeater_occupied(linked_to_id)
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal function to create the Indicator component of a Block Instrument
 # --------------------------------------------------------------------------------
 
 def create_block_indicator(canvas:int, x:int, y:int, block_id_tag):
@@ -526,38 +495,50 @@
     global instruments
     global list_of_instruments_to_publish
     logging.info ("Block Instrument "+str(block_id)+": Creating Block Instrument")
     # Find and store the root window (when the first block instrument is created)
     if common.root_window is None: common.find_root_window(canvas)
     # Establish whether the ID is a local or remote ID and set the type accordingly
     # We need to do this for the editor as the editor will give us an int as a string
-    if linked_to is None or linked_to == "":
-        linked_to_id = None
-    else:
-        try: linked_to_id = int(linked_to)
-        except: linked_to_id = str(linked_to)
+    linked_to_id = set_item_id_type(linked_to)
     # Do some basic validation on the parameters we have been given
     if instrument_exists(block_id):
         logging.error ("Block Instrument "+str(block_id)+": Instrument already exists")
     elif block_id < 1:
         logging.error ("Block Instrument "+str(block_id)+": Block ID must be greater than zero")
     elif linked_to_id == block_id:
         logging.error ("Block Instrument "+str(block_id)+": ID for linked instrument is the same as the instrument to create")
     elif isinstance(linked_to_id,str) and mqtt_interface.split_remote_item_identifier(linked_to_id) is None:
         logging.error ("Block Instrument "+str(block_id)+": Compound ID for remote-node instrument is invalid")
     else:
         ####################################################################################################################
         # DEPRECATED code to remove at a future release ####################################################################
+        ####################################################################################################################
         if single_line:
             logging.warning ("###########################################################################################")
             logging.warning ("Block Instrument "+str(block_id)+": single_line flag is DEPRECATED - use inst_type")
             logging.warning ("###########################################################################################")
         else:
             single_line = (inst_type == instrument_type.single_line)
+        # If the associated block instrument is associated with an external node (i.e. has a string-type
+        # compound identifier rather than an integer) then subscribe to updates from the remote node and
+        # publish the initial state of the local instrument (to be picked up by the remote node). State
+        # will only be published if the MQTT interface has been configured and we are connected to the broker
+        # Note that this function is DEPRECATED - you should always 'subscribe' to remote instruments beforehand
+        if isinstance(linked_to_id,str) and not instrument_exists(linked_to_id):
+            remote_node,remote_id = mqtt_interface.split_remote_item_identifier(linked_to_id)
+            subscribe_to_instrument_updates(remote_node,remote_id)
+            set_instruments_to_publish_state(block_id)
+            logging.warning ("###########################################################################################")
+            logging.warning ("Block Instrument "+str(block_id)+": Auto publish and subscribe is DEPRECATED - call the")
+            logging.warning ("'subscribe_to_instrument_updates'and 'set_instruments_to_publish_state' functions to")
+            logging.warning ("configure networking before creating the block instruments on the local schematic")
+            logging.warning ("###########################################################################################")
         ####################################################################################################################
+            
         # Define the "Tag" for all drawing objects for this instrument instance
         block_id_tag = "instrument"+str(block_id)
         # Create the Instrument background - this will vary in size depending on single or double line
         if single_line: canvas.create_rectangle (x-60, y-20, x+60, y+150, fill = "saddle brown",tags=block_id_tag)
         else: canvas.create_rectangle (x-60, y-80, x+60, y+150, fill = "saddle brown",tags=block_id_tag)
         # Create the button objects and their callbacks
         occup_button = Tk.Button (canvas, text="OCCUP", padx=common.xpadding, pady=common.ypadding,
@@ -580,30 +561,31 @@
         canvas.create_window(x, y+80, window=occup_button, anchor=Tk.SE, tags=block_id_tag)
         canvas.create_window(x, y+80, window=clear_button, anchor=Tk.SW, tags=block_id_tag)
         canvas.create_window(x, y+80, window=block_button, anchor=Tk.N, tags=block_id_tag)
         canvas.create_window(x, y+115, window=bell_button, anchor=Tk.N, tags=block_id_tag)
         # Create the main block section indicator for our instrument
         my_ind_block, my_ind_clear, my_ind_occup = create_block_indicator (canvas, x, y, block_id_tag)
         # If this is a double line indicator then create the repeater indicator
-        if single_line: rep_ind_block, rep_ind_clear, rep_ind_occup = None, None, None
+        # For a single line indicator, we use the main indicator as the repeater
+        if single_line: rep_ind_block, rep_ind_clear, rep_ind_occup = my_ind_block, my_ind_clear, my_ind_occup
         else: rep_ind_block, rep_ind_clear, rep_ind_occup = create_block_indicator (canvas, x, y-55, block_id_tag)
         # Try to Load the specified audio files for the bell rings and telegraph key if audio is enabled
         # if these fail to load for any reason then no sounds will be produced on these events
         if audio_enabled:
             bell_audio = load_audio_file(bell_sound_file)
             telegraph_audio = load_audio_file(telegraph_sound_file)
         else:
             logging.warning ("Block Instruments - Audio is not enabled - To enable: 'python3 -m pip install simpleaudio'")
             bell_audio = None
             telegraph_audio = None
         # Create the dictionary of elements that we need to track
         instruments[str(block_id)] = {}
         instruments[str(block_id)]["canvas"] = canvas                         # Tkinter drawing canvas
         instruments[str(block_id)]["extcallback"] = block_callback            # External callback to make
-        instruments[str(block_id)]["linkedto"] = linked_to_id                    # Id of the instrument this one is linked to
+        instruments[str(block_id)]["linkedto"] = linked_to_id                 # Id of the instrument this one is linked to
         instruments[str(block_id)]["singleline"] = single_line                # Single line (bi-directional) instrument
         instruments[str(block_id)]["sectionstate"] = None                     # State of this instrument (None = "BLOCKED")
         instruments[str(block_id)]["repeaterstate"] = None                    # State of repeater display (None = "BLOCKED")
         instruments[str(block_id)]["blockbutton"] = block_button              # Tkinter Button object
         instruments[str(block_id)]["clearbutton"] = clear_button              # Tkinter Button object
         instruments[str(block_id)]["occupbutton"] = occup_button              # Tkinter Button object
         instruments[str(block_id)]["bellbutton"] = bell_button                # Tkinter Button object
@@ -614,52 +596,56 @@
         instruments[str(block_id)]["repeatindicatoroccup"] = rep_ind_occup    # Tkinter Drawing object
         instruments[str(block_id)]["repeatindicatorblock"] = rep_ind_block    # Tkinter Drawing object
         instruments[str(block_id)]["telegraphsound"] = telegraph_audio        # Sound file for the telegraph "clack"
         instruments[str(block_id)]["bellsound"] = bell_audio                  # Sound file for the bell "Ting"
         # Get the initial state for the instrument (if layout state has been loaded)
         # if nothing has been loaded then the default state (of LINE BLOCKED) will be applied
         loaded_state = file_interface.get_initial_item_state("instruments",block_id)
-        # Set the initial state for the instrument (values will be 'None' for No state loaded)
-        # We need to inhibit the update of the linked instrument in this call to prevent trying
-        # to update a linked block instrument that might not have been created as yet 
-        if loaded_state["sectionstate"] == True: set_section_clear(block_id,update_remote_instrument=False)
-        elif loaded_state["sectionstate"] == False: set_section_occupied(block_id,update_remote_instrument=False)
-        else: set_section_blocked(block_id,update_remote_instrument=False)
-        # Only set the initial repeater state if this instrument has a repeater (i.e. not single line)
-        if not instruments[str(block_id)]["singleline"]:
-            if loaded_state["repeaterstate"] == True: set_repeater_clear(block_id,make_callback=False)
-            elif loaded_state["repeaterstate"] == False: set_repeater_occupied(block_id,make_callback=False)
-            else: set_repeater_blocked(block_id,make_callback=False)
+        # Set the initial block-state for the instrument (values will be 'None' for No state loaded)
+        if loaded_state["sectionstate"] == True: set_section_clear(block_id, update_remote_instrument=False)
+        elif loaded_state["sectionstate"] == False: set_section_occupied(block_id, update_remote_instrument=False)
+        else: set_section_blocked(block_id, update_remote_instrument=False)
+        # Set the initial repeater state (values will be 'None' for No state loaded)
+        if loaded_state["repeaterstate"] == True: set_repeater_clear(block_id,make_callback=False)
+        elif loaded_state["repeaterstate"] == False: set_repeater_occupied(block_id,make_callback=False)
+        else: set_repeater_blocked(block_id,make_callback=False)
+        # Update the repeater display of the linked instrument (if one is specified). This will update
+        # local instruments (block_id is an int) if they have already been created on the schematic or
+        # send an MQTT event to update remote instruments (block_id is a str) if the current instrument
+        # has already been configured to publish state to the MQTT broker.
+        update_linked_to(block_id,linked_to_id)
+        # If an instrument already exists that is already linked to this instrument then we need
+        # to set the repeater display of this instrument to reflect the state of that instrument.
+        # Note that when a remote instrument is subscribed to a 'dummy' instrument is created with
+        # a 'linked_to' element of None - so the we don't get an exception whilst iterating
+        for inst_id in instruments:
+            if instruments[inst_id]['linkedto'] == block_id:
+                # As we've got a match we know the inst_id must be local (an integer)
+                update_linked_to(int(inst_id), block_id)
+                # Raise a warning if the current instrument is not configured to point to that instrument
+                if instruments[str(block_id)]['linkedto'] != int(inst_id):
+                    logging.error ("Block Instrument "+str(block_id)+": linked instrument is"+str(linked_to_id)+
+                                   " but instrument "+inst_id+" is linked back to this instrument ")
+    return ()
 
-        ####################################################################################################################
-        # DEPRECATED code to remove at a future release ####################################################################
-        # If the associated block instrument is associated with an external node (i.e. has a string-type
-        # compound identifier rather than an integer) then subscribe to updates from the remote node and
-        # publish the initial state of the local instrument (to be picked up by the remote node). State
-        # will only be published if the MQTT interface has been configured and we are connected to the broker
-        # Note that this function is DEPRECATED - you should always 'subscribe' to remote instruments beforehand
-        if isinstance(linked_to_id,str) and not instrument_exists(linked_to_id):
-            remote_node,remote_id = mqtt_interface.split_remote_item_identifier(linked_to_id)
-            mqtt_interface.subscribe_to_mqtt_messages("instrument_updated_event",remote_node,
-                                            remote_id,handle_mqtt_instrument_updated_event)
-            mqtt_interface.subscribe_to_mqtt_messages("instrument_telegraph_event",remote_node,
-                                            remote_id,handle_mqtt_ring_section_bell_event)
-            list_of_instruments_to_publish.append(block_id)
-            logging.warning ("###########################################################################################")
-            logging.warning ("Block Instrument "+str(block_id)+": Auto publish and subscribe is DEPRECATED - call the")
-            logging.warning ("'subscribe_to_instrument_updates'and 'set_instruments_to_publish_state' functions to")
-            logging.warning ("configure networking before creating the block instruments on the local schematic")
-            logging.warning ("###########################################################################################")
-        ####################################################################################################################
+# --------------------------------------------------------------------------------
+# Public API function to find out if the block section ahead is clear.
+# This is represented by the current status of the REPEATER Indicator
+# --------------------------------------------------------------------------------
 
-        # Publish the initial state to the broker (for other nodes to consume). Note that changes will
-        # only be published if the MQTT interface has been configured for publishing updates for this
-        # instrument. This allows publish/subscribe to be configured prior to instrument creation
-        send_mqtt_instrument_updated_event(block_id)
-    return ()
+def block_section_ahead_clear(block_id:int):
+    # do some basic validation on the block ID we've been given
+    if not instrument_exists (block_id):
+        logging.error ("Block Instrument "+str(block_id)+": block_section_ahead_clear - Block instrument doesn't exist")
+        section_ahead_clear = False
+    elif instruments[str(block_id)]["repeaterstate"] == True:
+        section_ahead_clear = True
+    else:
+        section_ahead_clear = False
+    return(section_ahead_clear)
 
 #-----------------------------------------------------------------------------------------------
 # Public API Function to configure instruments to publish state changes to remote MQTT nodes
 # (i.e. effectively publish state changes to the local SECTION indicator)
 # Note that this function should be called BEFORE creating block instruments
 #-----------------------------------------------------------------------------------------------
 
@@ -687,38 +673,23 @@
     for inst_id in inst_ids:
         instrument_identifier = mqtt_interface.create_remote_item_identifier(inst_id,node)
         if not instrument_exists(instrument_identifier):
             # Create a dummy instrument object to enable 'instrument_exists' validation checks
             # Note that this does not hold state - as state is reflected on the local repeater indicator
             # The Identifier for a remote instrument is a string combining the the Node-ID and Section-ID
             instruments[instrument_identifier] = {}
+            instruments[instrument_identifier]["linkedto"] = None
             # Subscribe to updates from the remote block instrument
             mqtt_interface.subscribe_to_mqtt_messages("instrument_updated_event",node,
                                     inst_id,handle_mqtt_instrument_updated_event)
             mqtt_interface.subscribe_to_mqtt_messages("instrument_telegraph_event",node,
                                     inst_id,handle_mqtt_ring_section_bell_event)
     return()
 
 # --------------------------------------------------------------------------------
-# Public API function to find out if the block section ahead is clear.
-# This is represented by the current status of the REPEATER Indicator
-# --------------------------------------------------------------------------------
-
-def block_section_ahead_clear(block_id:int):
-    # do some basic validation on the block ID we've been given
-    if not instrument_exists (block_id):
-        logging.error ("Block Instrument "+str(block_id)+": block_section_ahead_clear - Block instrument doesn't exist")
-        section_ahead_clear = False
-    elif instruments[str(block_id)]["repeaterstate"] == True:
-        section_ahead_clear = True
-    else:
-        section_ahead_clear = False
-    return(section_ahead_clear)
-
-# --------------------------------------------------------------------------------
 # Callbacks for handling received MQTT messages (from a remote Instrument)
 # --------------------------------------------------------------------------------
 
 def handle_mqtt_instrument_updated_event(message):
     if "instrumentid" in message.keys() and "sectionstate" in message.keys():
         block_identifier = message["instrumentid"]
         section_state = message["sectionstate"]
@@ -781,14 +752,39 @@
         if block_id in list_of_instruments_to_publish:
             list_of_instruments_to_publish.remove(block_id)
         # Finally, delete the entry from the dictionary of instruments
         del instruments[str(block_id)]
     return()
 
 # ------------------------------------------------------------------------------------------
+# Non public API function for updating the ID of the linked block instrument without
+# needing to delete the block instrument and then create it in its new state. The main
+# use case is when bulk deleting objects via the schematic editor, where we want to avoid
+# interleaving tkinter 'create' commands in amongst the 'delete' commands outside of the
+# main tkinter loop as this can lead to problems with artefacts persisting on the canvas
+# ------------------------------------------------------------------------------------------
+
+def update_linked_to(inst_id:int, linked_to:Union[int,str]):
+    # Establish whether the ID is a local or remote ID and set the type accordingly
+    # We need to do this for the editor as the editor will give us an int as a string
+    linked_to_id = set_item_id_type(linked_to)
+    instruments[str(inst_id)]["linkedto"] = linked_to_id
+    if linked_to_id is not None:
+        if instruments[str(inst_id)]["sectionstate"] == True:
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(inst_id)
+            elif instrument_exists(linked_to_id): set_repeater_clear(linked_to_id,make_callback=False)
+        elif instruments[str(inst_id)]["sectionstate"] == False:
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(inst_id)
+            elif instrument_exists(linked_to_id): set_repeater_occupied(linked_to_id,make_callback=False)
+        else:
+            if isinstance(linked_to_id,str): send_mqtt_instrument_updated_event(inst_id)
+            elif instrument_exists(linked_to_id): set_repeater_blocked(linked_to_id,make_callback=False)
+    return()
+
+# ------------------------------------------------------------------------------------------
 # Non public API function to return the tkinter canvas 'tags' for the block instrument
 # ------------------------------------------------------------------------------------------
 
 def get_tags(block_id:int):
     return("instrument"+str(block_id))
 
 # ------------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/common.py` & `model-railway-signals-3.4.1/model_railway_signals/library/common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/dcc_control.py` & `model-railway-signals-3.4.1/model_railway_signals/library/dcc_control.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/file_interface.py` & `model-railway-signals-3.4.1/model_railway_signals/library/file_interface.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/mqtt_interface.py` & `model-railway-signals-3.4.1/model_railway_signals/library/mqtt_interface.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/pi_sprog_interface.py` & `model-railway-signals-3.4.1/model_railway_signals/library/pi_sprog_interface.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/points.py` & `model-railway-signals-3.4.1/model_railway_signals/library/points.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,14 +162,34 @@
         points[str(point_id)]["switched"] = False
         points[str(point_id)]["canvas"].itemconfig(points[str(point_id)]["blade2"],state="hidden") #switched 
         points[str(point_id)]["canvas"].itemconfig(points[str(point_id)]["blade1"],state="normal") #normal
         dcc_control.update_dcc_point(point_id,False)
     return
 
 # -------------------------------------------------------------------------
+# Internal Function to update any downstream points (i.e. points
+# 'autoswitched' by the current point) - called on point creation
+# (if a point exists) and when a point is toggled via the API
+# -------------------------------------------------------------------------
+
+def update_downstream_points(point_id:int):
+    if points[str(point_id)]["alsoswitch"] != 0:
+        if not point_exists(points[str(point_id)]["alsoswitch"]):
+            logging.error ("Point "+str(point_id)+": Toggle Point - Can't \'also switch\' point "
+                    +str(points[str(point_id)]["alsoswitch"]) +" as that point does not exist")
+        elif not points[str(points[str(point_id)]["alsoswitch"])]["automatic"]:
+            logging.error ("Point "+str(point_id)+": Toggle Point - Can't \'also switch\' point "
+                    +str(points[str(point_id)]["alsoswitch"]) +" as that point is not automatic")
+        elif point_switched(point_id) != point_switched(points[str(point_id)]["alsoswitch"]):
+            logging.info ("Point "+str(point_id)+": Also changing point "+str(points[str(point_id)]["alsoswitch"]))
+            # Recursively call back into the toggle_point function to change the point
+            toggle_point(points[str(point_id)]["alsoswitch"],switched_by_another_point=True)
+    return()
+
+# -------------------------------------------------------------------------
 # Public API Function to flip the route setting for the Point (to enable
 # route setting functions. Also called whenthe POINT button is pressed 
 # Will also recursivelly call itself to change any "also_switch" points
 # -------------------------------------------------------------------------
 
 def toggle_point (point_id:int, switched_by_another_point = False):
     global points
@@ -182,24 +202,15 @@
         if points[str(point_id)]["locked"]:
             logging.warning ("Point "+str(point_id)+": Toggle Point - Point is externally locked - Toggling anyway")
         elif points[str(point_id)]["hasfpl"] and points[str(point_id)]["fpllock"]:
             logging.warning ("Point "+str(point_id)+": Toggle Point - Facing Point Lock is active - Toggling anyway")
         # Call the internal function to toggle the point state and update the drawing objects
         toggle_point_state (point_id,switched_by_another_point)
         # Now change any other points we need (i.e. points switched with this one)
-        if points[str(point_id)]["alsoswitch"] != 0:
-            if not point_exists(points[str(point_id)]["alsoswitch"]):
-                logging.error ("Point "+str(point_id)+": Toggle Point - Can't \'also switch\' point "
-                        +str(points[str(point_id)]["alsoswitch"]) +" as that point does not exist")
-            elif not points[str(points[str(point_id)]["alsoswitch"])]["automatic"]:
-                logging.error ("Point "+str(point_id)+": Toggle Point - Can't \'also switch\' point "
-                        +str(points[str(point_id)]["alsoswitch"]) +" as that point is not automatic")
-            else:   
-                logging.info ("Point "+str(point_id)+": Also changing point "+str(points[str(point_id)]["alsoswitch"]))
-                toggle_point(points[str(point_id)]["alsoswitch"],switched_by_another_point=True)
+        update_downstream_points(point_id)
     return()
 
 # -------------------------------------------------------------------------
 # Public API function to create a Point (drawing objects + state)
 # By default the point is "NOT SWITCHED" (i.e. showing the default route)
 # If the point has a Facing Point Lock then this is set to locked
 # Function returns a list of the lines that have been drawn (so an
@@ -336,14 +347,26 @@
         # Note that Toggling the point will also send the DCC commands to set the initial state
         # If we don't toggle the point we need to send out the DCC commands for the default state
         if loaded_state["switched"]: toggle_point_state(point_id)
         else: dcc_control.update_dcc_point(point_id,False)
         # Externally lock the point if required
         if loaded_state["locked"]: lock_point(point_id)
 
+        # We need to ensure that all points in an 'auto switch' chain are set to the same
+        # switched/not-switched state so they switch together correctly. First, we test to
+        # see if any existing points have already been configured to "autoswitch' the newly
+        # created point and, if so, toggle the newly created point to the same state
+        for other_point_id in points:
+            if (points[other_point_id]["alsoswitch"] == point_id and
+                   point_switched(other_point_id) != point_switched(point_id)):
+                points.toggle_point_state(point_id,True)
+        # Update any downstream points (configured to be 'autoswitched' by this point
+        # but only if they have been created (allows them to be created after this point)
+        if point_exists(points[str(point_id)]["alsoswitch"]): update_downstream_points(point_id)
+
         # We'll also return a list of identifiers for the drawing objects
         # so we can change the colour of them later if required
         # [blade straight, blade switched, route straight, route switched]
         point_objects=[blade1,blade2,route1,route2]
         
     return(point_objects)
 
@@ -439,14 +462,27 @@
         points[str(point_id)]["changebutton"].destroy()
         points[str(point_id)]["lockbutton"].destroy()
         # Finally, delete the entry from the dictionary of points
         del points[str(point_id)]
     return()
 
 # ------------------------------------------------------------------------------------------
+# Non public API function for updating the ID of the point to be 'autoswitched' by this
+# point without needing to delete the point and then create it in its new state. The main
+# use case is when bulk deleting objects via the schematic editor, where we want to avoid
+# interleaving tkinter 'create' commands in amongst the 'delete' commands outside of the
+# main tkinter loop as this can lead to problems with artefacts persisting on the canvas
+# ------------------------------------------------------------------------------------------
+
+def update_autoswitch(point_id:int, autoswitch_id:int):
+    points[str(point_id)]["alsoswitch"] = autoswitch_id
+    update_downstream_points(point_id)
+    return()
+
+# ------------------------------------------------------------------------------------------
 # Non public API function to return the tkinter canvas 'tags' for the point
 # ------------------------------------------------------------------------------------------
 
 def get_tags(point_id:int):
     return("point"+str(point_id))
 
 ###############################################################################
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-01.wav` & `model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-02.wav` & `model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-02.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-03.wav` & `model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-03.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/resources/bell-ring-04.wav` & `model-railway-signals-3.4.1/model_railway_signals/library/resources/bell-ring-04.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/resources/telegraph-key-01.wav` & `model-railway-signals-3.4.1/model_railway_signals/library/resources/telegraph-key-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals_colour_lights.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals_colour_lights.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals_common.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals_common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_disc.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals_ground_disc.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals_ground_position.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals_ground_position.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/signals_semaphores.py` & `model-railway-signals-3.4.1/model_railway_signals/library/signals_semaphores.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/track_sections.py` & `model-railway-signals-3.4.1/model_railway_signals/library/track_sections.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals/library/track_sensors.py` & `model-railway-signals-3.4.1/model_railway_signals/library/track_sensors.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/model_railway_signals.egg-info/PKG-INFO` & `model-railway-signals-3.4.1/model_railway_signals.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.4.0
+Version: 3.4.1
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
@@ -25,26 +25,22 @@
         What's currently supported by the Editor:
         * Draw your schematic with lines, points, signals, track occupancy sections and block instruments
         * Define the DCC command sequences needed to drive the signals and points out on the layout
         * Configure the signals, points and block instruments for protototypical interlocking
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
         * Configure a level of automation for the signals as trains traverse the layout
         
-        What's New in Release 3.4.0:
-        * Point and line colour selections - to enable colour coding of routes
-        * Line end-style selections - end-stops and arrow styles can now be specified
-        * Enhanced error/warning reporting via popups - reduced reliance on logs
-        * Layout 'info' function (under Help) allows you to add notes for your layout
-        * Fixed issue when selecting objects if Canvas is scrolled within the main window
-        * Various window geometry improvements to keep key UI elements visible on resizing
-        * Track section occupancy logic corrected for passing shunt-ahead ground signals
+        What's new in Release 3.4.1:
+        * Minor bug fixes and enabling work for MQTT networking
+        * Improvements to the operation of single line block instruments
+        * Some block instrument library API functions have been DEPRECATED (see PUBLIC_API.md)
         
         What's coming soon:
         * MQTT networking (for linking layouts)
-        * Better pplication documentation
+        * Better application documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
         
         There are some example layout files in the 'configuration_examples' folder.
```

### Comparing `model-railway-signals-3.4.0/model_railway_signals.egg-info/SOURCES.txt` & `model-railway-signals-3.4.1/model_railway_signals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.4.0/setup.py` & `model-railway-signals-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="model-railway-signals",
-    version="3.4.0",
+    version="3.4.1",
     packages=find_packages(),
     include_package_data=True,
     description="Create your own DCC model railway signalling scheme",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/johnrm174/model-railway-signalling",
     author="johnrm174",
```

