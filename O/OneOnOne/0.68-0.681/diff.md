# Comparing `tmp/OneOnOne-0.68.tar.gz` & `tmp/OneOnOne-0.681.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.68.tar", last modified: Thu Jul 13 17:13:02 2023, max compression
+gzip compressed data, was "OneOnOne-0.681.tar", last modified: Thu Jul 13 17:15:12 2023, max compression
```

## Comparing `OneOnOne-0.68.tar` & `OneOnOne-0.681.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:13:02.872754 OneOnOne-0.68/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.68/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:13:02.869470 OneOnOne-0.68/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    33973 2023-07-13 17:12:57.000000 OneOnOne-0.68/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.68/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.68/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.68/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.68/OneOnOne/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:13:02.871761 OneOnOne-0.68/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1576 2023-07-13 17:13:02.000000 OneOnOne-0.68/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 17:13:02.000000 OneOnOne-0.68/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 17:13:02.000000 OneOnOne-0.68/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-13 17:13:02.000000 OneOnOne-0.68/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 17:13:02.000000 OneOnOne-0.68/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1576 2023-07-13 17:13:02.872269 OneOnOne-0.68/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.68/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 17:13:02.872897 OneOnOne-0.68/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1908 2023-07-13 17:12:57.000000 OneOnOne-0.68/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:15:12.909026 OneOnOne-0.681/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.681/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:15:12.906584 OneOnOne-0.681/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    33978 2023-07-13 17:14:57.000000 OneOnOne-0.681/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.681/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14754 2023-07-12 17:06:31.000000 OneOnOne-0.681/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1868 2023-07-12 19:25:09.000000 OneOnOne-0.681/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 OneOnOne-0.681/OneOnOne/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-13 17:15:12.908251 OneOnOne-0.681/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-13 17:15:12.000000 OneOnOne-0.681/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      307 2023-07-13 17:15:12.000000 OneOnOne-0.681/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-13 17:15:12.000000 OneOnOne-0.681/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      114 2023-07-13 17:15:12.000000 OneOnOne-0.681/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-13 17:15:12.000000 OneOnOne-0.681/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1577 2023-07-13 17:15:12.908663 OneOnOne-0.681/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     1606 2023-07-12 20:09:33.000000 OneOnOne-0.681/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-13 17:15:12.909138 OneOnOne-0.681/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1909 2023-07-13 17:15:06.000000 OneOnOne-0.681/setup.py
```

### Comparing `OneOnOne-0.68/LICENSE` & `OneOnOne-0.681/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.68/OneOnOne/__init__.py` & `OneOnOne-0.681/OneOnOne/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.sampling=sampling
 
         if self.dataset=="tinyimagenet":
             self.model_type="efficientnetb6"
             self.sampling="none"
 
         self.model=urllib.request.urlretrieve('https://github.com/sohini-bhattacharya/OneOnOne/blob/e4adf61b6c3b73a917b1f2b0d441318d981a5aa4/OneOnOne/resnet50_cifar10_none',f"{self.model_type}_{self.dataset}_{self.sampling}")
-        print(model)
+        print(self.model)
         self.model.summary()
 
 
 
 
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
```

### Comparing `OneOnOne-0.68/OneOnOne/classes.py` & `OneOnOne-0.681/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.68/OneOnOne/classification.py` & `OneOnOne-0.681/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.68/OneOnOne/contextdecider.py` & `OneOnOne-0.681/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.68/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.681/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.68
+Version: 0.681
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.68/PKG-INFO` & `OneOnOne-0.681/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.68
+Version: 0.681
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.68/README.md` & `OneOnOne-0.681/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.68/setup.py` & `OneOnOne-0.681/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.68
+VERSION=0.681
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

