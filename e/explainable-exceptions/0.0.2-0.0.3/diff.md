# Comparing `tmp/explainable-exceptions-0.0.2.tar.gz` & `tmp/explainable-exceptions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainable-exceptions-0.0.2.tar", last modified: Wed Jul 12 10:43:18 2023, max compression
+gzip compressed data, was "explainable-exceptions-0.0.3.tar", last modified: Wed Jul 12 10:53:53 2023, max compression
```

## Comparing `explainable-exceptions-0.0.2.tar` & `explainable-exceptions-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:43:18.904757 explainable-exceptions-0.0.2/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.2/LICENSE
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.2/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4912 2023-07-12 10:43:18.904757 explainable-exceptions-0.0.2/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3269 2023-07-12 10:42:31.000000 explainable-exceptions-0.0.2/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:43:18.904757 explainable-exceptions-0.0.2/explainable_exceptions/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-12 10:43:14.000000 explainable-exceptions-0.0.2/explainable_exceptions/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      852 2023-07-12 10:43:14.000000 explainable-exceptions-0.0.2/explainable_exceptions/_modidx.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     3117 2023-07-12 10:43:14.000000 explainable-exceptions-0.0.2/explainable_exceptions/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:43:18.904757 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4912 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-12 10:43:18.000000 explainable-exceptions-0.0.2/explainable_exceptions.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      892 2023-07-12 10:43:06.000000 explainable-exceptions-0.0.2/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-12 10:43:18.904757 explainable-exceptions-0.0.2/setup.cfg
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.2/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:53:53.780771 explainable-exceptions-0.0.3/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.3/LICENSE
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      111 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.3/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5203 2023-07-12 10:53:53.780771 explainable-exceptions-0.0.3/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3479 2023-07-12 10:53:47.000000 explainable-exceptions-0.0.3/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:53:53.780771 explainable-exceptions-0.0.3/explainable_exceptions/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       22 2023-07-12 10:53:44.000000 explainable-exceptions-0.0.3/explainable_exceptions/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      852 2023-07-12 10:53:44.000000 explainable-exceptions-0.0.3/explainable_exceptions/_modidx.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3117 2023-07-12 10:53:44.000000 explainable-exceptions-0.0.3/explainable_exceptions/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-07-12 10:53:53.780771 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     5203 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      474 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       87 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-07-11 10:07:23.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       15 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       23 2023-07-12 10:53:53.000000 explainable-exceptions-0.0.3/explainable_exceptions.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      924 2023-07-12 10:53:41.000000 explainable-exceptions-0.0.3/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-07-12 10:53:53.780771 explainable-exceptions-0.0.3/setup.cfg
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     2596 2023-07-10 10:17:06.000000 explainable-exceptions-0.0.3/setup.py
```

### Comparing `explainable-exceptions-0.0.2/LICENSE` & `explainable-exceptions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-0.0.2/PKG-INFO` & `explainable-exceptions-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 0.0.2
-Summary: A Python module to explain exceptions in execution-time using AOP
+Version: 0.0.3
+Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
         
@@ -53,14 +53,23 @@
         
         ``` python
         import random
         
         from explainable_exceptions.core import explain
         ```
         
+        The following cell must be preceded by:
+        
+        ``` py
+        %%explain <username>
+        ```
+        
+        Where `<username>` must be replaced (if provided) by the username of the
+        huggingchat account that will be used to request information.
+        
         ``` python
         random.choice([])
         ```
         
             CRITICAL:root:Traceback (most recent call last):
               File "/home/ruescog/explainable-exceptions/explainable_exceptions/core.py", line 78, in explain
                 exec(cell, globals(), local_ns)
```

### Comparing `explainable-exceptions-0.0.2/README.md` & `explainable-exceptions-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 
 ``` python
 import random
 
 from explainable_exceptions.core import explain
 ```
 
+The following cell must be preceded by:
+
+``` py
+%%explain <username>
+```
+
+Where `<username>` must be replaced (if provided) by the username of the
+huggingchat account that will be used to request information.
+
 ``` python
 random.choice([])
 ```
 
     CRITICAL:root:Traceback (most recent call last):
       File "/home/ruescog/explainable-exceptions/explainable_exceptions/core.py", line 78, in explain
         exec(cell, globals(), local_ns)
```

### Comparing `explainable-exceptions-0.0.2/explainable_exceptions/_modidx.py` & `explainable-exceptions-0.0.3/explainable_exceptions/_modidx.py`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-0.0.2/explainable_exceptions/core.py` & `explainable-exceptions-0.0.3/explainable_exceptions/core.py`

 * *Files identical despite different names*

### Comparing `explainable-exceptions-0.0.2/explainable_exceptions.egg-info/PKG-INFO` & `explainable-exceptions-0.0.3/explainable_exceptions.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: explainable-exceptions
-Version: 0.0.2
-Summary: A Python module to explain exceptions in execution-time using AOP
+Version: 0.0.3
+Summary: A Python module to explain exceptions in execution-time using a magic cell
 Home-page: https://github.com/ruescog/explainable-exceptions
 Author: ruescog
 Author-email: ruescog@unirioja.es
 License: Apache Software License 2.0
 Description: explainable-exceptions
         ================
         
@@ -53,14 +53,23 @@
         
         ``` python
         import random
         
         from explainable_exceptions.core import explain
         ```
         
+        The following cell must be preceded by:
+        
+        ``` py
+        %%explain <username>
+        ```
+        
+        Where `<username>` must be replaced (if provided) by the username of the
+        huggingchat account that will be used to request information.
+        
         ``` python
         random.choice([])
         ```
         
             CRITICAL:root:Traceback (most recent call last):
               File "/home/ruescog/explainable-exceptions/explainable_exceptions/core.py", line 78, in explain
                 exec(cell, globals(), local_ns)
```

### Comparing `explainable-exceptions-0.0.2/settings.ini` & `explainable-exceptions-0.0.3/settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = explainable-exceptions
 lib_name = explainable-exceptions
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = explainable_exceptions
 nbs_path = nbs
 recursive = True
@@ -17,19 +17,20 @@
 doc_baseurl = /explainable-exceptions
 git_url = https://github.com/ruescog/explainable-exceptions
 title = explainable-exceptions
 audience = Developers
 author = ruescog
 author_email = ruescog@unirioja.es
 copyright = 2023 onwards, ruescog
-description = A Python module to explain exceptions in execution-time using AOP
+description = A Python module to explain exceptions in execution-time using a magic cell
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = ruescog
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
+requirements = hugchat
```

### Comparing `explainable-exceptions-0.0.2/setup.py` & `explainable-exceptions-0.0.3/setup.py`

 * *Files identical despite different names*

