# Comparing `tmp/tellosync-0.0.8.tar.gz` & `tmp/tellosync-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tellosync-0.0.8.tar", last modified: Tue Jul 11 13:01:06 2023, max compression
+gzip compressed data, was "tellosync-0.1.0.tar", last modified: Thu Jul 13 02:53:53 2023, max compression
```

## Comparing `tellosync-0.0.8.tar` & `tellosync-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.351236 tellosync-0.0.8/
--rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2619 2023-07-11 13:01:06.343237 tellosync-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2041 2023-07-10 16:40:19.000000 tellosync-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 13:01:06.351236 tellosync-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-11 13:01:00.000000 tellosync-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.303367 tellosync-0.0.8/tellosync/
--rw-rw-rw-   0        0        0      275 2023-07-11 13:00:58.000000 tellosync-0.0.8/tellosync/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-07-10 16:48:37.000000 tellosync-0.0.8/tellosync/stats.py
--rw-rw-rw-   0        0        0     1072 2023-06-29 02:03:12.000000 tellosync-0.0.8/tellosync/synchro.py
--rw-rw-rw-   0        0        0     8453 2023-07-11 13:00:14.000000 tellosync-0.0.8/tellosync/tello.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:01:06.343237 tellosync-0.0.8/tellosync.egg-info/
--rw-rw-rw-   0        0        0     2619 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-11 13:01:06.000000 tellosync-0.0.8/tellosync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 02:53:53.945569 tellosync-0.1.0/
+-rw-rw-rw-   0        0        0     1070 2023-06-22 13:01:38.000000 tellosync-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2619 2023-07-13 02:53:53.944563 tellosync-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2041 2023-07-10 16:40:19.000000 tellosync-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 02:53:53.946570 tellosync-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-13 02:53:18.000000 tellosync-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 02:53:53.906582 tellosync-0.1.0/tellosync/
+-rw-rw-rw-   0        0        0      275 2023-07-13 02:53:11.000000 tellosync-0.1.0/tellosync/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-07-10 16:48:37.000000 tellosync-0.1.0/tellosync/stats.py
+-rw-rw-rw-   0        0        0     1544 2023-07-13 02:52:50.000000 tellosync-0.1.0/tellosync/synchro.py
+-rw-rw-rw-   0        0        0     8160 2023-07-13 02:52:50.000000 tellosync-0.1.0/tellosync/tello.py
+drwxrwxrwx   0        0        0        0 2023-07-13 02:53:53.942569 tellosync-0.1.0/tellosync.egg-info/
+-rw-rw-rw-   0        0        0     2619 2023-07-13 02:53:53.000000 tellosync-0.1.0/tellosync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-13 02:53:53.000000 tellosync-0.1.0/tellosync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 02:53:53.000000 tellosync-0.1.0/tellosync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-13 02:53:53.000000 tellosync-0.1.0/tellosync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 02:53:53.000000 tellosync-0.1.0/tellosync.egg-info/top_level.txt
```

### Comparing `tellosync-0.0.8/LICENSE` & `tellosync-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.8/PKG-INFO` & `tellosync-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.8
+Version: 0.1.0
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tellosync-0.0.8/README.md` & `tellosync-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.8/setup.py` & `tellosync-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tellosync',
-    version='0.0.8',
+    version='0.1.0',
     author='Ezra Fielding, Vincent Wu',
     author_email='ezra.fielding@gmail.com, vwu1888@gmail.com',
     description='An easy framework to support DJI Tello scripting in Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/vwu1888/easyTello',
     packages=setuptools.find_packages(),
```

### Comparing `tellosync-0.0.8/tellosync/stats.py` & `tellosync-0.1.0/tellosync/stats.py`

 * *Files identical despite different names*

### Comparing `tellosync-0.0.8/tellosync/synchro.py` & `tellosync-0.1.0/tellosync/synchro.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 import serial
 import time
+import platform
 
 class Synchro:
-    def __init__(self, port:int) -> None:
+    def __init__(self, port:int, numSynchros: int=0) -> None:
         self.ser = serial.Serial()
         self.ser.baudrate = 19200
         self.ser.timeout = 2.0
-        self.ser.port = f"COM{port}"
+        
+        match (platform.system()):
+            case "Windows":
+                self.ser.port = f"COM{port}"
+            case "Linux":
+                self.ser.port = f"/dev/ttyUSB{port}"
+            case "Darwin":
+                self.ser.port = f"/dev/tty.usbmodem{port}"
+            case _:
+                self.ser.port = f"COM{port}"
+
+        self.numSynchros = numSynchros
     
     def open(self) -> bool:
         try:
             self.ser.open()
             time.sleep(3.0)
             return True
         except serial.SerialException as e:
@@ -34,12 +46,14 @@
         self.ser.write(b"RESYNC")
     
     def start(self) -> None:
         self.ser.reset_input_buffer()
         self.ser.reset_output_buffer()
 
         self.ser.write(b"START")
+        time.sleep(1.0)
 
+        self.ser.write(str(self.numSynchros).encode("Ascii"))
         time.sleep(1.0)
     
     def finished(self) -> None:
         self.ser.write(b"FINISH")
```

### Comparing `tellosync-0.0.8/tellosync/tello.py` & `tellosync-0.1.0/tellosync/tello.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,252 @@
-import socket
-import threading
-import time
-import cv2
-from tellosync.stats import Stats
-from tellosync.synchro import Synchro
-
-class Tello:
-    def __init__(self, tello_ip: str='192.168.10.1', debug: bool=True, isSynced: bool=False, port: int=0):
-        # Opening local UDP port on 8889 for Tello communication
-        self.local_ip = ''
-        self.local_port = 8889
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.socket.bind((self.local_ip, self.local_port))
-        
-        # Setting Tello ip and port info
-        self.tello_ip = tello_ip
-        self.tello_port = 8889
-        self.tello_address = (self.tello_ip, self.tello_port)
-        self.log: list[Stats] = []
-
-        # Intializing response thread
-        self.receive_thread = threading.Thread(target=self._receive_thread)
-        self.receive_thread.daemon = True
-        self.receive_thread.start()
-
-        # easyTello runtime options
-        self.stream_state = False
-        self.last_frame = None
-        self.MAX_TIME_OUT = 15.0
-        self.debug = debug
-
-        self.isSynced = isSynced 
-        if isSynced:
-            self.synchro = Synchro(port)
-            self.isSynced = self.synchro.open()
-
-        # Setting Tello to command mode
-        self.command()
-
-    def send_command(self, command: str, delay: float=0.0, tries: int=0):
-        # New log entry created for the outbound command
-        self.log.append(Stats(command, len(self.log)))
-        currentStats = self.log[-1]
-
-        if delay > 0:
-            self.wait(delay)
-
-        # Sending command to Tello
-        self.socket.sendto(command.encode('utf-8'), self.tello_address)
-        # Displaying conformation message (if 'debug' os True)
-        if self.debug is True:
-            print(f'Sending command: {command}')
-
-        # Checking whether the command has timed out or not (based on value in 'MAX_TIME_OUT')
-        start = time.time()
-        while not currentStats.got_response():  # Runs while no repsonse has been received in log      
-            now = time.time()
-            difference = now - start
-            if difference > self.MAX_TIME_OUT:
-                currentStats.add_response('Connection timed out!')
-                break
-
-        # Prints out Tello response (if 'debug' is True)
-        if self.debug is True:
-            print(f'Response: {currentStats.get_response()}')
-
-        if currentStats.get_raw_response() == "error No valid imu" or currentStats.get_raw_response == "error Not joystick":
-            self.socket.sendto("stop".encode('utf-8'), self.tello_address)
-            time.sleep(1.0)
-
-        if delay < 0:
-            self.wait(abs(delay))
-
-        time.sleep(0.5)
-        self.wait_for_sync()
-
-    def _keep_alive(self):
-        # Sending command to Tello
-        print("Keeping connection alive")
-        self.socket.sendto("stop".encode('utf-8'), self.tello_address)
-
-    def _receive_thread(self):
-        while True:
-            # Checking for Tello response, throws socket error
-            try:
-                self.response, ip = self.socket.recvfrom(1024)
-                self.log[-1].add_response(self.response.decode('utf-8'))
-            except socket.error as exc:
-                print(f'Socket error: {exc}')
-
-            try:
-                self.log[-1].add_response(self.response.decode('utf-8'))
-            except UnicodeDecodeError as e:
-                self.log[-1].add_response("Response: utf-8 decode error")
-
-    def _video_thread(self):
-        # Creating stream capture object
-        cap = cv2.VideoCapture(f'udp://{self.tello_ip}:11111')
-        # Runs while 'stream_state' is True
-        while self.stream_state:
-            ret, self.last_frame = cap.read()
-            cv2.imshow('DJI Tello', self.last_frame)
-
-            # Video Stream is closed if escape key is pressed
-            k = cv2.waitKey(1) & 0xFF
-            if k == 27:
-                break
-        cap.release()
-        cv2.destroyAllWindows()
-    
-    def wait(self, delay: float):
-        if self.isSynced:
-            self.synchro.unsync()
-        # Displaying wait message (if 'debug' is True)
-        if self.debug:
-            print(f'Waiting {delay} seconds...')
-        # Log entry for delay added
-        self.log.append(Stats('wait', len(self.log)))
-
-        delay = abs(delay)
-        while delay > 0.0:
-            self._keep_alive()
-            delay = delay - 8.0 
-            if (delay < 0.0):
-                time.sleep(delay + 8.0)
-                continue
-            # Delay is activated
-            time.sleep(8.0)
-        if self.isSynced:
-            self.wait_for_sync()
-
-    def wait_for_sync(self):
-        # Syncs commands with other drones when using a synchronizer
-        if self.isSynced:
-            self.synchro.selfIsReady()
-            while not self.synchro.waitSync():
-                print("Waiting for other drones...")
-                self._keep_alive()
-        
-    def get_log(self):
-        return self.log
-    
-    def close(self):
-        self.socket.close()
-
-    # Controll Commands
-    def command(self):
-        if self.isSynced:
-            self.synchro.start()
-        self.send_command('command')
-    
-    def takeoff(self, delay: float=0.0):
-        self.send_command('takeoff', delay)
-
-    def land(self, delay: float=0.0):
-        if self.isSynced:
-            self.synchro.finished()
-            self.synchro.close()
-        self.send_command('land', delay)
-
-    def streamon(self):
-        self.send_command('streamon')
-        self.stream_state = True
-        self.video_thread = threading.Thread(target=self._video_thread)
-        self.video_thread.daemon = True
-        self.video_thread.start()
-
-    def streamoff(self):
-        self.stream_state = False
-        self.send_command('streamoff')
-
-    def emergency(self):
-        self.send_command('emergency')
-
-    def stop(self):
-        self.send_command('stop')
-    
-    # Movement Commands
-    def up(self, dist: int, delay: float=0.0):
-        self.send_command(f'up {dist}', delay)
-
-    def down(self, dist: int, delay: float=0.0):
-        self.send_command(f'down {dist}', delay)
-
-    def left(self, dist: int, delay: float=0.0):
-        self.send_command(f'left {dist}', delay)
-
-    def right(self, dist: int, delay: float=0.0):
-        self.send_command(f'right {dist}', delay)
-        
-    def forward(self, dist: int, delay: float=0.0):
-        self.send_command(f'forward {dist}', delay)
-
-    def back(self, dist: int, delay: float=0.0):
-        self.send_command(f'back {dist}', delay)
-
-    def cw(self, degr: int, delay: float=0.0):
-        self.send_command(f'cw {degr}', delay)
-    
-    def ccw(self, degr: int, delay: float=0.0):
-        self.send_command(f'ccw {degr}', delay)
-
-    def flip(self, direc: str, delay: float=0.0):
-        self.send_command(f'flip {direc}', delay)
-
-    def go(self, x: int, y: int, z: int, speed: int, delay: float=0.0):
-        self.send_command(f'go {x} {y} {z} {speed}', delay)
-
-    def curve(self, x1: int, y1: int, z1: int, x2: int, y2: int, z2: int, speed: int, delay: float=0.0):
-        self.send_command(f'curve {x1} {y1} {z1} {x2} {y2} {z2} {speed}', delay)
-
-    # Set Commands
-    def set_speed(self, speed: int):
-        self.send_command(f'speed {speed}')
-
-    def rc_control(self, a: int, b: int, c: int, d: int):
-        self.send_command(f'rc {a} {b} {c} {d}')
-
-    def set_wifi(self, ssid: str, passwrd: str):
-        self.send_command(f'wifi {ssid} {passwrd}')
-
-    # Read Commands
-    def get_speed(self):
-        self.send_command('speed?')
-
-    def get_battery(self):
-        self.send_command('battery?')
-
-    def get_time(self):
-        self.send_command('time?')
-
-    def get_height(self):
-        self.send_command('height?')
-    
-    def get_temp(self):
-        self.send_command('temp?')
-
-    def get_attitude(self):
-        self.send_command('attitude?')
-
-    def get_baro(self):
-        self.send_command('baro?')
-
-    def get_acceleration(self):
-        self.send_command('acceleration?')
-    
-    def get_tof(self):
-        self.send_command('tof?')
-
-    def get_wifi(self):
-        self.send_command('wifi?')
+import socket
+import threading
+import time
+import cv2
+from tellosync.stats import Stats
+from tellosync.synchro import Synchro
+
+class Tello:
+    def __init__(self, tello_ip: str='192.168.10.1', debug: bool=True, isSynced: bool=False, port: int=0, numSynchros: int=0):
+        # Opening local UDP port on 8889 for Tello communication
+        self.local_ip = ''
+        self.local_port = 8889
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self.socket.bind((self.local_ip, self.local_port))
+        
+        # Setting Tello ip and port info
+        self.tello_ip = tello_ip
+        self.tello_port = 8889
+        self.tello_address = (self.tello_ip, self.tello_port)
+        self.log: list[Stats] = []
+
+        # Intializing response thread
+        self.receive_thread = threading.Thread(target=self._receive_thread)
+        self.receive_thread.daemon = True
+        self.receive_thread.start()
+
+        # easyTello runtime options
+        self.stream_state = False
+        self.last_frame = None
+        self.MAX_TIME_OUT = 15.0
+        self.debug = debug
+
+        self.isSynced = isSynced 
+        if isSynced:
+            self.synchro = Synchro(port, numSynchros)
+            self.isSynced = self.synchro.open()
+
+        # Setting Tello to command mode
+        self.command()
+
+    def send_command(self, command: str, delay: float=0.0, tries: int=0):
+        # New log entry created for the outbound command
+        self.log.append(Stats(command, len(self.log)))
+        currentStats = self.log[-1]
+
+        if delay > 0:
+            self.wait(delay)
+
+        # Sending command to Tello
+        self.socket.sendto(command.encode('utf-8'), self.tello_address)
+        # Displaying conformation message (if 'debug' os True)
+        if self.debug is True:
+            print(f'Sending command: {command}')
+
+        # Checking whether the command has timed out or not (based on value in 'MAX_TIME_OUT')
+        start = time.time()
+        while not currentStats.got_response():  # Runs while no repsonse has been received in log      
+            now = time.time()
+            difference = now - start
+            if difference > self.MAX_TIME_OUT:
+                currentStats.add_response('Connection timed out!')
+                break
+
+        # Prints out Tello response (if 'debug' is True)
+        if self.debug is True:
+            print(f'Response: {currentStats.get_response()}')
+
+        if currentStats.get_raw_response() == "error No valid imu" or currentStats.get_raw_response == "error Not joystick":
+            self.socket.sendto("stop".encode('utf-8'), self.tello_address)
+            time.sleep(1.0)
+
+        if delay < 0:
+            self.wait(abs(delay))
+
+        time.sleep(0.5)
+        self.wait_for_sync()
+
+    def _keep_alive(self):
+        # Sending command to Tello
+        print("Keeping connection alive")
+        self.socket.sendto("stop".encode('utf-8'), self.tello_address)
+
+    def _receive_thread(self):
+        while True:
+            # Checking for Tello response, throws socket error
+            try:
+                self.response, ip = self.socket.recvfrom(1024)
+            except socket.error as exc:
+                print(f'Socket error: {exc}')
+
+            try:
+                self.log[-1].add_response(self.response.decode('utf-8'))
+            except UnicodeDecodeError as e:
+                self.log[-1].add_response("Response: utf-8 decode error")
+
+    def _video_thread(self):
+        # Creating stream capture object
+        cap = cv2.VideoCapture(f'udp://{self.tello_ip}:11111')
+        # Runs while 'stream_state' is True
+        while self.stream_state:
+            ret, self.last_frame = cap.read()
+            cv2.imshow('DJI Tello', self.last_frame)
+
+            # Video Stream is closed if escape key is pressed
+            k = cv2.waitKey(1) & 0xFF
+            if k == 27:
+                break
+        cap.release()
+        cv2.destroyAllWindows()
+    
+    def wait(self, delay: float):
+        if self.isSynced:
+            self.synchro.unsync()
+        # Displaying wait message (if 'debug' is True)
+        if self.debug:
+            print(f'Waiting {delay} seconds...')
+        # Log entry for delay added
+        self.log.append(Stats('wait', len(self.log)))
+
+        delay = abs(delay)
+        while delay > 0.0:
+            self._keep_alive()
+            delay = delay - 8.0 
+            if (delay < 0.0):
+                time.sleep(delay + 8.0)
+                continue
+            # Delay is activated
+            time.sleep(8.0)
+        if self.isSynced:
+            self.wait_for_sync()
+
+    def wait_for_sync(self):
+        # Syncs commands with other drones when using a synchronizer
+        if self.isSynced:
+            self.synchro.selfIsReady()
+            while not self.synchro.waitSync():
+                print("Waiting for other drones...")
+                self._keep_alive()
+        
+    def get_log(self):
+        return self.log
+    
+    def close(self):
+        self.socket.close()
+
+    # Controll Commands
+    def command(self):
+        if self.isSynced:
+            self.synchro.start()
+        self.send_command('command')
+    
+    def takeoff(self, delay: float=0.0):
+        self.send_command('takeoff', delay)
+
+    def land(self, delay: float=0.0):
+        if self.isSynced:
+            self.synchro.finished()
+            self.synchro.close()
+        self.send_command('land', delay)
+
+    def streamon(self):
+        self.send_command('streamon')
+        self.stream_state = True
+        self.video_thread = threading.Thread(target=self._video_thread)
+        self.video_thread.daemon = True
+        self.video_thread.start()
+
+    def streamoff(self):
+        self.stream_state = False
+        self.send_command('streamoff')
+
+    def emergency(self):
+        self.send_command('emergency')
+
+    def stop(self):
+        self.send_command('stop')
+    
+    # Movement Commands
+    def up(self, dist: int, delay: float=0.0):
+        self.send_command(f'up {dist}', delay)
+
+    def down(self, dist: int, delay: float=0.0):
+        self.send_command(f'down {dist}', delay)
+
+    def left(self, dist: int, delay: float=0.0):
+        self.send_command(f'left {dist}', delay)
+
+    def right(self, dist: int, delay: float=0.0):
+        self.send_command(f'right {dist}', delay)
+        
+    def forward(self, dist: int, delay: float=0.0):
+        self.send_command(f'forward {dist}', delay)
+
+    def back(self, dist: int, delay: float=0.0):
+        self.send_command(f'back {dist}', delay)
+
+    def cw(self, degr: int, delay: float=0.0):
+        self.send_command(f'cw {degr}', delay)
+    
+    def ccw(self, degr: int, delay: float=0.0):
+        self.send_command(f'ccw {degr}', delay)
+
+    def flip(self, direc: str, delay: float=0.0):
+        self.send_command(f'flip {direc}', delay)
+
+    def go(self, x: int, y: int, z: int, speed: int, delay: float=0.0):
+        self.send_command(f'go {x} {y} {z} {speed}', delay)
+
+    def curve(self, x1: int, y1: int, z1: int, x2: int, y2: int, z2: int, speed: int, delay: float=0.0):
+        self.send_command(f'curve {x1} {y1} {z1} {x2} {y2} {z2} {speed}', delay)
+
+    # Set Commands
+    def set_speed(self, speed: int):
+        self.send_command(f'speed {speed}')
+
+    def rc_control(self, a: int, b: int, c: int, d: int):
+        self.send_command(f'rc {a} {b} {c} {d}')
+
+    def set_wifi(self, ssid: str, passwrd: str):
+        self.send_command(f'wifi {ssid} {passwrd}')
+
+    # Read Commands
+    def get_speed(self):
+        self.send_command('speed?')
+
+    def get_battery(self):
+        self.send_command('battery?')
+
+    def get_time(self):
+        self.send_command('time?')
+
+    def get_height(self):
+        self.send_command('height?')
+    
+    def get_temp(self):
+        self.send_command('temp?')
+
+    def get_attitude(self):
+        self.send_command('attitude?')
+
+    def get_baro(self):
+        self.send_command('baro?')
+
+    def get_acceleration(self):
+        self.send_command('acceleration?')
+    
+    def get_tof(self):
+        self.send_command('tof?')
+
+    def get_wifi(self):
+        self.send_command('wifi?')
```

### Comparing `tellosync-0.0.8/tellosync.egg-info/PKG-INFO` & `tellosync-0.1.0/tellosync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tellosync
-Version: 0.0.8
+Version: 0.1.0
 Summary: An easy framework to support DJI Tello scripting in Python 3
 Home-page: https://github.com/vwu1888/easyTello
 Author: Ezra Fielding, Vincent Wu
 Author-email: ezra.fielding@gmail.com, vwu1888@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

