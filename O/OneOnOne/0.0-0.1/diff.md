# Comparing `tmp/OneOnOne-0.0.tar.gz` & `tmp/OneOnOne-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.0.tar", last modified: Wed Jul 12 15:25:28 2023, max compression
+gzip compressed data, was "OneOnOne-0.1.tar", last modified: Wed Jul 12 15:16:23 2023, max compression
```

## Comparing `OneOnOne-0.0.tar` & `OneOnOne-0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:25:28.666264 OneOnOne-0.0/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.0/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:25:28.661281 OneOnOne-0.0/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    14278 2023-07-12 15:24:01.000000 OneOnOne-0.0/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.0/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-10 13:11:12.000000 OneOnOne-0.0/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:02:49.000000 OneOnOne-0.0/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.0/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:25:28.664555 OneOnOne-0.0/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)      579 2023-07-12 15:25:28.000000 OneOnOne-0.0/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-12 15:25:28.000000 OneOnOne-0.0/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-12 15:25:28.000000 OneOnOne-0.0/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)       18 2023-07-12 15:25:28.000000 OneOnOne-0.0/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-12 15:25:28.000000 OneOnOne-0.0/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      579 2023-07-12 15:25:28.665441 OneOnOne-0.0/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)        7 2023-07-10 14:29:42.000000 OneOnOne-0.0/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-12 15:25:28.667885 OneOnOne-0.0/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)      770 2023-07-12 15:25:07.000000 OneOnOne-0.0/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:16:23.067580 OneOnOne-0.1/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.1/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:16:23.065435 OneOnOne-0.1/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-12 14:59:10.000000 OneOnOne-0.1/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.1/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-10 13:11:12.000000 OneOnOne-0.1/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:02:49.000000 OneOnOne-0.1/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.1/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:16:23.066783 OneOnOne-0.1/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)      470 2023-07-12 15:16:22.000000 OneOnOne-0.1/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      276 2023-07-12 15:16:22.000000 OneOnOne-0.1/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-12 15:16:22.000000 OneOnOne-0.1/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-12 15:16:22.000000 OneOnOne-0.1/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      470 2023-07-12 15:16:23.067169 OneOnOne-0.1/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)        7 2023-07-10 14:29:42.000000 OneOnOne-0.1/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-12 15:16:23.067707 OneOnOne-0.1/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)      703 2023-07-12 15:16:04.000000 OneOnOne-0.1/setup.py
```

### Comparing `OneOnOne-0.0/LICENSE` & `OneOnOne-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.0/OneOnOne/__init__.py` & `OneOnOne-0.1/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import datetime
 import seaborn as sns
 import zipfile
 from zipfile import ZipFile
 import random
 
+import classes.py
 import tensorflow as tf
 import tensorflow.keras
 from tensorflow.keras.models import load_model
 import tensorflow_datasets as tfds
 from tensorflow.keras.datasets import cifar10
 from tensorflow.python.keras.layers import Input, Dense
 from tensorflow.keras.layers import Dense, Flatten
```

### Comparing `OneOnOne-0.0/OneOnOne/classes.py` & `OneOnOne-0.1/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.0/OneOnOne/classification.py` & `OneOnOne-0.1/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.0/setup.py` & `OneOnOne-0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.0
+VERSION=0.1
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION=""
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","numpy","pandas"])
+setup(name="OneOnOne",version=VERSION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS)
```

