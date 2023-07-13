# Comparing `tmp/eelbrain-0.9.1.tar.gz` & `tmp/eelbrain-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eelbrain-0.9.1.tar", last modified: Thu Oct  2 17:00:41 2014, max compression
+gzip compressed data, was "dist/eelbrain-0.9.2.tar", last modified: Fri Oct  3 18:30:53 2014, max compression
```

## Comparing `eelbrain-0.9.1.tar` & `eelbrain-0.9.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/
--rw-r--r--   0 christian   (506) staff       (20)      969 2014-10-02 16:59:36.000000 eelbrain-0.9.1/eelbrain/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     7993 2014-09-30 16:49:59.000000 eelbrain-0.9.1/eelbrain/_colorspaces.py
--rw-r--r--   0 christian   (506) staff       (20)   222858 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/_data_obj.py
--rw-r--r--   0 christian   (506) staff       (20)    15697 2014-09-21 19:24:45.000000 eelbrain-0.9.1/eelbrain/_mne.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_stats/
--rw-r--r--   0 christian   (506) staff       (20)        0 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)    32219 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/glm.py
--rw-r--r--   0 christian   (506) staff       (20)  1844256 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/_stats/opt.c
--rw-r--r--   0 christian   (506) staff       (20)     4781 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_stats/permutation.py
--rw-r--r--   0 christian   (506) staff       (20)     7745 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/stats.py
--rw-r--r--   0 christian   (506) staff       (20)    26975 2014-09-10 02:47:51.000000 eelbrain-0.9.1/eelbrain/_stats/test.py
--rw-r--r--   0 christian   (506) staff       (20)   104183 2014-10-01 13:44:46.000000 eelbrain-0.9.1/eelbrain/_stats/testnd.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_stats/tests/
--rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_stats/tests/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     6744 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/tests/test_glm.py
--rw-r--r--   0 christian   (506) staff       (20)     1269 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_stats/tests/test_permutation.py
--rw-r--r--   0 christian   (506) staff       (20)     2809 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/tests/test_stats.py
--rw-r--r--   0 christian   (506) staff       (20)      631 2014-09-10 02:47:51.000000 eelbrain-0.9.1/eelbrain/_stats/tests/test_test.py
--rw-r--r--   0 christian   (506) staff       (20)    15968 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_stats/tests/test_testnd.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_utils/
--rw-r--r--   0 christian   (506) staff       (20)      143 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     7343 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/basic.py
--rw-r--r--   0 christian   (506) staff       (20)     3510 2014-07-24 17:35:52.000000 eelbrain-0.9.1/eelbrain/_utils/com.py
--rw-r--r--   0 christian   (506) staff       (20)     2020 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/kit.py
--rw-r--r--   0 christian   (506) staff       (20)     2166 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_utils/mne_utils.py
--rw-r--r--   0 christian   (506) staff       (20)     4714 2014-08-19 22:23:47.000000 eelbrain-0.9.1/eelbrain/_utils/nibabel_fs_io.py
--rw-r--r--   0 christian   (506) staff       (20)     3172 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/print_funcs.py
--rw-r--r--   0 christian   (506) staff       (20)    22888 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_utils/subp.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_utils/ui/
--rw-r--r--   0 christian   (506) staff       (20)     4943 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/ui/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     3116 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/ui/terminal_ui.py
--rw-r--r--   0 christian   (506) staff       (20)     2543 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/ui/tk_ui.py
--rw-r--r--   0 christian   (506) staff       (20)     6606 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_utils/ui/wx_ui.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_wxgui/
--rw-r--r--   0 christian   (506) staff       (20)       58 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_wxgui/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     1243 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_wxgui/about.py
--rw-r--r--   0 christian   (506) staff       (20)    11046 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/_wxgui/app.py
--rw-r--r--   0 christian   (506) staff       (20)     1046 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_wxgui/frame.py
--rw-r--r--   0 christian   (506) staff       (20)     3405 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxgui/history.py
--rw-r--r--   0 christian   (506) staff       (20)     8005 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/_wxgui/mpl_canvas.py
--rw-r--r--   0 christian   (506) staff       (20)    44663 2014-10-02 16:57:30.000000 eelbrain-0.9.1/eelbrain/_wxgui/select_epochs.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_wxterm/
--rw-r--r--   0 christian   (506) staff       (20)      531 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     2948 2014-08-21 01:56:15.000000 eelbrain-0.9.1/eelbrain/_wxterm/about_dialog.py
--rw-r--r--   0 christian   (506) staff       (20)     2088 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/app.py
--rw-r--r--   0 christian   (506) staff       (20)    13644 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/help.py
--rw-r--r--   0 christian   (506) staff       (20)     5132 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/mpl_tools.py
--rw-r--r--   0 christian   (506) staff       (20)     5424 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/preferences_dialog.py
--rw-r--r--   0 christian   (506) staff       (20)    21242 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/py_editor.py
--rw-r--r--   0 christian   (506) staff       (20)    64223 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/_wxterm/shell.py
--rw-r--r--   0 christian   (506) staff       (20)    15196 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxterm/table.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain/_wxutils/
--rw-r--r--   0 christian   (506) staff       (20)       31 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxutils/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     2887 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxutils/basic.py
--rw-r--r--   0 christian   (506) staff       (20)     4479 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxutils/draw.py
--rw-r--r--   0 christian   (506) staff       (20)     3428 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxutils/droptarget.py
--rw-r--r--   0 christian   (506) staff       (20)   121167 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/_wxutils/icons.py
--rw-r--r--   0 christian   (506) staff       (20)     1947 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/_wxutils/ID.py
--rw-r--r--   0 christian   (506) staff       (20)     8547 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/datasets.py
--rw-r--r--   0 christian   (506) staff       (20)    15442 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/design.py
--rw-r--r--   0 christian   (506) staff       (20)      164 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/eellab.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/experiment/
--rw-r--r--   0 christian   (506) staff       (20)      178 2013-10-10 21:12:19.000000 eelbrain-0.9.1/eelbrain/experiment/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)    41441 2014-08-18 03:32:53.000000 eelbrain-0.9.1/eelbrain/experiment/experiment.py
--rw-r--r--   0 christian   (506) staff       (20)   136888 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/experiment/mne_experiment.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/experiment/test/
--rw-r--r--   0 christian   (506) staff       (20)        0 2013-10-10 21:12:19.000000 eelbrain-0.9.1/eelbrain/experiment/test/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     1295 2014-08-14 20:42:09.000000 eelbrain-0.9.1/eelbrain/experiment/test/test_experiment.py
--rw-r--r--   0 christian   (506) staff       (20)    56536 2014-09-05 16:38:43.000000 eelbrain-0.9.1/eelbrain/fmtxt.py
--rw-r--r--   0 christian   (506) staff       (20)     3353 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/gui.py
--rw-r--r--   0 christian   (506) staff       (20)      161 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/lab.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/load/
--rw-r--r--   0 christian   (506) staff       (20)      445 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/load/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     2205 2014-07-24 17:35:52.000000 eelbrain-0.9.1/eelbrain/load/_pickle.py
--rw-r--r--   0 christian   (506) staff       (20)    10680 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/load/besa.py
--rw-r--r--   0 christian   (506) staff       (20)    21891 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/load/eyelink.py
--rw-r--r--   0 christian   (506) staff       (20)    28509 2014-08-14 20:42:09.000000 eelbrain-0.9.1/eelbrain/load/fiff.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/load/tests/
--rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/load/tests/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     1905 2014-08-14 20:42:09.000000 eelbrain-0.9.1/eelbrain/load/tests/test_fiff.py
--rw-r--r--   0 christian   (506) staff       (20)      843 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/load/tests/test_txt.py
--rw-r--r--   0 christian   (506) staff       (20)     5586 2014-07-18 15:16:38.000000 eelbrain-0.9.1/eelbrain/load/txt.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/mne_fixes/
--rw-r--r--   0 christian   (506) staff       (20)       89 2014-08-14 21:03:10.000000 eelbrain-0.9.1/eelbrain/mne_fixes/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     9207 2014-08-14 21:03:10.000000 eelbrain-0.9.1/eelbrain/mne_fixes/_label.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/plot/
--rw-r--r--   0 christian   (506) staff       (20)     2256 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)    34650 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_base.py
--rw-r--r--   0 christian   (506) staff       (20)      669 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/_nuts.py
--rw-r--r--   0 christian   (506) staff       (20)    21889 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_sensors.py
--rw-r--r--   0 christian   (506) staff       (20)    28880 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_topo.py
--rw-r--r--   0 christian   (506) staff       (20)    25448 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_uts.py
--rw-r--r--   0 christian   (506) staff       (20)    20991 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_utsnd.py
--rw-r--r--   0 christian   (506) staff       (20)    52227 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/_uv.py
--rw-r--r--   0 christian   (506) staff       (20)    25471 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/brain.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/plot/tests/
--rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/plot/tests/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     1183 2014-10-02 16:55:30.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_base.py
--rw-r--r--   0 christian   (506) staff       (20)     1004 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_sensors.py
--rw-r--r--   0 christian   (506) staff       (20)     1247 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_topo.py
--rw-r--r--   0 christian   (506) staff       (20)     2403 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_uts.py
--rw-r--r--   0 christian   (506) staff       (20)     1750 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_utsnd.py
--rw-r--r--   0 christian   (506) staff       (20)     1757 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/plot/tests/test_uv.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/save/
--rw-r--r--   0 christian   (506) staff       (20)      180 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/save/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)     3121 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/save/_besa.py
--rw-r--r--   0 christian   (506) staff       (20)      999 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/save/_pickle.py
--rw-r--r--   0 christian   (506) staff       (20)      888 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/save/_txt.py
--rw-r--r--   0 christian   (506) staff       (20)     9297 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/table.py
--rw-r--r--   0 christian   (506) staff       (20)      341 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/test.py
--rw-r--r--   0 christian   (506) staff       (20)     2119 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/testnd.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/eelbrain/tests/
--rw-r--r--   0 christian   (506) staff       (20)        0 2013-10-15 16:41:11.000000 eelbrain-0.9.1/eelbrain/tests/__init__.py
--rw-r--r--   0 christian   (506) staff       (20)    25271 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/tests/test_data.py
--rw-r--r--   0 christian   (506) staff       (20)     1914 2014-07-17 20:55:11.000000 eelbrain-0.9.1/eelbrain/tests/test_design.py
--rw-r--r--   0 christian   (506) staff       (20)    16375 2014-08-21 03:09:42.000000 eelbrain-0.9.1/eelbrain/tests/test_examples.py
--rw-r--r--   0 christian   (506) staff       (20)     1131 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/tests/test_fmtxt.py
--rw-r--r--   0 christian   (506) staff       (20)     5195 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/tests/test_mne.py
--rw-r--r--   0 christian   (506) staff       (20)     1209 2014-09-26 01:05:22.000000 eelbrain-0.9.1/eelbrain/tests/test_table.py
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/
--rw-r--r--   0 christian   (506) staff       (20)        1 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (506) staff       (20)      318 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/PKG-INFO
--rw-r--r--   0 christian   (506) staff       (20)      130 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/requires.txt
--rw-r--r--   0 christian   (506) staff       (20)     3053 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (506) staff       (20)        9 2014-10-02 17:00:40.000000 eelbrain-0.9.1/eelbrain.egg-info/top_level.txt
--rw-r--r--   0 christian   (506) staff       (20)    10474 2014-07-03 14:14:33.000000 eelbrain-0.9.1/ez_setup.py
--rw-r--r--   0 christian   (506) staff       (20)       20 2014-02-06 22:44:54.000000 eelbrain-0.9.1/MANIFEST.in
--rw-r--r--   0 christian   (506) staff       (20)      318 2014-10-02 17:00:41.000000 eelbrain-0.9.1/PKG-INFO
--rw-r--r--   0 christian   (506) staff       (20)       68 2014-06-09 18:58:10.000000 eelbrain-0.9.1/README.txt
-drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-02 17:00:41.000000 eelbrain-0.9.1/scripts/
--rwxr-xr-x   0 christian   (506) staff       (20)       73 2014-07-17 20:55:11.000000 eelbrain-0.9.1/scripts/eelbrain
--rw-r--r--   0 christian   (506) staff       (20)      192 2014-10-02 17:00:41.000000 eelbrain-0.9.1/setup.cfg
--rw-r--r--   0 christian   (506) staff       (20)     6678 2014-09-26 01:05:22.000000 eelbrain-0.9.1/setup.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/
+-rw-r--r--   0 christian   (506) staff       (20)      969 2014-10-03 18:29:49.000000 eelbrain-0.9.2/eelbrain/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     7993 2014-09-30 16:49:59.000000 eelbrain-0.9.2/eelbrain/_colorspaces.py
+-rw-r--r--   0 christian   (506) staff       (20)   222858 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/_data_obj.py
+-rw-r--r--   0 christian   (506) staff       (20)    15697 2014-09-21 19:24:45.000000 eelbrain-0.9.2/eelbrain/_mne.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_stats/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)    32219 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/glm.py
+-rw-r--r--   0 christian   (506) staff       (20)  1844256 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/_stats/opt.c
+-rw-r--r--   0 christian   (506) staff       (20)     4781 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_stats/permutation.py
+-rw-r--r--   0 christian   (506) staff       (20)     7745 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/stats.py
+-rw-r--r--   0 christian   (506) staff       (20)    26975 2014-09-10 02:47:51.000000 eelbrain-0.9.2/eelbrain/_stats/test.py
+-rw-r--r--   0 christian   (506) staff       (20)   104183 2014-10-01 13:44:46.000000 eelbrain-0.9.2/eelbrain/_stats/testnd.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_stats/tests/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_stats/tests/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     6744 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/tests/test_glm.py
+-rw-r--r--   0 christian   (506) staff       (20)     1269 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_stats/tests/test_permutation.py
+-rw-r--r--   0 christian   (506) staff       (20)     2809 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/tests/test_stats.py
+-rw-r--r--   0 christian   (506) staff       (20)      631 2014-09-10 02:47:51.000000 eelbrain-0.9.2/eelbrain/_stats/tests/test_test.py
+-rw-r--r--   0 christian   (506) staff       (20)    15968 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_stats/tests/test_testnd.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_utils/
+-rw-r--r--   0 christian   (506) staff       (20)      143 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     7343 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/basic.py
+-rw-r--r--   0 christian   (506) staff       (20)     3510 2014-07-24 17:35:52.000000 eelbrain-0.9.2/eelbrain/_utils/com.py
+-rw-r--r--   0 christian   (506) staff       (20)     2020 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/kit.py
+-rw-r--r--   0 christian   (506) staff       (20)     2166 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_utils/mne_utils.py
+-rw-r--r--   0 christian   (506) staff       (20)     4714 2014-08-19 22:23:47.000000 eelbrain-0.9.2/eelbrain/_utils/nibabel_fs_io.py
+-rw-r--r--   0 christian   (506) staff       (20)     3172 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/print_funcs.py
+-rw-r--r--   0 christian   (506) staff       (20)    22888 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_utils/subp.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_utils/ui/
+-rw-r--r--   0 christian   (506) staff       (20)     4943 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/ui/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     3116 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/ui/terminal_ui.py
+-rw-r--r--   0 christian   (506) staff       (20)     2543 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/ui/tk_ui.py
+-rw-r--r--   0 christian   (506) staff       (20)     6606 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_utils/ui/wx_ui.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_wxgui/
+-rw-r--r--   0 christian   (506) staff       (20)       58 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_wxgui/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     1243 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_wxgui/about.py
+-rw-r--r--   0 christian   (506) staff       (20)    11046 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/_wxgui/app.py
+-rw-r--r--   0 christian   (506) staff       (20)     1046 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_wxgui/frame.py
+-rw-r--r--   0 christian   (506) staff       (20)     3405 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxgui/history.py
+-rw-r--r--   0 christian   (506) staff       (20)     8005 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/_wxgui/mpl_canvas.py
+-rw-r--r--   0 christian   (506) staff       (20)    44663 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/_wxgui/select_epochs.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_wxterm/
+-rw-r--r--   0 christian   (506) staff       (20)      531 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     2948 2014-08-21 01:56:15.000000 eelbrain-0.9.2/eelbrain/_wxterm/about_dialog.py
+-rw-r--r--   0 christian   (506) staff       (20)     2088 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/app.py
+-rw-r--r--   0 christian   (506) staff       (20)    13644 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/help.py
+-rw-r--r--   0 christian   (506) staff       (20)     5132 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/mpl_tools.py
+-rw-r--r--   0 christian   (506) staff       (20)     5424 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/preferences_dialog.py
+-rw-r--r--   0 christian   (506) staff       (20)    21242 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/py_editor.py
+-rw-r--r--   0 christian   (506) staff       (20)    64223 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/_wxterm/shell.py
+-rw-r--r--   0 christian   (506) staff       (20)    15196 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxterm/table.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/_wxutils/
+-rw-r--r--   0 christian   (506) staff       (20)       31 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxutils/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     2887 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxutils/basic.py
+-rw-r--r--   0 christian   (506) staff       (20)     4479 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxutils/draw.py
+-rw-r--r--   0 christian   (506) staff       (20)     3428 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxutils/droptarget.py
+-rw-r--r--   0 christian   (506) staff       (20)   121167 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/_wxutils/icons.py
+-rw-r--r--   0 christian   (506) staff       (20)     1947 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/_wxutils/ID.py
+-rw-r--r--   0 christian   (506) staff       (20)     8547 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/datasets.py
+-rw-r--r--   0 christian   (506) staff       (20)    15442 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/design.py
+-rw-r--r--   0 christian   (506) staff       (20)      164 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/eellab.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/experiment/
+-rw-r--r--   0 christian   (506) staff       (20)      178 2013-10-10 21:12:19.000000 eelbrain-0.9.2/eelbrain/experiment/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)    41441 2014-08-18 03:32:53.000000 eelbrain-0.9.2/eelbrain/experiment/experiment.py
+-rw-r--r--   0 christian   (506) staff       (20)   136905 2014-10-03 18:29:30.000000 eelbrain-0.9.2/eelbrain/experiment/mne_experiment.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/experiment/test/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2013-10-10 21:12:19.000000 eelbrain-0.9.2/eelbrain/experiment/test/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     1295 2014-08-14 20:42:09.000000 eelbrain-0.9.2/eelbrain/experiment/test/test_experiment.py
+-rw-r--r--   0 christian   (506) staff       (20)    56536 2014-09-05 16:38:43.000000 eelbrain-0.9.2/eelbrain/fmtxt.py
+-rw-r--r--   0 christian   (506) staff       (20)     3353 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/gui.py
+-rw-r--r--   0 christian   (506) staff       (20)      161 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/lab.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/load/
+-rw-r--r--   0 christian   (506) staff       (20)      445 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/load/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     2205 2014-07-24 17:35:52.000000 eelbrain-0.9.2/eelbrain/load/_pickle.py
+-rw-r--r--   0 christian   (506) staff       (20)    10680 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/load/besa.py
+-rw-r--r--   0 christian   (506) staff       (20)    21891 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/load/eyelink.py
+-rw-r--r--   0 christian   (506) staff       (20)    28509 2014-08-14 20:42:09.000000 eelbrain-0.9.2/eelbrain/load/fiff.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/load/tests/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/load/tests/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     1905 2014-08-14 20:42:09.000000 eelbrain-0.9.2/eelbrain/load/tests/test_fiff.py
+-rw-r--r--   0 christian   (506) staff       (20)      843 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/load/tests/test_txt.py
+-rw-r--r--   0 christian   (506) staff       (20)     5586 2014-07-18 15:16:38.000000 eelbrain-0.9.2/eelbrain/load/txt.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/mne_fixes/
+-rw-r--r--   0 christian   (506) staff       (20)       89 2014-08-14 21:03:10.000000 eelbrain-0.9.2/eelbrain/mne_fixes/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     9207 2014-08-14 21:03:10.000000 eelbrain-0.9.2/eelbrain/mne_fixes/_label.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/plot/
+-rw-r--r--   0 christian   (506) staff       (20)     2256 2014-10-03 18:29:12.000000 eelbrain-0.9.2/eelbrain/plot/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)    34650 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_base.py
+-rw-r--r--   0 christian   (506) staff       (20)      669 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/_nuts.py
+-rw-r--r--   0 christian   (506) staff       (20)    21889 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_sensors.py
+-rw-r--r--   0 christian   (506) staff       (20)    28880 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_topo.py
+-rw-r--r--   0 christian   (506) staff       (20)    25448 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_uts.py
+-rw-r--r--   0 christian   (506) staff       (20)    20991 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_utsnd.py
+-rw-r--r--   0 christian   (506) staff       (20)    52227 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/_uv.py
+-rw-r--r--   0 christian   (506) staff       (20)    25471 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/brain.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/plot/tests/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/plot/tests/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     1183 2014-10-03 18:29:13.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_base.py
+-rw-r--r--   0 christian   (506) staff       (20)     1004 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_sensors.py
+-rw-r--r--   0 christian   (506) staff       (20)     1247 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_topo.py
+-rw-r--r--   0 christian   (506) staff       (20)     2403 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_uts.py
+-rw-r--r--   0 christian   (506) staff       (20)     1750 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_utsnd.py
+-rw-r--r--   0 christian   (506) staff       (20)     1757 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/plot/tests/test_uv.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/save/
+-rw-r--r--   0 christian   (506) staff       (20)      180 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/save/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)     3121 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/save/_besa.py
+-rw-r--r--   0 christian   (506) staff       (20)      999 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/save/_pickle.py
+-rw-r--r--   0 christian   (506) staff       (20)      888 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/save/_txt.py
+-rw-r--r--   0 christian   (506) staff       (20)     9297 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/table.py
+-rw-r--r--   0 christian   (506) staff       (20)      341 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/test.py
+-rw-r--r--   0 christian   (506) staff       (20)     2119 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/testnd.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain/tests/
+-rw-r--r--   0 christian   (506) staff       (20)        0 2013-10-15 16:41:11.000000 eelbrain-0.9.2/eelbrain/tests/__init__.py
+-rw-r--r--   0 christian   (506) staff       (20)    25271 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/tests/test_data.py
+-rw-r--r--   0 christian   (506) staff       (20)     1914 2014-07-17 20:55:11.000000 eelbrain-0.9.2/eelbrain/tests/test_design.py
+-rw-r--r--   0 christian   (506) staff       (20)    16375 2014-08-21 03:09:42.000000 eelbrain-0.9.2/eelbrain/tests/test_examples.py
+-rw-r--r--   0 christian   (506) staff       (20)     1131 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/tests/test_fmtxt.py
+-rw-r--r--   0 christian   (506) staff       (20)     5195 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/tests/test_mne.py
+-rw-r--r--   0 christian   (506) staff       (20)     1209 2014-09-26 01:05:22.000000 eelbrain-0.9.2/eelbrain/tests/test_table.py
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain.egg-info/
+-rw-r--r--   0 christian   (506) staff       (20)        1 2014-10-03 18:30:52.000000 eelbrain-0.9.2/eelbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (506) staff       (20)      318 2014-10-03 18:30:52.000000 eelbrain-0.9.2/eelbrain.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (506) staff       (20)      130 2014-10-03 18:30:52.000000 eelbrain-0.9.2/eelbrain.egg-info/requires.txt
+-rw-r--r--   0 christian   (506) staff       (20)     3053 2014-10-03 18:30:53.000000 eelbrain-0.9.2/eelbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (506) staff       (20)        9 2014-10-03 18:30:52.000000 eelbrain-0.9.2/eelbrain.egg-info/top_level.txt
+-rw-r--r--   0 christian   (506) staff       (20)    10474 2014-07-03 14:14:33.000000 eelbrain-0.9.2/ez_setup.py
+-rw-r--r--   0 christian   (506) staff       (20)       20 2014-02-06 22:44:54.000000 eelbrain-0.9.2/MANIFEST.in
+-rw-r--r--   0 christian   (506) staff       (20)      318 2014-10-03 18:30:53.000000 eelbrain-0.9.2/PKG-INFO
+-rw-r--r--   0 christian   (506) staff       (20)       68 2014-06-09 18:58:10.000000 eelbrain-0.9.2/README.txt
+drwxr-xr-x   0 christian   (506) staff       (20)        0 2014-10-03 18:30:53.000000 eelbrain-0.9.2/scripts/
+-rwxr-xr-x   0 christian   (506) staff       (20)       73 2014-07-17 20:55:11.000000 eelbrain-0.9.2/scripts/eelbrain
+-rw-r--r--   0 christian   (506) staff       (20)      192 2014-10-03 18:30:53.000000 eelbrain-0.9.2/setup.cfg
+-rw-r--r--   0 christian   (506) staff       (20)     6678 2014-09-26 01:05:22.000000 eelbrain-0.9.2/setup.py
```

### Comparing `eelbrain-0.9.1/eelbrain/__init__.py` & `eelbrain-0.9.2/eelbrain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 from . import table
 from . import test
 from . import testnd
 
 from .fmtxt import Report
 
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
```

### Comparing `eelbrain-0.9.1/eelbrain/_colorspaces.py` & `eelbrain-0.9.2/eelbrain/_colorspaces.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_data_obj.py` & `eelbrain-0.9.2/eelbrain/_data_obj.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_mne.py` & `eelbrain-0.9.2/eelbrain/_mne.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/glm.py` & `eelbrain-0.9.2/eelbrain/_stats/glm.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/opt.c` & `eelbrain-0.9.2/eelbrain/_stats/opt.c`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/permutation.py` & `eelbrain-0.9.2/eelbrain/_stats/permutation.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/stats.py` & `eelbrain-0.9.2/eelbrain/_stats/stats.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/test.py` & `eelbrain-0.9.2/eelbrain/_stats/test.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/testnd.py` & `eelbrain-0.9.2/eelbrain/_stats/testnd.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/tests/test_glm.py` & `eelbrain-0.9.2/eelbrain/_stats/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/tests/test_permutation.py` & `eelbrain-0.9.2/eelbrain/_stats/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/tests/test_stats.py` & `eelbrain-0.9.2/eelbrain/_stats/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/tests/test_test.py` & `eelbrain-0.9.2/eelbrain/_stats/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_stats/tests/test_testnd.py` & `eelbrain-0.9.2/eelbrain/_stats/tests/test_testnd.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/basic.py` & `eelbrain-0.9.2/eelbrain/_utils/basic.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/com.py` & `eelbrain-0.9.2/eelbrain/_utils/com.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/kit.py` & `eelbrain-0.9.2/eelbrain/_utils/kit.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/mne_utils.py` & `eelbrain-0.9.2/eelbrain/_utils/mne_utils.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/nibabel_fs_io.py` & `eelbrain-0.9.2/eelbrain/_utils/nibabel_fs_io.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/print_funcs.py` & `eelbrain-0.9.2/eelbrain/_utils/print_funcs.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/subp.py` & `eelbrain-0.9.2/eelbrain/_utils/subp.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/ui/__init__.py` & `eelbrain-0.9.2/eelbrain/_utils/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/ui/terminal_ui.py` & `eelbrain-0.9.2/eelbrain/_utils/ui/terminal_ui.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/ui/tk_ui.py` & `eelbrain-0.9.2/eelbrain/_utils/ui/tk_ui.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_utils/ui/wx_ui.py` & `eelbrain-0.9.2/eelbrain/_utils/ui/wx_ui.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/about.py` & `eelbrain-0.9.2/eelbrain/_wxgui/about.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/app.py` & `eelbrain-0.9.2/eelbrain/_wxgui/app.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/frame.py` & `eelbrain-0.9.2/eelbrain/_wxgui/frame.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/history.py` & `eelbrain-0.9.2/eelbrain/_wxgui/history.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/mpl_canvas.py` & `eelbrain-0.9.2/eelbrain/_wxgui/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxgui/select_epochs.py` & `eelbrain-0.9.2/eelbrain/_wxgui/select_epochs.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/__init__.py` & `eelbrain-0.9.2/eelbrain/_wxterm/__init__.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/about_dialog.py` & `eelbrain-0.9.2/eelbrain/_wxterm/about_dialog.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/app.py` & `eelbrain-0.9.2/eelbrain/_wxterm/app.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/help.py` & `eelbrain-0.9.2/eelbrain/_wxterm/help.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/mpl_tools.py` & `eelbrain-0.9.2/eelbrain/_wxterm/mpl_tools.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/preferences_dialog.py` & `eelbrain-0.9.2/eelbrain/_wxterm/preferences_dialog.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/py_editor.py` & `eelbrain-0.9.2/eelbrain/_wxterm/py_editor.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/shell.py` & `eelbrain-0.9.2/eelbrain/_wxterm/shell.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxterm/table.py` & `eelbrain-0.9.2/eelbrain/_wxterm/table.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxutils/basic.py` & `eelbrain-0.9.2/eelbrain/_wxutils/basic.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxutils/draw.py` & `eelbrain-0.9.2/eelbrain/_wxutils/draw.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxutils/droptarget.py` & `eelbrain-0.9.2/eelbrain/_wxutils/droptarget.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxutils/icons.py` & `eelbrain-0.9.2/eelbrain/_wxutils/icons.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/_wxutils/ID.py` & `eelbrain-0.9.2/eelbrain/_wxutils/ID.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/datasets.py` & `eelbrain-0.9.2/eelbrain/datasets.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/design.py` & `eelbrain-0.9.2/eelbrain/design.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/experiment/experiment.py` & `eelbrain-0.9.2/eelbrain/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/experiment/mne_experiment.py` & `eelbrain-0.9.2/eelbrain/experiment/mne_experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,17 +320,17 @@
     # "base": 'raw' for raw file, or epoch name
     # "rej": rejection setting to use (only applies for epoch projs)
     # r.g. {'ironcross': {'base': 'adj', 'rej': 'man'}}
     projs = {}
 
     # Pattern for subject names. The first group is used to determine what
     # MEG-system the data was recorded from
-    _subject_re = '(R|A|AD|QP)(\d{3,})$'
+    _subject_re = '(R|A|Y|AD|QP)(\d{3,})$'
     _meg_systems = {'R': 'KIT-NY',
-                    'A': 'KIT-AD', 'AD': 'KIT-AD', 'QP': 'KIT-AD'}
+                    'A': 'KIT-AD', 'Y': 'KIT-AD', 'AD': 'KIT-AD', 'QP': 'KIT-AD'}
 
     # state variables that are always shown in self.__repr__():
     _repr_kwargs = ('subject', 'rej')
 
     # Where to search for subjects (defined as a template name). If the
     # experiment searches for subjects automatically, it scans this directory
     # for subfolders matching _subject_re.
```

### Comparing `eelbrain-0.9.1/eelbrain/experiment/test/test_experiment.py` & `eelbrain-0.9.2/eelbrain/experiment/test/test_experiment.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/fmtxt.py` & `eelbrain-0.9.2/eelbrain/fmtxt.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/gui.py` & `eelbrain-0.9.2/eelbrain/gui.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/_pickle.py` & `eelbrain-0.9.2/eelbrain/load/_pickle.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/besa.py` & `eelbrain-0.9.2/eelbrain/load/besa.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/eyelink.py` & `eelbrain-0.9.2/eelbrain/load/eyelink.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/fiff.py` & `eelbrain-0.9.2/eelbrain/load/fiff.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/tests/test_fiff.py` & `eelbrain-0.9.2/eelbrain/load/tests/test_fiff.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/tests/test_txt.py` & `eelbrain-0.9.2/eelbrain/load/tests/test_txt.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/load/txt.py` & `eelbrain-0.9.2/eelbrain/load/txt.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/mne_fixes/_label.py` & `eelbrain-0.9.2/eelbrain/mne_fixes/_label.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/__init__.py` & `eelbrain-0.9.2/eelbrain/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_base.py` & `eelbrain-0.9.2/eelbrain/plot/_base.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_nuts.py` & `eelbrain-0.9.2/eelbrain/plot/_nuts.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_sensors.py` & `eelbrain-0.9.2/eelbrain/plot/_sensors.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_topo.py` & `eelbrain-0.9.2/eelbrain/plot/_topo.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_uts.py` & `eelbrain-0.9.2/eelbrain/plot/_uts.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_utsnd.py` & `eelbrain-0.9.2/eelbrain/plot/_utsnd.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/_uv.py` & `eelbrain-0.9.2/eelbrain/plot/_uv.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/brain.py` & `eelbrain-0.9.2/eelbrain/plot/brain.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_base.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_sensors.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_topo.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_topo.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_uts.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_uts.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_utsnd.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_utsnd.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/plot/tests/test_uv.py` & `eelbrain-0.9.2/eelbrain/plot/tests/test_uv.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/save/_besa.py` & `eelbrain-0.9.2/eelbrain/save/_besa.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/save/_pickle.py` & `eelbrain-0.9.2/eelbrain/save/_pickle.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/save/_txt.py` & `eelbrain-0.9.2/eelbrain/save/_txt.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/table.py` & `eelbrain-0.9.2/eelbrain/table.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/testnd.py` & `eelbrain-0.9.2/eelbrain/testnd.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_data.py` & `eelbrain-0.9.2/eelbrain/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_design.py` & `eelbrain-0.9.2/eelbrain/tests/test_design.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_examples.py` & `eelbrain-0.9.2/eelbrain/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_fmtxt.py` & `eelbrain-0.9.2/eelbrain/tests/test_fmtxt.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_mne.py` & `eelbrain-0.9.2/eelbrain/tests/test_mne.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain/tests/test_table.py` & `eelbrain-0.9.2/eelbrain/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/eelbrain.egg-info/SOURCES.txt` & `eelbrain-0.9.2/eelbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/ez_setup.py` & `eelbrain-0.9.2/ez_setup.py`

 * *Files identical despite different names*

### Comparing `eelbrain-0.9.1/setup.py` & `eelbrain-0.9.2/setup.py`

 * *Files identical despite different names*

