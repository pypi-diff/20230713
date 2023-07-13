# Comparing `tmp/airflow_dag_artifact-0.1.1.tar.gz` & `tmp/airflow_dag_artifact-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_dag_artifact-0.1.1.tar", last modified: Wed Jul 12 20:14:38 2023, max compression
+gzip compressed data, was "airflow_dag_artifact-0.2.1.tar", last modified: Thu Jul 13 01:12:20 2023, max compression
```

## Comparing `airflow_dag_artifact-0.1.1.tar` & `airflow_dag_artifact-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.325266 airflow_dag_artifact-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1131 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      328 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4788 2023-07-12 20:14:38.325096 airflow_dag_artifact-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3570 2023-07-12 20:10:49.000000 airflow_dag_artifact-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.322230 airflow_dag_artifact-0.1.1/airflow_dag_artifact/
--rw-r--r--   0 sanhehu    (501) staff       (20)      535 2023-07-12 19:48:54.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       63 2023-07-12 19:47:37.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.323124 airflow_dag_artifact-0.1.1/airflow_dag_artifact/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4052 2023-07-12 19:45:31.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/model.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.323591 airflow_dag_artifact-0.1.1/airflow_dag_artifact/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-12 19:42:18.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.324307 airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-07-12 19:41:57.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.323007 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4788 2023-07-12 20:14:38.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      875 2023-07-12 20:14:38.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-12 20:14:38.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      203 2023-07-12 20:14:38.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       21 2023-07-12 20:14:38.000000 airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      597 2023-07-12 20:06:47.000000 airflow_dag_artifact-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-12 19:41:20.000000 airflow_dag_artifact-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       84 2023-07-12 19:41:17.000000 airflow_dag_artifact-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-12 20:14:38.325323 airflow_dag_artifact-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7569 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-12 20:14:38.324670 airflow_dag_artifact-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      275 2023-07-12 19:47:54.000000 airflow_dag_artifact-0.1.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1683 2023-07-12 19:59:13.000000 airflow_dag_artifact-0.1.1/tests/test_model.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.021639 airflow_dag_artifact-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1131 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      328 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5172 2023-07-13 01:12:20.021505 airflow_dag_artifact-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3954 2023-07-13 01:10:58.000000 airflow_dag_artifact-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.018905 airflow_dag_artifact-0.2.1/airflow_dag_artifact/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      535 2023-07-12 19:48:54.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-13 01:11:06.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       94 2023-07-12 20:39:48.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5242 2023-07-13 01:07:57.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/aws_mwaa.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.019654 airflow_dag_artifact-0.2.1/airflow_dag_artifact/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4318 2023-07-13 00:46:45.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/model.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.020082 airflow_dag_artifact-0.2.1/airflow_dag_artifact/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-12 19:42:18.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.020841 airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7590 2023-07-12 19:41:57.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.019540 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5172 2023-07-13 01:12:20.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      908 2023-07-13 01:12:20.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-13 01:12:20.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      203 2023-07-13 01:12:20.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       21 2023-07-13 01:12:20.000000 airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      756 2023-07-13 01:11:42.000000 airflow_dag_artifact-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-12 19:41:20.000000 airflow_dag_artifact-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       84 2023-07-12 19:41:17.000000 airflow_dag_artifact-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-13 01:12:20.021679 airflow_dag_artifact-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7569 2023-07-12 19:39:29.000000 airflow_dag_artifact-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-13 01:12:20.021206 airflow_dag_artifact-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      275 2023-07-12 19:47:54.000000 airflow_dag_artifact-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1683 2023-07-12 19:59:13.000000 airflow_dag_artifact-0.2.1/tests/test_model.py
```

### Comparing `airflow_dag_artifact-0.1.1/AUTHORS.rst` & `airflow_dag_artifact-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/LICENSE.txt` & `airflow_dag_artifact-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/PKG-INFO` & `airflow_dag_artifact-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: airflow_dag_artifact
-Version: 0.1.1
+Version: 0.2.1
 Summary: Airflow Dag Artifact versioning and alias Management for blue/green, canary deployment, and roll back for production failure.
 Home-page: https://github.com/MacHu-GWU/airflow_dag_artifact-project
-Download-URL: https://pypi.python.org/pypi/airflow_dag_artifact/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/airflow_dag_artifact/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,14 +88,16 @@
 - `AWS StepFunction Versioning and Alias <https://docs.aws.amazon.com/step-functions/latest/dg/auth-version-alias.html>`_
 - `AWS SageMaker Model Registry Versioning <https://docs.aws.amazon.com/sagemaker/latest/dg/model-registry.html>`_
 
 However, Airflow DAG does not support this feature yet. This library provides a way to manage Airflow DAG versioning and alias so you can deploy Airflow DAG with confidence.
 
 Please `read this tutorial <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/deploy_versioned_airflow_dag_artifacts.ipynb>`_ to learn how to use this library.
 
+It also has native `AWS MWAA <https://aws.amazon.com/managed-workflows-for-apache-airflow/>`_ support for DAG deployment automation, with the DAG versioning manage, which is not official supported by Apache Airflow. Please `read this example <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/aws_mwaa.py>`_ to learn how to use this library with AWS MWAA.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``airflow_dag_artifact`` is released on PyPI, so all you need is to:
```

### Comparing `airflow_dag_artifact-0.1.1/README.rst` & `airflow_dag_artifact-0.2.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 - `AWS StepFunction Versioning and Alias <https://docs.aws.amazon.com/step-functions/latest/dg/auth-version-alias.html>`_
 - `AWS SageMaker Model Registry Versioning <https://docs.aws.amazon.com/sagemaker/latest/dg/model-registry.html>`_
 
 However, Airflow DAG does not support this feature yet. This library provides a way to manage Airflow DAG versioning and alias so you can deploy Airflow DAG with confidence.
 
 Please `read this tutorial <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/deploy_versioned_airflow_dag_artifacts.ipynb>`_ to learn how to use this library.
 
+It also has native `AWS MWAA <https://aws.amazon.com/managed-workflows-for-apache-airflow/>`_ support for DAG deployment automation, with the DAG versioning manage, which is not official supported by Apache Airflow. Please `read this example <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/aws_mwaa.py>`_ to learn how to use this library with AWS MWAA.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``airflow_dag_artifact`` is released on PyPI, so all you need is to:
```

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/__init__.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/model.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 PT = T.Union[str, _Path, Path]
 
 
 @dataclasses.dataclass
 class Base:
     """
-    Base class for AWS Glue artifact.
+    Base class for Airflow DAG artifact.
     """
 
     aws_region: str = dataclasses.field()
     s3_bucket: str = dataclasses.field()
     s3_prefix: str = dataclasses.field()
     dynamodb_table_name: str = dataclasses.field()
     artifact_name: str = dataclasses.field()
@@ -53,14 +53,22 @@
         self,
         bsm: BotoSesManager,
         dynamodb_write_capacity_units: T.Optional[int] = None,
         dynamodb_read_capacity_units: T.Optional[int] = None,
     ):
         """
         Create the required S3 bucket and DynamoDB table for the artifact store backend.
+
+        It also setup the underlying S3 and DynamoDB client session for
+        ``put_artifact``, ``put_artifact_version`` methods. You should always
+        call this method at begin of your program
+
+        .. note::
+
+            This operation is idempotent.
         """
         self.repo.bootstrap(
             bsm=bsm,
             dynamodb_write_capacity_units=dynamodb_write_capacity_units,
             dynamodb_read_capacity_units=dynamodb_read_capacity_units,
         )
```

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/paths.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/paths.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/tests/mock_aws.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/hashes.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact/vendor/pytest_cov_helper.py` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/PKG-INFO` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: airflow-dag-artifact
-Version: 0.1.1
+Version: 0.2.1
 Summary: Airflow Dag Artifact versioning and alias Management for blue/green, canary deployment, and roll back for production failure.
 Home-page: https://github.com/MacHu-GWU/airflow_dag_artifact-project
-Download-URL: https://pypi.python.org/pypi/airflow_dag_artifact/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/airflow_dag_artifact/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,14 +88,16 @@
 - `AWS StepFunction Versioning and Alias <https://docs.aws.amazon.com/step-functions/latest/dg/auth-version-alias.html>`_
 - `AWS SageMaker Model Registry Versioning <https://docs.aws.amazon.com/sagemaker/latest/dg/model-registry.html>`_
 
 However, Airflow DAG does not support this feature yet. This library provides a way to manage Airflow DAG versioning and alias so you can deploy Airflow DAG with confidence.
 
 Please `read this tutorial <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/deploy_versioned_airflow_dag_artifacts.ipynb>`_ to learn how to use this library.
 
+It also has native `AWS MWAA <https://aws.amazon.com/managed-workflows-for-apache-airflow/>`_ support for DAG deployment automation, with the DAG versioning manage, which is not official supported by Apache Airflow. Please `read this example <https://github.com/MacHu-GWU/airflow_dag_artifact-project/blob/main/examples/aws_mwaa.py>`_ to learn how to use this library with AWS MWAA.
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``airflow_dag_artifact`` is released on PyPI, so all you need is to:
```

### Comparing `airflow_dag_artifact-0.1.1/airflow_dag_artifact.egg-info/SOURCES.txt` & `airflow_dag_artifact-0.2.1/airflow_dag_artifact.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 airflow_dag_artifact/__init__.py
 airflow_dag_artifact/_version.py
 airflow_dag_artifact/api.py
+airflow_dag_artifact/aws_mwaa.py
 airflow_dag_artifact/model.py
 airflow_dag_artifact/paths.py
 airflow_dag_artifact.egg-info/PKG-INFO
 airflow_dag_artifact.egg-info/SOURCES.txt
 airflow_dag_artifact.egg-info/dependency_links.txt
 airflow_dag_artifact.egg-info/requires.txt
 airflow_dag_artifact.egg-info/top_level.txt
```

### Comparing `airflow_dag_artifact-0.1.1/release-history.rst` & `airflow_dag_artifact-0.2.1/release-history.rst`

 * *Files 17% similar despite different names*

```diff
@@ -13,12 +13,19 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.1 (2023-07-12)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Add AWS MWAA integration.
+
+
 0.1.1 (2023-07-12)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 - First release
 - Add the following public API:
     ``airflow_dag_artifact.api.AirflowDagArtifact``
```

### Comparing `airflow_dag_artifact-0.1.1/requirements-doc.txt` & `airflow_dag_artifact-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/setup.py` & `airflow_dag_artifact-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `airflow_dag_artifact-0.1.1/tests/test_model.py` & `airflow_dag_artifact-0.2.1/tests/test_model.py`

 * *Files identical despite different names*

