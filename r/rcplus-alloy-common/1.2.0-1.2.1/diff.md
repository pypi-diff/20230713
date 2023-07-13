# Comparing `tmp/rcplus_alloy_common-1.2.0.tar.gz` & `tmp/rcplus_alloy_common-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-1.2.0.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.2.1.tar", max compression
```

## Comparing `rcplus_alloy_common-1.2.0.tar` & `rcplus_alloy_common-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       77 2023-06-23 20:29:48.979650 rcplus_alloy_common-1.2.0/LICENSE
--rw-r--r--   0        0        0      571 2023-06-23 20:29:48.979650 rcplus_alloy_common-1.2.0/README.md
--rw-r--r--   0        0        0     1951 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2881 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0      567 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/__init__.py
--rw-r--r--   0        0        0     1179 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/dag.py
--rw-r--r--   0        0        0     1681 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/decorators.py
--rw-r--r--   0        0        0      703 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/hooks.py
--rw-r--r--   0        0        0     7448 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/observability.py
--rw-r--r--   0        0        0    18818 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/operators.py
--rw-r--r--   0        0        0     2611 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/sensors.py
--rw-r--r--   0        0        0     2799 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/utils.py
--rw-r--r--   0        0        0     2279 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     3866 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/logging.py
--rw-r--r--   0        0        0     6388 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/metrics.py
--rw-r--r--   0        0        0     3925 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/retry.py
--rw-r--r--   0        0        0       19 2023-06-23 20:29:48.983650 rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/version.py
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-07-13 09:20:28.905190 rcplus_alloy_common-1.2.1/LICENSE
+-rw-r--r--   0        0        0      571 2023-07-13 09:20:28.905190 rcplus_alloy_common-1.2.1/README.md
+-rw-r--r--   0        0        0     1951 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2881 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      567 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1681 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0      703 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/hooks.py
+-rw-r--r--   0        0        0     7448 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0    20030 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2799 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     3866 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6388 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3925 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-07-13 09:20:28.909190 rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.2.1/PKG-INFO
```

### Comparing `rcplus_alloy_common-1.2.0/README.md` & `rcplus_alloy_common-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.2.0**
+Current version: **v1.2.1**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

### Comparing `rcplus_alloy_common-1.2.0/pyproject.toml` & `rcplus_alloy_common-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "1.2.0"
+version = "1.2.1"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
```

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/__init__.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/__init__.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/dag.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/decorators.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/decorators.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/hooks.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/hooks.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/observability.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/observability.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/operators.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/operators.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,37 @@
     """Alloy PythonOperator"""
 
 
 @alloyize
 class AlloyGlueJobOperator(GlueJobOperator):
     """Alloy GlueJobOperator class with dag_run_id injected."""
     dest_s3_path = None
+    logzio_appender_jar_s3_path = None
+    job_default_args = None
+
+    def get_job_default_args(self):
+        if self.job_default_args is not None:
+            return self.job_default_args
+        boto3_session = boto3.Session()
+        glue_client = boto3_session.client("glue")
+        job = glue_client.get_job(JobName=self.job_name)
+        if "Job" in job and "DefaultArguments" in job["Job"]:
+            self.job_default_args = job["Job"]["DefaultArguments"]
+        else:
+            self.job_default_args = {}
+        return self.job_default_args
 
     def prepare_log4j2(self, dag_id, dag_run_id):
         # retrieve the log4j2.properties S3 url and extract the bucket name and object key
         boto3_session = boto3.Session()
         ssm = boto3_session.client("ssm")
         conf_s3_path = ssm.get_parameter(Name="/alloy/airflow/glue/logzio_appender_conf_s3_path")["Parameter"]["Value"]
+        self.logzio_appender_jar_s3_path = ssm.get_parameter(
+            Name="/alloy/airflow/glue/logzio_appender_jarball_s3_path"
+        )["Parameter"]["Value"]
         parsed_s3_url = urlparse(conf_s3_path, allow_fragments=False)
         s3_bucket_name = parsed_s3_url.netloc
         s3_key_src = parsed_s3_url.path.lstrip("/")
         #
         # read the log4j2.properties file from S3 as a template
         s3 = boto3_session.client("s3")
         templ = BytesIO()
@@ -66,32 +83,41 @@
             templ.getvalue().decode("utf-8"),
             flags=re.MULTILINE,
         )
         s3_key_dest = f"config/{dag_id}/{dag_run_id}/log4j2.properties"
         self.dest_s3_path = f"s3://{s3_bucket_name}/{s3_key_dest}"
         s3.upload_fileobj(BytesIO(conf_str_desc.encode("utf-8")), s3_bucket_name, s3_key_dest)
 
+    def get_default_script_args(self, key):
+        return self.get_job_default_args().get(key, None)
+
+    def set_script_args(self, key, value):
+        if key not in self.script_args:
+            default_value = self.get_default_script_args(key)
+            if default_value is not None:
+                self.script_args[key] = default_value
+
+        if key not in self.script_args:
+            self.script_args[key] = value
+        else:
+            if value not in self.script_args[key].split(","):
+                self.script_args[key] += f",{value}"
+
     def execute(self, context):
         # NOTE-zw: here we instruct the GlueJobOperator to use log4j2.properties from S3. This is a hack because there
         #         is no other way to pass the context attributes to log4j before it got initialized. The workaround we
         #         apply here is based on a BIG assumption: for each Glue Job run task there is a new Spark node
         #         initialized. This assumption is true for the current implementation of the GlueJobOperator as of
         #         2021-05-03 (Airflow 2.6.1).
         dag_id = context["dag"].dag_id
         dag_run_id = context["dag_run"].run_id
         self.prepare_log4j2(dag_id, dag_run_id)
-        if self.script_args is None:
-            self.script_args = {}
-
-        self.script_args["--extra-files"] = (
-            f"{self.script_args['--extra-files']},{self.dest_s3_path}"
-            if "--extra-files" in self.script_args and len(self.script_args["--extra-files"]) > 0
-            else self.dest_s3_path
-        )
-
+        # self.set_script_args("--conf", f"spark.driver.extraJavaOptions=-Dlog4j.configurationFile={self.dest_s3_path}")
+        self.set_script_args("--extra-files", self.dest_s3_path)
+        self.set_script_args("--extra-jars", self.logzio_appender_jar_s3_path)
         return super().execute(context)
 
 
 @alloyize
 class AlloyEcsRunTaskOperator(EcsRunTaskOperator):
     """Alloy ECSRunTaskOperator"""
```

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/sensors.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/sensors.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/airflow/utils.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/airflow/utils.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/constants.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/constants.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/logging.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/logging.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/metrics.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/metrics.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/src/rcplus_alloy_common/retry.py` & `rcplus_alloy_common-1.2.1/src/rcplus_alloy_common/retry.py`

 * *Files identical despite different names*

### Comparing `rcplus_alloy_common-1.2.0/PKG-INFO` & `rcplus_alloy_common-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 1.2.0
+Version: 1.2.1
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
 Requires-Python: >=3.10,<4
@@ -29,15 +29,15 @@
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
 ![Coverage badge](./coverage.svg)
 
-Current version: **v1.2.0**
+Current version: **v1.2.1**
 
 ---
 
 Python utilities for RC+/Alloy.
 
 _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
```

