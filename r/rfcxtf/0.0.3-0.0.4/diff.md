# Comparing `tmp/rfcxtf-0.0.3.tar.gz` & `tmp/rfcxtf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcxtf-0.0.3.tar", last modified: Fri May  5 11:19:31 2023, max compression
+gzip compressed data, was "rfcxtf-0.0.4.tar", last modified: Thu Jul 13 17:42:23 2023, max compression
```

## Comparing `rfcxtf-0.0.3.tar` & `rfcxtf-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:31.007766 rfcxtf-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 11:19:31.006429 rfcxtf-0.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:30.950410 rfcxtf-0.0.3/rfcxtf/
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.3/rfcxtf/ClassifierBase.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.3/rfcxtf/ClassifierTF2.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.3/rfcxtf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:31.000812 rfcxtf-0.0.3/rfcxtf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:11:18.000000 rfcxtf-0.0.3/rfcxtf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/io.py
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/postprocessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:30.978975 rfcxtf-0.0.3/rfcxtf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      326 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 11:19:31.008679 rfcxtf-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-05 11:17:07.000000 rfcxtf-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.487449 rfcxtf-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-13 17:42:23.486313 rfcxtf-0.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.436553 rfcxtf-0.0.4/rfcxtf/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.4/rfcxtf/ClassifierBase.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.4/rfcxtf/ClassifierTF2.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.4/rfcxtf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.481461 rfcxtf-0.0.4/rfcxtf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:11:18.000000 rfcxtf-0.0.4/rfcxtf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-04 09:05:14.000000 rfcxtf-0.0.4/rfcxtf/utils/postprocessor.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2023-07-08 19:32:57.000000 rfcxtf-0.0.4/rfcxtf/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 17:42:23.462453 rfcxtf-0.0.4/rfcxtf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-13 17:42:23.000000 rfcxtf-0.0.4/rfcxtf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 17:42:23.488033 rfcxtf-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-13 17:41:19.000000 rfcxtf-0.0.4/setup.py
```

### Comparing `rfcxtf-0.0.3/rfcxtf/ClassifierBase.py` & `rfcxtf-0.0.4/rfcxtf/ClassifierBase.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.3/rfcxtf/ClassifierTF2.py` & `rfcxtf-0.0.4/rfcxtf/ClassifierTF2.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.3/setup.py` & `rfcxtf-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 REQUIRED_PACKAGES = ['tensorflow', 'pysndfile', 'numpy']
 
 setup(name='rfcxtf',
-      version='0.0.3',
+      version='0.0.4',
       url='https://github.com/rfcx/rfcx-sdk-python',
       license='None',
       author='Rainforest Connection',
       author_email='antony@rfcx.org',
       install_requires=REQUIRED_PACKAGES,
       description='Support for building TensorFlow classifiers on Arbimon and Guardian platforms',
       packages=find_packages(exclude=['tests']),
```

