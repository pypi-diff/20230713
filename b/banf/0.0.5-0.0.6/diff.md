# Comparing `tmp/banf-0.0.5-py3-none-any.whl.zip` & `tmp/banf-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 15527 bytes, number of entries: 18
+Zip file size: 15620 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 02:05 banf/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-09 00:00 banf/communicate/__init__.py
 -rw-rw-rw-  2.0 fat     3025 b- defN 23-Feb-22 05:10 banf/communicate/db_inserter.py
 -rw-rw-rw-  2.0 fat     1694 b- defN 23-Mar-02 00:17 banf/communicate/kafka_consumer.py
 -rw-rw-rw-  2.0 fat     1750 b- defN 23-Mar-06 00:26 banf/communicate/mqtt_receiver.py
 -rw-rw-rw-  2.0 fat     3967 b- defN 23-May-26 03:55 banf/communicate/mqtt_sender.py
 -rw-rw-rw-  2.0 fat     2560 b- defN 23-May-26 03:56 banf/communicate/prometheus_sender.py
 -rw-rw-rw-  2.0 fat     2386 b- defN 23-Jul-03 09:20 banf/communicate/s3_sender.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-03 02:17 banf/data_processing/__init__.py
--rw-rw-rw-  2.0 fat    18505 b- defN 23-Jul-03 10:12 banf/data_processing/preprocessing.py
+-rw-rw-rw-  2.0 fat    18916 b- defN 23-Jul-12 22:57 banf/data_processing/preprocessing.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-09 00:00 banf/etc/__init__.py
 -rw-rw-rw-  2.0 fat      538 b- defN 23-May-25 05:45 banf/etc/bench.py
 -rw-rw-rw-  2.0 fat     2488 b- defN 23-May-30 22:47 banf/etc/observe.py
 -rw-rw-rw-  2.0 fat      240 b- defN 22-Dec-13 04:20 banf/etc/pattern.py
--rw-rw-rw-  2.0 fat     2824 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1453 b- defN 23-Jul-07 00:49 banf-0.0.5.dist-info/RECORD
-18 files, 41527 bytes uncompressed, 13139 bytes compressed:  68.4%
+-rw-rw-rw-  2.0 fat     2824 b- defN 23-Jul-12 23:50 banf-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 23:50 banf-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 23:50 banf-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1453 b- defN 23-Jul-12 23:50 banf-0.0.6.dist-info/RECORD
+18 files, 41938 bytes uncompressed, 13232 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: banf/etc/observe.py
 Comment: 
 
 Filename: banf/etc/pattern.py
 Comment: 
 
-Filename: banf-0.0.5.dist-info/METADATA
+Filename: banf-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: banf-0.0.5.dist-info/WHEEL
+Filename: banf-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: banf-0.0.5.dist-info/top_level.txt
+Filename: banf-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: banf-0.0.5.dist-info/RECORD
+Filename: banf-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## banf/data_processing/preprocessing.py

```diff
@@ -5,15 +5,16 @@
 import pandas as pd
 from datetime import datetime
 import struct
 import boto3
 import botocore
 import os
 import io
-
+from banf.etc.bench import logging_time  # method inference time check decorator
+from pprint import pprint
 
 class ForMeasurement:
     def __init__(self):
         # Data structure format for struct package, it is used to handle binary data stored in files
         self.struct_fmt = "<2HB14HI2fI2dbdb2f"
         # Data splitting step size for chunk processing
         self.STEP_SIZE = 2000
@@ -139,15 +140,15 @@
         return pd.DataFrame(lst, columns=self.packet_col)
 
     # Several data processing functions that convert sensor readings into meaningful values
     def _processingPlusMinus(self, target: pd.DataFrame, col: str) -> int:
         target.loc[target[col] > 32767, col] -= 65536
         return target
 
-    def _processingTemperatureCelcius(self, target: pd.Series) -> pd.Series:
+    def _processingTemperatureCelsius(self, target: pd.Series) -> pd.Series:
         return target / 10
 
     def _processingTemperatureFahrenheit(self, target: pd.Series) -> pd.Series:
         return ((target / 10) * 9 / 5) + 32
 
     def _processingHumidity(self, target: pd.Series) -> pd.Series:
         return target / 10
@@ -415,22 +416,22 @@
         return self._transformProfilerData(
             self._transformiSensorData(
                 self._combineDateTime(self._listToDataFrame(packet))
             )
         )
 
     def lookupS3Objects(self, file_type: str = "preprocessed") -> list:
-        session = boto3.Session(profile_name='default')
+        session = boto3.Session(profile_name="default")
         client = session.client(
             "s3",
             region_name=self.region,
         )
 
         if file_type == "preprocessed":
-            obj_list = client.list_objects(Bucket=self.preprocessed_bucket)
+            obj_list = client.list_objects(Bucket="banf-clientpc-preprocessing-parquet")
         else:
             obj_list = client.list_objects(Bucket=self.raw_bucket)
 
         content_list = obj_list["Contents"]
         key_list = [content["Key"] for content in content_list]
 
         dir_list = []
@@ -439,30 +440,32 @@
             dir_list.append("/".join(key.split("/")[:-1]))
 
         return sorted(list(set(dir_list))), sorted(key_list)
 
     def importS3Objects(
         self, file_name: list, file_type: str = "preprocessed"
     ) -> pd.DataFrame:
-        session = boto3.Session(profile_name='default')
+        session = boto3.Session(profile_name="default")
         client = session.client(
             "s3",
             region_name=self.region,
         )
 
         result = []
         if file_type == "preprocessed":
             for f in file_name:
-                obj = client.get_object(Bucket=self.preprocessed_bucket, Key=f)
-                result.append(pd.read_csv(io.BytesIO(obj["Body"].read())))
+                obj = client.get_object(
+                    Bucket="banf-clientpc-preprocessing-parquet", Key=f
+                )
+                result.append(pd.read_parquet(io.BytesIO(obj["Body"].read())))
 
         else:
             for f in file_name:
                 obj = client.get_object(Bucket=self.raw_bucket, Key=f)
-                result.append(pd.read_csv(io.BytesIO(obj["Body"].read())))
+                result.append(pd.read_parquet(io.BytesIO(obj["Body"].read())))
 
         return result
 
     def _transformiSensorData(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self._processingPlusMinus(df, "Acceleration_Temperature")
         df = self._processingPlusMinus(df, "P_Temperature")
         df = self._processingPlusMinus(df, "Acceleration_X")
@@ -473,33 +476,41 @@
         df["Acceleration_Y"] = self._processingAccel(df["Acceleration_Y"])
         df["Acceleration_Z"] = self._processingAccel(df["Acceleration_Z"])
 
         df["P33V_MON"] = self._processingPower(df["P33V_MON"], "33v")
         df["P5V_MON"] = self._processingPower(df["P5V_MON"], "5v")
         df["VBAT_MON"] = self._processingPower(df["VBAT_MON"], "vbat")
 
-        df["Acceleration_Temperature"] = self._processingTemperatureCelcius(
+        df["Acceleration_Temperature"] = self._processingTemperatureCelsius(
             df["Acceleration_Temperature"]
         )
-        df["P_Temperature"] = self._processingTemperatureCelcius(df["P_Temperature"])
+        df["P_Temperature"] = self._processingTemperatureCelsius(df["P_Temperature"])
         df["Pressure"] = self._processingPressureBar(df["Pressure"])
 
         return df
 
     def _transformProfilerData(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self._processingPlusMinus(df, "Temperature")
 
-        df["Temperature"] = self._processingTemperatureCelcius(df["Temperature"])
+        df["Temperature"] = self._processingTemperatureCelsius(df["Temperature"])
 
         df["Relative_Humidity"] = self._processingHumidity(df["Relative_Humidity"])
 
         return df
 
     def _transformGPSData(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self._combineDateTime(self._processingTime(df))
 
         return df
 
 
 if __name__ == "__main__":
     fm = ForMeasurement()
-    fm.transformToSendPacket("C:/logs/TP0010_TS0011_1000Hz_230220170949_1.txt")
+    _, csv_file_list = fm.lookup_s3_csv_objects()
+    pprint(csv_file_list[:10])
+    
+    _, parquet_file_list = fm.lookup_s3_parquet_objects()
+    pprint(parquet_file_list[:10])
+
+    fm.import_s3_csv_object(csv_file_list[:10])
+    time.sleep(2)
+    fm.import_s3_parquet_object(parquet_file_list[:10])
```

## Comparing `banf-0.0.5.dist-info/METADATA` & `banf-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banf
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package for BANF Co., Ltd.
 Author: BANF Co., Ltd.
 Author-email: gwjeon@banf.co.kr
 Keywords: tire sensor,mqtt,aws,BANF Co., Ltd.
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: bleach (>=6.0.0)
```

## Comparing `banf-0.0.5.dist-info/RECORD` & `banf-0.0.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 banf/communicate/db_inserter.py,sha256=AGycafJGXMVRv5dGvX54YZGsz1KldfW_gkBqxmVROEQ,3025
 banf/communicate/kafka_consumer.py,sha256=LOmctOeZgh5ABsz0v6TQJe39QIsSNiPLpmizvW-VkEY,1694
 banf/communicate/mqtt_receiver.py,sha256=BR85sb1_YkZC8eLYFpxpttyrNhtcv5WD2R7zI5suYto,1750
 banf/communicate/mqtt_sender.py,sha256=pfLiQPCxaG_KcyqtMG8KbRXEdrHmVVeQk_42-ekLRbk,3967
 banf/communicate/prometheus_sender.py,sha256=yrC2z12s10RTSmtXIiRl-XaIhTsZGpvnb_lFGP-iYGI,2560
 banf/communicate/s3_sender.py,sha256=iZ-I98BhIuL0t2Vje6B4Jvpfsw8AaW_5dWz6XC0mBZU,2386
 banf/data_processing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-banf/data_processing/preprocessing.py,sha256=qkvtXnMhMdM16jUv0UfNS-wpwb9ZkDK_rmH8jJ8K8lY,18505
+banf/data_processing/preprocessing.py,sha256=vZhpiSwBNsxjl9AW_7c8qZAFF52iSPxAyQE89RhhokI,18916
 banf/etc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 banf/etc/bench.py,sha256=2Cl_DZrIPLWZWOMRk7vJ37R5tgft04Vu0rPZUAKsg5Q,538
 banf/etc/observe.py,sha256=hsBzz3YEJdEBWCrFDAqz3_orQzVNuhc4IGFq8j_LweM,2488
 banf/etc/pattern.py,sha256=n_j7-mN-QvHRkTP0Tpk8XKfKxXGkZdJfT7eBa_nPQV4,240
-banf-0.0.5.dist-info/METADATA,sha256=qhnEKcsPkGZ-lHp68bz94RsMyB9LhABVZSANU3DXKYU,2824
-banf-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-banf-0.0.5.dist-info/top_level.txt,sha256=6ofKzRyfdu0ATVSHwt9hzGECFmXRGpQ9Fs0igCzbNgM,5
-banf-0.0.5.dist-info/RECORD,,
+banf-0.0.6.dist-info/METADATA,sha256=qCfP3O9GT9pUE4Z6E2mLwPLgJH0QtayNOKvktzJI21A,2824
+banf-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+banf-0.0.6.dist-info/top_level.txt,sha256=6ofKzRyfdu0ATVSHwt9hzGECFmXRGpQ9Fs0igCzbNgM,5
+banf-0.0.6.dist-info/RECORD,,
```

