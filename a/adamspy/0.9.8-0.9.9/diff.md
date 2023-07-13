# Comparing `tmp/adamspy-0.9.8.tar.gz` & `tmp/adamspy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adamspy-0.9.8.tar", last modified: Wed Mar  4 20:12:31 2020, max compression
+gzip compressed data, was "dist\adamspy-0.9.9.tar", last modified: Wed Mar  4 21:04:16 2020, max compression
```

## Comparing `adamspy-0.9.8.tar` & `adamspy-0.9.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/
--rw-rw-rw-   0        0        0     1091 2019-07-01 12:35:30.000000 adamspy-0.9.8/LICENSE
--rw-rw-rw-   0        0        0       60 2019-07-01 12:35:30.000000 adamspy-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0      649 2020-03-04 20:12:31.000000 adamspy-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      138 2019-07-01 12:35:30.000000 adamspy-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy/
--rw-rw-rw-   0        0        0      359 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/__init__.py
--rw-rw-rw-   0        0        0     4018 2019-11-20 17:58:13.000000 adamspy-0.9.8/adamspy/adamspy.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy/adripy/
--rw-rw-rw-   0        0        0      595 2019-09-18 13:31:31.000000 adamspy-0.9.8/adamspy/adripy/__init__.py
--rw-rw-rw-   0        0        0     5170 2019-09-19 13:09:00.000000 adamspy-0.9.8/adamspy/adripy/constants.py
--rw-rw-rw-   0        0        0     2396 2019-08-30 13:52:59.000000 adamspy-0.9.8/adamspy/adripy/database.py
--rw-rw-rw-   0        0        0    24824 2020-03-02 02:14:34.000000 adamspy-0.9.8/adamspy/adripy/drillsim.py
--rw-rw-rw-   0        0        0    20216 2019-08-30 13:52:59.000000 adamspy-0.9.8/adamspy/adripy/event.py
--rw-rw-rw-   0        0        0    17545 2019-12-18 16:52:22.000000 adamspy-0.9.8/adamspy/adripy/hole.py
--rw-rw-rw-   0        0        0    12396 2019-09-23 20:24:51.000000 adamspy-0.9.8/adamspy/adripy/solver_settings.py
--rw-rw-rw-   0        0        0    32559 2019-12-18 16:52:22.000000 adamspy-0.9.8/adamspy/adripy/string.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy/adripy/templates/
--rw-rw-rw-   0        0        0     1604 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template.cfg
--rw-rw-rw-   0        0        0     4693 2019-08-30 13:52:59.000000 adamspy-0.9.8/adamspy/adripy/templates/template.evt
--rw-rw-rw-   0        0        0     1994 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template.hol
--rw-rw-rw-   0        0        0     1767 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template.ssf
--rw-rw-rw-   0        0        0     1478 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template.sta
--rw-rw-rw-   0        0        0     3001 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template_1.str
--rw-rw-rw-   0        0        0      570 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template_2.str
--rw-rw-rw-   0        0        0      284 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template_3.str
--rwxrwxrwx   0        0        0      396 2019-07-01 12:35:30.000000 adamspy-0.9.8/adamspy/adripy/templates/template_build.cmd
--rw-rw-rw-   0        0        0    11489 2020-03-04 16:48:20.000000 adamspy-0.9.8/adamspy/adripy/tool.py
--rw-rw-rw-   0        0        0    58818 2020-03-04 20:11:59.000000 adamspy-0.9.8/adamspy/adripy/utilities.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy/postprocess/
--rw-rw-rw-   0        0        0     4487 2019-08-30 13:52:59.000000 adamspy-0.9.8/adamspy/postprocess/__init__.py
--rw-rw-rw-   0        0        0     4130 2020-02-28 16:03:02.000000 adamspy-0.9.8/adamspy/postprocess/animation.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy/postprocess/aview_scripts/
--rw-rw-rw-   0        0        0     2346 2020-03-03 17:48:09.000000 adamspy-0.9.8/adamspy/postprocess/aview_scripts/_get_lunar_results.py
--rw-rw-rw-   0        0        0     3020 2020-03-03 17:52:34.000000 adamspy-0.9.8/adamspy/postprocess/ppt.py
--rw-rw-rw-   0        0        0    15968 2020-02-25 15:26:52.000000 adamspy-0.9.8/adamspy/postprocess/xml.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/
--rw-rw-rw-   0        0        0      649 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1388 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-03-04 20:12:31.000000 adamspy-0.9.8/adamspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      811 2020-03-04 20:12:30.000000 adamspy-0.9.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-03-04 20:12:31.000000 adamspy-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      797 2020-03-03 18:26:12.000000 adamspy-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-03-04 20:12:31.000000 adamspy-0.9.8/test/
--rw-rw-rw-   0        0        0     3446 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_adamspy.py
--rw-rw-rw-   0        0        0    17264 2019-09-18 19:34:03.000000 adamspy-0.9.8/test/test_adripy_utilities.py
--rw-rw-rw-   0        0        0      713 2020-02-28 16:03:00.000000 adamspy-0.9.8/test/test_animation.py
--rw-rw-rw-   0        0        0     2855 2020-01-23 14:23:03.000000 adamspy-0.9.8/test/test_build.py
--rw-rw-rw-   0        0        0     1901 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_database.py
--rw-rw-rw-   0        0        0     6817 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_drill_event.py
--rw-rw-rw-   0        0        0     4267 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_drill_solver_settings.py
--rw-rw-rw-   0        0        0    37326 2019-09-19 15:35:35.000000 adamspy-0.9.8/test/test_drill_string.py
--rw-rw-rw-   0        0        0     5329 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_drill_tool.py
--rw-rw-rw-   0        0        0    28175 2019-09-24 18:28:52.000000 adamspy-0.9.8/test/test_drillsim.py
--rw-rw-rw-   0        0        0     6241 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_hole.py
--rw-rw-rw-   0        0        0     1303 2020-01-23 14:23:03.000000 adamspy-0.9.8/test/test_motor_curve_generator.py
--rw-rw-rw-   0        0        0     8293 2020-03-03 17:58:32.000000 adamspy-0.9.8/test/test_results.py
--rw-rw-rw-   0        0        0     6881 2019-08-30 13:52:59.000000 adamspy-0.9.8/test/test_tiem_orbit.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:16.000000 adamspy-0.9.9/
+-rw-rw-rw-   0        0        0     1091 2019-07-01 12:35:30.000000 adamspy-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0       60 2019-07-01 12:35:30.000000 adamspy-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      649 2020-03-04 21:04:16.000000 adamspy-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2019-07-01 12:35:30.000000 adamspy-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy/
+-rw-rw-rw-   0        0        0      359 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/__init__.py
+-rw-rw-rw-   0        0        0     4018 2019-11-20 17:58:13.000000 adamspy-0.9.9/adamspy/adamspy.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy/adripy/
+-rw-rw-rw-   0        0        0      595 2019-09-18 13:31:31.000000 adamspy-0.9.9/adamspy/adripy/__init__.py
+-rw-rw-rw-   0        0        0     5170 2019-09-19 13:09:00.000000 adamspy-0.9.9/adamspy/adripy/constants.py
+-rw-rw-rw-   0        0        0     2396 2019-08-30 13:52:59.000000 adamspy-0.9.9/adamspy/adripy/database.py
+-rw-rw-rw-   0        0        0    24824 2020-03-02 02:14:34.000000 adamspy-0.9.9/adamspy/adripy/drillsim.py
+-rw-rw-rw-   0        0        0    20216 2019-08-30 13:52:59.000000 adamspy-0.9.9/adamspy/adripy/event.py
+-rw-rw-rw-   0        0        0    17545 2019-12-18 16:52:22.000000 adamspy-0.9.9/adamspy/adripy/hole.py
+-rw-rw-rw-   0        0        0    12396 2019-09-23 20:24:51.000000 adamspy-0.9.9/adamspy/adripy/solver_settings.py
+-rw-rw-rw-   0        0        0    32559 2019-12-18 16:52:22.000000 adamspy-0.9.9/adamspy/adripy/string.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy/adripy/templates/
+-rw-rw-rw-   0        0        0     1604 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template.cfg
+-rw-rw-rw-   0        0        0     4693 2019-08-30 13:52:59.000000 adamspy-0.9.9/adamspy/adripy/templates/template.evt
+-rw-rw-rw-   0        0        0     1994 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template.hol
+-rw-rw-rw-   0        0        0     1767 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template.ssf
+-rw-rw-rw-   0        0        0     1478 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template.sta
+-rw-rw-rw-   0        0        0     3001 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template_1.str
+-rw-rw-rw-   0        0        0      570 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template_2.str
+-rw-rw-rw-   0        0        0      284 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template_3.str
+-rwxrwxrwx   0        0        0      396 2019-07-01 12:35:30.000000 adamspy-0.9.9/adamspy/adripy/templates/template_build.cmd
+-rw-rw-rw-   0        0        0    11489 2020-03-04 16:48:20.000000 adamspy-0.9.9/adamspy/adripy/tool.py
+-rw-rw-rw-   0        0        0    58816 2020-03-04 21:02:46.000000 adamspy-0.9.9/adamspy/adripy/utilities.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy/postprocess/
+-rw-rw-rw-   0        0        0     4487 2019-08-30 13:52:59.000000 adamspy-0.9.9/adamspy/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     4130 2020-02-28 16:03:02.000000 adamspy-0.9.9/adamspy/postprocess/animation.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy/postprocess/aview_scripts/
+-rw-rw-rw-   0        0        0     2346 2020-03-03 17:48:09.000000 adamspy-0.9.9/adamspy/postprocess/aview_scripts/_get_lunar_results.py
+-rw-rw-rw-   0        0        0     3020 2020-03-03 17:52:34.000000 adamspy-0.9.9/adamspy/postprocess/ppt.py
+-rw-rw-rw-   0        0        0    15968 2020-02-25 15:26:52.000000 adamspy-0.9.9/adamspy/postprocess/xml.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/
+-rw-rw-rw-   0        0        0      649 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1388 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2020-03-04 21:04:15.000000 adamspy-0.9.9/adamspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      811 2020-03-04 21:04:14.000000 adamspy-0.9.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2020-03-04 21:04:16.000000 adamspy-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      797 2020-03-03 18:26:12.000000 adamspy-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-03-04 21:04:16.000000 adamspy-0.9.9/test/
+-rw-rw-rw-   0        0        0     3446 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_adamspy.py
+-rw-rw-rw-   0        0        0    17264 2019-09-18 19:34:03.000000 adamspy-0.9.9/test/test_adripy_utilities.py
+-rw-rw-rw-   0        0        0      713 2020-02-28 16:03:00.000000 adamspy-0.9.9/test/test_animation.py
+-rw-rw-rw-   0        0        0     2855 2020-01-23 14:23:03.000000 adamspy-0.9.9/test/test_build.py
+-rw-rw-rw-   0        0        0     1901 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_database.py
+-rw-rw-rw-   0        0        0     6817 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_drill_event.py
+-rw-rw-rw-   0        0        0     4267 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_drill_solver_settings.py
+-rw-rw-rw-   0        0        0    37326 2019-09-19 15:35:35.000000 adamspy-0.9.9/test/test_drill_string.py
+-rw-rw-rw-   0        0        0     5329 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_drill_tool.py
+-rw-rw-rw-   0        0        0    28175 2019-09-24 18:28:52.000000 adamspy-0.9.9/test/test_drillsim.py
+-rw-rw-rw-   0        0        0     6241 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_hole.py
+-rw-rw-rw-   0        0        0     1303 2020-01-23 14:23:03.000000 adamspy-0.9.9/test/test_motor_curve_generator.py
+-rw-rw-rw-   0        0        0     8293 2020-03-03 17:58:32.000000 adamspy-0.9.9/test/test_results.py
+-rw-rw-rw-   0        0        0     6881 2019-08-30 13:52:59.000000 adamspy-0.9.9/test/test_tiem_orbit.py
```

### Comparing `adamspy-0.9.8/LICENSE` & `adamspy-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/PKG-INFO` & `adamspy-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adamspy
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python tools for working with Adams data
 Home-page: https://github.com/bthornton191/adamspy
 Author: Ben Thornton
 Author-email: ben.thornton@mscsoftware.com
 License: UNKNOWN
 Description: # adamspy
```

### Comparing `adamspy-0.9.8/adamspy/adamspy.py` & `adamspy-0.9.9/adamspy/adamspy.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/__init__.py` & `adamspy-0.9.9/adamspy/adripy/__init__.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/constants.py` & `adamspy-0.9.9/adamspy/adripy/constants.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/database.py` & `adamspy-0.9.9/adamspy/adripy/database.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/drillsim.py` & `adamspy-0.9.9/adamspy/adripy/drillsim.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/event.py` & `adamspy-0.9.9/adamspy/adripy/event.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/hole.py` & `adamspy-0.9.9/adamspy/adripy/hole.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/solver_settings.py` & `adamspy-0.9.9/adamspy/adripy/solver_settings.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/string.py` & `adamspy-0.9.9/adamspy/adripy/string.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template.cfg` & `adamspy-0.9.9/adamspy/adripy/templates/template.cfg`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template.evt` & `adamspy-0.9.9/adamspy/adripy/templates/template.evt`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template.hol` & `adamspy-0.9.9/adamspy/adripy/templates/template.hol`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template.ssf` & `adamspy-0.9.9/adamspy/adripy/templates/template.ssf`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template.sta` & `adamspy-0.9.9/adamspy/adripy/templates/template.sta`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template_1.str` & `adamspy-0.9.9/adamspy/adripy/templates/template_1.str`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/templates/template_2.str` & `adamspy-0.9.9/adamspy/adripy/templates/template_2.str`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/tool.py` & `adamspy-0.9.9/adamspy/adripy/tool.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/adripy/utilities.py` & `adamspy-0.9.9/adamspy/adripy/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
     # Create a block of code to add to the adm file
     code_block = {}
     for param in ADRILL_IDS:
         code_block[param] = "!\n"
         code_block[param] += "!                          adams_view_name='{}_Spline'\n".format(param.upper())
         code_block[param] += "SPLINE/{:d}\n".format(ADRILL_IDS[param]['spline'])
         code_block[param] += ", LINEAR_EXTRAPOLATE\n"
-        code_block[param] += ", X={}\n".format(str(splines[param][1]).replace('[','').replace(']',''))
+        code_block[param] += ", X={}\n".format(str(splines['time']).replace('[','').replace(']',''))
         
         val_string = ''
         for val in splines[param]:
             val_string += '{:1.2f},'.format(val)
         val_string = val_string[:-1]
         code_block[param] += ", Y={}\n".format(val_string)
```

### Comparing `adamspy-0.9.8/adamspy/postprocess/__init__.py` & `adamspy-0.9.9/adamspy/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/postprocess/animation.py` & `adamspy-0.9.9/adamspy/postprocess/animation.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/postprocess/aview_scripts/_get_lunar_results.py` & `adamspy-0.9.9/adamspy/postprocess/aview_scripts/_get_lunar_results.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/postprocess/ppt.py` & `adamspy-0.9.9/adamspy/postprocess/ppt.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy/postprocess/xml.py` & `adamspy-0.9.9/adamspy/postprocess/xml.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/adamspy.egg-info/PKG-INFO` & `adamspy-0.9.9/adamspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adamspy
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python tools for working with Adams data
 Home-page: https://github.com/bthornton191/adamspy
 Author: Ben Thornton
 Author-email: ben.thornton@mscsoftware.com
 License: UNKNOWN
 Description: # adamspy
```

### Comparing `adamspy-0.9.8/adamspy.egg-info/SOURCES.txt` & `adamspy-0.9.9/adamspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/requirements.txt` & `adamspy-0.9.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/setup.py` & `adamspy-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_adamspy.py` & `adamspy-0.9.9/test/test_adamspy.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_adripy_utilities.py` & `adamspy-0.9.9/test/test_adripy_utilities.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_animation.py` & `adamspy-0.9.9/test/test_animation.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_build.py` & `adamspy-0.9.9/test/test_build.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_database.py` & `adamspy-0.9.9/test/test_database.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_drill_event.py` & `adamspy-0.9.9/test/test_drill_event.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_drill_solver_settings.py` & `adamspy-0.9.9/test/test_drill_solver_settings.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_drill_string.py` & `adamspy-0.9.9/test/test_drill_string.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_drill_tool.py` & `adamspy-0.9.9/test/test_drill_tool.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_drillsim.py` & `adamspy-0.9.9/test/test_drillsim.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_hole.py` & `adamspy-0.9.9/test/test_hole.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_motor_curve_generator.py` & `adamspy-0.9.9/test/test_motor_curve_generator.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_results.py` & `adamspy-0.9.9/test/test_results.py`

 * *Files identical despite different names*

### Comparing `adamspy-0.9.8/test/test_tiem_orbit.py` & `adamspy-0.9.9/test/test_tiem_orbit.py`

 * *Files identical despite different names*

