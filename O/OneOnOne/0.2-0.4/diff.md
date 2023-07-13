# Comparing `tmp/OneOnOne-0.2.tar.gz` & `tmp/OneOnOne-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.2.tar", last modified: Thu Jul 13 13:53:16 2023, max compression
+gzip compressed data, was "OneOnOne-0.4.tar", last modified: Thu Jul 13 15:33:36 2023, max compression
```

## Comparing `OneOnOne-0.2.tar` & `OneOnOne-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 13:53:16.058111 OneOnOne-0.2/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.2/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 13:53:16.055589 OneOnOne-0.2/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    33852 2023-07-13 13:52:45.000000 OneOnOne-0.2/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.2/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.2/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.2/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.2/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 13:53:16.057325 OneOnOne-0.2/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1576 2023-07-13 13:53:15.000000 OneOnOne-0.2/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 13:53:16.000000 OneOnOne-0.2/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 13:53:15.000000 OneOnOne-0.2/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      112 2023-07-13 13:53:15.000000 OneOnOne-0.2/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 13:53:15.000000 OneOnOne-0.2/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1576 2023-07-13 13:53:16.057747 OneOnOne-0.2/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.2/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 13:53:16.058225 OneOnOne-0.2/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1918 2023-07-12 20:16:34.000000 OneOnOne-0.2/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 15:33:36.489889 OneOnOne-0.4/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.4/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 15:33:36.487206 OneOnOne-0.4/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    33881 2023-07-13 13:55:25.000000 OneOnOne-0.4/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.4/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.4/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.4/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.4/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 15:33:36.488829 OneOnOne-0.4/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 15:33:36.000000 OneOnOne-0.4/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 15:33:36.000000 OneOnOne-0.4/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 15:33:36.000000 OneOnOne-0.4/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)       93 2023-07-13 15:33:36.000000 OneOnOne-0.4/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 15:33:36.000000 OneOnOne-0.4/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1575 2023-07-13 15:33:36.489261 OneOnOne-0.4/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.4/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 15:33:36.490074 OneOnOne-0.4/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1892 2023-07-13 15:33:32.000000 OneOnOne-0.4/setup.py
```

### Comparing `OneOnOne-0.2/LICENSE` & `OneOnOne-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.2/OneOnOne/__init__.py` & `OneOnOne-0.4/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,27 +34,29 @@
 
 import torch
 from torchvision import transforms
 from torch.utils.data import Dataset
 from tqdm import keras
 
 
-class PretrainedModels:
+class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", sampling="none"):
 
         self.model_type=model_type
         self.dataset=dataset
         self.sampling=sampling
 
         if self.dataset=="tinyimagenet":
             self.model_type="efficientnetb6"
             self.sampling="none"
 
         self.model=load_model(OneOnOne/f"{self.model_type}_{self.dataset}_{self.sampling}")
 
+        self.model.summary()
+
 
 
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
 
         self.model_type = model_type
         self.date=datetime.datetime.now()
```

### Comparing `OneOnOne-0.2/OneOnOne/classes.py` & `OneOnOne-0.4/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.2/OneOnOne/classification.py` & `OneOnOne-0.4/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.2/OneOnOne/contextdecider.py` & `OneOnOne-0.4/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.2/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.4/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.2
+Version: 0.4
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-#Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
+Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
```

### Comparing `OneOnOne-0.2/PKG-INFO` & `OneOnOne-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.2
+Version: 0.4
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-#Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
+Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
```

### Comparing `OneOnOne-0.2/README.md` & `OneOnOne-0.4/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.2/setup.py` & `OneOnOne-0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.2
+VERSION=0.4
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
-LONG_DESCRIPTION="#Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
+LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","numpy","pandas","tensorflow","sklearn","datetime","os","zipfile","keras","math","torch","tensorflow_datasets","scipy","pickle","tqdm"])
+setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","numpy","pandas","tensorflow","datetime","keras","math","torch","tensorflow_datasets","scipy","pickle","tqdm"])
```

