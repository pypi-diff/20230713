# Comparing `tmp/deairequest-0.0.8.tar.gz` & `tmp/deairequest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deairequest-0.0.8.tar", last modified: Sat Jul  1 06:19:18 2023, max compression
+gzip compressed data, was "deairequest-0.0.9.tar", last modified: Sat Jul  1 10:10:17 2023, max compression
```

## Comparing `deairequest-0.0.8.tar` & `deairequest-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.209898 deairequest-0.0.8/
--rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 06:19:18.210025 deairequest-0.0.8/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)     1600 2023-06-30 11:32:54.000000 deairequest-0.0.8/README.md
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.198661 deairequest-0.0.8/deairequest/
--rw-r--r--   0 maarten    (501) staff       (20)     7942 2023-07-01 05:54:37.000000 deairequest-0.0.8/deairequest/BacalhauProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)     2072 2023-06-28 08:10:07.000000 deairequest-0.0.8/deairequest/DeProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)      320 2023-06-06 08:41:48.000000 deairequest-0.0.8/deairequest/DeProtocolSelector.py
--rw-r--r--   0 maarten    (501) staff       (20)     1594 2023-06-28 08:14:29.000000 deairequest-0.0.8/deairequest/ErrorProtocol.py
--rw-r--r--   0 maarten    (501) staff       (20)      122 2023-05-30 07:49:58.000000 deairequest-0.0.8/deairequest/__init__.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.202136 deairequest-0.0.8/deairequest/connectors/
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:00.000000 deairequest-0.0.8/deairequest/connectors/__init__.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.209214 deairequest-0.0.8/deairequest/connectors/bacalhau/
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:59.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/__init__.py
--rw-r--r--   0 maarten    (501) staff       (20)      826 2023-06-28 14:29:45.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/backends.py
--rw-r--r--   0 maarten    (501) staff       (20)     2289 2023-06-26 13:55:09.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/code.py
--rw-r--r--   0 maarten    (501) staff       (20)     6891 2023-06-30 10:20:51.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/deploy.py
--rw-r--r--   0 maarten    (501) staff       (20)      623 2023-06-28 16:29:54.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/main.py
--rw-r--r--   0 maarten    (501) staff       (20)    26812 2023-06-10 08:19:26.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/mapping.py
--rw-r--r--   0 maarten    (501) staff       (20)     4795 2023-06-28 14:30:52.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/notebooks.py
--rw-r--r--   0 maarten    (501) staff       (20)     3366 2023-07-01 05:28:17.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/querybhl.py
--rw-r--r--   0 maarten    (501) staff       (20)     4269 2023-07-01 06:18:34.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/render.py
--rw-r--r--   0 maarten    (501) staff       (20)    36617 2023-06-10 08:19:26.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/stdlib.py
--rw-r--r--   0 maarten    (501) staff       (20)     2246 2023-06-26 08:46:32.000000 deairequest-0.0.8/deairequest/connectors/bacalhau/step.py
--rw-r--r--   0 maarten    (501) staff       (20)     1571 2023-06-06 08:59:18.000000 deairequest-0.0.8/deairequest/logo.svg
--rw-r--r--   0 maarten    (501) staff       (20)     7484 2023-06-30 09:24:04.000000 deairequest-0.0.8/deairequest/test.ipynb
--rw-r--r--   0 maarten    (501) staff       (20)     7325 2023-07-01 06:14:39.000000 deairequest-0.0.8/deairequest/test_DeAIRequest.py
-drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 06:19:18.201395 deairequest-0.0.8/deairequest.egg-info/
--rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/PKG-INFO
--rw-r--r--   0 maarten    (501) staff       (20)      926 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/SOURCES.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/dependency_links.txt
--rw-r--r--   0 maarten    (501) staff       (20)       12 2023-07-01 06:19:18.000000 deairequest-0.0.8/deairequest.egg-info/top_level.txt
--rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-21 08:22:51.000000 deairequest-0.0.8/deairequest.egg-info/zip-safe
--rw-r--r--   0 maarten    (501) staff       (20)      983 2023-07-01 05:56:52.000000 deairequest-0.0.8/pyproject.toml
--rw-r--r--   0 maarten    (501) staff       (20)      152 2023-07-01 06:19:18.210482 deairequest-0.0.8/setup.cfg
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 10:10:17.980692 deairequest-0.0.9/
+-rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 10:10:17.980807 deairequest-0.0.9/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)     1600 2023-06-30 11:32:54.000000 deairequest-0.0.9/README.md
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 10:10:17.971433 deairequest-0.0.9/deairequest/
+-rw-r--r--   0 maarten    (501) staff       (20)     7942 2023-07-01 05:54:37.000000 deairequest-0.0.9/deairequest/BacalhauProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2072 2023-06-28 08:10:07.000000 deairequest-0.0.9/deairequest/DeProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)      320 2023-06-06 08:41:48.000000 deairequest-0.0.9/deairequest/DeProtocolSelector.py
+-rw-r--r--   0 maarten    (501) staff       (20)     1594 2023-06-28 08:14:29.000000 deairequest-0.0.9/deairequest/ErrorProtocol.py
+-rw-r--r--   0 maarten    (501) staff       (20)      122 2023-05-30 07:49:58.000000 deairequest-0.0.9/deairequest/__init__.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 10:10:17.974343 deairequest-0.0.9/deairequest/connectors/
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:00.000000 deairequest-0.0.9/deairequest/connectors/__init__.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 10:10:17.980223 deairequest-0.0.9/deairequest/connectors/bacalhau/
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-26 13:58:59.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/__init__.py
+-rw-r--r--   0 maarten    (501) staff       (20)      826 2023-06-28 14:29:45.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/backends.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2289 2023-06-26 13:55:09.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/code.py
+-rw-r--r--   0 maarten    (501) staff       (20)     6891 2023-06-30 10:20:51.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/deploy.py
+-rw-r--r--   0 maarten    (501) staff       (20)      623 2023-06-28 16:29:54.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/main.py
+-rw-r--r--   0 maarten    (501) staff       (20)    26812 2023-06-10 08:19:26.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/mapping.py
+-rw-r--r--   0 maarten    (501) staff       (20)     4795 2023-06-28 14:30:52.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/notebooks.py
+-rw-r--r--   0 maarten    (501) staff       (20)     3366 2023-07-01 05:28:17.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/querybhl.py
+-rw-r--r--   0 maarten    (501) staff       (20)     4289 2023-07-01 10:10:10.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/render.py
+-rw-r--r--   0 maarten    (501) staff       (20)    36617 2023-06-10 08:19:26.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/stdlib.py
+-rw-r--r--   0 maarten    (501) staff       (20)     2246 2023-06-26 08:46:32.000000 deairequest-0.0.9/deairequest/connectors/bacalhau/step.py
+-rw-r--r--   0 maarten    (501) staff       (20)     1571 2023-06-06 08:59:18.000000 deairequest-0.0.9/deairequest/logo.svg
+-rw-r--r--   0 maarten    (501) staff       (20)     7484 2023-06-30 09:24:04.000000 deairequest-0.0.9/deairequest/test.ipynb
+-rw-r--r--   0 maarten    (501) staff       (20)     7325 2023-07-01 06:14:39.000000 deairequest-0.0.9/deairequest/test_DeAIRequest.py
+drwxr-xr-x   0 maarten    (501) staff       (20)        0 2023-07-01 10:10:17.973656 deairequest-0.0.9/deairequest.egg-info/
+-rw-r--r--   0 maarten    (501) staff       (20)     2116 2023-07-01 10:10:17.000000 deairequest-0.0.9/deairequest.egg-info/PKG-INFO
+-rw-r--r--   0 maarten    (501) staff       (20)      926 2023-07-01 10:10:17.000000 deairequest-0.0.9/deairequest.egg-info/SOURCES.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-07-01 10:10:17.000000 deairequest-0.0.9/deairequest.egg-info/dependency_links.txt
+-rw-r--r--   0 maarten    (501) staff       (20)       12 2023-07-01 10:10:17.000000 deairequest-0.0.9/deairequest.egg-info/top_level.txt
+-rw-r--r--   0 maarten    (501) staff       (20)        1 2023-06-21 08:22:51.000000 deairequest-0.0.9/deairequest.egg-info/zip-safe
+-rw-r--r--   0 maarten    (501) staff       (20)      983 2023-07-01 10:09:52.000000 deairequest-0.0.9/pyproject.toml
+-rw-r--r--   0 maarten    (501) staff       (20)      152 2023-07-01 10:10:17.981260 deairequest-0.0.9/setup.cfg
```

### Comparing `deairequest-0.0.8/PKG-INFO` & `deairequest-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deairequest
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Decentralised AI library which allows to run remote AI jobs
 Author-email: Maarten Ectors <maarten@0011.ai>
 Project-URL: Homepage, https://github.com/0011ai/deairequest
 Project-URL: Bug Tracker, https://github.com/0011ai/deairequest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deairequest-0.0.8/README.md` & `deairequest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/BacalhauProtocol.py` & `deairequest-0.0.9/deairequest/BacalhauProtocol.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/DeProtocol.py` & `deairequest-0.0.9/deairequest/DeProtocol.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/ErrorProtocol.py` & `deairequest-0.0.9/deairequest/ErrorProtocol.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/backends.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/backends.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/code.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/code.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/deploy.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/deploy.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/main.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/main.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/mapping.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/mapping.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/notebooks.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/notebooks.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/querybhl.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/querybhl.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/render.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,26 +71,26 @@
             f3.close()
 
         # Download the remaining packages
         wheelsdir=os.path.join(target,"wheels")
         pythonversion=config.get('environments').get('default').get('python')
         for install in toinstall:
             try:
-                #download specific version
-                subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",install])        
+                #download specific version for specific platform
+                y=re.split("([A-z-?]+)",install)
+                subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "manylinux2014_x86_64", "-d",wheelsdir,"--only-binary=:all:",install])        
             except Exception as excep:
                 try:
-                    #download any version
-                    y=re.split("([A-z-?]+)",install)
-                    subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",y[1]])        
+                    #download specific version for linux
+                    subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",install])        
                 except Exception as excep:
                     try:
-                        #download without dependencies
+                        #download any version
                         y=re.split("([A-z-?]+)",install)
-                        subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "manylinux2014_x86_64", "-d",wheelsdir,"--only-binary=:all:",y[1]])        
+                        subprocess.check_call([sys.executable, "-m", "pip", "download", "--python-version", pythonversion, "--platform", "linux_x86_64", "-d",wheelsdir,"--only-binary=:all:",y[1]]) 
                     except Exception as excep:
                         # fail if neither works
                         raise Exception(f"Sorry but we cannot download the package {install}, please use a docker image that includes this package")
  
     else:
         # Nothing to install
         os.remove(req)
```

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/stdlib.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/stdlib.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/connectors/bacalhau/step.py` & `deairequest-0.0.9/deairequest/connectors/bacalhau/step.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/logo.svg` & `deairequest-0.0.9/deairequest/logo.svg`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/test.ipynb` & `deairequest-0.0.9/deairequest/test.ipynb`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest/test_DeAIRequest.py` & `deairequest-0.0.9/deairequest/test_DeAIRequest.py`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/deairequest.egg-info/PKG-INFO` & `deairequest-0.0.9/deairequest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deairequest
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Decentralised AI library which allows to run remote AI jobs
 Author-email: Maarten Ectors <maarten@0011.ai>
 Project-URL: Homepage, https://github.com/0011ai/deairequest
 Project-URL: Bug Tracker, https://github.com/0011ai/deairequest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deairequest-0.0.8/deairequest.egg-info/SOURCES.txt` & `deairequest-0.0.9/deairequest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deairequest-0.0.8/pyproject.toml` & `deairequest-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deairequest"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Maarten Ectors", email="maarten@0011.ai" }
 ]
 description = "A Decentralised AI library which allows to run remote AI jobs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

