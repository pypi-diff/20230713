# Comparing `tmp/influxdb3-python-0.1.8.tar.gz` & `tmp/influxdb3-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.8.tar", last modified: Tue Jul 11 13:07:29 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.9.tar", last modified: Thu Jul 13 11:25:05 2023, max compression
```

## Comparing `influxdb3-python-0.1.8.tar` & `influxdb3-python-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 13:07:29.000000 influxdb3-python-0.1.8/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:07:29.939871 influxdb3-python-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 13:07:18.000000 influxdb3-python-0.1.8/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:25:05.000000 influxdb3-python-0.1.9/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:25:05.259034 influxdb3-python-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-13 11:24:50.000000 influxdb3-python-0.1.9/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.8/LICENSE` & `influxdb3-python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.8/PKG-INFO` & `influxdb3-python-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.8/README.md` & `influxdb3-python-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.8/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.1.9/influxdb3_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `influxdb3-python-0.1.8/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.9/influxdb_client_3/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 def default_client_options(**kwargs):
     return kwargs
 
 def flight_client_options(**kwargs):
     return kwargs  # You can replace this with a specific data structure if needed
 
+
 class InfluxDBClient3:
     def __init__(
             self,
             host=None,
             org=None,
             database=None,
             token=None,
@@ -43,70 +44,76 @@
         :type write_client_options: dict
         :param flight_client_options: Options for the FlightClient.
         :type flight_client_options: dict
         :param kwargs: Additional arguments for the InfluxDB Client.
         """
         self._org = org
         self._database = database
+        self._token = token
         self._write_client_options = write_client_options if write_client_options is not None else default_client_options(write_options=SYNCHRONOUS)
 
         # Extracting the hostname from URL if provided
         parsed_url = urllib.parse.urlparse(host)
         host = parsed_url.hostname or host
 
         self._client = _InfluxDBClient(
             url=f"https://{host}",
-            token=token,
+            token=self._token,
             org=self._org,
             **kwargs)
         
         self._write_api = _WriteApi(influxdb_client=self._client, **self._write_client_options)
         self._flight_client_options = flight_client_options or {}
         self._flight_client = FlightClient(f"grpc+tls://{host}:443", **self._flight_client_options)
         
-        # Create an authorization header
-        self._options = FlightCallOptions(headers=[(b"authorization", f"Bearer {token}".encode('utf-8'))])
 
-    def write(self, record=None, **kwargs):
+
+    def write(self, record=None, database=None ,**kwargs):
         """
         Write data to InfluxDB.
 
         :param record: The data point(s) to write.
         :type record: Point or list of Point objects
         :param kwargs: Additional arguments to pass to the write API.
         """
+        if database is None:
+            database = self._database
+
         try:
-            self._write_api.write(bucket=self._database, record=record, **kwargs)
+            self._write_api.write(bucket=database, record=record, **kwargs)
         except InfluxDBError as e:
             raise e
           
 
-    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', **kwargs):
+    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', database=None, **kwargs):
         """
         Write data from a file to InfluxDB.
 
         :param file: The file to write.
         :type file: str
         :param measurement_name: The name of the measurement.
         :type measurement_name: str
         :param tag_columns: Tag columns.
         :type tag_columns: list
         :param timestamp_column: Timestamp column name. Defaults to 'time'.
         :type timestamp_column: str
         :param kwargs: Additional arguments to pass to the write API.
         """
+        if database is None:
+            database = self._database
+
         try:
             table = upload_file(file).load_file()
             df = table.to_pandas() if isinstance(table, pa.Table) else table
-            self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column)
+            self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column, database=database, **kwargs)
         except Exception as e:
             raise e
             
 
-    def _process_dataframe(self, df, measurement_name, tag_columns, timestamp_column):
+    def _process_dataframe(self, df, measurement_name, tag_columns, timestamp_column, database, **kwargs):
         # This function is factored out for clarity.
         # It processes a DataFrame before writing to InfluxDB.
 
         measurement_column = None
         if measurement_name is None:
             measurement_column = next((col for col in ['measurement', 'iox::measurement'] if col in df.columns), None)
             if measurement_column:
@@ -116,35 +123,40 @@
                                           data_frame_measurement_name=measurement,
                                           data_frame_tag_columns=tag_columns,
                                           data_frame_timestamp_column=timestamp_column)
             else:
                 print("'measurement' column not found in the dataframe.")
         else:
             df = df.drop(columns=['measurement'], errors='ignore')
-            self._write_api.write(bucket=self._database, record=df,
+            self._write_api.write(bucket=database, record=df,
                                   data_frame_measurement_name=measurement_name,
                                   data_frame_tag_columns=tag_columns,
-                                  data_frame_timestamp_column=timestamp_column)
+                                  data_frame_timestamp_column=timestamp_column, **kwargs)
 
-    def query(self, query, language="sql", mode="all"):
+    def query(self, query, language="sql", mode="all", database=None, **kwargs ):
         """
         Query data from InfluxDB.
 
         :param query: The query string.
         :type query: str
         :param language: The query language (default is "sql").
         :type language: str
         :param mode: The mode of fetching data (all, pandas, chunk, reader, schema).
         :type mode: str
         :return: The queried data.
         """
+        if database is None:
+            database = self._database
+        
         try:
-            ticket_data = {"database": self._database, "sql_query": query, "query_type": language}
+            # Create an authorization header
+            _options = FlightCallOptions(headers=[(b"authorization", f"Bearer {self._token}".encode('utf-8'))], **kwargs)
+            ticket_data = {"database": database, "sql_query": query, "query_type": language}
             ticket = Ticket(json.dumps(ticket_data).encode('utf-8'))
-            flight_reader = self._flight_client.do_get(ticket, self._options)
+            flight_reader = self._flight_client.do_get(ticket, _options)
 
             mode_func = {
                 "all": flight_reader.read_all,
                 "pandas": flight_reader.read_pandas,
                 "chunk": lambda: flight_reader,
                 "reader": flight_reader.to_reader,
                 "schema": lambda: flight_reader.schema
```

### Comparing `influxdb3-python-0.1.8/influxdb_client_3/read_file.py` & `influxdb3-python-0.1.9/influxdb_client_3/read_file.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.8/setup.py` & `influxdb3-python-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.8/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.9/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

