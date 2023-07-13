# Comparing `tmp/feagi_agent_freenove-0.0.7.tar.gz` & `tmp/feagi_agent_freenove-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_freenove-0.0.7.tar", last modified: Fri Jul  7 14:25:14 2023, max compression
+gzip compressed data, was "feagi_agent_freenove-0.0.8.tar", last modified: Thu Jul 13 15:50:48 2023, max compression
```

## Comparing `feagi_agent_freenove-0.0.7.tar` & `feagi_agent_freenove-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/LICENSE
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4824 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/README.md
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/feagi_agent_freenove/
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/ADC.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6227 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/Led.py
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/PCA9685.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/__init__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2096 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/__main__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2432 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/configuration.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    26148 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/controller.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/requirements.txt
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/setup.sh
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/verify.sh
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/SOURCES.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/dependency_links.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/requires.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/top_level.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/pyproject.toml
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-07-07 14:25:14.834376 feagi_agent_freenove-0.0.7/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4824 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.180426 feagi_agent_freenove-0.0.8/feagi_agent_freenove/
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/ADC.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6227 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/Led.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/PCA9685.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2112 2023-07-13 15:26:51.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2432 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/configuration.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    26436 2023-07-13 15:42:18.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/controller.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/requirements.txt
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/setup.sh
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove/verify.sh
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-07-13 15:50:48.000000 feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-12 16:47:26.000000 feagi_agent_freenove-0.0.8/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-07-13 15:50:48.184426 feagi_agent_freenove-0.0.8/setup.cfg
```

### Comparing `feagi_agent_freenove-0.0.7/LICENSE` & `feagi_agent_freenove-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/PKG-INFO` & `feagi_agent_freenove-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_agent_freenove
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_freenove-0.0.7/README.md` & `feagi_agent_freenove-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/ADC.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/ADC.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/Led.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/Led.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/PCA9685.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/PCA9685.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/__main__.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import subprocess
 import sys
 import os
 import sysconfig
 import feagi_agent_freenove
 import traceback
+import requests
 from time import sleep
 from feagi_agent_freenove.configuration import *
 
 if __name__ == '__main__':
     # Check if feagi_agent has arg
     parser = argparse.ArgumentParser(description='configuration for any webcam')
     parser.add_argument('-ip', '--ip', help='to connect FEAGI, required=False')
```

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/configuration.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/controller.py` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,24 @@
 #         adc = Adc()
 #         Power = adc.recvADC(2) * 3
 #         # print(Power)
 #         return Power
 
 def main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi, args):
     GPIO.cleanup()
+    # # FEAGI REACHABLE CHECKER # #
+    feagi_flag = False
+    print("retrying...")
+    print("Waiting on FEAGI...")
+    while not feagi_flag:
+        feagi_flag = FEAGI.is_FEAGI_reachable(feagi_settings["feagi_host"], 3000)
+        sleep(2)
+
+    # # FEAGI REACHABLE CHECKER COMPLETED # #
+
     # # # FEAGI registration # # # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # - - - - - - - - - - - - - - - - - - #
     print("Connecting to FEAGI resources...")
     runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_auth_url=feagi_auth_url,
                                                            feagi_settings=feagi_settings,
                                                            agent_settings=agent_settings,
                                                            capabilities=capabilities)
@@ -415,22 +425,15 @@
     agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
 
     # todo: to obtain this info directly from FEAGI as part of registration
     # ipu_channel_address = FEAGI.feagi_inbound(agent_settings["agent_data_port"])
     ipu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
-    # if args['http_type']:
-    #     http = args['http_type']
-    # else:
-    #     http = 'http://'
-    # if args['port_disabled'] == 'true':
-    #     api_address = http + feagi_host
-    # else:
-    #     api_address = http + feagi_host + ':' + api_port
+
     print("IPU_channel_address=", ipu_channel_address)
     opu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'],
                                                runtime_data["feagi_state"]['feagi_opu_port'])
 
     feagi_ipu_channel = FEAGI.pub_initializer(ipu_channel_address, bind=False)
     feagi_opu_channel = FEAGI.sub_initializer(opu_address=opu_channel_address)
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
@@ -595,9 +598,18 @@
                             feagi_settings['feagi_burst_speed'] = feagi_burst_speed
                 for id in range(motor_count):
                     motor_power = window_average(rolling_window[id])
                     motor_power = motor_power * capabilities["motor"]["power_amount"]
                     motor.move(id, motor_power)
         except KeyboardInterrupt as ke:  # Keyboard error
             motor.stop()
+            camera.stop_preview()
+            camera.close()
             keyboard_flag = False
-            print(ke)
+            print("ke: ", ke)
+            break
+        except Exception as e:
+            print("ERROR: ", e)
+            motor.stop()
+            camera.stop_preview()
+            camera.close()
+            break
```

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/setup.sh` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/setup.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove/verify.sh` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove/verify.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/PKG-INFO` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi-agent-freenove
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feagi agent freenove to connect feagi with your freenove_smartcar.
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/SOURCES.txt` & `feagi_agent_freenove-0.0.8/feagi_agent_freenove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.7/setup.cfg` & `feagi_agent_freenove-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_freenove
-version = 0.0.7
+version = 0.0.8
 author = Neuraville LLC
 author_email = info@feagi.org
 description = Feagi agent freenove to connect feagi with your freenove_smartcar.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```

