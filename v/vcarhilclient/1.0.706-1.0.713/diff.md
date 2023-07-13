# Comparing `tmp/vcarhilclient-1.0.706.tar.gz` & `tmp/vcarhilclient-1.0.713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.706.tar", last modified: Wed Jul  5 10:04:05 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.713.tar", last modified: Thu Jul 13 06:04:43 2023, max compression
```

## Comparing `vcarhilclient-1.0.706.tar` & `vcarhilclient-1.0.713.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.855490 vcarhilclient-1.0.706/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.706/LICENSE
--rw-rw-rw-   0        0        0     2596 2023-07-05 10:04:05.855490 vcarhilclient-1.0.706/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.706/README.md
--rw-rw-rw-   0        0        0       86 2023-07-05 10:04:05.856486 vcarhilclient-1.0.706/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-07-05 10:03:33.000000 vcarhilclient-1.0.706/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.838337 vcarhilclient-1.0.706/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.706/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.706/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.706/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50918 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    14192 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.706/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2383 2023-07-05 09:39:43.000000 vcarhilclient-1.0.706/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.706/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-07-05 10:04:05.852970 vcarhilclient-1.0.706/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2596 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-05 10:04:05.000000 vcarhilclient-1.0.706/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 06:04:43.942643 vcarhilclient-1.0.713/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.713/LICENSE
+-rw-rw-rw-   0        0        0     2596 2023-07-13 06:04:43.943639 vcarhilclient-1.0.713/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.713/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-13 06:04:43.944701 vcarhilclient-1.0.713/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-07-13 06:01:12.000000 vcarhilclient-1.0.713/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:04:43.932687 vcarhilclient-1.0.713/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.713/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.713/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.713/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.713/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50423 2023-07-13 05:59:17.000000 vcarhilclient-1.0.713/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.713/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    14192 2023-07-05 09:39:43.000000 vcarhilclient-1.0.713/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.713/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2383 2023-07-05 09:39:43.000000 vcarhilclient-1.0.713/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.713/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:04:43.941646 vcarhilclient-1.0.713/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2596 2023-07-13 06:04:43.000000 vcarhilclient-1.0.713/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-13 06:04:43.000000 vcarhilclient-1.0.713/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:04:43.000000 vcarhilclient-1.0.713/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-13 06:04:43.000000 vcarhilclient-1.0.713/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-13 06:04:43.000000 vcarhilclient-1.0.713/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.706/LICENSE` & `vcarhilclient-1.0.713/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/PKG-INFO` & `vcarhilclient-1.0.713/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.706
+Version: 1.0.713
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vcarhilclient-1.0.706/README.md` & `vcarhilclient-1.0.713/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/setup.py` & `vcarhilclient-1.0.713/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.706",
+    version="1.0.713",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.706/vcarhilclient/Enums.py` & `vcarhilclient-1.0.713/vcarhilclient/Enums.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.713/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.713/vcarhilclient/kunyi_mrt.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         arr = bytearray(512)
         char_array = c_char * len(arr)
         buf_c = char_array.from_buffer(arr)
         size_pointer = pointer(c_int32(512))
         mrt_lib.mrt_get_enviroment_name.argtypes = [c_void_p, c_uint32, c_char_p, POINTER(c_int32)]
         mrt_lib.mrt_get_enviroment_name.restype = mrt_status_t
         error_code = mrt_lib.mrt_get_enviroment_name(self.context, idx, buf_c, size_pointer)
-        return error_code, buf_c.value.decode('utf-8')
+        return error_code, buf_c.value.decode('utf-8', errors='ignore')
 
     @staticmethod
     def call_back(error_code, current_process, total_process):
         if error_code.value != 0:
             mrt_client.dispatch_progress = 100
         if float(total_process) != 0:
             mrt_client.dispatch_progress = float(current_process) / float(total_process)
@@ -683,22 +683,14 @@
             mrt_lib.mrt_daq_read.argtypes = [c_void_p, c_char_p, c_uint64, POINTER(POINTER(None))]
             mrt_lib.mrt_daq_read.restype = c_int32
             buf_size = mrt_lib.mrt_daq_read(self.context, en_pointer, c_uint64(daq_handle), msg_pp)
             if buf_size == 0:
                 print(f"The experimental environment({env_name}) Is Starting:{buf_size}")
                 return msg_list
             elif buf_size == -6:
-                with open("./readErro.erro", "a") as f:
-                    try:
-                        self.log_write(3,f"{env_name}",f"{time.strftime('%m%d_%H:%M:%S')}:daqhandle>>{daq_handle},"
-                                                 f"{env_name}>>MRT_ERR_RPC_CALL_FAIL -6\n")
-                    except:
-                        pass
-                    f.write(f"{time.strftime('%m%d_%H:%M:%S')}:daqhandle>>{daq_handle},{env_name}>>MRT_ERR_RPC_CALL_FAIL -6\n")
-                    f.flush()
                 raise Exception("MRT_ERR_RPC_CALL_FAIL -6")
             elif buf_size < 0:
                 with open("./readErro.erro", "a") as f:
                     try:
                         self.log_write(3, f"{env_name}",f"Experiment environment:daqhandle>>{daq_handle},{env_name} "
                                                   f">>error code:{buf_size}\n")
                     except:
```

### Comparing `vcarhilclient-1.0.706/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.713/vcarhilclient/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.713/vcarhilclient/kunyi_util.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.713/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.713/vcarhilclient/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.713/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.706/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.713/vcarhilclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.706
+Version: 1.0.713
 Summary: vcarhilclient
 Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

