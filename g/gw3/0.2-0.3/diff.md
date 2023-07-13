# Comparing `tmp/gw3-0.2.tar.gz` & `tmp/gw3-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw3-0.2.tar", last modified: Thu Jul 13 09:20:49 2023, max compression
+gzip compressed data, was "gw3-0.3.tar", last modified: Thu Jul 13 10:02:46 2023, max compression
```

## Comparing `gw3-0.2.tar` & `gw3-0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 09:20:49.003909 gw3-0.2/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 09:20:49.003628 gw3-0.2/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)     1447 2023-07-13 09:18:18.000000 gw3-0.2/README.md
-drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 09:20:49.003142 gw3-0.2/gw3.egg-info/
--rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 09:20:48.000000 gw3-0.2/gw3.egg-info/PKG-INFO
--rw-r--r--   0 colt       (501) staff       (20)      152 2023-07-13 09:20:48.000000 gw3-0.2/gw3.egg-info/SOURCES.txt
--rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 09:20:48.000000 gw3-0.2/gw3.egg-info/dependency_links.txt
--rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-13 09:20:48.000000 gw3-0.2/gw3.egg-info/requires.txt
--rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 09:20:48.000000 gw3-0.2/gw3.egg-info/top_level.txt
--rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-13 09:20:49.004036 gw3-0.2/setup.cfg
--rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-13 09:18:18.000000 gw3-0.2/setup.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:02:46.267163 gw3-0.3/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:02:46.246812 gw3-0.3/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)     1447 2023-07-13 09:18:18.000000 gw3-0.3/README.md
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:02:46.244243 gw3-0.3/gw3/
+-rw-r--r--   0 colt       (501) staff       (20)        0 2023-07-13 10:01:50.000000 gw3-0.3/gw3/__init__.py
+-rw-r--r--   0 colt       (501) staff       (20)     5084 2023-07-13 09:18:18.000000 gw3-0.3/gw3/client.py
+drwxr-xr-x   0 colt       (501) staff       (20)        0 2023-07-13 10:02:46.246154 gw3-0.3/gw3.egg-info/
+-rw-r--r--   0 colt       (501) staff       (20)      643 2023-07-13 10:02:46.000000 gw3-0.3/gw3.egg-info/PKG-INFO
+-rw-r--r--   0 colt       (501) staff       (20)      182 2023-07-13 10:02:46.000000 gw3-0.3/gw3.egg-info/SOURCES.txt
+-rw-r--r--   0 colt       (501) staff       (20)        1 2023-07-13 10:02:46.000000 gw3-0.3/gw3.egg-info/dependency_links.txt
+-rw-r--r--   0 colt       (501) staff       (20)        9 2023-07-13 10:02:46.000000 gw3-0.3/gw3.egg-info/requires.txt
+-rw-r--r--   0 colt       (501) staff       (20)        4 2023-07-13 10:02:46.000000 gw3-0.3/gw3.egg-info/top_level.txt
+-rw-r--r--   0 colt       (501) staff       (20)       38 2023-07-13 10:02:46.267404 gw3-0.3/setup.cfg
+-rw-r--r--   0 colt       (501) staff       (20)      781 2023-07-13 09:59:29.000000 gw3-0.3/setup.py
```

### Comparing `gw3-0.2/PKG-INFO` & `gw3-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.2
+Version: 0.3
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.2/README.md` & `gw3-0.3/README.md`

 * *Files identical despite different names*

### Comparing `gw3-0.2/gw3.egg-info/PKG-INFO` & `gw3-0.3/gw3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gw3
-Version: 0.2
+Version: 0.3
 Summary: A Python client for the Gateway3 API
 Home-page: https://github.com/photon-storage/gw3-sdk-python
 Author: photon team
 Author-email: admin@photon.storage
 License: UNKNOWN
 Keywords: gw3,ipfs,gateway3
 Platform: UNKNOWN
```

### Comparing `gw3-0.2/setup.py` & `gw3-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gw3',
-    version='0.2',
+    version='0.3',
     description='A Python client for the Gateway3 API',
     keywords=["gw3", "ipfs", "gateway3"],
     author='photon team',
     author_email='admin@photon.storage',
     url='https://github.com/photon-storage/gw3-sdk-python',
     packages=find_packages(),
     install_requires=[
```

