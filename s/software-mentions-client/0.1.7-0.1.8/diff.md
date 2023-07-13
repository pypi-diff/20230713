# Comparing `tmp/software_mentions_client-0.1.7.tar.gz` & `tmp/software_mentions_client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_mentions_client-0.1.7.tar", last modified: Tue May 30 14:16:17 2023, max compression
+gzip compressed data, was "software_mentions_client-0.1.8.tar", last modified: Thu Jul 13 18:41:17 2023, max compression
```

## Comparing `software_mentions_client-0.1.7.tar` & `software_mentions_client-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/
--rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.7/LICENSE
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.7/MANIFEST.in
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     6694 2023-05-22 13:05:07.000000 software_mentions_client-0.1.7/Readme.md
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.7/config.json
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       33 2023-05-30 14:14:03.000000 software_mentions_client-0.1.7/requirements.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/setup.cfg
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      921 2023-05-30 14:14:40.000000 software_mentions_client-0.1.7/setup.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/S3.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/__init__.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)    52167 2023-05-30 13:10:19.000000 software_mentions_client-0.1.7/software_mentions_client/client.py
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.7/software_mentions_client/consistency_check.py
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client/resources/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.7/software_mentions_client/resources/covid_blacklist.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.7/software_mentions_client/resources/stopwords_en.txt
-drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-05-30 14:16:17.021753 software_mentions_client-0.1.7/software_mentions_client.egg-info/
--rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/PKG-INFO
--rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/SOURCES.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/dependency_links.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/requires.txt
--rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-05-30 14:16:16.000000 software_mentions_client-0.1.7/software_mentions_client.egg-info/top_level.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/
+-rwxrwxr-x   0 lopez     (1000) lopez     (1000)    11184 2023-03-07 10:52:06.000000 software_mentions_client-0.1.8/LICENSE
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      112 2023-03-07 19:00:06.000000 software_mentions_client-0.1.8/MANIFEST.in
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     6694 2023-05-22 13:05:07.000000 software_mentions_client-0.1.8/Readme.md
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      504 2023-03-07 18:31:51.000000 software_mentions_client-0.1.8/config.json
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       34 2023-07-13 18:40:17.000000 software_mentions_client-0.1.8/requirements.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       38 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/setup.cfg
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      921 2023-07-13 18:40:28.000000 software_mentions_client-0.1.8/setup.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     2908 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/S3.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        0 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/__init__.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)    52167 2023-05-30 13:10:19.000000 software_mentions_client-0.1.8/software_mentions_client/client.py
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3620 2022-02-17 14:19:32.000000 software_mentions_client-0.1.8/software_mentions_client/consistency_check.py
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client/resources/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3605 2021-08-30 13:06:10.000000 software_mentions_client-0.1.8/software_mentions_client/resources/covid_blacklist.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     3191 2021-08-08 01:18:57.000000 software_mentions_client-0.1.8/software_mentions_client/resources/stopwords_en.txt
+drwxrwxr-x   0 lopez     (1000) lopez     (1000)        0 2023-07-13 18:41:17.320822 software_mentions_client-0.1.8/software_mentions_client.egg-info/
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)     7215 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/PKG-INFO
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)      562 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)        1 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       35 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/requires.txt
+-rw-rw-r--   0 lopez     (1000) lopez     (1000)       25 2023-07-13 18:41:17.000000 software_mentions_client-0.1.8/software_mentions_client.egg-info/top_level.txt
```

### Comparing `software_mentions_client-0.1.7/LICENSE` & `software_mentions_client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/PKG-INFO` & `software_mentions_client-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software_mentions_client
-Version: 0.1.7
+Version: 0.1.8
 Summary: A client for extracting software mentions in scholar publications
 Home-page: https://github.com/kermitt2/software_mentions_client
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `software_mentions_client-0.1.7/Readme.md` & `software_mentions_client-0.1.8/Readme.md`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/setup.py` & `software_mentions_client-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt', 'r') as f:
     reqs = f.readlines()
 
 setup(
     name="software_mentions_client",
-    version="0.1.7",
+    version="0.1.8",
     author="Patrice Lopez",
     author_email="patrice.lopez@science-miner.com",
     description="A client for extracting software mentions in scholar publications",
     long_description=open("Readme.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url='https://github.com/kermitt2/software_mentions_client',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests", "my_config*", "*.log"]),
```

### Comparing `software_mentions_client-0.1.7/software_mentions_client/S3.py` & `software_mentions_client-0.1.8/software_mentions_client/S3.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/software_mentions_client/client.py` & `software_mentions_client-0.1.8/software_mentions_client/client.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/software_mentions_client/consistency_check.py` & `software_mentions_client-0.1.8/software_mentions_client/consistency_check.py`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/software_mentions_client/resources/covid_blacklist.txt` & `software_mentions_client-0.1.8/software_mentions_client/resources/covid_blacklist.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/software_mentions_client/resources/stopwords_en.txt` & `software_mentions_client-0.1.8/software_mentions_client/resources/stopwords_en.txt`

 * *Files identical despite different names*

### Comparing `software_mentions_client-0.1.7/software_mentions_client.egg-info/PKG-INFO` & `software_mentions_client-0.1.8/software_mentions_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software-mentions-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: A client for extracting software mentions in scholar publications
 Home-page: https://github.com/kermitt2/software_mentions_client
 Author: Patrice Lopez
 Author-email: patrice.lopez@science-miner.com
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `software_mentions_client-0.1.7/software_mentions_client.egg-info/SOURCES.txt` & `software_mentions_client-0.1.8/software_mentions_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

