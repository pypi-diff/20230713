# Comparing `tmp/Py-SPW-1.5.0h.tar.gz` & `tmp/Py-SPW-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Py-SPW-1.5.0.tar", last modified: Thu Jul 13 13:28:20 2023, max compression
+gzip compressed data, was "Py-SPW-1.5.1.tar", last modified: Thu Jul 13 13:50:07 2023, max compression
```

## Comparing `Py-SPW-1.5.0h.tar` & `Py-SPW-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:28:20.955751 Py-SPW-1.5.0/
--rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-1.5.0/LICENSE
--rw-r--r--   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-1.5.0/MANIFEST.in
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:28:20.955751 Py-SPW-1.5.0/PKG-INFO
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:28:20.955751 Py-SPW-1.5.0/Py_SPW.egg-info/
--rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:28:20.000000 Py-SPW-1.5.0/Py_SPW.egg-info/PKG-INFO
--rw-rw-r--   0 stepan    (1000) stepan    (1000)      285 2023-07-13 13:28:20.000000 Py-SPW-1.5.0/Py_SPW.egg-info/SOURCES.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-07-13 13:28:20.000000 Py-SPW-1.5.0/Py_SPW.egg-info/dependency_links.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-07-13 13:28:20.000000 Py-SPW-1.5.0/Py_SPW.egg-info/requires.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-07-13 13:28:20.000000 Py-SPW-1.5.0/Py_SPW.egg-info/top_level.txt
--rw-r--r--   0 stepan    (1000) stepan    (1000)      945 2023-05-09 10:37:44.000000 Py-SPW-1.5.0/README.md
-drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:28:20.955751 Py-SPW-1.5.0/pyspw/
--rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-09 10:37:42.000000 Py-SPW-1.5.0/pyspw/Parameters.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     3634 2023-05-09 10:37:42.000000 Py-SPW-1.5.0/pyspw/User.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       19 2023-07-13 13:19:16.000000 Py-SPW-1.5.0/pyspw/__init__.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     9956 2023-05-09 10:37:42.000000 Py-SPW-1.5.0/pyspw/api.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-09 10:37:41.000000 Py-SPW-1.5.0/pyspw/errors.py
--rw-r--r--   0 stepan    (1000) stepan    (1000)       85 2023-05-09 10:37:41.000000 Py-SPW-1.5.0/requirements.txt
--rw-rw-r--   0 stepan    (1000) stepan    (1000)       38 2023-07-13 13:28:20.955751 Py-SPW-1.5.0/setup.cfg
--rw-r--r--   0 stepan    (1000) stepan    (1000)      826 2023-07-13 13:19:16.000000 Py-SPW-1.5.0/setup.py
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/
+-rwxrwxr-x   0 stepan    (1000) stepan    (1000)     1085 2023-05-09 10:37:44.000000 Py-SPW-1.5.1/LICENSE
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       58 2023-07-13 13:18:30.000000 Py-SPW-1.5.1/MANIFEST.in
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/PKG-INFO
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/Py_SPW.egg-info/
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)     1355 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/PKG-INFO
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)      285 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/SOURCES.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        1 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/dependency_links.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)       86 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/requires.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)        6 2023-07-13 13:50:07.000000 Py-SPW-1.5.1/Py_SPW.egg-info/top_level.txt
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      945 2023-05-09 10:37:44.000000 Py-SPW-1.5.1/README.md
+drwxrwxr-x   0 stepan    (1000) stepan    (1000)        0 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/pyspw/
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     2661 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/Parameters.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     3634 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/User.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       19 2023-07-13 13:19:16.000000 Py-SPW-1.5.1/pyspw/__init__.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     9956 2023-05-09 10:37:42.000000 Py-SPW-1.5.1/pyspw/api.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)     1728 2023-05-09 10:37:41.000000 Py-SPW-1.5.1/pyspw/errors.py
+-rw-r--r--   0 stepan    (1000) stepan    (1000)       85 2023-05-09 10:37:41.000000 Py-SPW-1.5.1/requirements.txt
+-rw-rw-r--   0 stepan    (1000) stepan    (1000)       38 2023-07-13 13:50:07.135835 Py-SPW-1.5.1/setup.cfg
+-rw-r--r--   0 stepan    (1000) stepan    (1000)      826 2023-07-13 13:50:06.000000 Py-SPW-1.5.1/setup.py
```

### Comparing `Py-SPW-1.5.0/LICENSE` & `Py-SPW-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/PKG-INFO` & `Py-SPW-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
```

### Comparing `Py-SPW-1.5.0/Py_SPW.egg-info/PKG-INFO` & `Py-SPW-1.5.1/Py_SPW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Py-SPW
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python library for spworlds API
 Home-page: https://github.com/teleportx/Py-SPW
 Author: Stepan Khozhempo
 Author-email: stepan@xstl.ru
 License: MIT License
 Project-URL: Docs, https://pyspw.xstl.ru/en/latest/
 Project-URL: GitHub, https://github.com/teleport2/Py-SPW/
```

### Comparing `Py-SPW-1.5.0/README.md` & `Py-SPW-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/pyspw/Parameters.py` & `Py-SPW-1.5.1/pyspw/Parameters.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/pyspw/User.py` & `Py-SPW-1.5.1/pyspw/User.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/pyspw/api.py` & `Py-SPW-1.5.1/pyspw/api.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/pyspw/errors.py` & `Py-SPW-1.5.1/pyspw/errors.py`

 * *Files identical despite different names*

### Comparing `Py-SPW-1.5.0/setup.py` & `Py-SPW-1.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     description_md = f.read()
 
 requirements = open('requirements.txt', 'r').read().split('\n')
 
 setup(
     name='Py-SPW',
-    version='1.5.0',
+    version='1.5.1',
     packages=['pyspw'],
     url='https://github.com/teleportx/Py-SPW',
     license='MIT License',
     author='Stepan Khozhempo',
     author_email='stepan@xstl.ru',
     description='Python library for spworlds API',
     long_description=description_md,
```

