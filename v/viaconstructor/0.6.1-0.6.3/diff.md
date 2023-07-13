# Comparing `tmp/viaconstructor-0.6.1.tar.gz` & `tmp/viaconstructor-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viaconstructor-0.6.1.tar", last modified: Mon Apr  3 15:12:43 2023, max compression
+gzip compressed data, was "viaconstructor-0.6.3.tar", last modified: Thu Jul 13 13:01:22 2023, max compression
```

## Comparing `viaconstructor-0.6.1.tar` & `viaconstructor-0.6.3.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    35147 2022-07-12 07:19:47.000000 viaconstructor-0.6.1/LICENSE
--rw-r--r--   0 odippel   (1002) odippel   (1002)      194 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/MANIFEST.in
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3867 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/PKG-INFO
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3606 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/README.md
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/bin/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       36 2022-07-12 07:19:47.000000 viaconstructor-0.6.1/bin/dxfpreview
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       38 2022-07-12 07:19:47.000000 viaconstructor-0.6.1/bin/gcodepreview
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       42 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/bin/viaconstructor
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/dxfpreview/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/dxfpreview/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/dxfpreview/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     4131 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/dxfpreview/dxfpreview.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/gcodepreview/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/gcodepreview/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       96 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/gcodepreview/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3630 2022-07-22 08:53:05.000000 viaconstructor-0.6.1/gcodepreview/gcodepreview.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       38 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/setup.cfg
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     1208 2023-04-03 15:12:23.000000 viaconstructor-0.6.1/setup.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/tests/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    33786 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/tests/test_calc.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)      524 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/tests/test_dxf.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    66994 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/tests/test_gcodeparser.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     8606 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/tests/test_machine_cmds.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)      965 2023-03-28 15:03:16.000000 viaconstructor-0.6.1/tests/test_output.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.597623 viaconstructor-0.6.1/viaconstructor/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/viaconstructor/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.1/viaconstructor/__main__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    49934 2023-04-03 13:53:48.000000 viaconstructor-0.6.1/viaconstructor/calc.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    24883 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/draw2d.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16161 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/dxfcolors.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/viaconstructor/ext/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.597623 viaconstructor-0.6.1/viaconstructor/ext/HersheyFonts/
--rw-r--r--   0 odippel   (1002) odippel   (1002)    91220 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/HersheyFonts/HersheyFonts.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       63 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/HersheyFonts/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      101 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/HersheyFonts/__main__.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.597623 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/
--rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     8813 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/cavaliercontours.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.597623 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/lib/
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)   872112 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)  1383488 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.601623 viaconstructor-0.6.1/viaconstructor/ext/meshcut/
--rw-r--r--   0 odippel   (1002) odippel   (1002)    12866 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/meshcut/meshcut.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.601623 viaconstructor-0.6.1/viaconstructor/ext/stl/
--rw-r--r--   0 odippel   (1002) odippel   (1002)      321 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/__about__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      375 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    22397 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/base.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3277 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/main.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)       55 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/mesh.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    15642 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/stl.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)      541 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/stl/utils.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.601623 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1097 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    14309 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/bezier.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    18496 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/document.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2026 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/misctools.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3939 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/parser.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)   133535 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/path.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    18991 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/paths2svg.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2473 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/polytools.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7642 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/smoothing.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7089 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/svg_io_sax.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)    11331 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/svg_to_paths.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    52801 2023-04-03 15:12:12.000000 viaconstructor-0.6.1/viaconstructor/gldraw.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.605624 viaconstructor-0.6.1/viaconstructor/icons/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1577 2023-03-30 09:02:24.000000 viaconstructor-0.6.1/viaconstructor/icons/camotics.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2046 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/delete.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     2633 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/exit.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1606 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/flip-x.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1348 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/flip-y.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    20293 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/load-setup-gcode.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16209 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/load-setup.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/load-tooltable.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      523 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/nesting.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/open.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    11071 2023-03-30 09:03:41.000000 viaconstructor-0.6.1/viaconstructor/icons/openscad.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      912 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/pause.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1473 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/play.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2120 2023-03-28 10:32:37.000000 viaconstructor-0.6.1/viaconstructor/icons/redraw.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1843 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/repair.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2967 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/rotate.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    12941 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/save-gcode.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)    16787 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/save-setup-as.png
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3096 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/save-setup.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3484 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/save-tooltable.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3196 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/save.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1254 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/scale.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      291 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/select.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1759 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/start.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)      729 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/stop.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     1500 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/tab-selector.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2496 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/view-2d.png
--rw-r--r--   0 odippel   (1002) odippel   (1002)     4342 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/icons/view-reset.png
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/viaconstructor/input_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    26361 2023-03-30 09:38:54.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/dxfread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     6793 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/hpglread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2455 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/imgread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7546 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/stlread.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10642 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/svgread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9340 2023-04-03 12:13:33.000000 viaconstructor-0.6.1/viaconstructor/input_plugins/ttfread.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2958 2023-03-24 15:51:38.000000 viaconstructor-0.6.1/viaconstructor/input_plugins_base.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/viaconstructor/locales/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.593623 viaconstructor-0.6.1/viaconstructor/locales/de/
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/viaconstructor/locales/de/LC_MESSAGES/
--rw-r--r--   0 odippel   (1002) odippel   (1002)      345 2023-04-03 13:42:40.000000 viaconstructor-0.6.1/viaconstructor/locales/de/LC_MESSAGES/base.mo
--rw-r--r--   0 odippel   (1002) odippel   (1002)     8067 2023-04-03 13:42:40.000000 viaconstructor-0.6.1/viaconstructor/locales/de/LC_MESSAGES/base.po
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    41278 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/machine_cmd.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/viaconstructor/output_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/output_plugins/__init__.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9571 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/output_plugins/gcode_grbl.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9719 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/output_plugins/gcode_linuxcnc.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     7300 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/output_plugins/hpgl.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.609624 viaconstructor-0.6.1/viaconstructor/preview_plugins/
--rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/preview_plugins/__init__.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10913 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/preview_plugins/gcode.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     9321 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/preview_plugins/hpgl.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)    21314 2023-04-03 07:39:09.000000 viaconstructor-0.6.1/viaconstructor/setupdefaults.py
--rw-r--r--   0 odippel   (1002) odippel   (1002)     2560 2023-03-23 12:12:02.000000 viaconstructor-0.6.1/viaconstructor/vc_types.py
--rwxr-xr-x   0 odippel   (1002) odippel   (1002)   122985 2023-04-03 15:06:30.000000 viaconstructor-0.6.1/viaconstructor/viaconstructor.py
-drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-04-03 15:12:43.597623 viaconstructor-0.6.1/viaconstructor.egg-info/
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3867 2023-04-03 15:12:43.000000 viaconstructor-0.6.1/viaconstructor.egg-info/PKG-INFO
--rw-r--r--   0 odippel   (1002) odippel   (1002)     3608 2023-04-03 15:12:43.000000 viaconstructor-0.6.1/viaconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)        1 2023-04-03 15:12:43.000000 viaconstructor-0.6.1/viaconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)      109 2023-04-03 15:12:43.000000 viaconstructor-0.6.1/viaconstructor.egg-info/requires.txt
--rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-04-03 15:12:43.000000 viaconstructor-0.6.1/viaconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    35147 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/LICENSE
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      194 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/MANIFEST.in
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/PKG-INFO
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3624 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/README.md
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/bin/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       36 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/bin/dxfpreview
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       38 2022-07-12 07:19:47.000000 viaconstructor-0.6.3/bin/gcodepreview
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       42 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/bin/viaconstructor
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/dxfpreview/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/dxfpreview/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/dxfpreview/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     4131 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/dxfpreview/dxfpreview.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/gcodepreview/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/gcodepreview/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       96 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/gcodepreview/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3630 2022-07-22 08:53:05.000000 viaconstructor-0.6.3/gcodepreview/gcodepreview.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       38 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/setup.cfg
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     1208 2023-07-13 13:01:13.000000 viaconstructor-0.6.3/setup.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/tests/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    33786 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/tests/test_calc.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)      524 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/tests/test_dxf.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    67024 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/tests/test_gcodeparser.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     8905 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/tests/test_machine_cmds.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)      965 2023-03-28 15:03:16.000000 viaconstructor-0.6.3/tests/test_output.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/viaconstructor/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)       92 2022-07-12 07:19:48.000000 viaconstructor-0.6.3/viaconstructor/__main__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    50033 2023-04-20 07:22:35.000000 viaconstructor-0.6.3/viaconstructor/calc.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    24883 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/draw2d.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16161 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/dxfcolors.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/ext/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    91220 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/HersheyFonts.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       63 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      101 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/__main__.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     8813 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/cavaliercontours.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)   872112 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)  1383488 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/meshcut/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    12866 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/meshcut/meshcut.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/stl/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      321 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/__about__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      375 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    22397 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/base.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3277 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/main.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       55 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/mesh.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    15642 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/stl.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      541 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/stl/utils.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.090757 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1097 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    14309 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/bezier.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    18496 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/document.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2026 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/misctools.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3939 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/parser.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)   133535 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/path.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    18991 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/paths2svg.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2473 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/polytools.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7642 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/smoothing.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7089 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    11331 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_to_paths.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    53077 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/gldraw.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.094757 viaconstructor-0.6.3/viaconstructor/icons/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1577 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/camotics.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2046 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/delete.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     2633 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/exit.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1606 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/flip-x.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1348 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/flip-y.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2413 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/fonts.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3221 2023-04-26 14:19:44.000000 viaconstructor-0.6.3/viaconstructor/icons/gears.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    20293 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-setup-gcode.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16209 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-setup.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/load-tooltable.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      523 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/nesting.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2237 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/open.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    11071 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/icons/openscad.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      912 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/pause.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1473 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/play.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2120 2023-03-28 10:32:37.000000 viaconstructor-0.6.3/viaconstructor/icons/redraw.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1843 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/repair.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2967 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/rotate.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    12941 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-gcode.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    16787 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-setup-as.png
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)     3096 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-setup.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3484 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save-tooltable.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3196 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/save.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1254 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/scale.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      291 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/select.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1759 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/start.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      729 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/stop.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     1500 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/tab-selector.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2496 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/view-2d.png
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     4342 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/icons/view-reset.png
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/input_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    26370 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/dxfread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     6793 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/hpglread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2455 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/imgread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7853 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/stlread.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10642 2023-03-24 15:51:38.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/svgread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     9352 2023-04-20 07:22:35.000000 viaconstructor-0.6.3/viaconstructor/input_plugins/ttfread.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2958 2023-04-04 14:20:30.000000 viaconstructor-0.6.3/viaconstructor/input_plugins_base.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/locales/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.082757 viaconstructor-0.6.3/viaconstructor/locales/de/
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      345 2023-04-20 07:25:24.000000 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     8633 2023-04-20 07:25:24.000000 viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.po
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    41909 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/machine_cmd.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/output_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/__init__.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    10499 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_grbl.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)    10647 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_linuxcnc.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     7450 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/output_plugins/hpgl.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.098757 viaconstructor-0.6.3/viaconstructor/preview_plugins/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        0 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/__init__.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    10939 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/gcode.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     9321 2023-04-17 11:32:29.000000 viaconstructor-0.6.3/viaconstructor/preview_plugins/hpgl.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)    22468 2023-04-20 07:22:38.000000 viaconstructor-0.6.3/viaconstructor/setupdefaults.py
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     2560 2023-03-23 12:12:02.000000 viaconstructor-0.6.3/viaconstructor/vc_types.py
+-rwxr-xr-x   0 odippel   (1002) odippel   (1002)   126674 2023-04-26 14:20:44.000000 viaconstructor-0.6.3/viaconstructor/viaconstructor.py
+drwxr-xr-x   0 odippel   (1002) odippel   (1002)        0 2023-07-13 13:01:22.086757 viaconstructor-0.6.3/viaconstructor.egg-info/
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3885 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 odippel   (1002) odippel   (1002)     3670 2023-07-13 13:01:22.000000 viaconstructor-0.6.3/viaconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)        1 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)      109 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/requires.txt
+-rw-r--r--   0 odippel   (1002) odippel   (1002)       39 2023-07-13 13:01:21.000000 viaconstructor-0.6.3/viaconstructor.egg-info/top_level.txt
```

### Comparing `viaconstructor-0.6.1/LICENSE` & `viaconstructor-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/PKG-INFO` & `viaconstructor-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.1
+Version: 0.6.3
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
 
@@ -69,16 +69,17 @@
 ### thumbnail generator: dxf to jpg
 ```
 ./bin/dxfpreview tests/data/simple.dxf -o tests/data/simple.jpg
 ```
 
 ### running on macos/osx
 ```
-git clone https://github.com/multigcs/viaconstructor.git
 brew install python@3.10
+git clone https://github.com/multigcs/viaconstructor.git
+cd viaconstructor
 /usr/local/bin/python3 -m pip install -r requirements-install.txt
 /usr/local/bin/python3 -m viaconstructor tests/data/simple.dxf
 ```
 
 ### running on Windows10
 you can simply extract this zip file to you disk and execute the start.bat:
```

### Comparing `viaconstructor-0.6.1/README.md` & `viaconstructor-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,17 @@
 ### thumbnail generator: dxf to jpg
 ```
 ./bin/dxfpreview tests/data/simple.dxf -o tests/data/simple.jpg
 ```
 
 ### running on macos/osx
 ```
-git clone https://github.com/multigcs/viaconstructor.git
 brew install python@3.10
+git clone https://github.com/multigcs/viaconstructor.git
+cd viaconstructor
 /usr/local/bin/python3 -m pip install -r requirements-install.txt
 /usr/local/bin/python3 -m viaconstructor tests/data/simple.dxf
 ```
 
 ### running on Windows10
 you can simply extract this zip file to you disk and execute the start.bat:
```

### Comparing `viaconstructor-0.6.1/dxfpreview/dxfpreview.py` & `viaconstructor-0.6.3/dxfpreview/dxfpreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/gcodepreview/gcodepreview.py` & `viaconstructor-0.6.3/gcodepreview/gcodepreview.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/setup.py` & `viaconstructor-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from setuptools import setup
 
 
 setup(
     name='viaconstructor',
-    version='0.6.1',
+    version='0.6.3',
     author='Oliver Dippel',
     author_email='o.dippel@gmx.de',
     packages=['viaconstructor', 'viaconstructor.ext.cavaliercontours', 'viaconstructor.ext.HersheyFonts', 'viaconstructor.ext.meshcut', 'viaconstructor.ext.stl', 'viaconstructor.ext.svgpathtools', 'viaconstructor.input_plugins', 'viaconstructor.output_plugins', 'viaconstructor.preview_plugins', 'gcodepreview', 'dxfpreview'],
     package_data={'viaconstructor.ext.cavaliercontours': ['lib/libCavalierContours.x86_64-linux.so'], 'viaconstructor/ext/nest2D': ['nest2D.cpython-39-x86_64-linux-gnu.so']},
     scripts=['bin/viaconstructor','bin/gcodepreview','bin/dxfpreview'],
     url='https://github.com/multigcs/viaconstructor',
     license='LICENSE',
```

### Comparing `viaconstructor-0.6.1/tests/test_calc.py` & `viaconstructor-0.6.3/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/tests/test_dxf.py` & `viaconstructor-0.6.3/tests/test_dxf.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/tests/test_gcodeparser.py` & `viaconstructor-0.6.3/tests/test_gcodeparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1770,14 +1770,15 @@
                 "metric": "MM",
                 "absolute": True,
                 "feedrate": 1000.0,
                 "tool": 1,
                 "scale": 1.0,
                 "spindle": {"dir": "OFF", "rpm": 10000.0},
                 "position": {"X": 0.0, "Y": 0.0, "Z": 5.0},
+                "minmax": {},
             },
             [-22.0, -22.0, -9.0, 92.0, 42.0, 5.0],
             [114.0, 64.0, 14.0],
         ),
     ],
 )
 def test_GcodeParser_get_path(
```

### Comparing `viaconstructor-0.6.1/tests/test_machine_cmds.py` & `viaconstructor-0.6.3/tests/test_machine_cmds.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
             "mill": mill,
             "tool": {
                 "number": 1,
                 "speed": 10000,
                 "pause": 1,
                 "rate_h": 10000,
                 "rate_v": 1000,
+                "mist": False,
+                "flood": False,
             },
             "tabs": {"active": False},
             "leads": {"in": False, "out": False},
             "pockets": {
                 "insideout": False,
             },
         }
@@ -167,16 +169,19 @@
                     "view": {"path": "simple"},
                     "leads": {"active": False},
                     "machine": {
                         "mode": "mill",
                         "unit": "mm",
                         "comments": True,
                         "g54": False,
+                        "supports_toolchange": True,
                         "toolchange_pre": "",
                         "toolchange_post": "",
+                        "spindle_on_pre": "M07 (start mist)",
+                        "spindle_off_post": "M09 (stop coolant)",
                     },
                 },
                 "tablewidget": "",
                 "textwidget": "",
             },
             """(--------------------------------------------------)
 (Generator: viaConstructor)
@@ -185,14 +190,15 @@
 (--------------------------------------------------)
 
 G21 (Metric/mm)
 G40 (No Offsets)
 G90 (Absolute-Mode)
 G64 P0.05
 M05 (Spindle off)
+M09 (stop coolant)
 F1000
 G00 Z20.000000
 
 
 (--------------------------------------------------)
 (Level: 1)
 (Order: 0)
@@ -202,14 +208,15 @@
 (isPocket: False)
 (Depth: -7.0mm / -4.0mm)
 (Tool-Diameter: 4.0mm)
 (Tool-Offset: 2.0mm inside)
 (--------------------------------------------------)
 G00 Z20.0
 M06 T1
+M07 (start mist)
 M03 S10000 (Spindle on / CW)
 G04 P1 (pause in sec)
 G00 X22.000000 Y24.828427
 (- Depth: -4.0mm -)
 F1000
 G01 Z-4.000000
 F10000
@@ -261,14 +268,15 @@
 G03 X8.012233 Y100.220863 I-0.181071 J-1.991786
 G01 X-1.987767 Y10.220863
 G03 X-0.181071 Y8.008214 I1.987767 J-0.220863
 
 (- end -)
 G00 Z20.000000
 M05 (Spindle off)
+M09 (stop coolant)
 G00 X0.000000 Y0.000000
 M02
 """,
         ),
     ],
 )
 def test_polylines2machine_cmd(project, expected):
```

### Comparing `viaconstructor-0.6.1/tests/test_output.py` & `viaconstructor-0.6.3/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/calc.py` & `viaconstructor-0.6.3/viaconstructor/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 TWO_PI = math.pi * 2
 
 
 # ########## helper Functions ###########
 def external_command(cmd: str):
     known_paths = {
+        "camotics": [
+            "/Applications/CAMotics.app/Contents/MacOS/camotics",
+        ],
         "camotics.exe": [
             "c:\\Program Files\\CAMotics\\camotics.exe",
             "c:\\Program Files (x86)\\CAMotics\\camotics.exe",
         ],
         "openscad.exe": [
             "c:\\Program Files\\OpenSCAD\\openscad.exe",
             "c:\\Program Files (x86)\\OpenSCAD\\openscad.exe",
```

### Comparing `viaconstructor-0.6.1/viaconstructor/draw2d.py` & `viaconstructor-0.6.3/viaconstructor/draw2d.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/dxfcolors.py` & `viaconstructor-0.6.3/viaconstructor/dxfcolors.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/HersheyFonts/HersheyFonts.py` & `viaconstructor-0.6.3/viaconstructor/ext/HersheyFonts/HersheyFonts.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/cavaliercontours.py` & `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/cavaliercontours.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so` & `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-darwin.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so` & `viaconstructor-0.6.3/viaconstructor/ext/cavaliercontours/lib/libCavalierContours.x86_64-linux.so`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/meshcut/meshcut.py` & `viaconstructor-0.6.3/viaconstructor/ext/meshcut/meshcut.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/stl/base.py` & `viaconstructor-0.6.3/viaconstructor/ext/stl/base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/stl/main.py` & `viaconstructor-0.6.3/viaconstructor/ext/stl/main.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/stl/stl.py` & `viaconstructor-0.6.3/viaconstructor/ext/stl/stl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/stl/utils.py` & `viaconstructor-0.6.3/viaconstructor/ext/stl/utils.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/__init__.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/bezier.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/document.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/misctools.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/parser.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/path.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/path.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/paths2svg.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/polytools.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/smoothing.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/svg_io_sax.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/ext/svgpathtools/svg_to_paths.py` & `viaconstructor-0.6.3/viaconstructor/ext/svgpathtools/svg_to_paths.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/gldraw.py` & `viaconstructor-0.6.3/viaconstructor/gldraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -989,31 +989,38 @@
         GL.glBegin(GL.GL_LINES)
         draw_text(
             f"{round(size_y, 2)}", end_x + 5, center_y, mill_depth, 0.5, False, True
         )
         GL.glEnd()
 
 
-def draw_object_ids(project: dict) -> None:
+def draw_object_ids(project: dict, selected: int = -1) -> None:
     """draws the object id's as text"""
     GL.glNormal3f(0, 0, 1)
-    GL.glLineWidth(2)
-    GL.glColor3f(0.63, 0.36, 0.11)
-    GL.glBegin(GL.GL_LINES)
     for obj_idx, obj in project["objects"].items():
+
+        if obj_idx.split(":")[0] == selected:
+            GL.glLineWidth(2)
+            GL.glColor3f(1.0, 1.0, 1.01)
+        else:
+            GL.glLineWidth(2)
+            GL.glColor3f(0.63, 0.36, 0.11)
+
+        GL.glBegin(GL.GL_LINES)
+
         if obj.get("layer", "").startswith("BREAKS:") or obj.get(
             "layer", ""
         ).startswith("_TABS"):
             continue
         p_x = obj["segments"][0]["start"][0]
         p_y = obj["segments"][0]["start"][1]
         for (x_1, y_1), (x_2, y_2) in font.lines_for_text(f"#{obj_idx.split(':')[0]}"):
             GL.glVertex3f(p_x + x_1, p_y + y_1, 5.0)
             GL.glVertex3f(p_x + x_2, p_y + y_2, 5.0)
-    GL.glEnd()
+        GL.glEnd()
 
 
 def draw_object_edges(project: dict, selected: int = -1) -> None:
     """draws the edges of an object"""
     unit = project["setup"]["machine"]["unit"]
     depth = project["setup"]["mill"]["depth"]
     tabs_height = project["setup"]["tabs"]["height"]
@@ -1047,19 +1054,18 @@
                 color = dxfcolors[obj.color][0:3]
 
             odepth = obj["setup"]["mill"]["depth"]
             if odepth > depth:
                 continue
 
             if obj_idx.split(":")[0] == selected:
-                GL.glLineWidth(5)
-                GL.glColor4f(1.0, 0.0, 0.0, 1.0)
+                GL.glLineWidth(4)
+                GL.glColor4f(1.0, 1.0, 1.0, 1.0)
             else:
                 GL.glLineWidth(2)
-                # GL.glColor4f(1.0, 1.0, 1.0, 1.0)
                 GL.glColor3f(*color)
 
             # side
             GL.glBegin(GL.GL_LINES)
             for segment in obj.segments:
                 p_x = segment.start[0]
                 p_y = segment.start[1]
@@ -1376,43 +1382,47 @@
                         line[0]["Z"],
                         0.2,
                         True,
                         True,
                     )
                     GL.glEnd()
                 draw_line(line[0], line[1], line[2], project, tool_number)
+            project["outputMinMax"] = gcode_parser.get_minmax()
+
         elif project["suffix"] in {"hpgl", "hpg"}:
             project["setup"]["machine"]["g54"] = False
             project["setup"]["workpiece"]["offset_z"] = 0.0
             hpgl_parser = HpglParser(project["machine_cmd"])
             toolpath = hpgl_parser.get_path()
             for line in toolpath:
                 draw_line(line[0], line[1], line[2], project)
+            project["outputMinMax"] = gcode_parser.get_minmax()
+
     except Exception as error_string:  # pylint: disable=W0703:
         print(f"ERROR: parsing machine_cmd: {error_string}")
         return False
     return True
 
 
 def draw_all(project: dict) -> None:
+    selected = project["object_active"]
+
     project["gllist"] = GL.glGenLists(1)
     GL.glNewList(project["gllist"], GL.GL_COMPILE)
     draw_grid(project)
 
     if project["setup"]["view"]["3d_show"]:
         if hasattr(project["draw_reader"], "draw_3d"):
             project["draw_reader"].draw_3d()
 
     if project["glwidget"] and project["glwidget"].selector_mode != "repair":
         if not draw_machinecode_path(project):
             print("error while drawing machine commands")
 
     if project["setup"]["view"]["object_ids"]:
-        draw_object_ids(project)
-
-    selected = project["object_active"]
+        draw_object_ids(project, selected=selected)
 
     draw_object_edges(project, selected=selected)
     if project["setup"]["view"]["polygon_show"]:
         draw_object_faces(project)
 
     GL.glEndList()
```

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/camotics.png` & `viaconstructor-0.6.3/viaconstructor/icons/camotics.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/delete.png` & `viaconstructor-0.6.3/viaconstructor/icons/delete.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/exit.png` & `viaconstructor-0.6.3/viaconstructor/icons/exit.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/flip-x.png` & `viaconstructor-0.6.3/viaconstructor/icons/flip-x.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/flip-y.png` & `viaconstructor-0.6.3/viaconstructor/icons/flip-y.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/load-setup-gcode.png` & `viaconstructor-0.6.3/viaconstructor/icons/load-setup-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/load-setup.png` & `viaconstructor-0.6.3/viaconstructor/icons/load-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/load-tooltable.png` & `viaconstructor-0.6.3/viaconstructor/icons/load-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/nesting.png` & `viaconstructor-0.6.3/viaconstructor/icons/nesting.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/open.png` & `viaconstructor-0.6.3/viaconstructor/icons/open.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/openscad.png` & `viaconstructor-0.6.3/viaconstructor/icons/openscad.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/pause.png` & `viaconstructor-0.6.3/viaconstructor/icons/pause.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/play.png` & `viaconstructor-0.6.3/viaconstructor/icons/play.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/redraw.png` & `viaconstructor-0.6.3/viaconstructor/icons/redraw.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/repair.png` & `viaconstructor-0.6.3/viaconstructor/icons/repair.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/rotate.png` & `viaconstructor-0.6.3/viaconstructor/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/save-gcode.png` & `viaconstructor-0.6.3/viaconstructor/icons/save-gcode.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/save-setup-as.png` & `viaconstructor-0.6.3/viaconstructor/icons/save-setup-as.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/save-setup.png` & `viaconstructor-0.6.3/viaconstructor/icons/save-setup.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/save-tooltable.png` & `viaconstructor-0.6.3/viaconstructor/icons/save-tooltable.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/save.png` & `viaconstructor-0.6.3/viaconstructor/icons/save.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/scale.png` & `viaconstructor-0.6.3/viaconstructor/icons/scale.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/start.png` & `viaconstructor-0.6.3/viaconstructor/icons/start.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/stop.png` & `viaconstructor-0.6.3/viaconstructor/icons/stop.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/tab-selector.png` & `viaconstructor-0.6.3/viaconstructor/icons/tab-selector.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/view-2d.png` & `viaconstructor-0.6.3/viaconstructor/icons/view-2d.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/icons/view-reset.png` & `viaconstructor-0.6.3/viaconstructor/icons/view-reset.png`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/dxfread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/dxfread.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
             print(f"dxfread: selected layers: {', '.join(self.selected_layers)}")
 
     def add_entity(self, element, offset: tuple = (0, 0)):
         dxftype = element.dxftype()
         layer = element.dxf.layer
         color = element.dxf.color
         if color == 256:
-            color = self.layer_colors[layer]
+            color = self.layer_colors.get(layer) or 1
 
         if self.color_layers:
             colorname = dxfcolors[color][3] or f"c{color}"
             layer = f"{layer}-{colorname}"
 
         if self.select_layers and layer not in self.select_layers:
             if layer not in self.filtered_layers:
```

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/hpglread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/hpglread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/imgread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/imgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/stlread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/stlread.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,27 @@
                 min_z = self.verts_3d[0][2]
                 max_z = min_z
                 for vert in self.verts_3d:
                     value_z = vert[2]
                     min_z = min(min_z, value_z)
                     max_z = max(max_z, value_z)
 
+        """
+        zlayers = {}
+        for vert in verts:
+            #print(vert[2])
+            if vert[2] not in zlayers:
+                zlayers[vert[2]] = 0
+            zlayers[vert[2]] += 1
+
+        for h, n in zlayers.items():
+            if n > 2:
+                print("### ", h, n)
+        """
+
         mesh = meshcut.TriangleMesh(verts, faces)
         self.diff_z = max_z - min_z
 
         print(f"STL: INFO: z_min={min_z}, z_max={max_z}")
 
         slice_z = None
         if args.stlread_zslice:  # type: ignore
```

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/svgread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/svgread.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins/ttfread.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins/ttfread.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         message = QLabel("Import-Options")
         dialog.layout.addWidget(message)
 
         label = QLabel("Text")
         dialog.layout.addWidget(label)
 
         ttfread_text = QPlainTextEdit()
-        ttfread_text.setPlainText("Via")
+        ttfread_text.setPlainText(args.ttfread_text)
         dialog.layout.addWidget(ttfread_text)
 
         label = QLabel("Height")
         dialog.layout.addWidget(label)
         ttfread_height = QDoubleSpinBox()
         ttfread_height.setDecimals(3)
         ttfread_height.setSingleStep(0.1)
```

### Comparing `viaconstructor-0.6.1/viaconstructor/input_plugins_base.py` & `viaconstructor-0.6.3/viaconstructor/input_plugins_base.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/locales/de/LC_MESSAGES/base.po` & `viaconstructor-0.6.3/viaconstructor/locales/de/LC_MESSAGES/base.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2023-04-03 15:42+0200\n"
+"POT-Creation-Date: 2023-04-20 09:25+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -137,14 +137,26 @@
 
 msgid "Pause"
 msgstr ""
 
 msgid "tool spin up time (G04 Pn)"
 msgstr ""
 
+msgid "Mist"
+msgstr ""
+
+msgid "activate mist"
+msgstr ""
+
+msgid "Flood"
+msgstr ""
+
+msgid "activate flood"
+msgstr ""
+
 msgid "Tools"
 msgstr ""
 
 msgid "tooltable"
 msgstr ""
 
 msgid "original"
@@ -329,26 +341,41 @@
 
 msgid "Unit of the machine"
 msgstr ""
 
 msgid "machine supports g54"
 msgstr ""
 
+msgid "machine supports toolchange"
+msgstr ""
+
 msgid "toolchange pre cmd"
 msgstr ""
 
 msgid "add gcode before tool-change"
 msgstr ""
 
 msgid "toolchange post cmd"
 msgstr ""
 
 msgid "add gcode after tool-change"
 msgstr ""
 
+msgid "spindle on pre cmd"
+msgstr ""
+
+msgid "add gcode before turning the spindle on"
+msgstr ""
+
+msgid "spindle off post cmd"
+msgstr ""
+
+msgid "add gcode after turning the spindle off"
+msgstr ""
+
 msgid "Comments in output"
 msgstr ""
 
 msgid "add comments to output"
 msgstr ""
 
 msgid "line numbers"
@@ -605,14 +632,20 @@
 
 msgid "update calculation and redraw"
 msgstr ""
 
 msgid "Calculation"
 msgstr ""
 
+msgid "Font-Tool"
+msgstr ""
+
+msgid "open fonttool"
+msgstr ""
+
 msgid "select this row"
 msgstr ""
 
 msgid "move left"
 msgstr ""
 
 msgid "move right"
@@ -620,18 +653,30 @@
 
 msgid "move up"
 msgstr ""
 
 msgid "move down"
 msgstr ""
 
-msgid "rotate left"
+msgid "CCW"
+msgstr ""
+
+msgid "rotate counter clockwise"
 msgstr ""
 
-msgid "rotate right"
+msgid "CW"
+msgstr ""
+
+msgid "rotate clockwise"
+msgstr ""
+
+msgid "scale"
+msgstr ""
+
+msgid "clone object"
 msgstr ""
 
 msgid "Manipulate"
 msgstr ""
 
 msgid "Reader-Selection"
 msgstr ""
@@ -670,7 +715,10 @@
 msgstr ""
 
 msgid "&Objects"
 msgstr ""
 
 msgid "&Layers"
 msgstr ""
+
+msgid "&Infos"
+msgstr ""
```

### Comparing `viaconstructor-0.6.1/viaconstructor/machine_cmd.py` & `viaconstructor-0.6.3/viaconstructor/machine_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,23 @@
 
     def move(self, x_pos=None, y_pos=None, z_pos=None) -> None:
         pass
 
     def tool(self, number="1") -> None:
         pass
 
+    def coolant_mist(self) -> None:
+        pass
+
+    def coolant_flood(self) -> None:
+        pass
+
+    def coolant_off(self) -> None:
+        pass
+
     def spindle_off(self) -> None:
         pass
 
     def spindle_cw(self, speed: int, pause: int = 1) -> None:
         pass
 
     def spindle_ccw(self, speed: int, pause: int = 1) -> None:
@@ -649,14 +658,16 @@
                     polylines_n += 1
 
                     milling.add(nearest_idx)
                     polyline = polylines[nearest_idx]
                     vertex_data = vertex_data_cache(polyline)
                     is_closed = polyline.is_closed()
 
+                    coolant_mist = polyline.setup["tool"]["mist"]
+                    coolant_flood = polyline.setup["tool"]["flood"]
                     max_depth = polyline.setup["mill"]["depth"]
                     step = polyline.setup["mill"]["step"]
                     if step >= -0.01:
                         step = -0.01
                     if unit == "inch":
                         unitscale = 25.4
                         max_depth *= unitscale
@@ -736,25 +747,31 @@
                         post.comment(
                             "--------------------------------------------------"
                         )
 
                     # toolchange
                     if project["setup"]["machine"]["mode"] == "mill":
                         post.move(z_pos=fast_move_z)
-                        post.tool(polyline.setup["tool"]["number"])
+                        if project["setup"]["machine"]["supports_toolchange"]:
+                            post.tool(polyline.setup["tool"]["number"])
                         post.spindle_cw(
                             polyline.setup["tool"]["speed"],
                             polyline.setup["tool"]["pause"],
                         )
 
                     depth = step
                     depth = max(depth, max_depth)
                     min_depth = polyline.setup["mill"]["start_depth"]
                     depth = min(depth, min_depth)
 
+                    if coolant_mist:
+                        post.coolant_mist()
+                    if coolant_flood:
+                        post.coolant_flood()
+
                     if (
                         project["setup"]["machine"]["mode"] == "mill"
                         and "Z" in project["axis"]
                     ):
                         if not (was_pocket and nearest_dist < diameter):
                             post.move(z_pos=fast_move_z)
                         elif helix_mode:
@@ -1028,13 +1045,17 @@
                         post.spindle_off()
 
                     if is_closed:
                         last_pos = points[0]
                     else:
                         last_pos = points[-1]
                     order += 1
+
+                    if coolant_mist or coolant_flood:
+                        post.coolant_off()
+
                 else:
                     break
 
     machine_cmd_end(project, post)
     print("")
     return post.get(numbers=project["setup"]["machine"].get("numbers", False))
```

### Comparing `viaconstructor-0.6.1/viaconstructor/output_plugins/gcode_grbl.py` & `viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_grbl.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,18 +153,35 @@
 
     def spindle_off(self) -> None:
         if self.comments:
             self.gcode.append("M05 (Spindle off)")
         else:
             self.gcode.append("M05")
         self.tool_running = 0
+        if self.project["setup"]["machine"]["spindle_off_post"]:
+            for part in self.project["setup"]["machine"]["spindle_off_post"].split(
+                "\n"
+            ):
+                self.gcode.append(part)
+
+    def coolant_mist(self) -> None:
+        self.gcode.append("M07 (mist on)")
+
+    def coolant_flood(self) -> None:
+        self.gcode.append("M08 (flood on)")
+
+    def coolant_off(self) -> None:
+        self.gcode.append("M09 (coolant off)")
 
     def spindle_cw(self, speed: int, pause: int = 1) -> None:
         if self.tool_running != 0 and self.tool_running == speed:
             return
+        if self.project["setup"]["machine"]["spindle_on_pre"]:
+            for part in self.project["setup"]["machine"]["spindle_on_pre"].split("\n"):
+                self.gcode.append(part)
         cmd = "M03"
         if self.speed != speed:
             self.speed = speed
             cmd += f" S{speed}"
         if self.comments:
             cmd += " (Spindle on / CW)"
         self.gcode.append(cmd)
@@ -174,14 +191,18 @@
                 self.gcode.append(f"G04 P{pause} (pause in sec)")
             else:
                 self.gcode.append(f"G04 P{pause}")
 
         self.tool_running = self.speed
 
     def spindle_ccw(self, speed: int, pause: int = 1) -> None:
+        # no if self.tool_running != 0 and self.tool_running == speed test?
+        if self.project["setup"]["machine"]["spindle_on_pre"]:
+            for part in self.project["setup"]["machine"]["spindle_on_pre"].split("\n"):
+                self.gcode.append(part)
         cmd = "M04"
         if self.speed != speed:
             self.speed = speed
             cmd += f" S{speed}"
         if self.comments:
             cmd += " (Spindle on / CW)"
         self.gcode.append(cmd)
```

### Comparing `viaconstructor-0.6.1/viaconstructor/output_plugins/gcode_linuxcnc.py` & `viaconstructor-0.6.3/viaconstructor/output_plugins/gcode_linuxcnc.py`

 * *Files 11% similar despite different names*

```diff
@@ -152,18 +152,35 @@
 
     def spindle_off(self) -> None:
         if self.comments:
             self.gcode.append("M05 (Spindle off)")
         else:
             self.gcode.append("M05")
         self.tool_running = 0
+        if self.project["setup"]["machine"]["spindle_off_post"]:
+            for part in self.project["setup"]["machine"]["spindle_off_post"].split(
+                "\n"
+            ):
+                self.gcode.append(part)
+
+    def coolant_mist(self) -> None:
+        self.gcode.append("M07 (mist on)")
+
+    def coolant_flood(self) -> None:
+        self.gcode.append("M08 (flood on)")
+
+    def coolant_off(self) -> None:
+        self.gcode.append("M09 (coolant off)")
 
     def spindle_cw(self, speed: int, pause: int = 1) -> None:
         if self.tool_running != 0 and self.tool_running == speed:
             return
+        if self.project["setup"]["machine"]["spindle_on_pre"]:
+            for part in self.project["setup"]["machine"]["spindle_on_pre"].split("\n"):
+                self.gcode.append(part)
         cmd = "M03"
         if self.speed != speed:
             self.speed = speed
             cmd += f" S{speed}"
         if self.comments:
             cmd += " (Spindle on / CW)"
         self.gcode.append(cmd)
@@ -173,14 +190,18 @@
                 self.gcode.append(f"G04 P{pause} (pause in sec)")
             else:
                 self.gcode.append(f"G04 P{pause}")
 
         self.tool_running = self.speed
 
     def spindle_ccw(self, speed: int, pause: int = 1) -> None:
+        # no if self.tool_running != 0 and self.tool_running == speed test?
+        if self.project["setup"]["machine"]["spindle_on_pre"]:
+            for part in self.project["setup"]["machine"]["spindle_on_pre"].split("\n"):
+                self.gcode.append(part)
         cmd = "M04"
         if self.speed != speed:
             self.speed = speed
             cmd += f" S{speed}"
         if self.comments:
             cmd += " (Spindle on / CW)"
         self.gcode.append(cmd)
```

### Comparing `viaconstructor-0.6.1/viaconstructor/output_plugins/hpgl.py` & `viaconstructor-0.6.3/viaconstructor/output_plugins/hpgl.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,23 @@
     def comment(self, text) -> None:
         if self.comments:
             self.hpgl.append(f"CO {text}")
 
     def tool(self, number="1") -> None:
         self.hpgl.append(f"SP{number}")
 
+    def coolant_mist(self) -> None:
+        pass
+
+    def coolant_flood(self) -> None:
+        pass
+
+    def coolant_off(self) -> None:
+        pass
+
     def spindle_cw(self, speed: int, pause: int = 1) -> None:  # pylint: disable=W0613
         self.toolrun = True
 
     def spindle_ccw(self, speed: int, pause: int = 1) -> None:  # pylint: disable=W0613
         self.toolrun = True
 
     def spindle_off(self) -> None:
```

### Comparing `viaconstructor-0.6.1/viaconstructor/preview_plugins/gcode.py` & `viaconstructor-0.6.3/viaconstructor/preview_plugins/gcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             "offsets": "OFF",
             "metric": "",
             "absolute": True,
             "feedrate": "0",
             "tool": None,
             "spindle": {"dir": "OFF", "rpm": 0},
             "position": {"X": 0.0, "Y": 0.0, "Z": 0.0},
+            "minmax": {},
         }
 
         self.path: list[list] = []
         self.gcode = gcode
         for line in self.gcode:
             line = line.strip()
             if not line or line[0] == "(":
```

### Comparing `viaconstructor-0.6.1/viaconstructor/preview_plugins/hpgl.py` & `viaconstructor-0.6.3/viaconstructor/preview_plugins/hpgl.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/setupdefaults.py` & `viaconstructor-0.6.3/viaconstructor/setupdefaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,14 +168,28 @@
                 "min": 0,
                 "max": 60,
                 "title": _("Pause"),
                 "tooltip": _("tool spin up time (G04 Pn)"),
                 "unit": "s",
                 "per_object": True,
             },
+            "mist": {
+                "default": False,
+                "type": "bool",
+                "per_object": True,
+                "title": _("Mist"),
+                "tooltip": _("activate mist"),
+            },
+            "flood": {
+                "default": False,
+                "type": "bool",
+                "per_object": True,
+                "title": _("Flood"),
+                "tooltip": _("activate flood"),
+            },
             "tooltable": {
                 "type": "table",
                 "selectable": True,
                 "default": [
                     {
                         "name": "Wood cutter (small)",
                         "number": 1,
@@ -504,26 +518,44 @@
             },
             "g54": {
                 "default": False,
                 "type": "bool",
                 "title": _("machine supports g54"),
                 "tooltip": _("machine supports g54"),
             },
+            "supports_toolchange": {
+                "default": True,
+                "type": "bool",
+                "title": _("machine supports toolchange"),
+                "tooltip": _("machine supports toolchange"),
+            },
             "toolchange_pre": {
                 "default": "",
                 "type": "mstr",
                 "title": _("toolchange pre cmd"),
                 "tooltip": _("add gcode before tool-change"),
             },
             "toolchange_post": {
                 "default": "",
                 "type": "mstr",
                 "title": _("toolchange post cmd"),
                 "tooltip": _("add gcode after tool-change"),
             },
+            "spindle_on_pre": {
+                "default": "",
+                "type": "mstr",
+                "title": _("spindle on pre cmd"),
+                "tooltip": _("add gcode before turning the spindle on"),
+            },
+            "spindle_off_post": {
+                "default": "",
+                "type": "mstr",
+                "title": _("spindle off post cmd"),
+                "tooltip": _("add gcode after turning the spindle off"),
+            },
             "comments": {
                 "default": True,
                 "type": "bool",
                 "title": _("Comments in output"),
                 "tooltip": _("add comments to output"),
             },
             "numbers": {
```

### Comparing `viaconstructor-0.6.1/viaconstructor/vc_types.py` & `viaconstructor-0.6.3/viaconstructor/vc_types.py`

 * *Files identical despite different names*

### Comparing `viaconstructor-0.6.1/viaconstructor/viaconstructor.py` & `viaconstructor-0.6.3/viaconstructor/viaconstructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     get_tmp_prefix,
     mirror_objects,
     move_object,
     move_objects,
     object2points,
     objects2minmax,
     objects2polyline_offsets,
+    points_to_boundingbox,
     points_to_center,
     rotate_object,
     rotate_objects,
     scale_object,
     scale_objects,
     segments2objects,
 )
@@ -75,14 +76,16 @@
 from .gldraw import draw_all as draw_all_gl
 from .machine_cmd import polylines2machine_cmd
 from .output_plugins.gcode_grbl import PostProcessorGcodeGrbl
 from .output_plugins.gcode_linuxcnc import PostProcessorGcodeLinuxCNC
 from .output_plugins.hpgl import PostProcessorHpgl
 from .preview_plugins.gcode import GcodeParser
 from .setupdefaults import setup_defaults
+from .tools.font import FontTool
+from .tools.gear import GearTool
 
 try:
     from .ext.nest2D.nest2D import (  # pylint: disable=E0611
         Box,
         Item,
         Point,
         SVGWriter,
@@ -164,14 +167,15 @@
         "machine_cmd": "",
         "segments": {},
         "objects": {},
         "offsets": {},
         "gllist": [],
         "maxOuter": [],
         "minMax": [],
+        "outputMinMax": [],
         "table": [],
         "glwidget": None,
         "imgwidget": None,
         "preview_generate": None,
         "preview_open": None,
         "status": "INIT",
         "tabs": {
@@ -190,14 +194,15 @@
         "object_active": "",
     }
     info = ""
     save_tabs = "no"
     save_starts = "no"
     combobjwidget = None
     status_bar: Optional[QStatusBar] = None
+    infotext_widget: Optional[QPlainTextEdit] = None
     main: Optional[QMainWindow] = None
     toolbar: Optional[QToolBar] = None
     menubar: Optional[QMenuBar] = None
     toolbuttons: dict = {}
 
     module_root = Path(__file__).resolve().parent
 
@@ -322,14 +327,20 @@
         if self.project["textwidget"]:
             self.project["textwidget"].clear()
             self.project["textwidget"].insertPlainText(self.project["machine_cmd"])
             self.project["textwidget"].verticalScrollBar().setValue(0)
 
         debug("run_calculation: done")
 
+    def _toolbar_fonttool(self) -> None:
+        self.font_tool.show()
+
+    def _toolbar_geartool(self) -> None:
+        self.gear_tool.show()
+
     def _toolbar_flipx(self) -> None:
         mirror_objects(self.project["objects"], self.project["minMax"], vertical=True)
         self.project["minMax"] = objects2minmax(self.project["objects"])
         self.update_tabs_data()
         self.update_drawing()
 
     def _toolbar_flipy(self) -> None:
@@ -766,14 +777,24 @@
 
         if self.project["engine"] == "2D":
             draw_all_2d(self.project)
         else:
             draw_all_gl(self.project)
 
         self.info = f"{round(self.project['minMax'][2] - self.project['minMax'][0], 2)}x{round(self.project['minMax'][3] - self.project['minMax'][1], 2)}mm"
+
+        infotext = f"Drawing: {self.info}\n"
+        if self.project["outputMinMax"]:
+            infotext += "Machine-Limits:\n"
+            infotext += f" X: {round(self.project['outputMinMax'][0])} mm -> {round(self.project['outputMinMax'][3])} mm\n"
+            infotext += f" Y: {round(self.project['outputMinMax'][1])} mm -> {round(self.project['outputMinMax'][4])} mm\n"
+            infotext += f" Z: {round(self.project['outputMinMax'][2])} mm -> {round(self.project['outputMinMax'][5])} mm\n"
+        if self.infotext_widget is not None:
+            self.infotext_widget.setPlainText(infotext)
+
         if self.main:
             self.main.setWindowTitle("viaConstructor")
         self.status_bar_message(f"{self.info} - calculate..done")
         self.update_layers()
         debug("update_drawing: done")
 
     def save_project(self, filename: str) -> bool:
@@ -1629,15 +1650,15 @@
                 True,
                 _("Mouse"),
                 "set",
                 None,
             ],
             _("Repair-Selector"): [
                 "repair.png",
-                "Ctrl+F",
+                "",
                 _("Repair-Selector"),
                 self._toolbar_toggle_repair_selector,
                 True,
                 True,
                 True,
                 _("Mouse"),
                 "edit",
@@ -1711,14 +1732,38 @@
                 True,
                 True,
                 False,
                 _("Calculation"),
                 "",
                 None,
             ],
+            _("Font-Tool"): [
+                "fonts.png",
+                "Ctrl+F",
+                _("open fonttool"),
+                self._toolbar_fonttool,
+                False,
+                True,
+                False,
+                _("Tools"),
+                "exit",
+                None,
+            ],
+            _("Gear-Tool"): [
+                "gears.png",
+                "Ctrl+G",
+                _("open geartool"),
+                self._toolbar_geartool,
+                False,
+                True,
+                False,
+                _("Tools"),
+                "exit",
+                None,
+            ],
         }
 
     def create_toolbar(self) -> None:
         """creates the_toolbar."""
         if self.toolbar is None:
             self.toolbar = QToolBar("top toolbar")
             self.main.addToolBar(self.toolbar)  # type: ignore
@@ -1972,15 +2017,15 @@
                             item = QTableWidgetItem(str(row[key]))
                             table.setItem(
                                 row_idx,
                                 col_idx + idxf_offset,
                                 item,
                             )
                             # if entry["columns"][key].get("ro", False):
-                            #    item.setFlags(QtCore.Qt.ItemIsEditable)
+                            #    item.setFlags(Qt.ItemIsEditable)
                             table.resizeColumnToContents(col_idx + idxf_offset)
                     table.itemChanged.connect(self.global_changed)  # type: ignore
                     vlayout.addWidget(table)
                     entry["widget"] = table
                 else:
                     eprint(f"Unknown setup-type: {entry['type']}")
 
@@ -2250,15 +2295,15 @@
                             item = QTableWidgetItem(str(row[key]))
                             table.setItem(
                                 row_idx,
                                 col_idx + idxf_offset,
                                 item,
                             )
                             # if entry["columns"][key].get("ro", False):
-                            #    item.setFlags(QtCore.Qt.ItemIsEditable)
+                            #    item.setFlags(Qt.ItemIsEditable)
                             table.resizeColumnToContents(col_idx + idxf_offset)
                     table.itemChanged.connect(self.object_changed)  # type: ignore
                     vlayout.addWidget(table)
                     entry["widget_obj"] = table
                 else:
                     eprint(f"Unknown setup-type: {entry['type']}")
 
@@ -2345,17 +2390,17 @@
         button.clicked.connect(partial(object_move, dspinbox, checkbox, "down"))  # type: ignore
         glayout.addWidget(button, 2, 1)
 
         def object_rotate(spinbox_angle, checkbox_childs, direction):
             object_active = self.project["object_active"]
             with_childs = checkbox_childs.isChecked()
             diff = spinbox_angle.value()
-            if direction == "left":
+            if direction == "ccw":
                 angle = diff
-            elif direction == "right":
+            elif direction == "cw":
                 angle = -diff
 
             object_active_obj = None
             for obj_idx, obj in self.project["objects"].items():
                 if obj_idx.startswith(f"{object_active}:"):
                     object_active_obj = obj
 
@@ -2394,22 +2439,22 @@
         vlayout.addWidget(checkbox)
 
         gcontainer = QWidget()
         glayout = QGridLayout()
         gcontainer.setLayout(glayout)
         vlayout.addWidget(gcontainer)
 
-        button = QPushButton("Left")
-        button.setToolTip(_("rotate left"))
-        button.clicked.connect(partial(object_rotate, dspinbox, checkbox, "left"))  # type: ignore
+        button = QPushButton(_("CCW"))
+        button.setToolTip(_("rotate counter clockwise"))
+        button.clicked.connect(partial(object_rotate, dspinbox, checkbox, "ccw"))  # type: ignore
         glayout.addWidget(button, 0, 0)
 
-        button = QPushButton("Right")
-        button.setToolTip(_("rotate right"))
-        button.clicked.connect(partial(object_rotate, dspinbox, checkbox, "right"))  # type: ignore
+        button = QPushButton(_("CW"))
+        button.setToolTip(_("rotate clockwise"))
+        button.clicked.connect(partial(object_rotate, dspinbox, checkbox, "cw"))  # type: ignore
         glayout.addWidget(button, 0, 1)
 
         def object_scale(spinbox_scale, checkbox_childs):
             object_active = self.project["object_active"]
             with_childs = checkbox_childs.isChecked()
             scale = spinbox_scale.value()
 
@@ -2457,47 +2502,76 @@
         vlayout.addWidget(gcontainer)
 
         button = QPushButton("Scale")
         button.setToolTip(_("scale"))
         button.clicked.connect(partial(object_scale, dspinbox, checkbox))  # type: ignore
         glayout.addWidget(button, 0, 0)
 
-        def clone_object(obj_idx):
+        def clone_object(obj_idx, offset_x=0, offset_y=0):
+            if not obj_idx:
+                return None
             main_idx = obj_idx.split(":")[0]
             main_uid = obj_idx.split(":")[1]
             idx_list = [oid.split(":")[0] for oid in self.project["objects"]]
             sub_idx = 1
             while f"{main_idx},{sub_idx}" in idx_list:
                 sub_idx += 1
             new_obj_idx = f"{main_idx},{sub_idx}:{main_uid}"
             self.project["objects"][new_obj_idx] = deepcopy(
                 self.project["objects"][obj_idx]
             )
+
             move_object(
                 self.project["objects"][new_obj_idx],
-                (self.project["minMax"][2] - self.project["minMax"][0]) + 10,
-                0,
+                offset_x,
+                offset_y,
             )
             return new_obj_idx
 
-        def object_copy(checkbox_childs):
+        def object_copy(checkbox_childs, offset_direction):
             object_active = self.project["object_active"]
             with_childs = checkbox_childs.isChecked()
 
             object_active_obj = None
             object_active_obj_idx = ""
             for obj_idx, obj in self.project["objects"].items():
                 if obj_idx.startswith(f"{object_active}:"):
                     object_active_obj = obj
                     object_active_obj_idx = obj_idx
 
-            new_obj_idx = clone_object(object_active_obj_idx)
-            if with_childs:
+            bounding_box = points_to_boundingbox(
+                object2points(self.project["objects"][object_active_obj_idx])
+            )
+            offset_x = 0
+            offset_y = 0
+            if offset_direction == "left":
+                offset_x = (
+                    0 - (bounding_box[2] - bounding_box[0]) - bounding_box[0] - 10
+                )
+            elif offset_direction == "right":
+                offset_x = (
+                    (self.project["minMax"][2] - self.project["minMax"][0])
+                    - bounding_box[0]
+                    + 10
+                )
+            elif offset_direction == "top":
+                offset_y = (
+                    (self.project["minMax"][3] - self.project["minMax"][1])
+                    - bounding_box[1]
+                    + 10
+                )
+            elif offset_direction == "bottom":
+                offset_y = (
+                    0 - (bounding_box[3] - bounding_box[1]) - bounding_box[1] - 10
+                )
+
+            new_obj_idx = clone_object(object_active_obj_idx, offset_x, offset_y)
+            if new_obj_idx is not None and with_childs:
                 for inner in object_active_obj["inner_objects"]:
-                    clone_object(inner)
+                    clone_object(inner, offset_x, offset_y)
 
             self.combobjwidget.clear()
             for idx in self.project["objects"]:
                 self.combobjwidget.addItem(idx.split(":")[0])
 
             self.project["maxOuter"] = find_tool_offsets(self.project["objects"])
 
@@ -2514,18 +2588,33 @@
         vlayout.addWidget(checkbox)
 
         gcontainer = QWidget()
         glayout = QGridLayout()
         gcontainer.setLayout(glayout)
         vlayout.addWidget(gcontainer)
 
-        button = QPushButton("Clone")
+        button = QPushButton("Clone Top")
         button.setToolTip(_("clone object"))
-        button.clicked.connect(partial(object_copy, checkbox))  # type: ignore
-        glayout.addWidget(button, 0, 0)
+        button.clicked.connect(partial(object_copy, checkbox, "top"))  # type: ignore
+        glayout.addWidget(button, 0, 1)
+
+        button = QPushButton("Clone Left")
+        button.setToolTip(_("clone object"))
+        button.clicked.connect(partial(object_copy, checkbox, "left"))  # type: ignore
+        glayout.addWidget(button, 1, 0)
+
+        button = QPushButton("Clone Right")
+        button.setToolTip(_("clone object"))
+        button.clicked.connect(partial(object_copy, checkbox, "right"))  # type: ignore
+        glayout.addWidget(button, 1, 2)
+
+        button = QPushButton("Clone Bottom")
+        button.setToolTip(_("clone object"))
+        button.clicked.connect(partial(object_copy, checkbox, "bottom"))  # type: ignore
+        glayout.addWidget(button, 2, 1)
 
         vlayout.addStretch(1)
         tabwidget.addTab(vcontainer, _("Manipulate"))
 
     def update_tabs_data(self) -> None:
         self.project["tabs"]["data"] = []
         for obj in self.project["objects"].values():
@@ -2581,15 +2670,15 @@
         debug("prepare_segments: update_tabs_data")
         self.update_tabs_data()
         if not self.args.laser:
             debug("prepare_segments: find_tool_offsets")
             self.project["maxOuter"] = find_tool_offsets(self.project["objects"])
         debug("prepare_segments: done")
 
-    def load_drawing(self, filename: str) -> bool:
+    def load_drawing(self, filename: str, no_setup: bool = False) -> bool:
         # clean project
         debug("load_drawing: cleanup")
         self.project["filename_draw"] = ""
         self.project["filename_machine_cmd"] = ""
         self.project["suffix"] = "ngc"
         self.project["axis"] = ["X", "Y", "Z"]
         self.project["machine_cmd"] = ""
@@ -2643,15 +2732,19 @@
             dialog.setLayout(dialog.layout)  # type: ignore
 
             if dialog.exec():
                 plugin_name = combobox.currentText()
                 reader_plugin = reader_plugins[plugin_name]
 
         reader_plugin = reader_plugins[plugin_name]
-        if self.main is not None and hasattr(reader_plugin, "preload_setup"):
+        if (
+            not no_setup
+            and self.main is not None
+            and hasattr(reader_plugin, "preload_setup")
+        ):
             reader_plugin.preload_setup(filename, self.args)
         self.project["draw_reader"] = reader_plugin(filename, self.args)
         if reader_plugin.can_save_tabs:
             self.save_tabs = "ask"
 
         if self.project["draw_reader"]:
             debug("load_drawing: get segments")
@@ -2999,19 +3092,23 @@
         self.combobjwidget.setToolTip("Global/Object settings")
         self.combobjwidget.currentTextChanged.connect(self.setup_select_object)  # type: ignore
 
         object_vbox.addWidget(QLabel(_("Object:")))
         object_vbox.addWidget(self.combobjwidget, stretch=0)
         object_vbox.addWidget(self.tabobjwidget, stretch=1)
 
+        self.infotext_widget = QPlainTextEdit()
+        self.infotext_widget.setPlainText("info:")
+
         ltabwidget = QTabWidget()
         ltabwidget.addTab(self.tabwidget, _("&Global"))
         ltabwidget.addTab(self.objwidget, _("&Objects"))
-
         ltabwidget.addTab(self.project["layerwidget"], _("&Layers"))
+        ltabwidget.addTab(self.infotext_widget, _("&Infos"))
+
         left_gridlayout.addWidget(ltabwidget)
 
         if self.combobjwidget is not None:
             self.combobjwidget.clear()
             for idx in self.project["objects"]:
                 self.combobjwidget.addItem(idx.split(":")[0])
             self.project["object_active"] = "0"
@@ -3027,14 +3124,18 @@
         right_widget = QWidget()
         right_widget.setLayout(right_gridlayout)
 
         hlay = QHBoxLayout(self.project["window"])
         hlay.addWidget(left_widget, stretch=1)
         hlay.addWidget(right_widget, stretch=3)
 
+        # Tools
+        self.font_tool = FontTool(self)
+        self.gear_tool = GearTool(self)
+
         self.main.resize(1600, 1200)
         self.main.show()
         debug("main: gui ready")
 
         if self.project["engine"] == "2D":
             if self.project["status"] == "INIT":
                 self.project["status"] = "READY"
```

### Comparing `viaconstructor-0.6.1/viaconstructor.egg-info/PKG-INFO` & `viaconstructor-0.6.3/viaconstructor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viaconstructor
-Version: 0.6.1
+Version: 0.6.3
 Summary: python based cam-tool to convert dxf into gcode
 Home-page: https://github.com/multigcs/viaconstructor
 Author: Oliver Dippel
 Author-email: o.dippel@gmx.de
 License: LICENSE
 License-File: LICENSE
 
@@ -69,16 +69,17 @@
 ### thumbnail generator: dxf to jpg
 ```
 ./bin/dxfpreview tests/data/simple.dxf -o tests/data/simple.jpg
 ```
 
 ### running on macos/osx
 ```
-git clone https://github.com/multigcs/viaconstructor.git
 brew install python@3.10
+git clone https://github.com/multigcs/viaconstructor.git
+cd viaconstructor
 /usr/local/bin/python3 -m pip install -r requirements-install.txt
 /usr/local/bin/python3 -m viaconstructor tests/data/simple.dxf
 ```
 
 ### running on Windows10
 you can simply extract this zip file to you disk and execute the start.bat:
```

### Comparing `viaconstructor-0.6.1/viaconstructor.egg-info/SOURCES.txt` & `viaconstructor-0.6.3/viaconstructor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 viaconstructor/ext/svgpathtools/svg_io_sax.py
 viaconstructor/ext/svgpathtools/svg_to_paths.py
 viaconstructor/icons/camotics.png
 viaconstructor/icons/delete.png
 viaconstructor/icons/exit.png
 viaconstructor/icons/flip-x.png
 viaconstructor/icons/flip-y.png
+viaconstructor/icons/fonts.png
+viaconstructor/icons/gears.png
 viaconstructor/icons/load-setup-gcode.png
 viaconstructor/icons/load-setup.png
 viaconstructor/icons/load-tooltable.png
 viaconstructor/icons/nesting.png
 viaconstructor/icons/open.png
 viaconstructor/icons/openscad.png
 viaconstructor/icons/pause.png
```

