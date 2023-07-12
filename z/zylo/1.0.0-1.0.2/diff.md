# Comparing `tmp/zylo-1.0.0.tar.gz` & `tmp/zylo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.0.tar", last modified: Wed Jul 12 21:48:52 2023, max compression
+gzip compressed data, was "zylo-1.0.2.tar", last modified: Wed Jul 12 21:55:43 2023, max compression
```

## Comparing `zylo-1.0.0.tar` & `zylo-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:48:52.216118 zylo-1.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 21:48:52.216118 zylo-1.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 21:48:52.216118 zylo-1.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-07-12 21:48:18.000000 zylo-1.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:48:52.216118 zylo-1.0.0/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.0/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 21:37:48.000000 zylo-1.0.0/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.0/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.0/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.0/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.0/zylo/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.0/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:48:52.216118 zylo-1.0.0/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 21:48:52.000000 zylo-1.0.0/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:55:43.415308 zylo-1.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 21:55:43.415308 zylo-1.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 21:55:43.415308 zylo-1.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1000 2023-07-12 21:54:51.000000 zylo-1.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:55:43.415308 zylo-1.0.2/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.2/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 21:37:48.000000 zylo-1.0.2/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.2/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.2/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.2/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.2/zylo/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.2/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 21:55:43.415308 zylo-1.0.2/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 21:55:43.000000 zylo-1.0.2/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.0/PKG-INFO` & `zylo-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.0
+Version: 1.0.2
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zylo-1.0.0/setup.py` & `zylo-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.0',
+    version='1.0.2',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
-    packages=['zylo'],
+    packages=find_packages(),
     install_requires=['werkzeug', 'jinja2', 'cryptography'],  
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `zylo-1.0.0/zylo/JwT.py` & `zylo-1.0.2/zylo/JwT.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo/blueprint.py` & `zylo-1.0.2/zylo/blueprint.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo/chiper.py` & `zylo-1.0.2/zylo/chiper.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo/mailer.py` & `zylo-1.0.2/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo/main.py` & `zylo-1.0.2/zylo/main.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo/sessions.py` & `zylo-1.0.2/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.0/zylo.egg-info/PKG-INFO` & `zylo-1.0.2/zylo.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.0
+Version: 1.0.2
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

