# Comparing `tmp/gender-detection-local-0.0.7.tar.gz` & `tmp/gender-detection-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.0.7.tar", last modified: Thu Jul 13 09:30:40 2023, max compression
+gzip compressed data, was "gender-detection-local-0.0.8.tar", last modified: Thu Jul 13 09:59:02 2023, max compression
```

## Comparing `gender-detection-local-0.0.7.tar` & `gender-detection-local-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:30:40.486442 gender-detection-local-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:30:40.486442 gender-detection-local-0.0.7/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 09:30:40.486442 gender-detection-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:30:40.486442 gender-detection-local-0.0.7/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 09:30:40.000000 gender-detection-local-0.0.7/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 09:30:40.000000 gender-detection-local-0.0.7/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:30:40.000000 gender-detection-local-0.0.7/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 09:30:40.000000 gender-detection-local-0.0.7/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:30:40.486442 gender-detection-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 09:30:25.000000 gender-detection-local-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:02.837083 gender-detection-local-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:02.837083 gender-detection-local-0.0.8/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:58:51.000000 gender-detection-local-0.0.8/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-07-13 09:58:51.000000 gender-detection-local-0.0.8/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-13 09:58:51.000000 gender-detection-local-0.0.8/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-13 09:58:51.000000 gender-detection-local-0.0.8/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 09:59:02.837083 gender-detection-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 09:58:52.000000 gender-detection-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:59:02.837083 gender-detection-local-0.0.8/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-13 09:59:02.000000 gender-detection-local-0.0.8/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 09:59:02.000000 gender-detection-local-0.0.8/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:59:02.000000 gender-detection-local-0.0.8/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 09:59:02.000000 gender-detection-local-0.0.8/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 09:58:52.000000 gender-detection-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:59:02.837083 gender-detection-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-13 09:58:52.000000 gender-detection-local-0.0.8/setup.py
```

### Comparing `gender-detection-local-0.0.7/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.0.8/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.7/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.0.8/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tensorflow.io import read_file
 from tensorflow.image import decode_jpeg,resize,flip_left_right
 from tensorflow.keras.utils import image_dataset_from_directory
 from keras.models import Model,Sequential,load_model
 from keras.layers import Input,Conv2D,MaxPooling2D,Dropout,Flatten,Dense,GlobalAveragePooling2D,BatchNormalization
 from dotenv import load_dotenv
 load_dotenv()
-from CirclesLocalLoggerPython.LoggerServiceSingleton import LoggerServiceSingleton
+from LoggerLocalPythonPackage.LoggerServiceSingleton import locallgr
 
 
 
 
 
 
 
@@ -99,16 +99,15 @@
         """
         GenderClassifier is a class that detects the gender of a person through webcam images.
 
         Args:
             train (bool): a boolean indicating whether to train the model or not. Defaults to False.
             predict (bool): a boolean indicating whether to predict the gender or not. Defaults to True.
         """
-        self.logger = LoggerServiceSingleton()
-        self.lgrins = self.logger.get_instance()
+        self.lgrins = locallgr
 
     def predict_gender(self,model_path,image_path=None):
         """
         This function captures an image from the webcam and predicts the gender of the person.
 
         Returns:
             str: a string indicating the predicted gender ('Male' or 'Female').
```

### Comparing `gender-detection-local-0.0.7/README.md` & `gender-detection-local-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.0.7/setup.py` & `gender-detection-local-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.0.7',
+     version='0.0.8',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

