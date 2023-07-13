# Comparing `tmp/data_collect-0.8.8.tar.gz` & `tmp/data_collect-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_collect-0.8.8.tar", last modified: Thu Jun 15 02:32:29 2023, max compression
+gzip compressed data, was "data_collect-0.8.9.tar", last modified: Thu Jul 13 07:26:17 2023, max compression
```

## Comparing `data_collect-0.8.8.tar` & `data_collect-0.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.185801 data_collect-0.8.8/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-15 02:32:29.185896 data_collect-0.8.8/PKG-INFO
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.183364 data_collect-0.8.8/data_collect/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)    12756 2023-06-15 02:29:17.000000 data_collect-0.8.8/data_collect/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      283 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/correlation_id.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.185309 data_collect-0.8.8/data_collect/data_types/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/data_types/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-14 19:41:14.000000 data_collect-0.8.8/data_collect/data_types/blob.py
--rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-14 19:39:14.000000 data_collect-0.8.8/data_collect/data_types/image.py
--rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-14 19:28:54.000000 data_collect-0.8.8/data_collect/data_types/text.py
--rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-14 19:39:04.000000 data_collect-0.8.8/data_collect/logger.py
--rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-05-08 13:37:11.000000 data_collect-0.8.8/data_collect/queue.py
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-04-12 08:56:34.000000 data_collect-0.8.8/data_collect/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-05-08 13:37:11.000000 data_collect-0.8.8/data_collect/thread.py
--rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-04-11 15:51:48.000000 data_collect-0.8.8/data_collect/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-15 02:32:29.184363 data_collect-0.8.8/data_collect.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      582 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)       75 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       13 2023-06-15 02:32:29.000000 data_collect-0.8.8/data_collect.egg-info/top_level.txt
--rw-r--r--   0 jojo       (501) staff       (20)      720 2023-06-15 02:32:29.186327 data_collect-0.8.8/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      179 2023-06-15 02:32:28.000000 data_collect-0.8.8/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 07:26:17.288180 data_collect-0.8.9/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-07-13 07:26:17.288287 data_collect-0.8.9/PKG-INFO
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 07:26:17.286195 data_collect-0.8.9/data_collect/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)    12925 2023-07-13 07:25:57.000000 data_collect-0.8.9/data_collect/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1097 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      283 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/correlation_id.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 07:26:17.288026 data_collect-0.8.9/data_collect/data_types/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/data_types/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-06-19 17:19:03.000000 data_collect-0.8.9/data_collect/data_types/blob.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3426 2023-06-19 17:19:03.000000 data_collect-0.8.9/data_collect/data_types/image.py
+-rw-r--r--   0 jojo       (501) staff       (20)      388 2023-06-19 17:19:03.000000 data_collect-0.8.9/data_collect/data_types/text.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7416 2023-06-19 17:19:03.000000 data_collect-0.8.9/data_collect/logger.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5564 2023-06-19 17:18:59.000000 data_collect-0.8.9/data_collect/queue.py
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6629 2023-06-19 17:18:59.000000 data_collect-0.8.9/data_collect/thread.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1108 2023-05-10 19:20:29.000000 data_collect-0.8.9/data_collect/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 07:26:17.287420 data_collect-0.8.9/data_collect.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      535 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      582 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       75 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       13 2023-07-13 07:26:17.000000 data_collect-0.8.9/data_collect.egg-info/top_level.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      720 2023-07-13 07:26:17.288696 data_collect-0.8.9/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      179 2023-07-13 07:26:16.000000 data_collect-0.8.9/setup.py
```

### Comparing `data_collect-0.8.8/PKG-INFO` & `data_collect-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_collect
-Version: 0.8.8
+Version: 0.8.9
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.8/data_collect/client.py` & `data_collect-0.8.9/data_collect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
     log_path: str = ''
     blob_path: str = ''
     input_enable: bool = True
     prediction_enable: bool = True
     ground_truth_enable: bool = True
     max_workers: int = 1
 
+    class Config:
+        """Config model config"""
+        protected_namespaces = ()
+
 
 class DataCollectClient:
     """
     DataCollectClient
     """
 
     def __init__(self, config):
@@ -113,15 +117,15 @@
         file_name = correlation_id
         if metadata.get('sub_name'):
             file_name = f'{file_name}_{metadata.get("sub_name")}'
         file_path = f"{dir_name}/{file_name}"
         # validate content type and set file extension
         content_type = metadata.get('content_type', 'image/jpeg')
         if content_type is not None and content_type not in CV2_IMWRITE_VALID_CONTENT_TYPE:
-            content_type = 'image/jpeg' # default content type .jpeg
+            content_type = 'image/jpeg'  # default content type .jpeg
         ext = mimetypes.guess_extension(content_type)
         file_path += ext
         return file_path
 
     def _gen_default_message(self, correlation_id: str) -> {}:
         """
         generate default message
@@ -160,15 +164,16 @@
         :param time_series: 时间序列，本期未支持
         :param prediction: 模型预测结果
         :param ground_truth: ground truth 本期未支持
         :param config: DataCollectConfig 支持在log时重新执行DataCollectConfig
         :return:
         """
         if prediction is not None:
-            assert isinstance(prediction, (dict, list, str)), "prediction must be a dict, list, or str"
+            assert isinstance(prediction, (dict, list, str)
+                              ), "prediction must be a dict, list, or str"
 
         if config is not None:
             self._load_env_setting_and_config(config)
             self._init_base_logger()
 
         message = None
 
@@ -197,29 +202,30 @@
             message['ground_truth'] = ground_truth if isinstance(ground_truth, str) else json.dumps(ground_truth,
                                                                                                     cls=NpEncoder)
         if image is not None and self.input_enable:
             self._log_image(correlation_id, image, designation)
 
         if blob is not None and self._is_data_capture_enable():
             self._log_blob(correlation_id, blob, designation)
-        
+
         if blob_paths is not None and self._is_data_capture_enable():
             message['blob_paths'] = blob_paths
-            
+
         if self._is_data_capture_enable() and message is not None:
             self._logger.log(message)
 
     def _load_env_setting_and_config(self, config: DataCollectConfig):
         """
         load env setting and config
         :param config:
         :return:
         """
         # config优先级高于env
-        self.model_name = config.model_name if len(config.model_name) > 0 else get_model_name()
+        self.model_name = config.model_name if len(
+            config.model_name) > 0 else get_model_name()
 
         self.log_path = os.environ.get(CAPTURE_LOG_DIR).rstrip("/") if os.environ.get(
             CAPTURE_LOG_DIR) is not None else DEFAULT_CAPTURE_LOG_DIR
         if len(config.log_path) > 0:
             self.log_path = config.log_path.rstrip("/")
 
         self.blob_path = os.environ.get(CAPTURE_BLOB_DIR).rstrip("/") if os.environ.get(
@@ -227,19 +233,21 @@
         if len(config.blob_path) > 0:
             self.blob_path = config.blob_path.rstrip("/")
 
         self.input_enable = os.environ.get(ENABLE_CAPTURE_INPUT) == "True"
         if config.input_enable is not None:
             self.input_enable = config.input_enable
 
-        self.prediction_enable = os.environ.get(ENABLE_CAPTURE_PREDICTION) == "True"
+        self.prediction_enable = os.environ.get(
+            ENABLE_CAPTURE_PREDICTION) == "True"
         if config.prediction_enable is not None:
             self.prediction_enable = config.prediction_enable
 
-        self.ground_truth_enable = os.environ.get(ENABLE_CAPTURE_GROUND_TRUTH) == "True"
+        self.ground_truth_enable = os.environ.get(
+            ENABLE_CAPTURE_GROUND_TRUTH) == "True"
         if config.ground_truth_enable is not None:
             self.ground_truth_enable = config.ground_truth_enable
 
         self.log_rotation = os.environ.get(CAPTURE_LOG_ROTATION) if os.environ.get(
             CAPTURE_LOG_ROTATION) is not None else DEFAULT_CAPTURE_LOG_ROTATION
 
         self.log_retention = int(os.environ.get(CAPTURE_LOG_RETENTION)) if os.environ.get(
@@ -284,20 +292,22 @@
                     - H x W x 4 (an RGBA channel order is assumed)
 
         :param correlation_id: Correlation ID of the image.
         :param image: Image to log.
         :param designation: Designation of the image.
         """
         if image.designation is None:
-            image.designation = self.gen_image_save_path(correlation_id, designation, image.metadata)
+            image.designation = self.gen_image_save_path(
+                correlation_id, designation, image.metadata)
         self._image_logger.log(image)
 
     def _log_blob(self, correlation_id: str, blob: WindmillBlob, designation: str = ''):
         if blob.designation is None:
-            blob.designation = self.gen_blob_save_path(correlation_id, designation, blob.metadata)
+            blob.designation = self.gen_blob_save_path(
+                correlation_id, designation, blob.metadata)
         self._blob_logger.log(blob)
 
     def gen_blob_save_path(self, correlation_id: str, designation: str = '', metadata=None) -> str:
         """
         generate blob save path
         :param correlation_id:
         :return:
@@ -313,12 +323,12 @@
             if metadata is not None else "application/octet-stream"
         ext = mimetypes.guess_extension(content_type)
         extension = ext if ext is not None else "bin"
         file_name = correlation_id
         if metadata.get('sub_name'):
             file_name = f"{file_name}_{metadata.get('sub_name')}"
         return f"{dir_name}/{file_name}{extension}"
-    
+
     def close(self):
         self._logger.close()
         self._image_logger.close()
-        self._blob_logger.close()
+        self._blob_logger.close()
```

### Comparing `data_collect-0.8.8/data_collect/constants.py` & `data_collect-0.8.9/data_collect/constants.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/data_types/blob.py` & `data_collect-0.8.9/data_collect/data_types/blob.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/data_types/image.py` & `data_collect-0.8.9/data_collect/data_types/image.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/logger.py` & `data_collect-0.8.9/data_collect/logger.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/queue.py` & `data_collect-0.8.9/data_collect/queue.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/thread.py` & `data_collect-0.8.9/data_collect/thread.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect/utils.py` & `data_collect-0.8.9/data_collect/utils.py`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/data_collect.egg-info/PKG-INFO` & `data_collect-0.8.9/data_collect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-collect
-Version: 0.8.8
+Version: 0.8.9
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `data_collect-0.8.8/data_collect.egg-info/SOURCES.txt` & `data_collect-0.8.9/data_collect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_collect-0.8.8/setup.cfg` & `data_collect-0.8.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = data_collect
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.8.8
+version = 0.8.9
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

