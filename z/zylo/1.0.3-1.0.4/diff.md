# Comparing `tmp/zylo-1.0.3.tar.gz` & `tmp/zylo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.3.tar", last modified: Wed Jul 12 22:00:33 2023, max compression
+gzip compressed data, was "zylo-1.0.4.tar", last modified: Wed Jul 12 22:09:21 2023, max compression
```

## Comparing `zylo-1.0.3.tar` & `zylo-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:00:32.995623 zylo-1.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:00:32.995623 zylo-1.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 22:00:32.995623 zylo-1.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-07-12 21:59:50.000000 zylo-1.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:00:32.991623 zylo-1.0.3/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.3/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 21:59:54.000000 zylo-1.0.3/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.3/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.3/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.3/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.3/zylo/sessions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.3/zylo/zylo.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:00:32.991623 zylo-1.0.3/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 22:00:32.000000 zylo-1.0.3/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:09:21.243657 zylo-1.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:09:21.243657 zylo-1.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.4/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 22:09:21.243657 zylo-1.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      900 2023-07-12 22:08:39.000000 zylo-1.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:09:21.239657 zylo-1.0.4/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.4/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2023-07-12 22:08:32.000000 zylo-1.0.4/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.4/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.4/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.4/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.4/zylo/sessions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.4/zylo/zylo.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:09:21.243657 zylo-1.0.4/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:09:21.000000 zylo-1.0.4/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2023-07-12 22:09:21.000000 zylo-1.0.4/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 22:09:21.000000 zylo-1.0.4/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 22:09:21.000000 zylo-1.0.4/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 22:09:21.000000 zylo-1.0.4/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.3/PKG-INFO` & `zylo-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zylo-1.0.3/setup.py` & `zylo-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.3',
+    version='1.0.4',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
@@ -19,13 +19,8 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-    entry_points={
-        'console_scripts': [
-            'zylo = zylo.zylo',  
-        ],
-    },
 )
```

### Comparing `zylo-1.0.3/zylo/JwT.py` & `zylo-1.0.4/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo/blueprint.py` & `zylo-1.0.4/zylo/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo/chiper.py` & `zylo-1.0.4/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo/mailer.py` & `zylo-1.0.4/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo/sessions.py` & `zylo-1.0.4/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo/zylo.py` & `zylo-1.0.4/zylo/zylo.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.3/zylo.egg-info/PKG-INFO` & `zylo-1.0.4/zylo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.3
+Version: 1.0.4
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

