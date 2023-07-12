# Comparing `tmp/zylo-1.0.6.tar.gz` & `tmp/zylo-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.6.tar", last modified: Wed Jul 12 22:29:07 2023, max compression
+gzip compressed data, was "zylo-1.0.7.tar", last modified: Wed Jul 12 22:34:00 2023, max compression
```

## Comparing `zylo-1.0.6.tar` & `zylo-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:29:07.709672 zylo-1.0.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:29:07.709672 zylo-1.0.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.6/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 22:29:07.709672 zylo-1.0.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-07-12 22:27:58.000000 zylo-1.0.6/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:29:07.709672 zylo-1.0.6/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.6/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 22:27:01.000000 zylo-1.0.6/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.6/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.6/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.6/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.6/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.6/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:29:07.709672 zylo-1.0.6/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 22:29:07.000000 zylo-1.0.6/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.531790 zylo-1.0.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:34:00.531790 zylo-1.0.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.7/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 22:34:00.531790 zylo-1.0.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-07-12 22:33:12.000000 zylo-1.0.7/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.527789 zylo-1.0.7/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.7/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 22:27:01.000000 zylo-1.0.7/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.7/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.7/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.7/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.7/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.7/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.531790 zylo-1.0.7/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.6/PKG-INFO` & `zylo-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.6
+Version: 1.0.7
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zylo-1.0.6/setup.py` & `zylo-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.6',
+    version='1.0.7',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
@@ -21,11 +21,11 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     entry_points={
         'console_scripts': [
-            'zylo = zylo.app:app',  
+            'zylo = zylo.app',  
         ],
     },
 )
```

### Comparing `zylo-1.0.6/zylo/JwT.py` & `zylo-1.0.7/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo/app.py` & `zylo-1.0.7/zylo/app.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo/blueprint.py` & `zylo-1.0.7/zylo/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo/chiper.py` & `zylo-1.0.7/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo/mailer.py` & `zylo-1.0.7/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo/sessions.py` & `zylo-1.0.7/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.6/zylo.egg-info/PKG-INFO` & `zylo-1.0.7/zylo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.6
+Version: 1.0.7
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

