# Comparing `tmp/upk2esphome-1.1.2.tar.gz` & `tmp/upk2esphome-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upk2esphome-1.1.2.tar", max compression
+gzip compressed data, was "upk2esphome-1.2.0.tar", max compression
```

## Comparing `upk2esphome-1.1.2.tar` & `upk2esphome-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1076 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/LICENSE
--rw-r--r--   0        0        0      531 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/README.md
--rw-r--r--   0        0        0      641 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/ltctplugin/upk2esphome/__init__.py
--rw-r--r--   0        0        0    11818 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/ltctplugin/upk2esphome/gui.py
--rw-r--r--   0        0        0    10935 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/ltctplugin/upk2esphome/upk2esphome.wxui
--rw-r--r--   0        0        0    13366 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/ltctplugin/upk2esphome/upk2esphome.xrc
--rw-r--r--   0        0        0     4841 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/ltctplugin/upk2esphome/work.py
--rw-r--r--   0        0        0      567 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      256 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/generator.py
--rw-r--r--   0        0        0     1442 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/input.py
--rw-r--r--   0        0        0      400 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/opts.py
--rw-r--r--   0        0        0       48 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/__init__.py
--rw-r--r--   0        0        0     8371 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/bulb.py
--rw-r--r--   0        0        0     1406 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/module.py
--rw-r--r--   0        0        0     3403 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/monitor.py
--rw-r--r--   0        0        0      775 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/netled.py
--rw-r--r--   0        0        0     1355 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/static.py
--rw-r--r--   0        0        0     3009 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/parts/switch.py
--rw-r--r--   0        0        0     1834 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/result.py
--rw-r--r--   0        0        0      651 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/test.py
--rw-r--r--   0        0        0      444 2023-05-22 14:38:20.399144 upk2esphome-1.1.2/upk2esphome/tests/bulb_cw_pwm.txt
--rw-r--r--   0        0        0      563 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbc_2135_2.txt
--rw-r--r--   0        0        0      430 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_2135.txt
--rw-r--r--   0        0        0      543 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
--rw-r--r--   0        0        0      599 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_2235.txt
--rw-r--r--   0        0        0      496 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_5758d.txt
--rw-r--r--   0        0        0        0 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/empty.txt
--rw-r--r--   0        0        0     2936 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/plug_monitor_bl0937.txt
--rw-r--r--   0        0        0      476 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/plug_monitor_bl0942.txt
--rw-r--r--   0        0        0      497 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/plug_monitor_hlw8032.txt
--rw-r--r--   0        0        0      914 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/plug_total.txt
--rw-r--r--   0        0        0      777 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/tests/switch_monitor.txt
--rw-r--r--   0        0        0      922 2023-05-22 14:38:20.403144 upk2esphome-1.1.2/upk2esphome/web.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 upk2esphome-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/LICENSE
+-rw-r--r--   0        0        0      531 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/README.md
+-rw-r--r--   0        0        0      641 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/ltctplugin/upk2esphome/__init__.py
+-rw-r--r--   0        0        0    11818 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/ltctplugin/upk2esphome/gui.py
+-rw-r--r--   0        0        0    10935 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/ltctplugin/upk2esphome/upk2esphome.wxui
+-rw-r--r--   0        0        0    13366 2023-07-13 18:00:06.193489 upk2esphome-1.2.0/ltctplugin/upk2esphome/upk2esphome.xrc
+-rw-r--r--   0        0        0     4841 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/ltctplugin/upk2esphome/work.py
+-rw-r--r--   0        0        0      567 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      256 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/generator.py
+-rw-r--r--   0        0        0     1442 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/input.py
+-rw-r--r--   0        0        0      403 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/opts.py
+-rw-r--r--   0        0        0       48 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/__init__.py
+-rw-r--r--   0        0        0     8371 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/bulb.py
+-rw-r--r--   0        0        0     1400 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/module.py
+-rw-r--r--   0        0        0     3403 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/monitor.py
+-rw-r--r--   0        0        0      775 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/netled.py
+-rw-r--r--   0        0        0     1355 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/static.py
+-rw-r--r--   0        0        0     3009 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/parts/switch.py
+-rw-r--r--   0        0        0     1834 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/result.py
+-rw-r--r--   0        0        0      651 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/test.py
+-rw-r--r--   0        0        0      444 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_cw_pwm.txt
+-rw-r--r--   0        0        0      563 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbc_2135_2.txt
+-rw-r--r--   0        0        0      430 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_2135.txt
+-rw-r--r--   0        0        0      543 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt
+-rw-r--r--   0        0        0      599 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_2235.txt
+-rw-r--r--   0        0        0      496 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_5758d.txt
+-rw-r--r--   0        0        0        0 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/empty.txt
+-rw-r--r--   0        0        0     2936 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/plug_monitor_bl0937.txt
+-rw-r--r--   0        0        0      476 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/plug_monitor_bl0942.txt
+-rw-r--r--   0        0        0      497 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/plug_monitor_hlw8032.txt
+-rw-r--r--   0        0        0      914 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/plug_total.txt
+-rw-r--r--   0        0        0      777 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/tests/switch_monitor.txt
+-rw-r--r--   0        0        0      922 2023-07-13 18:00:06.197489 upk2esphome-1.2.0/upk2esphome/web.py
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 upk2esphome-1.2.0/PKG-INFO
```

### Comparing `upk2esphome-1.1.2/LICENSE` & `upk2esphome-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/README.md` & `upk2esphome-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/ltctplugin/upk2esphome/__init__.py` & `upk2esphome-1.2.0/ltctplugin/upk2esphome/__init__.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/ltctplugin/upk2esphome/gui.py` & `upk2esphome-1.2.0/ltctplugin/upk2esphome/gui.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/ltctplugin/upk2esphome/upk2esphome.wxui` & `upk2esphome-1.2.0/ltctplugin/upk2esphome/upk2esphome.wxui`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/ltctplugin/upk2esphome/upk2esphome.xrc` & `upk2esphome-1.2.0/ltctplugin/upk2esphome/upk2esphome.xrc`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/ltctplugin/upk2esphome/work.py` & `upk2esphome-1.2.0/ltctplugin/upk2esphome/work.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/pyproject.toml` & `upk2esphome-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upk2esphome"
-version = "1.1.2"
+version = "1.2.0"
 description = "Convert Tuya device configuration to ESPHome YAML (ltchiptool plugin)"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "upk2esphome" },
     { include = "ltctplugin/upk2esphome" },
```

### Comparing `upk2esphome-1.1.2/upk2esphome/generator.py` & `upk2esphome-1.2.0/upk2esphome/generator.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/input.py` & `upk2esphome-1.2.0/upk2esphome/input.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/bulb.py` & `upk2esphome-1.2.0/upk2esphome/parts/bulb.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/module.py` & `upk2esphome-1.2.0/upk2esphome/parts/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         yr.warn("No module type found! You have to set the board: manually")
         if opts.esphome_block:
             yr.data["esphome"] = {
                 "name": "upk2esphome",
             }
             if opts.name_mac:
                 yr.data["esphome"]["name_add_mac_suffix"] = True
-            yr.data["libretiny"] = {
+            yr.data["bk72xx"] = {
                 "board": "REPLACEME",
                 "framework": {
                     "version": "dev",
                 },
             }
         return
 
@@ -36,13 +36,13 @@
 
     if opts.esphome_block:
         yr.data["esphome"] = {
             "name": config["module"].lower(),
         }
         if opts.name_mac:
             yr.data["esphome"]["name_add_mac_suffix"] = True
-        yr.data["libretiny"] = {
+        yr.data["bk72xx"] = {
             "board": board,
             "framework": {
                 "version": "dev",
             },
         }
```

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/monitor.py` & `upk2esphome-1.2.0/upk2esphome/parts/monitor.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/netled.py` & `upk2esphome-1.2.0/upk2esphome/parts/netled.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/static.py` & `upk2esphome-1.2.0/upk2esphome/parts/static.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/parts/switch.py` & `upk2esphome-1.2.0/upk2esphome/parts/switch.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/result.py` & `upk2esphome-1.2.0/upk2esphome/result.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/test.py` & `upk2esphome-1.2.0/upk2esphome/test.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbc_2135_2.txt` & `upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbc_2135_2.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt` & `upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_2135_ampere.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/bulb_rgbcw_2235.txt` & `upk2esphome-1.2.0/upk2esphome/tests/bulb_rgbcw_2235.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/plug_monitor_bl0937.txt` & `upk2esphome-1.2.0/upk2esphome/tests/plug_monitor_bl0937.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/plug_total.txt` & `upk2esphome-1.2.0/upk2esphome/tests/plug_total.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/tests/switch_monitor.txt` & `upk2esphome-1.2.0/upk2esphome/tests/switch_monitor.txt`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/upk2esphome/web.py` & `upk2esphome-1.2.0/upk2esphome/web.py`

 * *Files identical despite different names*

### Comparing `upk2esphome-1.1.2/PKG-INFO` & `upk2esphome-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upk2esphome
-Version: 1.1.2
+Version: 1.2.0
 Summary: Convert Tuya device configuration to ESPHome YAML (ltchiptool plugin)
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

