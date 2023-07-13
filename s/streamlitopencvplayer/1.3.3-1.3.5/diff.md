# Comparing `tmp/streamlitopencvplayer-1.3.3.tar.gz` & `tmp/streamlitopencvplayer-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.3.3.tar", last modified: Mon Jul 10 16:23:08 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.3.5.tar", last modified: Thu Jul 13 13:06:02 2023, max compression
```

## Comparing `streamlitopencvplayer-1.3.3.tar` & `streamlitopencvplayer-1.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.463556 streamlitopencvplayer-1.3.3/
--rw-rw-rw-   0        0        0      419 2023-07-10 16:23:08.462555 streamlitopencvplayer-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 16:23:08.464555 streamlitopencvplayer-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-07-10 16:18:16.000000 streamlitopencvplayer-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.432174 streamlitopencvplayer-1.3.3/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6770 2023-07-10 16:23:02.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.449896 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-10 16:23:08.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-10 16:23:07.000000 streamlitopencvplayer-1.3.3/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 16:23:08.457554 streamlitopencvplayer-1.3.3/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.3/test/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-07-04 20:30:14.000000 streamlitopencvplayer-1.3.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.478446 streamlitopencvplayer-1.3.5/
+-rw-rw-rw-   0        0        0      419 2023-07-13 13:06:02.476444 streamlitopencvplayer-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-07-10 16:34:21.000000 streamlitopencvplayer-1.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:06:02.479447 streamlitopencvplayer-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-07-13 13:05:56.000000 streamlitopencvplayer-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.452445 streamlitopencvplayer-1.3.5/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6514 2023-07-13 13:05:38.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.467446 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-13 13:06:02.000000 streamlitopencvplayer-1.3.5/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 13:06:02.473444 streamlitopencvplayer-1.3.5/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.3.5/test/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-07-11 08:43:30.000000 streamlitopencvplayer-1.3.5/test/test.py
```

### Comparing `streamlitopencvplayer-1.3.3/README.md` & `streamlitopencvplayer-1.3.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -26,10 +26,9 @@
 
 
 
 ### Run Test script 
 
 * Run the app:
     ```
-    
-    streamlit run test\test.py
+    streamlit run test/test.py -- -V "video path or url"
     ```
```

### Comparing `streamlitopencvplayer-1.3.3/setup.py` & `streamlitopencvplayer-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.3' 
+VERSION = '1.3.5' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.3.3/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.3.5/streamlitopencvplayer/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,179 +1,146 @@
 import time
-import urllib.request,json
+import urllib.request
+import json
 
 import cv2
 import streamlit as st
 
-# Initiate all session states used
-if 'counter' not in st.session_state:
-    st.session_state['counter'] = 0
-if 'cap' not in st.session_state:
-    st.session_state['cap'] = None
-if 'frames' not in st.session_state:
-    st.session_state['frames'] = []
-if 'alerts' not in st.session_state:
-    st.session_state['alerts'] = []
-if 'data' not in st.session_state:
-    st.session_state['data'] = []
-if 'alerts_list' not in st.session_state:
-    st.session_state['alerts_list'] = []
-if 'name_vid_sel' not in st.session_state:
-    st.session_state['name_vid_sel'] = "1687441603.4032989_1687441609.4032989"
-
 
+if "name_vid_sel" not in st.session_state:
+    st.session_state['name_vid_sel'] = "1689004947.7068138_1689004953.7068138"
 # Function to display video in the Streamlit app
 
 def display_video(video_path, json_file):
     # Open the video file
-    
-    st.session_state['cap'] = cv2.VideoCapture(video_path)
-    fps = st.session_state['cap'].get(cv2.CAP_PROP_FPS)
+    if "capture" not in st.session_state or st.session_state['old_vid_name'] != st.session_state['name_vid_sel']:
+        st.session_state['capture'] = cv2.VideoCapture(video_path)
+    if "fps" not in st.session_state:
+        st.session_state['fps'] = st.session_state['capture'].get(cv2.CAP_PROP_FPS)
+    if not st.session_state["capture"].isOpened():
+        st.write("No much video to open")
+        exit()
+    if "resume" not in st.session_state:
+        st.session_state["resume"] = False
+    if "frame" not in st.session_state:
+        ret, frame = st.session_state["capture"].read()
+        st.session_state["frame"] = frame
+
     # Opening JSON file and returns JSON object as a dictionnary
     if json_file is not None:
         response = urllib.request.urlopen(json_file)
         fileReader = json.loads(response.read())
         list_ts = []
         list_data = []
 
         for alert in fileReader["alerts"]:
             list_ts.append(alert["timestamp"])
             list_data.append(alert["data"])
-        
+
         st.session_state['alerts_list'] = list_ts
-        #print(list_ts)
-        #print(st.session_state['name_vid_sel'])
         alerts = []
         data = []
 
         for x in range(len(list_ts)):
-                time_alert = float(list_ts[x])-float(
-                    st.session_state['name_vid_sel'].partition('_')[0])
-                alerts.append(int((time_alert)*fps))
-                
-                data.append(list_data[x])
-    i = 0
+            time_alert = float(list_ts[x])-float(
+                st.session_state['name_vid_sel'].partition('_')[0])
+            alerts.append(int((time_alert)*st.session_state['fps']))
+            data.append(list_data[x])
 
-    draw_detections = st.checkbox("Draw detections",value=True)
-    resume = False
+    draw_detections = st.checkbox("Draw detections", value=True)
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
         # zone to display images
         stframe = st.empty()
     with column3:
         # Alerts
         st.subheader('Alerts :')
         num_buttons = len(alerts)
 
         button_values = {f'{i}': 0 for i in range(num_buttons)}
 
         for button_label, button_value in button_values.items():
             if st.button(str('Alert ')+button_label):
-                button_values = {label: 1 if label == button_label else 0 for label in button_values}
+                button_values = {label: 1 if label ==
+                                 button_label else 0 for label in button_values}
 
         for button_label, button_value in button_values.items():
             if button_value == 1:
-                #print(alerts[int(button_label)])
-                st.session_state['counter'] = alerts[int(button_label)]
-                resume = True
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, alerts[int(button_label)])
+                st.session_state["resume"] = True
 
     # Buttons and zone of display
-    col1, col2, col3, col4, col5,col6,col7 = st.columns(7, gap="small")
+    col1, col2, col3, col4, col5, col6, col7 = st.columns(7, gap="small")
     with col1:
-
         container_2 = st.empty()
         pause = container_2.button('⏸')
-
     with col2:
-
         plus = st.button("➕")
     with col4:
-
         replay = st.button("↻")
     with col3:
-
         minus = st.button("➖")
     with col5:
         st.write('')
 
-
     if replay:
-        st.session_state['counter'] = 0
-        st.session_state['frames'] = []
-        resume = False
+        st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, 0)
+        st.session_state["resume"] = False
 
+    while st.session_state["resume"] is False:
+        for x in range(int(st.session_state['fps'])):
+            ret, frame = st.session_state["capture"].read()
+            st.session_state["frame"] = frame
+            for i in range(len(data)):
+                if draw_detections:
+                    if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(alerts[i]):
+                        # draw all detections on the frame
+                        for j in range(len(data[i])):
+                            output = cv2.rectangle(st.session_state["frame"], (data[i][j][0][0], data[i][j][0][1]), (
+                                data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
+                            output = cv2.putText(
+                                st.session_state["frame"], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
+                        # update image zone with detections
+                        stframe.image(output, caption='', width=500)
+                        time.sleep(0.05)
+            stframe.image(
+                st.session_state["frame"], caption='', width=500)
+            time.sleep(0.05)
 
-        # get all the frames from video when the list is empty
-    if not st.session_state['frames']:
-        while True:
-            successs, frames = st.session_state['cap'].read()
-            if successs:
-                frames = cv2.cvtColor(frames, cv2.COLOR_BGR2RGB)
-                st.session_state['frames'].append(frames)
-            else:
+            if pause:
+                st.session_state["resume"] = True
+                break
+            if plus:
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-1)
+                st.write(int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)))
+                st.session_state["resume"] = True
                 break
-        st.session_state['cap'].release()
-    # back to the first frame if the video is finished
-    if st.session_state['counter'] == len(st.session_state['frames']):
-        st.session_state['counter'] = 0
-    #print(len(data))
-    stframe.image(st.session_state['frames']
-                  [st.session_state['counter']], caption='', width=450)
-    if not resume:
-        while st.session_state['counter'] < len(st.session_state['frames']):         
-                for i in range(len(data)):
-                    if draw_detections:
-                        if st.session_state['counter'] == int(alerts[i]):
-                            # draw all detections on the frame
-                            for j in range(len(data[i])):
-                                output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
-                                    data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
-                                output = cv2.putText(
-                                    st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
-                            # update image zone with detections
-                            stframe.image(output, caption='', width=500)
-                            time.sleep(0.05)
-                            # the detection is drawn, to the next one
-                            st.session_state['counter'] += 1
-
-                stframe.image(
-                    st.session_state['frames'][st.session_state['counter']], caption='', width=500)
-                time.sleep(0.05)
-                st.session_state['counter'] += 1
-                    
-
-                if pause:
-                    resume = True
-                    break
-                if plus:
-                    resume = True
-                    break
-                if minus:
-                    st.session_state['counter'] = st.session_state['counter']-2           
-                    resume = True
-                    break
-
-                    # back to the first frame if the video is finished
-                if st.session_state['counter'] == len(st.session_state['frames']):
-                    st.session_state['counter'] = 0
-                    resume = True
-                    break
+            if minus:
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-3)
+                st.write(int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES))-3)
+                st.session_state["resume"] = True
+                break
+
+            # back to the first frame if the video is finished
+            if int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)) == int(st.session_state['capture'].get(cv2.CAP_PROP_FRAME_COUNT)):
+                st.write("fps : ",int(st.session_state['capture'].get(cv2.CAP_PROP_FRAME_COUNT)))
+                st.write("cap : ",int(st.session_state["capture"].get(cv2.CAP_PROP_POS_FRAMES)))
 
+                st.session_state["capture"].set(cv2.CAP_PROP_POS_FRAMES, 0)
+                st.session_state["resume"] = True
+                break
 
-    if resume:
+    if st.session_state["resume"]:
         container_2.empty()
         pause = container_2.button('▶')
-        resume = False
+        st.session_state["resume"] = False
 
 def main():
 
-
-    video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?se=2023-07-11T11%3A34%3A13Z&sp=r&sv=2021-08-06&sr=b&sig=GW3M0UHASHtfWJ9wbHV5v7oDbreSv5F6ApGIRW6Ypz8%3D"
-    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989_global.json?sv=2021-10-04&st=2023-07-10T11%3A21%3A13Z&se=2023-07-18T11%3A21%3A00Z&sr=b&sp=r&sig=NvwsYEALxwRizyL2eOAsPxQbCV7SpywLVepv6S%2FNUiQ%3D"
+    video_path = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138.webm?sv=2021-10-04&st=2023-07-11T15%3A21%3A27Z&se=2023-07-26T15%3A21%3A00Z&sr=b&sp=r&sig=u6uuOUo9wvn5KJFNUnUR3axYtC815SUQBuDqNIC4L%2Bw%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/json-concat-files/1689004947.7068138_1689004953.7068138_global.json?sv=2021-10-04&st=2023-07-11T15%3A22%3A03Z&se=2023-07-26T15%3A22%3A00Z&sr=b&sp=r&sig=qSHWvDUIOOT%2F%2Bff270JVX7ucSRn5Lylgw5%2Fh9iTa4BY%3D"
     if video_path is not None:
         display_video(video_path, down_json)
 
 
-
 if __name__ == "__main__":
     main()
-
```

### Comparing `streamlitopencvplayer-1.3.3/test/test.py` & `streamlitopencvplayer-1.3.5/test/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 """Test script."""
 
 import argparse
 import uuid
 
 import streamlit as st
-from streamlitopencvplayer.app import display_video
 
+from streamlitopencvplayer.app import display_video
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
-if 'alerts' not in st.session_state:
-    st.session_state['alerts'] = []
-if 'data' not in st.session_state:
-    st.session_state['data'] = []
-if 'alerts_list' not in st.session_state:
-    st.session_state['alerts_list'] = []
-if 'name_vid_sel' not in st.session_state:
-    st.session_state['name_vid_sel'] = "1687441603.4032989_1687441609.4032989"
+
 
 class opencvplayer:
     """Class streamlit opencv player."""
 
-    def __init__(self, video_path, json_file):
+    def __init__(self, video_path, json_path):
         self.video_path = video_path
-        self.json_file = json_file
-
+        self.json_path = json_path
 
     def main(self):
         """Test function.
 
         Args:
-            video_path (required): video file path or video url.
-            json_file
+            video_path : video file path or video url.
+            json_path : Json file path or url.
+            alerts (Required when data is used) : List of alerts time
+            Json file elements :
+                guid (Optional) : unique ID
+                timestamp : required just when alerts are used
+                messageType (Optional) : message type is it an image(0), Log(1) or an Alert(2)
+                containerName (Optional)
+                data (Optional) : list of bounding box coordinates, score and class
 
         Returns:
             The video Player.
         """
         if self.video_path is not None:
-            return display_video(self.video_path, self.json_file)
+            return display_video(self.video_path, self.json_path)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Runnnig...")
     parser.add_argument(
         "--video-path",
         "-V",
         help="Enter the video path",
         default=str(uuid.uuid4().hex),
     )
-    parser.add_argument(
-        "--json-file",
-        "-J",
-        help="Enter the json file path",
-    )
+    parser.add_argument("--json-path",
+                        "-J",
+                        help="Json file path"
+                        )
+
     args = parser.parse_args()
     opencvplayer = opencvplayer(
-        args.video_path, args.json_file)
+        args.video_path, args.json_path)
     opencvplayer.main()
-
-'''
-    video_path = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989.webm?sp=r&st=2023-07-04T15:19:38Z&se=2023-07-06T23:19:38Z&spr=https&sv=2022-11-02&sr=b&sig=beK2pXlTRKEEPSEQ31sZjkpc%2FPtQU1vpDLUN4gvX2xQ%3D"
-    down_json = "https://cvlogger.blob.core.windows.net/jsonconcat/1687441603.4032989_1687441609.4032989_global.json?se=2023-07-05T20%3A24%3A12Z&sp=r&sv=2021-08-06&sr=b&sig=q0O120LhDaxSl63TIYOCcsKUeZDQ2ANwGV1rZT0bkPU%3D"
-'''
```

