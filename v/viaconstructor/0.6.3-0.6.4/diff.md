# Comparing `tmp/viaconstructor-0.6.3.tar.gz` & `tmp/viaconstructor-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viaconstructor-0.6.3.tar", last modified: Thu Jul 13 13:01:22 2023, max compression
+gzip compressed data, was "viaconstructor-0.6.4.tar", last modified: Thu Jul 13 13:08:55 2023, max compression
```

## Comparing `viaconstructor-0.6.3.tar` & `viaconstructor-0.6.4.tar`

### file list

```diff
@@ -1,129 +1,133 @@
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    35147 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/LICENSE
--rw-r--r--   0 odippel   (1002) odippel   (1002)      194 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/MANIFEST.in
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/PKG-INFO
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3624 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/README.md
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/bin/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       36 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/bin/dxfpreview
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       38 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/bin/gcodepreview
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       42 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/bin/viaconstructor
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/dxfpreview/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/dxfpreview/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/dxfpreview/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     4131 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/dxfpreview/dxfpreview.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/gcodepreview/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/gcodepreview/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       96 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/gcodepreview/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3630 2022-07-22 08:53:05.000000 viaconstructor-0.6.3/gcodepreview/gcodepreview.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       38 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/setup.cfg
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     1208 2023-07-13 13:01:13.000000 viaconstructor-0.6.3/setup.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/tests/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    33786 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/tests/test_calc.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)      524 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/tests/test_dxf.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    67024 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/tests/test_gcodeparser.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     8905 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/tests/test_machine_cmds.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)      965 2023-03-28 15:03:16.000000 viaconstructor-0.6.3/tests/test_output.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/viaconstructor/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/viaconstructor/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    50033 2023-04-20 07:22:35.000000 viaconstructor-0.6.3/viaconstructor/calc.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    24883 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/draw2d.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16161 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/dxfcolors.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/ext/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/
--rw-r--r--   0 odippel   (1002) odippel   (1002)    91220 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/HersheyFonts.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       63 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      101 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/__main__.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/
--rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     8813 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/cavaliercontours.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)   872112 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)  1383488 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/meshcut/
--rw-r--r--   0 odippel   (1002) odippel   (1002)    12866 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/meshcut/meshcut.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/stl/
--rw-r--r--   0 odippel   (1002) odippel   (1002)      321 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/__about__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      375 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    22397 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/base.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3277 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/main.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       55 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/mesh.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    15642 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/stl.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      541 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/utils.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1097 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    14309 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/bezier.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    18496 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/document.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2026 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/misctools.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3939 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/parser.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)   133535 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/path.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    18991 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/paths2svg.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2473 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/polytools.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7642 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/smoothing.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7089 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_io_sax.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    11331 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_to_paths.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    53077 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/gldraw.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.094757 viaconstructor-0.6.3/viaconstructor/icons/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1577 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/camotics.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2046 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/delete.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     2633 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/exit.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1606 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/flip-x.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1348 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/flip-y.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2413 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/fonts.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3221 2023-04-26 14:19:44.000000 viaconstructor-0.6.3/viaconstructor/icons/gears.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    20293 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-setup-gcode.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16209 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-setup.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-tooltable.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      523 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/nesting.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/open.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    11071 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/openscad.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      912 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/pause.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1473 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/play.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2120 2023-03-28 10:32:37.000000 viaconstructor-0.6.3/viaconstructor/icons/redraw.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1843 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/repair.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2967 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/rotate.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    12941 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-gcode.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16787 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-setup-as.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3096 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-setup.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3484 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-tooltable.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3196 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1254 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/scale.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      291 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/select.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1759 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/start.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      729 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/stop.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1500 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/tab-selector.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2496 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/view-2d.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     4342 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/view-reset.png
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/input_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    26370 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/dxfread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     6793 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/hpglread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2455 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/imgread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7853 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/stlread.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10642 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/svgread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9352 2023-04-20 07:22:35.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/ttfread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2958 2023-04-04 14:20:30.000000 viaconstructor-0.6.3/viaconstructor/input_plugins_base.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/locales/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/locales/de/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/
--rw-r--r--   0 odippel   (1002) odippel   (1002)      345 2023-04-20 07:25:24.000000 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 odippel   (1002) odippel   (1002)     8633 2023-04-20 07:25:24.000000 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.po
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    41909 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/machine_cmd.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/output_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    10499 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_grbl.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    10647 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_linuxcnc.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7450 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/hpgl.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/preview_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10939 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/gcode.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9321 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/hpgl.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    22468 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/setupdefaults.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2560 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/vc_types.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)   126674 2023-04-26 14:20:44.000000 viaconstructor-0.6.3/viaconstructor/viaconstructor.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor.egg-info/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/PKG-INFO
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3670 2023-07-13 13:01:22.000000 viaconstructor-0.6.3/viaconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)        1 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)      109 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/requires.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    35147 2022-07-12 07:19:47.000000 viaconstructor-0.6.4/LICENSE
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      194 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/MANIFEST.in
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/PKG-INFO
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3624 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/README.md
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/bin/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       36 2022-07-12 07:19:47.000000 viaconstructor-0.6.4/bin/dxfpreview
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       38 2022-07-12 07:19:47.000000 viaconstructor-0.6.4/bin/gcodepreview
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       42 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/bin/viaconstructor
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/dxfpreview/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/dxfpreview/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/dxfpreview/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     4131 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/dxfpreview/dxfpreview.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/gcodepreview/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/gcodepreview/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       96 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/gcodepreview/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3630 2022-07-22 08:53:05.000000 viaconstructor-0.6.4/gcodepreview/gcodepreview.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       38 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/setup.cfg
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     1232 2023-07-13 13:08:10.000000 viaconstructor-0.6.4/setup.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/tests/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    33786 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/tests/test_calc.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)      524 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/tests/test_dxf.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    67024 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/tests/test_gcodeparser.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     8905 2023-04-20 07:22:38.000000 viaconstructor-0.6.4/tests/test_machine_cmds.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)      965 2023-03-28 15:03:16.000000 viaconstructor-0.6.4/tests/test_output.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.593535 viaconstructor-0.6.4/viaconstructor/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/viaconstructor/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.4/viaconstructor/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    50033 2023-04-20 07:22:35.000000 viaconstructor-0.6.4/viaconstructor/calc.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    24883 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/draw2d.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16161 2023-03-24 15:51:38.000000 viaconstructor-0.6.4/viaconstructor/dxfcolors.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/viaconstructor/ext/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.593535 viaconstructor-0.6.4/viaconstructor/ext/HersheyFonts/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    91220 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/HersheyFonts/HersheyFonts.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       63 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/HersheyFonts/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      101 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/HersheyFonts/__main__.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.593535 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     8813 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/cavaliercontours.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.593535 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/lib/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)   872112 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)  1383488 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.597535 viaconstructor-0.6.4/viaconstructor/ext/meshcut/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    12866 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/meshcut/meshcut.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.597535 viaconstructor-0.6.4/viaconstructor/ext/stl/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      321 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/__about__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      375 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    22397 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/base.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3277 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/main.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       55 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/mesh.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    15642 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/stl.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      541 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/stl/utils.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.597535 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1097 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    14309 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/bezier.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    18496 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/document.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2026 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/misctools.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3939 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/parser.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)   133535 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/path.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    18991 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/paths2svg.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2473 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/polytools.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7642 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/smoothing.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7089 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    11331 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/svg_to_paths.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    53077 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/gldraw.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.601535 viaconstructor-0.6.4/viaconstructor/icons/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1577 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/icons/camotics.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2046 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/delete.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     2633 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/exit.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1606 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/flip-x.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1348 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/flip-y.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2413 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/icons/fonts.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3221 2023-04-26 14:19:44.000000 viaconstructor-0.6.4/viaconstructor/icons/gears.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    20293 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/load-setup-gcode.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16209 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/load-setup.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/load-tooltable.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      523 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/nesting.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/open.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    11071 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/icons/openscad.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      912 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/pause.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1473 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/play.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2120 2023-03-28 10:32:37.000000 viaconstructor-0.6.4/viaconstructor/icons/redraw.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1843 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/repair.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2967 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/rotate.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    12941 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/save-gcode.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16787 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/save-setup-as.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3096 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/save-setup.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3484 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/save-tooltable.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3196 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/save.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1254 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/scale.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      291 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/select.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1759 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/start.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      729 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/stop.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1500 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/tab-selector.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2496 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/view-2d.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     4342 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/icons/view-reset.png
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.601535 viaconstructor-0.6.4/viaconstructor/input_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    26370 2023-04-20 07:22:38.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/dxfread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     6793 2023-03-24 15:51:38.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/hpglread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2455 2023-03-24 15:51:38.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/imgread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7853 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/stlread.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10642 2023-03-24 15:51:38.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/svgread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     9352 2023-04-20 07:22:35.000000 viaconstructor-0.6.4/viaconstructor/input_plugins/ttfread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2958 2023-04-04 14:20:30.000000 viaconstructor-0.6.4/viaconstructor/input_plugins_base.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/viaconstructor/locales/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.589535 viaconstructor-0.6.4/viaconstructor/locales/de/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/viaconstructor/locales/de/LC_MESSAGES/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      345 2023-04-20 07:25:24.000000 viaconstructor-0.6.4/viaconstructor/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     8633 2023-04-20 07:25:24.000000 viaconstructor-0.6.4/viaconstructor/locales/de/LC_MESSAGES/base.po
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    41909 2023-04-20 07:22:38.000000 viaconstructor-0.6.4/viaconstructor/machine_cmd.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/viaconstructor/output_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/output_plugins/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    10499 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/output_plugins/gcode_grbl.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    10647 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/output_plugins/gcode_linuxcnc.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7450 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/output_plugins/hpgl.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/viaconstructor/preview_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/preview_plugins/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10939 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/preview_plugins/gcode.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     9321 2023-04-17 11:32:29.000000 viaconstructor-0.6.4/viaconstructor/preview_plugins/hpgl.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    22468 2023-04-20 07:22:38.000000 viaconstructor-0.6.4/viaconstructor/setupdefaults.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.605535 viaconstructor-0.6.4/viaconstructor/tools/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:06:45.000000 viaconstructor-0.6.4/viaconstructor/tools/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     9012 2023-04-26 13:08:51.000000 viaconstructor-0.6.4/viaconstructor/tools/font.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     6833 2023-04-26 14:23:54.000000 viaconstructor-0.6.4/viaconstructor/tools/gear.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2560 2023-03-23 12:12:02.000000 viaconstructor-0.6.4/viaconstructor/vc_types.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)   126674 2023-04-26 14:20:44.000000 viaconstructor-0.6.4/viaconstructor/viaconstructor.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:08:55.593535 viaconstructor-0.6.4/viaconstructor.egg-info/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:08:55.000000 viaconstructor-0.6.4/viaconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3761 2023-07-13 13:08:55.000000 viaconstructor-0.6.4/viaconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        1 2023-07-13 13:08:55.000000 viaconstructor-0.6.4/viaconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      109 2023-07-13 13:08:55.000000 viaconstructor-0.6.4/viaconstructor.egg-info/requires.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-07-13 13:08:55.000000 viaconstructor-0.6.4/viaconstructor.egg-info/top_level.txt
```

### Comparing `viaconstructor-0.6.3/LICENSE` & `viaconstructor-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/PKG-INFO` & `viaconstructor-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.3
+Version: 0.6.4
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.3/README.md` & `viaconstructor-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/dxfpreview/dxfpreview.py` & `viaconstructor-0.6.4/dxfpreview/dxfpreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/gcodepreview/gcodepreview.py` & `viaconstructor-0.6.4/gcodepreview/gcodepreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/setup.py` & `viaconstructor-0.6.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import os
 from setuptools import setup
 
 
 setup(
     name='viaconstructor',
-    version='0.6.3',
+    version='0.6.4',
     author='Oliver Dippel',
     author_email='o.dippel@gmx.de',
-    packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'gcodepreview', 'dxfpreview'],
+    packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'viaconstructor.tools', 'gcodepreview', 'dxfpreview'],
     package_data={'viaconstructor.ext.cavaliercontours': ['lib/libCavalierContours.x86_64-linux.so'], 'viaconstructor/ext/nest2D': ['nest2D.cpython-39-x86_64-linux-gnu.so']},
     scripts=['bin/viaconstructor','bin/gcodepreview','bin/dxfpreview'],
     url='https://github.com/multigcs/viaconstructor',
     license='LICENSE',
     description='python based cam-tool to convert dxf into gcode',
     long_description=open('README.md').read(),
     install_requires=["PyQt5", "ezdxf", "PyOpenGL", "Pillow", "pygame", "pyclipper", "setproctitle", "freetype-py", "python-utils", "svgwrite", "matplotlib", "numpy"],
```

### Comparing `viaconstructor-0.6.3/tests/test_calc.py` & `viaconstructor-0.6.4/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/tests/test_dxf.py` & `viaconstructor-0.6.4/tests/test_dxf.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/tests/test_gcodeparser.py` & `viaconstructor-0.6.4/tests/test_gcodeparser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/tests/test_machine_cmds.py` & `viaconstructor-0.6.4/tests/test_machine_cmds.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/tests/test_output.py` & `viaconstructor-0.6.4/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/calc.py` & `viaconstructor-0.6.4/viaconstructor/calc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/draw2d.py` & `viaconstructor-0.6.4/viaconstructor/draw2d.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/dxfcolors.py` & `viaconstructor-0.6.4/viaconstructor/dxfcolors.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/HersheyFonts.py` & `viaconstructor-0.6.4/viaconstructor/ext/HersheyFonts/HersheyFonts.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/cavaliercontours.py` & `viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/cavaliercontours.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so` & `viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so` & `viaconstructor-0.6.4/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/meshcut/meshcut.py` & `viaconstructor-0.6.4/viaconstructor/ext/meshcut/meshcut.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/stl/base.py` & `viaconstructor-0.6.4/viaconstructor/ext/stl/base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/stl/main.py` & `viaconstructor-0.6.4/viaconstructor/ext/stl/main.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/stl/stl.py` & `viaconstructor-0.6.4/viaconstructor/ext/stl/stl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/stl/utils.py` & `viaconstructor-0.6.4/viaconstructor/ext/stl/utils.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/__init__.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/bezier.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/document.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/misctools.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/parser.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/path.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/paths2svg.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/polytools.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/smoothing.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_io_sax.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_to_paths.py` & `viaconstructor-0.6.4/viaconstructor/ext/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/gldraw.py` & `viaconstructor-0.6.4/viaconstructor/gldraw.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/camotics.png` & `viaconstructor-0.6.4/viaconstructor/icons/camotics.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/delete.png` & `viaconstructor-0.6.4/viaconstructor/icons/delete.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/exit.png` & `viaconstructor-0.6.4/viaconstructor/icons/exit.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/flip-x.png` & `viaconstructor-0.6.4/viaconstructor/icons/flip-x.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/flip-y.png` & `viaconstructor-0.6.4/viaconstructor/icons/flip-y.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/fonts.png` & `viaconstructor-0.6.4/viaconstructor/icons/fonts.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/gears.png` & `viaconstructor-0.6.4/viaconstructor/icons/gears.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/load-setup-gcode.png` & `viaconstructor-0.6.4/viaconstructor/icons/load-setup-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/load-setup.png` & `viaconstructor-0.6.4/viaconstructor/icons/load-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/load-tooltable.png` & `viaconstructor-0.6.4/viaconstructor/icons/load-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/nesting.png` & `viaconstructor-0.6.4/viaconstructor/icons/nesting.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/open.png` & `viaconstructor-0.6.4/viaconstructor/icons/open.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/openscad.png` & `viaconstructor-0.6.4/viaconstructor/icons/openscad.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/pause.png` & `viaconstructor-0.6.4/viaconstructor/icons/pause.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/play.png` & `viaconstructor-0.6.4/viaconstructor/icons/play.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/redraw.png` & `viaconstructor-0.6.4/viaconstructor/icons/redraw.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/repair.png` & `viaconstructor-0.6.4/viaconstructor/icons/repair.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/rotate.png` & `viaconstructor-0.6.4/viaconstructor/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/save-gcode.png` & `viaconstructor-0.6.4/viaconstructor/icons/save-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/save-setup-as.png` & `viaconstructor-0.6.4/viaconstructor/icons/save-setup-as.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/save-setup.png` & `viaconstructor-0.6.4/viaconstructor/icons/save-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/save-tooltable.png` & `viaconstructor-0.6.4/viaconstructor/icons/save-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/save.png` & `viaconstructor-0.6.4/viaconstructor/icons/save.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/scale.png` & `viaconstructor-0.6.4/viaconstructor/icons/scale.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/start.png` & `viaconstructor-0.6.4/viaconstructor/icons/start.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/stop.png` & `viaconstructor-0.6.4/viaconstructor/icons/stop.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/tab-selector.png` & `viaconstructor-0.6.4/viaconstructor/icons/tab-selector.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/view-2d.png` & `viaconstructor-0.6.4/viaconstructor/icons/view-2d.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/icons/view-reset.png` & `viaconstructor-0.6.4/viaconstructor/icons/view-reset.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/dxfread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/dxfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/hpglread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/hpglread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/imgread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/imgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/stlread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/stlread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/svgread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/svgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins/ttfread.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins/ttfread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/input_plugins_base.py` & `viaconstructor-0.6.4/viaconstructor/input_plugins_base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.po` & `viaconstructor-0.6.4/viaconstructor/locales/de/LC_MESSAGES/base.po`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/machine_cmd.py` & `viaconstructor-0.6.4/viaconstructor/machine_cmd.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_grbl.py` & `viaconstructor-0.6.4/viaconstructor/output_plugins/gcode_grbl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_linuxcnc.py` & `viaconstructor-0.6.4/viaconstructor/output_plugins/gcode_linuxcnc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/output_plugins/hpgl.py` & `viaconstructor-0.6.4/viaconstructor/output_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/preview_plugins/gcode.py` & `viaconstructor-0.6.4/viaconstructor/preview_plugins/gcode.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/preview_plugins/hpgl.py` & `viaconstructor-0.6.4/viaconstructor/preview_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/setupdefaults.py` & `viaconstructor-0.6.4/viaconstructor/setupdefaults.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/vc_types.py` & `viaconstructor-0.6.4/viaconstructor/vc_types.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor/viaconstructor.py` & `viaconstructor-0.6.4/viaconstructor/viaconstructor.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.3/viaconstructor.egg-info/PKG-INFO` & `viaconstructor-0.6.4/viaconstructor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.3
+Version: 0.6.4
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
```

### Comparing `viaconstructor-0.6.3/viaconstructor.egg-info/SOURCES.txt` & `viaconstructor-0.6.4/viaconstructor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,8 +99,11 @@
 viaconstructor/locales/de/LC_MESSAGES/base.po
 viaconstructor/output_plugins/__init__.py
 viaconstructor/output_plugins/gcode_grbl.py
 viaconstructor/output_plugins/gcode_linuxcnc.py
 viaconstructor/output_plugins/hpgl.py
 viaconstructor/preview_plugins/__init__.py
 viaconstructor/preview_plugins/gcode.py
-viaconstructor/preview_plugins/hpgl.py
+viaconstructor/preview_plugins/hpgl.py
+viaconstructor/tools/__init__.py
+viaconstructor/tools/font.py
+viaconstructor/tools/gear.py
```

