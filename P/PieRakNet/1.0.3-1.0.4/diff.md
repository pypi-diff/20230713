# Comparing `tmp/PieRakNet-1.0.3.tar.gz` & `tmp/PieRakNet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieRakNet-1.0.3.tar", last modified: Fri Jul  7 09:15:55 2023, max compression
+gzip compressed data, was "PieRakNet-1.0.4.tar", last modified: Thu Jul 13 07:17:06 2023, max compression
```

## Comparing `PieRakNet-1.0.3.tar` & `PieRakNet-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 09:15:55.184651 PieRakNet-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      985 2023-07-07 09:15:55.178669 PieRakNet-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 09:15:54.772142 PieRakNet-1.0.3/PieRakNet.egg-info/
--rw-rw-rw-   0        0        0      985 2023-07-07 09:15:54.000000 PieRakNet-1.0.3/PieRakNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-07 09:15:54.000000 PieRakNet-1.0.3/PieRakNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 09:15:54.000000 PieRakNet-1.0.3/PieRakNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-07 09:15:54.000000 PieRakNet-1.0.3/PieRakNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 09:15:55.071951 PieRakNet-1.0.3/pieraknet/
--rw-rw-rw-   0        0        0      119 2023-07-07 07:59:21.000000 PieRakNet-1.0.3/pieraknet/__init__.py
--rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.3/pieraknet/buffer.py
--rw-rw-rw-   0        0        0    10384 2023-07-06 11:36:48.000000 PieRakNet-1.0.3/pieraknet/connection.py
--rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.3/pieraknet/protocol_info.py
--rw-rw-rw-   0        0        0     3695 2023-07-07 08:44:14.000000 PieRakNet-1.0.3/pieraknet/server.py
--rw-rw-rw-   0        0        0       42 2023-07-07 09:15:55.185649 PieRakNet-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-07-07 07:28:11.000000 PieRakNet-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:17:06.270688 PieRakNet-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      985 2023-07-13 07:17:06.267691 PieRakNet-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 07:17:02.760366 PieRakNet-1.0.4/PieRakNet.egg-info/
+-rw-rw-rw-   0        0        0      985 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 07:17:05.194071 PieRakNet-1.0.4/pieraknet/
+-rw-rw-rw-   0        0        0      119 2023-07-07 07:59:21.000000 PieRakNet-1.0.4/pieraknet/__init__.py
+-rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.4/pieraknet/buffer.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:36:48.000000 PieRakNet-1.0.4/pieraknet/connection.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:17:05.480377 PieRakNet-1.0.4/pieraknet/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 07:13:46.000000 PieRakNet-1.0.4/pieraknet/handlers/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-07-06 10:31:49.000000 PieRakNet-1.0.4/pieraknet/handlers/connection_request.py
+-rw-rw-rw-   0        0        0     1636 2023-07-04 11:31:23.000000 PieRakNet-1.0.4/pieraknet/handlers/offline_ping.py
+-rw-rw-rw-   0        0        0      473 2023-07-06 10:31:49.000000 PieRakNet-1.0.4/pieraknet/handlers/online_ping.py
+-rw-rw-rw-   0        0        0     2658 2023-07-04 12:22:51.000000 PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_1.py
+-rw-rw-rw-   0        0        0     1955 2023-07-06 10:40:18.000000 PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_2.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:17:06.263703 PieRakNet-1.0.4/pieraknet/packets/
+-rw-rw-rw-   0        0        0        0 2023-07-13 07:13:46.000000 PieRakNet-1.0.4/pieraknet/packets/__init__.py
+-rw-rw-rw-   0        0        0     2558 2023-07-04 10:50:56.000000 PieRakNet-1.0.4/pieraknet/packets/acknowledgement.py
+-rw-rw-rw-   0        0        0      462 2023-07-06 09:33:49.000000 PieRakNet-1.0.4/pieraknet/packets/connection_request.py
+-rw-rw-rw-   0        0        0      627 2023-07-06 09:49:21.000000 PieRakNet-1.0.4/pieraknet/packets/connection_request_accepted.py
+-rw-rw-rw-   0        0        0      130 2023-07-04 09:50:06.000000 PieRakNet-1.0.4/pieraknet/packets/disconnect.py
+-rw-rw-rw-   0        0        0     3245 2023-07-06 07:52:28.000000 PieRakNet-1.0.4/pieraknet/packets/frame_set.py
+-rw-rw-rw-   0        0        0      865 2023-07-06 10:03:10.000000 PieRakNet-1.0.4/pieraknet/packets/game_packet.py
+-rw-rw-rw-   0        0        0      403 2023-07-04 10:03:15.000000 PieRakNet-1.0.4/pieraknet/packets/incompatible_protocol.py
+-rw-rw-rw-   0        0        0      525 2023-07-06 09:26:49.000000 PieRakNet-1.0.4/pieraknet/packets/new_incoming_connection.py
+-rw-rw-rw-   0        0        0      391 2023-07-03 09:27:19.000000 PieRakNet-1.0.4/pieraknet/packets/offline_ping.py
+-rw-rw-rw-   0        0        0      719 2023-07-13 07:15:53.000000 PieRakNet-1.0.4/pieraknet/packets/offline_pong.py
+-rw-rw-rw-   0        0        0      331 2023-07-06 08:55:38.000000 PieRakNet-1.0.4/pieraknet/packets/online_ping.py
+-rw-rw-rw-   0        0        0      463 2023-07-06 08:55:38.000000 PieRakNet-1.0.4/pieraknet/packets/online_pong.py
+-rw-rw-rw-   0        0        0      487 2023-07-04 10:03:16.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_reply_1.py
+-rw-rw-rw-   0        0        0      612 2023-07-04 10:03:16.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_reply_2.py
+-rw-rw-rw-   0        0        0      419 2023-07-06 10:04:05.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_request_1.py
+-rw-rw-rw-   0        0        0      514 2023-07-04 09:44:42.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_request_2.py
+-rw-rw-rw-   0        0        0      548 2023-07-03 09:29:51.000000 PieRakNet-1.0.4/pieraknet/packets/packet.py
+-rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.4/pieraknet/protocol_info.py
+-rw-rw-rw-   0        0        0     3695 2023-07-07 08:44:14.000000 PieRakNet-1.0.4/pieraknet/server.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:17:06.270688 PieRakNet-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-07-13 07:12:27.000000 PieRakNet-1.0.4/setup.py
```

### Comparing `PieRakNet-1.0.3/LICENSE` & `PieRakNet-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.3/PKG-INFO` & `PieRakNet-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.3
+Version: 1.0.4
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.3/PieRakNet.egg-info/PKG-INFO` & `PieRakNet-1.0.4/PieRakNet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.3
+Version: 1.0.4
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.3/pieraknet/buffer.py` & `PieRakNet-1.0.4/pieraknet/buffer.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.3/pieraknet/connection.py` & `PieRakNet-1.0.4/pieraknet/connection.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.3/pieraknet/protocol_info.py` & `PieRakNet-1.0.4/pieraknet/protocol_info.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.3/pieraknet/server.py` & `PieRakNet-1.0.4/pieraknet/server.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.3/setup.py` & `PieRakNet-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='PieRakNet',
-    version='1.0.3',
+    version='1.0.4',
     author='lapismyt',
     author_email='nikitagavrilin005@gmail.com',
     description='RakNet implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieRakNet',
     packages=find_packages(),
```

