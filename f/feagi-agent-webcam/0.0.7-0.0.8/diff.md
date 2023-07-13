# Comparing `tmp/feagi_agent_webcam-0.0.7.tar.gz` & `tmp/feagi_agent_webcam-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_webcam-0.0.7.tar", last modified: Fri Jul  7 14:42:14 2023, max compression
+gzip compressed data, was "feagi_agent_webcam-0.0.8.tar", last modified: Thu Jul 13 14:51:25 2023, max compression
```

## Comparing `feagi_agent_webcam-0.0.7.tar` & `feagi_agent_webcam-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:42:14.663980 feagi_agent_webcam-0.0.7/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.7/LICENSE
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-07 14:42:14.663980 feagi_agent_webcam-0.0.7/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      766 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.7/README.md
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:42:14.659980 feagi_agent_webcam-0.0.7/feagi_agent_webcam/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam/__init__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1979 2023-07-07 14:33:55.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam/__main__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1538 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam/configuration.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     9277 2023-07-07 14:33:55.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam/controller.py
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:42:14.663980 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-07 14:42:14.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      390 2023-07-07 14:42:14.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/SOURCES.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:42:14.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/dependency_links.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       64 2023-07-07 14:42:14.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/requires.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       19 2023-07-07 14:42:14.000000 feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/top_level.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.7/pyproject.toml
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      742 2023-07-07 14:42:14.663980 feagi_agent_webcam-0.0.7/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 14:51:25.927583 feagi_agent_webcam-0.0.8/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-12 16:47:26.000000 feagi_agent_webcam-0.0.8/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-13 14:51:25.931583 feagi_agent_webcam-0.0.8/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      766 2023-07-12 16:47:26.000000 feagi_agent_webcam-0.0.8/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 14:51:25.927583 feagi_agent_webcam-0.0.8/feagi_agent_webcam/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-12 16:47:26.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2532 2023-07-12 21:15:58.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1538 2023-07-12 16:47:26.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam/configuration.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    10434 2023-07-13 14:09:33.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam/controller.py
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-13 14:51:25.927583 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-13 14:51:25.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      390 2023-07-13 14:51:25.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-13 14:51:25.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       64 2023-07-13 14:51:25.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       19 2023-07-13 14:51:25.000000 feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-12 16:47:26.000000 feagi_agent_webcam-0.0.8/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      742 2023-07-13 14:51:25.931583 feagi_agent_webcam-0.0.8/setup.cfg
```

### Comparing `feagi_agent_webcam-0.0.7/LICENSE` & `feagi_agent_webcam-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.7/PKG-INFO` & `feagi_agent_webcam-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_agent_webcam
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feagi agent webcam to connect feagi with your webcam
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_webcam-0.0.7/README.md` & `feagi_agent_webcam-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.7/feagi_agent_webcam/__main__.py` & `feagi_agent_webcam-0.0.8/feagi_agent_webcam/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 #!/usr/bin/env python3
 import argparse
 import subprocess
 import sys
 import os
 import sysconfig
 import feagi_agent_webcam
+import traceback
+from time import sleep
 from feagi_agent_webcam.configuration import *
 
 if __name__ == '__main__':
     # Check if feagi_agent has arg
     parser = argparse.ArgumentParser(description='configuration for any webcam')
     parser.add_argument('-loop', '--loop', help='Enable loop for the video', required=False)
     parser.add_argument('-ip', '--ip', help='Description for ip address argument', required=False)
-    parser.add_argument('-device', '--device', help='To bind the location or index of webcam.', required=False)
+    parser.add_argument('-device', '--device', help='To bind the location or index of webcam.',
+                        required=False)
     parser.add_argument('-video', '--video', help='Use the path to video to read', required=False)
-    parser.add_argument('-port', '--port', help='Change the port instead of default 8000.', required=False)
+    parser.add_argument('-port', '--port', help='Change the port instead of default 8000.',
+                        required=False)
     args = vars(parser.parse_args())
     if args['ip']:
         feagi_settings["feagi_host"] = args['ip']
     if args['loop'] == "true" or args['loop'] == "True":
         capabilities["camera"]["video_loop"] = bool(args['loop'])
     if args['device']:
         capabilities["camera"]["video_device_index"] = int(args['device'])
     else:
         capabilities["camera"]["video_device_index"] = 0
     if args['video']:
         capabilities["camera"]["video_device_index"] = args['video']
     if args['port']:
         feagi_settings["feagi_api_port"] = args['port']
     if __name__ == '__main__':
-        from feagi_agent_webcam import controller as webcam_controller
-
-        feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
-        print("FEAGI AUTH URL ------- ", feagi_auth_url)
+        inital_feagi_setting = feagi_settings.copy()
+        inital_agent_settings = agent_settings.copy()
+        inital_capabilities = capabilities.copy()
+        inital_message_to_feagi = message_to_feagi.copy()
         while True:
             try:
+                from feagi_agent_webcam import controller as webcam_controller
+                feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
+                print("FEAGI AUTH URL ------- ", feagi_auth_url)
                 webcam_controller.main(feagi_auth_url, feagi_settings, agent_settings,
-                                       capabilities,
-                      message_to_feagi)
+                                       capabilities, message_to_feagi)
             except Exception as e:
+                feagi_settings = inital_feagi_setting.copy()
+                agent_settings = inital_agent_settings.copy()
+                capabilities = inital_capabilities.copy()
+                message_to_feagi = inital_message_to_feagi.copy()
                 print(f"Controller run failed", e)
-                traceback.print_exc()
+                # traceback.print_exc()
                 sleep(2)
```

### Comparing `feagi_agent_webcam-0.0.7/feagi_agent_webcam/configuration.py` & `feagi_agent_webcam-0.0.8/feagi_agent_webcam/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.7/feagi_agent_webcam/controller.py` & `feagi_agent_webcam-0.0.8/feagi_agent_webcam/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,50 +2,53 @@
 # -*- coding: utf-8 -*-
 
 """
 Demo of dot kinematogram
 """
 
 import sys
+
 sys.path.append('../../feagi_agent_core/')
 import cv2
 import requests
 from time import sleep
 from datetime import datetime
 from feagi_agent import retina as retina
 from feagi_agent import feagi_interface as feagi
 import traceback
 
 
 def chroma_keyer(frame, size, name_id):
     """
-    This function allows you to remove the specific color. In psychopy window, it shows a gray which is 128,128,128.
-    So this function will remove the 128 and focus on something else than the gray. Consider this as making the data
-    into a transparent.
+    This function allows you to remove the specific color. In psychopy window, it shows a gray
+    which is 128,128,128. So this function will remove the 128 and focus on something else than
+    the gray. Consider this as making the data into a transparent.
 
     Currently, this is in BETA and not used in any of this code.
     """
     vision_dict = dict()
     frame_row_count = size[0]  # width
     frame_col_count = size[1]  # height
 
     x_vision = 0  # row counter
     y_vision = 0  # col counter
     z_vision = 0  # RGB counter
 
     previous_frame = {}
     frame_len = frame_row_count * frame_col_count * 3  # hardcoded. Needs to update this section.
     try:
-        if frame_len == frame_row_count * frame_col_count * 3:  # check to ensure frame length matches the
-            # resolution setting
+        if frame_len == frame_row_count * frame_col_count * 3:  # check to ensure frame length
+            # matches the resolution setting
             for index in range(frame_len):
                 if frame[index] != 128:
-                    dict_key = str(y_vision) + '-' + str(abs((frame_row_count - 1) - x_vision)) + '-' + str(
+                    dict_key = str(y_vision) + '-' + str(
+                        abs((frame_row_count - 1) - x_vision)) + '-' + str(
                         0)
-                    vision_dict[dict_key] = frame[index]  # save the value for the changed index to the dict
+                    vision_dict[dict_key] = frame[
+                        index]  # save the value for the changed index to the dict
                 z_vision += 1
                 if z_vision == 3:
                     z_vision = 0
                     y_vision += 1
                     if y_vision == frame_col_count:
                         y_vision = 0
                         x_vision += 1
@@ -56,37 +59,40 @@
     if len(vision_dict) > 3500:
         return {'camera': {name_id: {}}}
     else:
         return {'camera': {name_id: vision_dict}}
 
 
 def main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi):
-    print("feagi setting: ", feagi_settings)
-    print("agent setting: ", agent_settings)
-    print("capa: ", capabilities)
-    print("message: ", message_to_feagi)
     # Generate runtime dictionary
     previous_data_frame = dict()
     runtime_data = {"cortical_data": {}, "current_burst_id": None, "stimulation_period": None,
                     "feagi_state": None,
                     "feagi_network": None}
-
+    feagi_flag = False
+    print("retrying...")
+    print("Waiting on FEAGI...")
+    while not feagi_flag:
+        feagi_flag = feagi.is_FEAGI_reachable(feagi_settings["feagi_host"], 3000)
+        sleep(2)
+    burst_counter_endpoint = feagi.feagi_api_burst_counter()
     # FEAGI section start
     print("Connecting to FEAGI resources...")
-    runtime_data["feagi_state"] = feagi.feagi_registration(feagi_auth_url=feagi_auth_url, 
-            feagi_settings=feagi_settings, agent_settings=agent_settings, capabilities=capabilities)
+    runtime_data["feagi_state"] = feagi.feagi_registration(feagi_auth_url=feagi_auth_url,
+                                                           feagi_settings=feagi_settings,
+                                                           agent_settings=agent_settings,
+                                                           capabilities=capabilities)
+    print("FEAGI REGISTERED!")
     api_address = runtime_data['feagi_state']["feagi_url"]
 
-    stimulation_period_endpoint = feagi.feagi_api_burst_engine()
-    burst_counter_endpoint = feagi.feagi_api_burst_counter()
-    
     # agent_data_port = agent_settings["agent_data_port"]
     agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
+    stimulation_period_endpoint = feagi.feagi_api_burst_engine()
 
     # todo: to obtain this info directly from FEAGI as part of registration
     # ipu_channel_address = feagi.feagi_inbound(agent_settings["agent_data_port"])
     ipu_channel_address = feagi.feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
     print("IPU_channel_address=", ipu_channel_address)
     opu_channel_address = feagi.feagi_outbound(feagi_settings['feagi_host'],
                                                runtime_data["feagi_state"]['feagi_opu_port'])
@@ -100,94 +106,106 @@
     checkpoint_total = 5
     flag_counter = 0
     rgb['camera'] = dict()
 
     cam = cv2.VideoCapture(capabilities['camera']['video_device_index'])
 
     while True:
-        message_from_feagi = feagi_opu_channel.receive()
-        check, pixels = cam.read()
-        if bool(capabilities["camera"]["video_loop"]):
-            if check:
-                pass
-            else:
-                cam.set(cv2.CAP_PROP_POS_FRAMES, 0)
-                # check, pixels = cam.read()
-        retina_data = retina.frame_split(pixels, capabilities['camera']['retina_width_percent'],
-                                         capabilities['camera']['retina_height_percent'])
-        for i in retina_data:
-            if 'C' in i:
-                retina_data[i] = retina.center_data_compression(retina_data[i],
-                                                                capabilities['camera']["central_vision_compression"]
-                                                                )
-            else:
-                retina_data[i] = retina.center_data_compression(retina_data[i],
-                                                                capabilities['camera']
-                                                                ['peripheral_vision_compression'])
-        opu_data = feagi.opu_processor(message_from_feagi)
-        if previous_data_frame == {}:
+        try:
+            message_from_feagi = feagi_opu_channel.receive()
+            check, pixels = cam.read()
+            if bool(capabilities["camera"]["video_loop"]):
+                if check:
+                    pass
+                else:
+                    cam.set(cv2.CAP_PROP_POS_FRAMES, 0)
+                    # check, pixels = cam.read()
+            retina_data = retina.frame_split(pixels, capabilities['camera']['retina_width_percent'],
+                                             capabilities['camera']['retina_height_percent'])
             for i in retina_data:
-                previous_name = str(i) + "_prev"
-                previous_data_frame[previous_name] = {}
-        for i in retina_data:
-            name = i
-            if 'prev' not in i:
-                data = retina.ndarray_to_list(retina_data[i])
                 if 'C' in i:
-                    previous_name = str(i) + "_prev"
-                    rgb_data, previous_data_frame[previous_name] = retina.get_rgb(data,
-                                                                                  capabilities['camera'][
-                                                                                      'central_vision_compression'],
-                                                                                  previous_data_frame[previous_name],
-                                                                                  name,
-                                                                                  capabilities[
-                                                                                      'camera']['deviation_threshold'])
+                    retina_data[i] = retina.center_data_compression(
+                        retina_data[i],
+                        capabilities['camera'][
+                            "central_vision_compression"]
+                    )
                 else:
+                    retina_data[i] = retina.center_data_compression(
+                        retina_data[i],
+                        capabilities['camera']
+                        ['peripheral_vision_compression'])
+            opu_data = feagi.opu_processor(message_from_feagi)
+            if previous_data_frame == {}:
+                for i in retina_data:
                     previous_name = str(i) + "_prev"
-                    rgb_data, previous_data_frame[previous_name] = retina.get_rgb(data,
-                                                                                  capabilities['camera'][
-                                                                                      'peripheral_vision_compression'],
-                                                                                  previous_data_frame[previous_name],
-                                                                                  name,
-                                                                                  capabilities[
-                                                                                      'camera']['deviation_threshold'])
-                for a in rgb_data['camera']:
-                    rgb['camera'][a] = rgb_data['camera'][a]
-        try:
-            if "data" not in message_to_feagi:
-                message_to_feagi["data"] = dict()
-            if "sensory_data" not in message_to_feagi["data"]:
-                message_to_feagi["data"]["sensory_data"] = dict()
-            message_to_feagi["data"]["sensory_data"]['camera'] = rgb['camera']
-        except Exception as e:
-            pass
-        # Psychopy game ends
-        message_to_feagi['timestamp'] = datetime.now()
-        message_to_feagi['counter'] = msg_counter
-        msg_counter += 1
-        flag_counter += 1
-        if flag_counter == int(checkpoint_total):
-            feagi_burst_speed = requests.get(api_address + stimulation_period_endpoint).json()
-            feagi_burst_counter = requests.get(api_address + burst_counter_endpoint).json()
-            flag_counter = 0
-            if feagi_burst_speed > 1:
-                checkpoint_total = 5
-            if feagi_burst_speed < 1:
-                checkpoint_total = 5 / feagi_burst_speed
-            if msg_counter < feagi_burst_counter:
-                feagi_opu_channel = feagi.sub_initializer(opu_address=opu_channel_address)
+                    previous_data_frame[previous_name] = {}
+            for i in retina_data:
+                name = i
+                if 'prev' not in i:
+                    data = retina.ndarray_to_list(retina_data[i])
+                    if 'C' in i:
+                        previous_name = str(i) + "_prev"
+                        rgb_data, previous_data_frame[previous_name] = retina.get_rgb(data,
+                                                                                      capabilities[
+                                                                                          'camera'][
+                                                                                          'central_vision_compression'],
+                                                                                      previous_data_frame[
+                                                                                          previous_name],
+                                                                                      name,
+                                                                                      capabilities[
+                                                                                          'camera'][
+                                                                                          'deviation_threshold'])
+                    else:
+                        previous_name = str(i) + "_prev"
+                        rgb_data, previous_data_frame[previous_name] = retina.get_rgb(data,
+                                                                                      capabilities[
+                                                                                          'camera'][
+                                                                                          'peripheral_vision_compression'],
+                                                                                      previous_data_frame[
+                                                                                          previous_name],
+                                                                                      name,
+                                                                                      capabilities[
+                                                                                          'camera'][
+                                                                                          'deviation_threshold'])
+                    for a in rgb_data['camera']:
+                        rgb['camera'][a] = rgb_data['camera'][a]
+            try:
+                if "data" not in message_to_feagi:
+                    message_to_feagi["data"] = dict()
+                if "sensory_data" not in message_to_feagi["data"]:
+                    message_to_feagi["data"]["sensory_data"] = dict()
+                message_to_feagi["data"]["sensory_data"]['camera'] = rgb['camera']
+            except Exception as e:
+                pass
+            # Psychopy game ends
+            message_to_feagi['timestamp'] = datetime.now()
+            message_to_feagi['counter'] = msg_counter
+            msg_counter += 1
+            flag_counter += 1
+            if flag_counter == int(checkpoint_total):
+                feagi_burst_speed = requests.get(api_address + stimulation_period_endpoint).json()
+                feagi_burst_counter = requests.get(api_address + burst_counter_endpoint).json()
+                flag_counter = 0
+                if feagi_burst_speed > 1:
+                    checkpoint_total = 5
+                if feagi_burst_speed < 1:
+                    checkpoint_total = 5 / feagi_burst_speed
+                if msg_counter < feagi_burst_counter:
+                    feagi_opu_channel = feagi.sub_initializer(opu_address=opu_channel_address)
+                    if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
+                        feagi_settings['feagi_burst_speed'] = feagi_burst_speed
                 if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
                     feagi_settings['feagi_burst_speed'] = feagi_burst_speed
-            if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
-                feagi_settings['feagi_burst_speed'] = feagi_burst_speed
-                msg_counter = feagi_burst_counter
-        sleep(feagi_settings['feagi_burst_speed'])
-        try:
-            print("Len --", len(message_to_feagi['data']['sensory_data']['camera']['C']))
-        except:
-            pass
-        feagi_ipu_channel.send(message_to_feagi)
-        message_to_feagi.clear()
-        for i in rgb['camera']:
-            rgb['camera'][i].clear()
-    win.close()
-    core.quit()
+                    msg_counter = feagi_burst_counter
+            sleep(feagi_settings['feagi_burst_speed'])
+            try:
+                print("Len --", len(message_to_feagi['data']['sensory_data']['camera']['C']))
+            except:
+                pass
+            feagi_ipu_channel.send(message_to_feagi)
+            message_to_feagi.clear()
+            for i in rgb['camera']:
+                rgb['camera'][i].clear()
+        except Exception as e:
+            print("ERROR! : ", e)
+            cam.release()
+            break
```

### Comparing `feagi_agent_webcam-0.0.7/feagi_agent_webcam.egg-info/PKG-INFO` & `feagi_agent_webcam-0.0.8/feagi_agent_webcam.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi-agent-webcam
-Version: 0.0.7
+Version: 0.0.8
 Summary: Feagi agent webcam to connect feagi with your webcam
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_webcam-0.0.7/setup.cfg` & `feagi_agent_webcam-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_webcam
-version = 0.0.7
+version = 0.0.8
 author = Neuraville LLC
 author_email = info@neuraville.com
 description = Feagi agent webcam to connect feagi with your webcam
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```

