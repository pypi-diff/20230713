# Comparing `tmp/sac_tello-0.0.8.tar.gz` & `tmp/sac_tello-0.0.9.tar.gz`

## Comparing `sac_tello-0.0.8.tar` & `sac_tello-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/SAC-Tello.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0    13779 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/dictionaries/Michael.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/face_encoder.py
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_cmd.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_drive.py
--rw-r--r--   0        0        0    11777 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_drone.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_face_hud.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_hud.py
--rw-r--r--   0        0        0    10953 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_rc.py
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_remote.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_state.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 sac_tello-0.0.8/sac_tello/tello_video.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.8/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.8/LICENSE
--rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 sac_tello-0.0.8/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    48264 2020-02-02 00:00:00.000000 sac_tello-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/SAC-Tello.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    14555 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/workspace.xml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/dictionaries/Michael.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/__init__.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/face_encoder.py
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_cmd.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_drive.py
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_drone.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_face_hud.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_hud.py
+-rw-r--r--   0        0        0    11207 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_rc.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_remote.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_state.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 sac_tello-0.0.9/sac_tello/tello_video.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 sac_tello-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sac_tello-0.0.9/LICENSE
+-rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 sac_tello-0.0.9/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 sac_tello-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    48264 2020-02-02 00:00:00.000000 sac_tello-0.0.9/PKG-INFO
```

### Comparing `sac_tello-0.0.8/.idea/workspace.xml` & `sac_tello-0.0.9/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `sac_tello-0.0.8/.idea/workspace.xml` & `sac_tello-0.0.9/.idea/workspace.xml`

```diff
@@ -1,13 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="232f03d1-54a9-425b-9ce0-d606395cbea5" name="Changes" comment="Emergency fixes and some speed improvements">
       <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sac_tello/tello_drone.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_drone.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sac_tello/tello_rc.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_rc.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sac_tello/tello_remote.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_remote.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sac_tello/tello_state.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_state.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/sac_tello/tello_video.py" beforeDir="false" afterPath="$PROJECT_DIR$/sac_tello/tello_video.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
```

### Comparing `sac_tello-0.0.8/sac_tello/face_encoder.py` & `sac_tello-0.0.9/sac_tello/face_encoder.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/sac_tello/tello_cmd.py` & `sac_tello-0.0.9/sac_tello/tello_cmd.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/sac_tello/tello_drive.py` & `sac_tello-0.0.9/sac_tello/tello_drive.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/sac_tello/tello_drone.py` & `sac_tello-0.0.9/sac_tello/tello_drone.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,26 +102,32 @@
     # Precond:
     #   None.
     #
     # Postcond:
     #   Closes down communication with the drone and writes the log to a file.
     def close(self):
         self.running = False
-        self.cmd_thread.join()
-        self.state_thread.join()
-        self.video_thread.join()
-        self.video_haltQ.put("halt")
-        TelloDrone.__clear_q(self.video_recQ)
-        self.video_process.join()
-        self.state_haltQ.put("halt")
-        TelloDrone.__clear_q(self.state_recQ)
-        self.state_process.join()
-        self.cmdQ.put("halt")
-        TelloDrone.__clear_q(self.cmd_confQ)
-        self.cmd_process.join()
+        if self.cmd_thread.is_alive():
+            self.cmd_thread.join()
+        if self.state_thread.is_alive():
+            self.state_thread.join()
+        if self.video_thread.is_alive():
+            self.video_thread.join()
+        if self.video_process.is_alive():
+            self.video_haltQ.put("halt")
+            TelloDrone.__clear_q(self.video_recQ)
+            self.video_process.join()
+        if self.state_process.is_alive():
+            self.state_haltQ.put("halt")
+            TelloDrone.__clear_q(self.state_recQ)
+            self.state_process.join()
+        if self.cmd_process.is_alive():
+            self.cmdQ.put("halt")
+            TelloDrone.__clear_q(self.cmd_confQ)
+            self.cmd_process.join()
         
     # Precond:
     #   None.
     #
     # Postcond:
     #   Waits until all commands are complete.
     def complete(self):
```

### Comparing `sac_tello-0.0.8/sac_tello/tello_face_hud.py` & `sac_tello-0.0.9/sac_tello/tello_face_hud.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/sac_tello/tello_hud.py` & `sac_tello-0.0.9/sac_tello/tello_hud.py`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/sac_tello/tello_rc.py` & `sac_tello-0.0.9/sac_tello/tello_rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,25 +145,30 @@
     # Precond:
     #   None.
     #
     # Postcond:
     #   Closes down communication with the drone and writes the log to a file.
     def close(self):
         self.running = False
-        self.state_thread.join()
-        self.video_thread.join()
-        self.video_haltQ.put("halt")
-        TelloRC.__clear_q(self.video_recQ)
-        self.video_process.join()
-        self.state_haltQ.put("halt")
-        TelloRC.__clear_q(self.state_recQ)
-        self.state_process.join()
-        self.rcQ.put("halt")
-        TelloRC.__clear_q(self.rc_confQ)
-        self.rc_process.join()
+        if self.state_thread.is_alive():
+            self.state_thread.join()
+        if self.video_thread.is_alive():
+            self.video_thread.join()
+        if self.video_process.is_alive():
+            self.video_haltQ.put("halt")
+            TelloRC.__clear_q(self.video_recQ)
+            self.video_process.join()
+        if self.state_process.is_alive():
+            self.state_haltQ.put("halt")
+            TelloRC.__clear_q(self.state_recQ)
+            self.state_process.join()
+        if self.rc_process.is_alive():
+            self.rcQ.put("halt")
+            TelloRC.__clear_q(self.rc_confQ)
+            self.rc_process.join()
 
     # ======================================
     # COMMAND METHODS
     # ======================================
     # Section Notes:
     #   All commands check to see if the drone has been connected and put into SDK mode before sending commands.
```

### Comparing `sac_tello-0.0.8/sac_tello/tello_remote.py` & `sac_tello-0.0.9/sac_tello/tello_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,8 +353,11 @@
     #
     # Postcond:
     #   Sends RC messages to the tello based on internal throttle numbers.
     def __rc_beat(self):
         while not self.stop:
             if (perf_counter() - self.last_beat) > self.rc_tick and not self.waiting:
                 cmd = 'rc ' + ' '.join(map(str, self.rc))
-                self.__send_nowait(cmd)
+                self.__send_nowait(cmd)
+                
+if __name__ == '__main__':
+    mp.freeze_support()
```

### Comparing `sac_tello-0.0.8/sac_tello/tello_state.py` & `sac_tello-0.0.9/sac_tello/tello_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,8 +129,12 @@
                     label, val = item.split(':')
                     state[label] = val
                 state_time = perf_counter() - self.mission_start
                 self.state_log.append((state, state_time))
             except OSError as exc:
                 if not self.stop:
                     print("Caught exception socket.error : %s" % exc)
-                    
+                    
+                    
+if __name__ == '__main__':
+    mp.freeze_support()
+
```

### Comparing `sac_tello-0.0.8/sac_tello/tello_video.py` & `sac_tello-0.0.9/sac_tello/tello_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,8 +111,13 @@
     def __receive(self):
         while self.stream_active:
             ret, img = self.video_stream.read()
             if ret:
                 self.last_frame = (img, self.frame_width, self.frame_height)
                 self.frame_update = True
         self.video_stream.release()
-        cv2.destroyAllWindows()
+        cv2.destroyAllWindows()
+        
+        
+if __name__ == '__main__':
+    mp.freeze_support()
+
```

### Comparing `sac_tello-0.0.8/.gitignore` & `sac_tello-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/LICENSE` & `sac_tello-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/README.md` & `sac_tello-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sac_tello-0.0.8/pyproject.toml` & `sac_tello-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "SAC-Tello"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Michael Huelsman", email="michael.huelsman@gmail.com" },
 ]
 description = "A Python-based DJI Tello interface which utilizes parallel processing."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

### Comparing `sac_tello-0.0.8/PKG-INFO` & `sac_tello-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAC-Tello
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python-based DJI Tello interface which utilizes parallel processing.
 Project-URL: Homepage, https://github.com/xLeachimx/SAC-Tello
 Project-URL: Bug Tracker, https://github.com/xLeachimx/SAC-Tello/issues
 Author-email: Michael Huelsman <michael.huelsman@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

