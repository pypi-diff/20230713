# Comparing `tmp/gw3-0.4.tar.gz` & `tmp/gw3-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw3-0.4.tar", last modified: Thu Jul 13 10:12:42 2023, max compression
+gzip compressed data, was "gw3-0.5.tar", last modified: Thu Jul 13 10:14:43 2023, max compression
```

## Comparing `gw3-0.4.tar` & `gw3-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:12:42.505637 gw3-0.4/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:12:42.505348 gw3-0.4/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)     1447 2023-07-13 09:18:18.000000 gw3-0.4/README.md
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:12:42.502554 gw3-0.4/gw3/
--rw-r--r--   0 colt       (501) staff       (20)       45 2023-07-13 10:10:43.000000 gw3-0.4/gw3/__init__.py
--rw-r--r--   0 colt       (501) staff       (20)     5084 2023-07-13 09:18:18.000000 gw3-0.4/gw3/client.py
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:12:42.504855 gw3-0.4/gw3.egg-info/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:12:42.000000 gw3-0.4/gw3.egg-info/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-13 10:12:42.000000 gw3-0.4/gw3.egg-info/SOURCES.txt
--rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 10:12:42.000000 gw3-0.4/gw3.egg-info/dependency_links.txt
--rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-13 10:12:42.000000 gw3-0.4/gw3.egg-info/requires.txt
--rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-13 10:12:42.000000 gw3-0.4/gw3.egg-info/top_level.txt
--rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-13 10:12:42.505884 gw3-0.4/setup.cfg
--rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-13 10:11:32.000000 gw3-0.4/setup.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.267149 gw3-0.5/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:14:43.266664 gw3-0.5/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)     1447 2023-07-13 09:18:18.000000 gw3-0.5/README.md
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.264538 gw3-0.5/gw3/
+-rw-r--r--   0 colt       (501) staff       (20)       45 2023-07-13 10:10:43.000000 gw3-0.5/gw3/__init__.py
+-rw-r--r--   0 colt       (501) staff       (20)     5084 2023-07-13 09:18:18.000000 gw3-0.5/gw3/client.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:14:43.266147 gw3-0.5/gw3.egg-info/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/SOURCES.txt
+-rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/dependency_links.txt
+-rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/requires.txt
+-rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-13 10:14:43.000000 gw3-0.5/gw3.egg-info/top_level.txt
+-rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-13 10:14:43.267309 gw3-0.5/setup.cfg
+-rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-13 10:14:27.000000 gw3-0.5/setup.py
```

### Comparing `gw3-0.4/PKG-INFO` & `gw3-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.4
+Version: 0.5
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.4/README.md` & `gw3-0.5/README.md`

 * *Files identical despite different names*

### Comparing `gw3-0.4/gw3/client.py` & `gw3-0.5/gw3/client.py`

 * *Files identical despite different names*

### Comparing `gw3-0.4/gw3.egg-info/PKG-INFO` & `gw3-0.5/gw3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.4
+Version: 0.5
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.4/setup.py` & `gw3-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gw3',
-    version='0.4',
+    version='0.5',
     description='A Python client for the Gateway3 API',
     keywords=["gw3", "ipfs", "gateway3"],
     author='photon team',
     author_email='admin@photon.storage',
     url='https://github.com/photon-storage/gw3-sdk-python',
     packages=find_packages(),
     install_requires=[
```

