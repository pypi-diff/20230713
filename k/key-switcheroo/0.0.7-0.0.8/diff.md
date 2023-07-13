# Comparing `tmp/key_switcheroo-0.0.7.tar.gz` & `tmp/key_switcheroo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.7.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.8.tar", max compression
```

## Comparing `key_switcheroo-0.0.7.tar` & `key_switcheroo-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     5060 2023-07-09 19:13:51.612702 key_switcheroo-0.0.7/README.md
--rw-r--r--   0        0        0      788 2023-07-12 16:58:29.038276 key_switcheroo-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.7/switcheroo/__init__.py
--rw-r--r--   0        0        0      135 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/__init__.py
--rw-r--r--   0        0        0     3654 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/__init__.py
--rw-r--r--   0        0        0     1909 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/s3.py
--rw-r--r--   0        0        0       92 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/data_store/util.py
--rw-r--r--   0        0        0      356 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/exceptions/s3.py
--rw-r--r--   0        0        0      287 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/base/serializer.py
--rw-r--r--   0        0        0     1774 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/paths.py
--rw-r--r--   0        0        0      205 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/__init__.py
--rw-r--r--   0        0        0     1296 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/s3.py
--rw-r--r--   0        0        0     2957 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/__init__.py
--rw-r--r--   0        0        0     1809 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/s3.py
--rw-r--r--   0        0        0      931 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/data_stores/__init__.py
--rw-r--r--   0        0        0      834 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/exceptions.py
--rw-r--r--   0        0        0      183 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/objects/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/objects/key.py
--rw-r--r--   0        0        0        0 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/scripts/__init__.py
--rw-r--r--   0        0        0     1966 2023-07-11 19:31:10.959146 key_switcheroo-0.0.7/switcheroo/ssh/scripts/publish.py
--rwxr-xr-x   0        0        0     2002 2023-07-11 21:36:01.857025 key_switcheroo-0.0.7/switcheroo/ssh/scripts/retrieve.py
--rw-r--r--   0        0        0     2997 2023-07-12 16:58:29.038276 key_switcheroo-0.0.7/switcheroo/util.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     5060 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/README.md
+-rw-r--r--   0        0        0      802 2023-07-13 17:18:04.957594 key_switcheroo-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/__init__.py
+-rw-r--r--   0        0        0     3654 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/data_store/__init__.py
+-rw-r--r--   0        0        0     1909 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/data_store/s3.py
+-rw-r--r--   0        0        0       92 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/data_store/util.py
+-rw-r--r--   0        0        0      356 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/exceptions/s3.py
+-rw-r--r--   0        0        0      287 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/base/serializer.py
+-rw-r--r--   0        0        0     1774 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/paths.py
+-rw-r--r--   0        0        0      205 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_org/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_org/publisher/__init__.py
+-rw-r--r--   0        0        0     1296 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_org/publisher/s3.py
+-rw-r--r--   0        0        0     2957 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_org/retriever/__init__.py
+-rw-r--r--   0        0        0     1809 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_org/retriever/s3.py
+-rw-r--r--   0        0        0      931 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/data_stores/__init__.py
+-rw-r--r--   0        0        0      834 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/exceptions.py
+-rw-r--r--   0        0        0      183 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/objects/__init__.py
+-rw-r--r--   0        0        0     4638 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/objects/key.py
+-rw-r--r--   0        0        0        0 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/scripts/__init__.py
+-rw-r--r--   0        0        0     1966 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/scripts/publish.py
+-rwxr-xr-x   0        0        0     2002 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/ssh/scripts/retrieve.py
+-rw-r--r--   0        0        0     2997 2023-07-12 22:26:14.720254 key_switcheroo-0.0.8/switcheroo/util.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.8/PKG-INFO
```

### Comparing `key_switcheroo-0.0.7/README.md` & `key_switcheroo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/pyproject.toml` & `key_switcheroo-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 boto3 = "^1.27.0"
 
 [tool.poetry.group.dev.dependencies]
 PyHamcrest = "^2.0.4"
 pyright = "^1.1.316"
 pylint = "^2.17.4"
 black = "^23.3.0"
-boto3-stubs = {version = "1.27.0", extras = ["s3", "sts"]}
+boto3-stubs = {version = "1.28.2", extras = ["cloudwatch", "s3", "sts"]}
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.0"
 
 [tool.poetry.scripts]
 
 switcheroo_publish = "switcheroo.ssh.scripts.publish:main"
 switcheroo_retrieve = "switcheroo.ssh.scripts.retrieve:main"
```

### Comparing `key_switcheroo-0.0.7/switcheroo/base/data_store/__init__.py` & `key_switcheroo-0.0.8/switcheroo/base/data_store/__init__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/base/data_store/s3.py` & `key_switcheroo-0.0.8/switcheroo/base/data_store/s3.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/paths.py` & `key_switcheroo-0.0.8/switcheroo/paths.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/__init__.py` & `key_switcheroo-0.0.8/switcheroo/ssh/data_org/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/data_org/publisher/s3.py` & `key_switcheroo-0.0.8/switcheroo/ssh/data_org/publisher/s3.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/__init__.py` & `key_switcheroo-0.0.8/switcheroo/ssh/data_org/retriever/__init__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/data_org/retriever/s3.py` & `key_switcheroo-0.0.8/switcheroo/ssh/data_org/retriever/s3.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/data_stores/__init__.py` & `key_switcheroo-0.0.8/switcheroo/ssh/data_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/exceptions.py` & `key_switcheroo-0.0.8/switcheroo/ssh/exceptions.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/objects/key.py` & `key_switcheroo-0.0.8/switcheroo/ssh/objects/key.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/scripts/publish.py` & `key_switcheroo-0.0.8/switcheroo/ssh/scripts/publish.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/ssh/scripts/retrieve.py` & `key_switcheroo-0.0.8/switcheroo/ssh/scripts/retrieve.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/switcheroo/util.py` & `key_switcheroo-0.0.8/switcheroo/util.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.7/PKG-INFO` & `key_switcheroo-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: key-switcheroo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Rotate SSH keys, stored in the cloud!
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.27.0,<2.0.0)
```

