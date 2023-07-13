# Comparing `tmp/taichu-storage-0.0.8.tar.gz` & `tmp/taichu-storage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-storage-0.0.8.tar", last modified: Tue Jul 11 10:55:58 2023, max compression
+gzip compressed data, was "taichu-storage-0.0.9.tar", last modified: Wed Jul 12 01:12:00 2023, max compression
```

## Comparing `taichu-storage-0.0.8.tar` & `taichu-storage-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:55:58.792700 taichu-storage-0.0.8/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:55:58.792389 taichu-storage-0.0.8/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-11 10:55:58.792802 taichu-storage-0.0.8/setup.cfg
--rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/setup.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:55:58.790182 taichu-storage-0.0.8/taichu_storage/
--rw-r--r--   0 wangkun    (501) staff       (20)     2597 2023-07-11 09:19:04.000000 taichu-storage-0.0.8/taichu_storage/__init__.py
--rw-r--r--   0 wangkun    (501) staff       (20)     5005 2023-07-11 09:39:29.000000 taichu-storage-0.0.8/taichu_storage/b3.py
--rw-r--r--   0 wangkun    (501) staff       (20)     3167 2023-07-11 09:19:04.000000 taichu-storage-0.0.8/taichu_storage/boto_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1116 2023-06-14 01:52:14.000000 taichu-storage-0.0.8/taichu_storage/env.py
--rw-r--r--   0 wangkun    (501) staff       (20)     2640 2023-07-11 01:58:58.000000 taichu-storage-0.0.8/taichu_storage/minio_client.py
--rw-r--r--   0 wangkun    (501) staff       (20)     1643 2023-07-11 09:19:04.000000 taichu-storage-0.0.8/taichu_storage/obs.py
-drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-11 10:55:58.792030 taichu-storage-0.0.8/taichu_storage.egg-info/
--rw-r--r--   0 wangkun    (501) staff       (20)      244 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/taichu_storage.egg-info/PKG-INFO
--rw-r--r--   0 wangkun    (501) staff       (20)      350 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/taichu_storage.egg-info/SOURCES.txt
--rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/taichu_storage.egg-info/dependency_links.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       76 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/taichu_storage.egg-info/requires.txt
--rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-11 10:55:58.000000 taichu-storage-0.0.8/taichu_storage.egg-info/top_level.txt
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-12 01:12:00.091796 taichu-storage-0.0.9/
+-rw-r--r--   0 wangkun    (501) staff       (20)      255 2023-07-12 01:12:00.091385 taichu-storage-0.0.9/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-07-12 01:12:00.091950 taichu-storage-0.0.9/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      757 2023-07-12 01:11:59.000000 taichu-storage-0.0.9/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-12 01:12:00.089052 taichu-storage-0.0.9/taichu_storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)     2591 2023-07-12 00:53:24.000000 taichu-storage-0.0.9/taichu_storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     4719 2023-07-12 01:04:52.000000 taichu-storage-0.0.9/taichu_storage/b3.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     3621 2023-07-12 01:03:11.000000 taichu-storage-0.0.9/taichu_storage/boto_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     2499 2023-07-12 01:09:26.000000 taichu-storage-0.0.9/taichu_storage/minio_client.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1610 2023-07-12 01:04:52.000000 taichu-storage-0.0.9/taichu_storage/obs.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-07-12 01:12:00.090842 taichu-storage-0.0.9/taichu_storage.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      255 2023-07-12 01:12:00.000000 taichu-storage-0.0.9/taichu_storage.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      328 2023-07-12 01:12:00.000000 taichu-storage-0.0.9/taichu_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-07-12 01:12:00.000000 taichu-storage-0.0.9/taichu_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       76 2023-07-12 01:12:00.000000 taichu-storage-0.0.9/taichu_storage.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       15 2023-07-12 01:12:00.000000 taichu-storage-0.0.9/taichu_storage.egg-info/top_level.txt
```

### Comparing `taichu-storage-0.0.8/setup.py` & `taichu-storage-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     long_description = 'storage sdks aggregation'
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='0.0.8',
+        version='0.0.9',
         description='storage sdks aggregation',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-storage-0.0.8/taichu_storage/__init__.py` & `taichu-storage-0.0.9/taichu_storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,9 +82,9 @@
     if protocol == Protocol.OBS:
         from taichu_storage.obs import StorageObs
         return StorageObs(cfgs)
     if protocol == Protocol.BOTO3:
         from taichu_storage.b3 import StorageBoto3
         return StorageBoto3(cfgs)
     else:
-        from taichu_storage.boto_client import StorageAlluxio
-        return StorageAlluxio()
+        from taichu_storage.boto_client import StorageBoto
+        return StorageBoto()
```

### Comparing `taichu-storage-0.0.8/taichu_storage/b3.py` & `taichu-storage-0.0.9/taichu_storage/b3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 import boto3
 import botocore.exceptions
 from botocore.config import Config
 
 from taichu_storage import StorageInterface
-from taichu_storage.env import *
+import os
 
 
 class StorageBoto3(StorageInterface):
     def __init__(self, cfgs=None):
         if cfgs is None:
             cfgs = {}
 
@@ -76,40 +76,36 @@
                 'get_object',
                 Params={'Bucket': self._bucket, 'Key': key},
                 ExpiresIn=expiration
             )
             if not host_url:
                 return url
             h = self._boto_host
-            if self._boto_port is not 80:
+            if self._boto_port != 80:
                 h = self._boto_host + ':' + str(self._boto_port)
             url = url.replace(h, host_url)
             print("URL_RETURN: ", url)
             return url
         except botocore.exceptions.ClientError as e:
             logging.error("Error generating presigned URL:", e)
             return None
 
     def generate_upload_credentials(self, key, expiration=3600):
         return self._client.generate_presigned_post(self._bucket, key, ExpiresIn=expiration)
-        # {'url': 'http://192.168.0.149:39999/api/v1/s3/publish-data', 'fields': {'key': 'sys/test/abc.txt',
+        # {'url': 'http://xxxx', 'fields': {'key': 'sys/test/abc.txt',
         # 'x-amz-algorithm': 'AWS4-HMAC-SHA256', 'x-amz-credential': 'root/20230704/cn/s3/aws4_request',
         # 'x-amz-date': '20230704T073038Z',
         # 'policy':
         # 'eyJleHBpcmF0aW9uIjogIjIwMjMtMDctMDRUMDg6MzA6MzhaIiwgImNvbmRpdGlvbnMiOiBbeyJidWNrZXQiOiAicHVibGlzaC1kYXRhIn0sIHsia2V5IjogInN5cy90ZXN0L2FiYy50eHQifSwgeyJ4LWFtei1hbGdvcml0aG0iOiAiQVdTNC1ITUFDLVNIQTI1NiJ9LCB7IngtYW16LWNyZWRlbnRpYWwiOiAicm9vdC8yMDIzMDcwNC9jbi9zMy9hd3M0X3JlcXVlc3QifSwgeyJ4LWFtei1kYXRlIjogIjIwMjMwNzA0VDA3MzAzOFoifV19',
         # 'x-amz-signature': 'accdd539815bb170132a109c1802630ab3bf1e582f7792e19d51100158cb5057'}}
 
 
 if __name__ == '__main__':
     c = StorageBoto3({
-        'bucket': 'publish-data',
-        'boto3_ak': 'root',
-        'boto3_sk': 'CBF5CCEC7425C19221F00D6A03B43B08',
-        'boto3_region_name': 'cn',
-        'boto3_endpoint_url': 'http://192.168.0.149:39999/api/v1/s3'
+
     })
     # c.write_string('abc', 'sys/test/abc.txt')
     # print(c.generate_signed_url('sys/test/abc.txt'))
     print(c.generate_upload_credentials('sys/test/abc.txt'))
     # c.write_json({'abc': "123"}, 'sys/test/json.json')
     # c.upload_file('test/b.txt', 'sys/test/b.txt')
     # c.upload_directory('test', 'sys/test/directory')
```

### Comparing `taichu-storage-0.0.8/taichu_storage/boto_client.py` & `taichu-storage-0.0.9/taichu_storage/minio_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,93 @@
+import io
 import logging
 
 from taichu_storage import StorageInterface
-import boto.s3.connection
-from taichu_storage.env import *
-import boto.exception
+from minio import Minio
+from io import BytesIO
 
 
-class StorageAlluxio(StorageInterface):
-    _boto_host = ''
-    _boto_port = ''
+class StorageMinio(StorageInterface):
+    _use_alluxio_path = True
 
     def __init__(self, cfgs=None):
         if cfgs is None:
             cfgs = {}
 
-        boto_ak = cfgs.get('boto_ak')
-        boto_sk = cfgs.get('boto_sk')
-        self._boto_host = cfgs.get('boto_host')
-        self._boto_port = cfgs.get('boto_port')
-        boto_path = cfgs.get('boto_path')
-        boto_bucket = cfgs.get('boto_bucket')
-
-        self._client = boto.connect_s3(
-            aws_access_key_id=boto_ak,
-            aws_secret_access_key=boto_sk,
-            host=self._boto_host,
-            port=self._boto_port,
-            path=boto_path,
-            is_secure=False,
-            calling_format=boto.s3.connection.OrdinaryCallingFormat(),
+        endpoint = cfgs.get('minio_endpoint')
+        ak = cfgs.get('minio_ak')
+        sk = cfgs.get('minio_sk')
+        self._bucket = cfgs.get('bucket')
+        self._use_alluxio_path = cfgs.get('use_alluxio_path', True)
+        print(self._use_alluxio_path, self._bucket)
+
+        self._client = Minio(
+            endpoint,
+            ak,
+            sk,
+            secure=False,
         )
-        self._bucket = self._client.get_bucket(boto_bucket)
+
+    def _prefix_key(self, key):
+        alluxio_path = 'data/%s/' % self._bucket
+        print('alluxio_path: %s' % alluxio_path)
+        if self._use_alluxio_path is False or key.startswith(alluxio_path):
+            k = key
+        else:
+            k = alluxio_path + key.lstrip('/')
+        print(k)
+        return k
+
+    def _alluxio_bucket(self):
+        return 'alluxio' if self._use_alluxio_path else self._bucket
 
     def write_bytes(self, content_bytes, key):
+        key = self._prefix_key(key)
+        # o = StrReader(content_bytes)
         try:
-            s3_key = self._bucket.new_key(key)
-            s3_key.set_contents_from_file(content_bytes)
-        except boto.exception.BotoClientError:
-            pass
+            self._client.put_object(
+                self._alluxio_bucket(),
+                key,
+                io.BytesIO(content_bytes),
+                len(content_bytes)
+            )
         except Exception as e:
-            logging.info("key: " + key)
-            logging.error("TaichuStorageError", e)
+            logging.error(e)
 
     def write_string(self, content_string, key):
-        try:
-            s3_key = self._bucket.new_key(key)
-            s3_key.set_contents_from_string(content_string)
-        except boto.exception.BotoClientError:
-            pass
-        except Exception as e:
-            logging.info("key: " + key)
-            logging.error("TaichuStorageError", e)
+        key = self._prefix_key(key)
+        return self.write_bytes(content_string.encode('utf-8'), key)
 
     def upload_file(self, file_path, key):
-        s3_key = self._bucket.new_key(key)
-        with open(file_path, "rb") as f:
-            try:
-                s3_key.set_contents_from_file(f)
-            except:
-                return
-
-    def download_dir(self, src, dest):
-        rps = self._bucket.list(prefix=src)
-        for r in rps:
-            os.makedirs(dest, exist_ok=True)
-            local_file = f'{dest}{r.name.replace(src, "")}'
-            try:
-                key = self._bucket.get_key(r.name)
-                with open(local_file, 'wb') as f:
-                    key.get_contents_to_file(f)
-            except Exception as e:
-                if 'SAXParseException' in str(type(e)):
-                    pass
-                else:
-                    logging.error(e)
-
-    def generate_signed_url(self, key, expiration=600, host_url=None):
+        key = self._prefix_key(key)
+        print(key)
         try:
-            k = self._bucket.get_key(key)
-            if k is None:
-                logging.info(key, "：不存在")
-                return key + "：不存在"
-            url = k.generate_url(expiration)
-            print("URL_ORIGIN: ", url)
-            if not host_url:
-                return url
-            h = self._boto_host
-            if self._boto_port is not 80:
-                h = self._boto_host + ':' + str(self._boto_port)
-            url = url.replace(h, host_url)
-            print("URL_RETURN: ", url)
-            return url
+            self._client.fput_object(
+                self._alluxio_bucket(),
+                key,
+                file_path
+            )
         except Exception as e:
             logging.error(e)
-            return None
+
+
+class StrReader:
+
+    def __init__(self, strs):
+        self.str = strs if isinstance(strs, bytes) else strs.encode('utf-8')
+
+    def read(self, n=-1):
+        return self.str
+
+    def len(self):
+        return len(self.str)
+
+
+if __name__ == '__main__':
+    c = StorageMinio({
+
+    })
+    c.write_string('abc', 'sys/test/abc.txt')
+    # c.write_bytes(b"hello", 'sys/test/abc_bytes.txt')
+    c.upload_file('test/b.txt', 'sys/test/b.txt')
+    # print(c.generate_signed_url('sys/test/abc.txt'))
+    # print(c.generate_upload_credentials('sys/test/abc.txt'))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `taichu-storage-0.0.8/taichu_storage/obs.py` & `taichu-storage-0.0.9/taichu_storage/obs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import logging
 
 from taichu_storage import StorageInterface
-from taichu_storage.env import *
 from obs import ObsClient, PutObjectHeader
 
 
 class StorageObs(StorageInterface):
 
     def __init__(self, cfgs=None):
         if cfgs is None:
```

