# Comparing `tmp/strangeworks_qiskit-0.4.3.tar.gz` & `tmp/strangeworks_qiskit-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit-0.4.3.tar", max compression
+gzip compressed data, was "strangeworks_qiskit-0.4.4.tar", max compression
```

## Comparing `strangeworks_qiskit-0.4.3.tar` & `strangeworks_qiskit-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      457 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/LICENSE
--rw-r--r--   0        0        0     1126 2023-05-26 06:38:52.581667 strangeworks_qiskit-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      392 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/__init__.py
--rw-r--r--   0        0        0     6009 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/_runtime_client.py
--rw-r--r--   0        0        0      916 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/__init__.py
--rw-r--r--   0        0        0     1427 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/_utils.py
--rw-r--r--   0        0        0     1563 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/aws.py
--rw-r--r--   0        0        0      604 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/honeywell.py
--rw-r--r--   0        0        0     8413 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ibm.py
--rw-r--r--   0        0        0      599 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ionq.py
--rw-r--r--   0        0        0      932 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/rigetti.py
--rw-r--r--   0        0        0     3497 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/strangeworks.py
--rw-r--r--   0        0        0        0 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/__init__.py
--rw-r--r--   0        0        0     5038 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/job.py
--rw-r--r--   0        0        0      884 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/status.py
--rw-r--r--   0        0        0       74 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/__init__.py
--rw-r--r--   0        0        0     4649 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/backends.py
--rw-r--r--   0        0        0     4350 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/provider.py
--rw-r--r--   0        0        0     9110 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/runtimes.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-07-13 17:01:17.467644 strangeworks_qiskit-0.4.4/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-07-13 17:01:17.467644 strangeworks_qiskit-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1119 2023-07-13 17:01:35.779820 strangeworks_qiskit-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/__init__.py
+-rw-r--r--   0        0        0     6009 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/_runtime_client.py
+-rw-r--r--   0        0        0      916 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/__init__.py
+-rw-r--r--   0        0        0     1427 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/_utils.py
+-rw-r--r--   0        0        0     1563 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/aws.py
+-rw-r--r--   0        0        0      604 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/honeywell.py
+-rw-r--r--   0        0        0     8413 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/ibm.py
+-rw-r--r--   0        0        0      599 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/ionq.py
+-rw-r--r--   0        0        0      932 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/rigetti.py
+-rw-r--r--   0        0        0     3497 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/strangeworks.py
+-rw-r--r--   0        0        0        0 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/jobs/__init__.py
+-rw-r--r--   0        0        0     5038 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/jobs/job.py
+-rw-r--r--   0        0        0      884 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/jobs/status.py
+-rw-r--r--   0        0        0       74 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/platform/__init__.py
+-rw-r--r--   0        0        0     4649 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/platform/backends.py
+-rw-r--r--   0        0        0     4350 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/provider.py
+-rw-r--r--   0        0        0     9110 2023-07-13 17:01:17.471644 strangeworks_qiskit-0.4.4/strangeworks_qiskit/runtimes.py
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.4/PKG-INFO
```

### Comparing `strangeworks_qiskit-0.4.3/LICENSE` & `strangeworks_qiskit-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/pyproject.toml` & `strangeworks_qiskit-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 max-line-length = 88
 per-file-ignores = [
     "__init__.py:F401"
 ]
 
 [tool.poetry]
 name = "strangeworks-qiskit"
-version = "0.4.3"
+version = "0.4.4"
 description = "Strangeworks Qiskit SDK Extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_qiskit"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 strangeworks = "^0.4.2"
 qiskit = "<=0.40.0"
-strangeworks-python-core = "^0.1.5"
+strangeworks-core = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 Flake8-pyproject = "^1.1.0"
 Flask = "^2.0.2"
 mdformat = "^0.7.14"
 mdformat-black = "^0.1.1"
```

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/_runtime_client.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/_runtime_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/__init__.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/_utils.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/_utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/aws.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/aws.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/honeywell.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/honeywell.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ibm.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/ibm.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ionq.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/rigetti.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/strangeworks.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/backends/strangeworks.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/job.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/jobs/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/status.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/jobs/status.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/backends.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/platform/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/provider.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/strangeworks_qiskit/runtimes.py` & `strangeworks_qiskit-0.4.4/strangeworks_qiskit/runtimes.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.3/PKG-INFO` & `strangeworks_qiskit-0.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks-qiskit
-Version: 0.4.3
+Version: 0.4.4
 Summary: Strangeworks Qiskit SDK Extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: qiskit (<=0.40.0)
 Requires-Dist: strangeworks (>=0.4.2,<0.5.0)
-Requires-Dist: strangeworks-python-core (>=0.1.5,<0.2.0)
+Requires-Dist: strangeworks-core (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
 more info or access to test features check out the
 [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |
 |---------------|:------------------------|
```

