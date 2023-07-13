# Comparing `tmp/OneOnOne-0.5.tar.gz` & `tmp/OneOnOne-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.5.tar", last modified: Thu Jul 13 16:10:00 2023, max compression
+gzip compressed data, was "OneOnOne-0.6.tar", last modified: Thu Jul 13 16:12:57 2023, max compression
```

## Comparing `OneOnOne-0.5.tar` & `OneOnOne-0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:10:00.242258 OneOnOne-0.5/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.5/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:10:00.238462 OneOnOne-0.5/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    33881 2023-07-13 13:55:25.000000 OneOnOne-0.5/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.5/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.5/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.5/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.5/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:10:00.241007 OneOnOne-0.5/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 16:10:00.000000 OneOnOne-0.5/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 16:10:00.000000 OneOnOne-0.5/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 16:10:00.000000 OneOnOne-0.5/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      118 2023-07-13 16:10:00.000000 OneOnOne-0.5/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 16:10:00.000000 OneOnOne-0.5/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 16:10:00.241623 OneOnOne-0.5/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.5/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 16:10:00.242514 OneOnOne-0.5/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1915 2023-07-13 16:09:55.000000 OneOnOne-0.5/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:12:57.024516 OneOnOne-0.6/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:12:57.022233 OneOnOne-0.6/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    33881 2023-07-13 13:55:25.000000 OneOnOne-0.6/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.6/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.6/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.6/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 16:12:57.023739 OneOnOne-0.6/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 16:12:56.000000 OneOnOne-0.6/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 16:12:56.000000 OneOnOne-0.6/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 16:12:56.000000 OneOnOne-0.6/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      111 2023-07-13 16:12:56.000000 OneOnOne-0.6/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 16:12:56.000000 OneOnOne-0.6/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 16:12:57.024146 OneOnOne-0.6/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.6/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 16:12:57.024626 OneOnOne-0.6/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1906 2023-07-13 16:12:52.000000 OneOnOne-0.6/setup.py
```

### Comparing `OneOnOne-0.5/LICENSE` & `OneOnOne-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/OneOnOne/__init__.py` & `OneOnOne-0.6/OneOnOne/__init__.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/OneOnOne/classes.py` & `OneOnOne-0.6/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/OneOnOne/classification.py` & `OneOnOne-0.6/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/OneOnOne/contextdecider.py` & `OneOnOne-0.6/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6/OneOnOne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.5
+Version: 0.6
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.5/PKG-INFO` & `OneOnOne-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.5
+Version: 0.6
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.5/README.md` & `OneOnOne-0.6/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.5/setup.py` & `OneOnOne-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.5
+VERSION=0.6
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","numpy","pandas","tensorflow","datetime","keras==1.2.2","torch","tensorflow_datasets==4.9.2","scipy==1.10.1","pickle","tqdm==4.65.0"])
+setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","numpy","pandas","tensorflow","datetime","keras==1.2.2","torch","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
```

