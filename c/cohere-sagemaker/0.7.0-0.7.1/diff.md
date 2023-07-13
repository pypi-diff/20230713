# Comparing `tmp/cohere-sagemaker-0.7.0.tar.gz` & `tmp/cohere-sagemaker-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-sagemaker-0.7.0.tar", last modified: Wed Jul 12 17:22:52 2023, max compression
+gzip compressed data, was "cohere-sagemaker-0.7.1.tar", last modified: Thu Jul 13 11:25:18 2023, max compression
```

## Comparing `cohere-sagemaker-0.7.0.tar` & `cohere-sagemaker-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1066 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/LICENSE
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/PKG-INFO
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      948 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/README.md
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/cohere_sagemaker/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       57 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/__init__.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1222 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/classification.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)    21487 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/client.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      623 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/embeddings.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      591 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/error.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      796 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/generation.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     2069 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/rerank.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      337 2023-07-11 10:58:17.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/response.py
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      491 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/cohere_sagemaker/summary.py
-drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      488 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        1 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       16 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/requires.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       17 2023-07-12 17:22:52.000000 cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       38 2023-07-12 17:22:52.891793 cohere-sagemaker-0.7.0/setup.cfg
--rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1525 2023-07-12 17:22:44.000000 cohere-sagemaker-0.7.0/setup.py
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1066 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/LICENSE
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/PKG-INFO
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      948 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/README.md
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.966277 cohere-sagemaker-0.7.1/cohere_sagemaker/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       57 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/__init__.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1222 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/classification.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)    21487 2023-07-13 11:05:48.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/client.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      623 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/embeddings.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      591 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/error.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      796 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/generation.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     2069 2023-07-11 10:29:34.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/rerank.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      337 2023-07-11 10:58:17.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/response.py
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      491 2023-07-13 11:04:25.000000 cohere-sagemaker-0.7.1/cohere_sagemaker/summary.py
+drwxr-xr-x   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        0 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1412 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)      488 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)        1 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       16 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       17 2023-07-13 11:25:18.000000 cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)       38 2023-07-13 11:25:18.970277 cohere-sagemaker-0.7.1/setup.cfg
+-rw-r--r--   0 leila_cohere_com (1108800906) leila_cohere_com (1108800906)     1525 2023-07-13 11:25:09.000000 cohere-sagemaker-0.7.1/setup.py
```

### Comparing `cohere-sagemaker-0.7.0/LICENSE` & `cohere-sagemaker-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/PKG-INFO` & `cohere-sagemaker-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.7.0/README.md` & `cohere-sagemaker-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/classification.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/client.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         self,
         text: str,
         length: Optional[str] = "auto",
         format_: Optional[str] = "auto",
         # Only summarize-xlarge is supported on Sagemaker
         # model: Optional[str] = "summarize-xlarge",
         extractiveness: Optional[str] = "auto",
-        temperature: Optional[float] = 1.0,
+        temperature: Optional[float] = 0.3,
         additional_command: Optional[str] = "",
         variant: Optional[str] = None
     ) -> Summary:
 
         if self._endpoint_name is None:
             raise CohereError("No endpoint connected. "
                               "Run connect_to_endpoint() first.")
```

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/embeddings.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/error.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/error.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/generation.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker/rerank.py` & `cohere-sagemaker-0.7.1/cohere_sagemaker/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-sagemaker-0.7.0/cohere_sagemaker.egg-info/PKG-INFO` & `cohere-sagemaker-0.7.1/cohere_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-sagemaker
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker
 Home-page: https://github.com/cohere-ai/cohere-sagemaker
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-sagemaker-0.7.0/setup.py` & `cohere-sagemaker-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-sagemaker',
-                 version='0.7.0',
+                 version='0.7.1',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-sagemaker',
                  packages=setuptools.find_packages(),
```

